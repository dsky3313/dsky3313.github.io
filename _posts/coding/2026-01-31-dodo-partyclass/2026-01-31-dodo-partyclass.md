---
# bundle exec jekyll serve
## <span style="color:#0b89ff">■ </span>생태지구 알다니
#**<span style="color:#26beff">■ </span>**123
search: true
lastmod: 2026-01-31 00:00:00
sitemap: 
    changefreq : weekly
    priority : 0.5

title: "파티원 클래스 현황 &#124; 와우 한밤 애드온"
categories: # 카테고리 설정
  - Coding # Plater, Weakauras, WOWinfo, Achievement, Coding,
tags:
  - [lua]
toc: true # 목차 사용할지
toc_label: 파티원 클래스 현황
header:
  teaser: "/_posts/coding/2026-01-27-dodo-browsegroup/dodoLogo-teaser.webp"
---

'**Gemini**'로 제작했습니다. (한밤 12.0.0 기준)
{: .notice--warning}  

## <span style="color:#0b89ff">■ </span> 다운로드

[dodo](https://github.com/dsky3313/dodo/archive/refs/heads/main.zip){: .btn .btn--info} (GitHub)
<br>

## <span style="color:#0b89ff">■ </span> 설명

![alt text](/_posts/coding/2026-01-31-dodo-partyclass/partyclass1.webp)

파티모집 창 하단에 현재 파티원의 해제, 블러드, 전부 등 유무를 보여줍니다.

마우스를 직업아이콘에 올려두면 각 직업별 스킬을 볼 수 있습니다.
<br>
<br>

## <span style="color:#0b89ff">■ </span> 설정법

![alt text](/_posts/coding/2026-01-31-dodo-partyclass/partyclass2.webp)

설정창 (`/dd`) 에서 기능을 활성화/비활성화 할 수 있습니다.
<br>
<br>

## <span style="color:#0b89ff">■ </span> 애로사항

**<span style="color:#26beff">■ </span>** 배경프레임 생성
```
local partyClassFrame = CreateFrame("Frame", "PartyClassFrame", UIParent, "DefaultPanelBaseTemplate")
partyClassFrame:SetSize(542, 214)
partyClassFrame:SetPoint("TOPLEFT", PVEFrame, "BOTTOMLEFT", 20, 2)
partyClassFrame:SetFrameStrata("MEDIUM")
```
- `DefaultPanelBaseTemplate`을 사용하여, 자동으로 NineSlice가 적용된 창을 만들 수 있었다.
<br>
<br>

**<span style="color:#26beff">■ </span>** 현재 파티원 추적
```
local _, _, pID = UnitClass("player")
    if pID then activeIDs[pID] = true end

    local numMembers = GetNumGroupMembers()
    if numMembers > 0 then
        for i=1, numMembers do
            local unit = IsInRaid() and "raid"..i or "party"..i
            local _, _, cID = UnitClass(unit)
            if cID then activeIDs[cID] = true end
        end
    end
```
- 내 직업이 자꾸 확인이 안됨.  
`UnitClass("player")`을 사용해서 내 직업을 먼저 추적 > 파티원 추적.
<br>
<br>
