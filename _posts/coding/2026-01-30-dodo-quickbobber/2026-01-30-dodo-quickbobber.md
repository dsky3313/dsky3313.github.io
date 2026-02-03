---
# bundle exec jekyll serve
## <span style="color:#0b89ff">■ </span>생태지구 알다니
#**<span style="color:#26beff">■ </span>**123
search: true
lastmod: 2026-01-30 00:00:00
sitemap: 
    changefreq : weekly
    priority : 0.5

title: "빠른 낚시찌 버튼 &#124; 와우 한밤 애드온"
categories: # 카테고리 설정
  - Coding # Plater, Weakauras, WOWinfo, Achievement, Coding,
tags:
  - [lua]
toc: true # 목차 사용할지
toc_label: 빠른 낚시찌 버튼
header:
  teaser: "/_posts/coding/2026-01-27-dodo-browsegroup/dodoLogo-teaser.webp"
---

'**Gemini**'로 제작했습니다. (한밤 12.0.0 기준)
{: .notice--warning}  

## <span style="color:#0b89ff">■ </span> 원본 위크오라

[Clickable Weakaura](https://wago.io/cdNaS-9Oo) (Wago)
<br>

## <span style="color:#0b89ff">■ </span> 다운로드

[dodo](https://github.com/dsky3313/dodo/archive/refs/heads/main.zip){: .btn .btn--info} (GitHub)
<br>

## <span style="color:#0b89ff">■ </span> 설명

![alt text](/_posts/coding/2026-01-30-dodo-quickbobber/quickbobber1.webp)

전문기술창에서 낚시찌 장난감 사용버튼을 띄워줍니다. (재활용 가능한 심하게 큰 낚시찌)
<br>
<br>

## <span style="color:#0b89ff">■ </span> 설정법

![alt text](/_posts/coding/2026-01-30-dodo-quickbobber/quickbobber2.webp)

설정창 (`/dd`) 에서 기능을 활성화/비활성화 할 수 있습니다. (기본값 - 활성화)  

기본적으로 파티장일 때만 알림이 뜨고,

`파티원 기능 활성화`를 체크하면 파티원일 때도 알림이 뜹니다.
<br>
<br>

![alt text](/_posts/coding/2026-01-27-dodo-expfilter/expfilter3.webp)

성능 최적화를 위해, 쐐기와 레이드에선 작동하지 않습니다.
<br>
<br>

## <span style="color:#0b89ff">■ </span> 애로사항

**<span style="color:#26beff">■ </span>** 버튼 구현

```
if data.type == "spell" then
if data.isAction then
  self:SetAttribute("type", "spell")
  self:SetAttribute("spell", data.id)
end
```

- 클릭가능 위크오라를 참고하여, `SecureActionButtonTemplate`로 프레임 생성.
- 다른 기능에서도 많이 쓸 것 같아, `Icon.lua` 라이브러리를 제작.
- `spell`, `item`, `macro` 모두 사용할 수 있게 제작.
<br>
<br>

**<span style="color:#26beff">■ </span>** 아이콘 커스터마이징
```
local BobberConfig = {
    isAction = true,
    type = "item",
    -- macrotext = "/cast 낚시\n/use 13",
    id = 202207,
    icon = nil,
    iconsize = {34, 34},
    iconposition = {"TOPLEFT", "SecondaryProfession2", "TOPLEFT", 250, -7},
    label = "낚시찌",
    fontsize = 12,
    fontposition = {"BOTTOMRIGHT", "self", "BOTTOMLEFT", -2, 2},
    cooldownSize = 12,
    outline = false,
    framestrata = "HIGH",
}
```
- 기능을 추가할 때마다 일일히 작성하는게 번거로웠음.    
테이블 형식의 템플릿을 만들고, 거기에 맞춰 아이콘을 만들 수 있게 구현.
<br>
<br>