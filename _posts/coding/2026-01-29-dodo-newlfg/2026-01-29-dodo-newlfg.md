---
# bundle exec jekyll serve
## <span style="color:#0b89ff">■ </span>생태지구 알다니
#**<span style="color:#26beff">■ </span>**123
search: true
lastmod: 2026-01-29 00:00:00
sitemap: 
    changefreq : weekly
    priority : 0.5

title: "새로운 파티신청 알림 &#124; 와우 한밤 애드온"
categories: # 카테고리 설정
  - Coding # Plater, Weakauras, WOWinfo, Achievement, Coding,
tags:
  - [Lua]
toc: true # 목차 사용할지
toc_label: 새로운 파티신청 알림
header:
  teaser: "/_posts/coding/2026-01-27-dodo-browsegroup/dodoLogo-teaser.webp"
---

'**Gemini**'로 제작했습니다. (한밤 12.0.0 기준)
{: .notice--warning}  

## <span style="color:#0b89ff">■ </span> 원본 위크오라

[파티 지원자를 알려주는 위크오라](https://www.inven.co.kr/board/wow/17/40511) (와우 인벤)
<br>

## <span style="color:#0b89ff">■ </span> 다운로드

[dodo](https://github.com/dsky3313/dodo/archive/refs/heads/main.zip){: .btn .btn--info} (GitHub)
<br>

## <span style="color:#0b89ff">■ </span> 설명

![alt text](/_posts/coding/2026-01-29-dodo-newlfg/newlfg1.webp)

파티 모집 중, 새로운 신청이 왔을때 알림문구를 표시 & 알림음 재생.
<br>
<br>

## <span style="color:#0b89ff">■ </span> 설정법

![alt text](/_posts/coding/2026-01-29-dodo-newlfg/newlfg2.webp)

설정창 (`/dd`) 에서 기능을 활성화/비활성화 & 알림음 변경할 수 있습니다. (기본값 - 활성화)  

기본적으로 파티장일 때만 알림이 뜨고,

`파티원 기능 활성화`를 체크하면 파티원일 때도 알림이 뜹니다.
<br>
<br>

## <span style="color:#0b89ff">■ </span> 애로사항

**<span style="color:#26beff">■ </span>** 전투중 작동 오류

```
function NewLFG()
    if isIns() or InCombatLockdown() then return end
```

- `InCombatLockdown()`을 추가하여, 전투중 작동을 막음.
<br>
<br>

**<span style="color:#26beff">■ </span>** 체크박스 + 드롭다운 메뉴 구현 오류
```
<Frame name="dodoCheckboxDropdownTemplate" inherits="SettingsCheckBoxDropDownControlTemplate" virtual="true"/>
```
```
local initializer = Settings.CreateSettingInitializer("dodoCheckboxDropdownTemplate", data)
```
- `initializer = CreateSettingsCheckboxSliderInitializer`를 통해  
기본 설정창에 있는 체크박스 + 드롭다운을 구현하려 했으나 실패  
([Blizzard_SettingsDefinitions_Frame/Controls.lua](https://www.townlong-yak.com/framexml/live/Blizzard_SettingsDefinitions_Frame/Controls.lua#171)  )
- XML 파일을 제작하니 오류 해결..?
<br>
<br>