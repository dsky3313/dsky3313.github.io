---
# bundle exec jekyll serve
## <span style="color:#0b89ff">■ </span>생태지구 알다니
#**<span style="color:#26beff">■ </span>**123
search: true
lastmod: 2026-01-31 00:00:00
sitemap: 
    changefreq : weekly
    priority : 0.5

title: "쐐기돌 굴리세요! &#124; 와우 한밤 애드온"
categories: # 카테고리 설정
  - Coding # Plater, Weakauras, WOWinfo, Achievement, Coding,
tags:
  - [lua]
toc: true # 목차 사용할지
toc_label: 돌 굴리세요 알림
header:
  teaser: "/_posts/coding/2026-01-27-dodo-browsegroup/dodoLogo-teaser.webp"
---

'**Gemini**'로 제작했습니다. (한밤 12.0.0 기준)
{: .notice--warning}  

## <span style="color:#0b89ff">■ </span> 원본 위크오라

[Reroll Your Key?](https://wago.io/AT6ZmGDlK) (Wago)
<br>

## <span style="color:#0b89ff">■ </span> 다운로드

[dodo](https://github.com/dsky3313/dodo/archive/refs/heads/main.zip){: .btn .btn--info} (GitHub)
<br>

## <span style="color:#0b89ff">■ </span> 설명

![alt text](/_posts/coding/2026-01-31-dodo-keyroll/keyroll1.webp)

쐐기 완료 후, 돌을 바꾸라고 채팅으로 알려줍니다.

파티원 돌 현황 보여주는 기능은 `디테일즈`가 설치된 플레이어끼리만 보여줍니다.
<br>
<br>

## <span style="color:#0b89ff">■ </span> 설정법

![alt text](/_posts/coding/2026-01-31-dodo-keyroll/keyroll2.webp)

설정창 (`/dd`) 에서 기능을 활성화/비활성화 할 수 있습니다.
<br>
<br>

## <span style="color:#0b89ff">■ </span> 애로사항

**<span style="color:#26beff">■ </span>** 파티원 쐐기돌 현황 불러오기
```
local displayText = ""
    for _, unit in ipairs(partyMembers) do
        local info = LibOpenRaid.GetKeystoneInfo(unit)
        local uName = UnitName(unit)
        local _, class = UnitClass(unit)
        local color = (RAID_CLASS_COLORS[class] and RAID_CLASS_COLORS[class].colorStr) or "ffffffff"

        if info then
            displayText = displayText .. string.format("|c%s%s|r: %s\n", color, uName, GetKeyLink(info))
        end
    end
```
- `LibOpenRaid` 라이브러리를 통해, 정보를 가져오는 것으로 해결 (Details!에 포함되어 있음)  
하지만, 한밤 업데이트로 디테일즈를 사용하는 사람이 적어져서, 전부 다 가져오진 못하게 됨.
<br>
<br>