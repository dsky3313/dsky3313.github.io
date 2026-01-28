---
# bundle exec jekyll serve
## <span style="color:#0b89ff">■ </span>생태지구 알다니
#**<span style="color:#26beff">■ </span>**123
search: true
lastmod: 2026-01-27 00:00:00
sitemap: 
    changefreq : weekly
    priority : 0.5

title: "지금 삭제 &#124; 와우 한밤 애드온"
categories: # 카테고리 설정
  - Coding # Plater, Weakauras, WOWinfo, Achievement, Coding,
tags:
  - [lua]
toc: true # 목차 사용할지
toc_label: 지금 삭제
header:
  teaser: "/_posts/coding/dodoLogo-teaser.webp"
---

'**Gemini**'로 제작했습니다. (한밤 12.0.0 기준)
{: .notice--warning}  

## <span style="color:#0b89ff">■ </span> 원본 애드온

[Leatrix Plus](https://www.curseforge.com/wow/addons/leatrix-plus) (커스포지)
<br>

## <span style="color:#0b89ff">■ </span> 다운로드

[dodo](https://github.com/dsky3313/dodo/archive/refs/heads/main.zip){: .btn .btn--info} (GitHub)
<br>

## <span style="color:#0b89ff">■ </span> 설명

![alt text](/_posts/coding/2026-01-27-dodo-deletenow/deletenow3.webp)

☑ "지금파괴" 자동기입  
☐ 아이템 파괴 간소화  
- `지금파괴` 문구를 자동으로 입력해줍니다.
<br>

![alt text](/_posts/coding/2026-01-27-dodo-deletenow/deletenow1.webp)

☑ "지금파괴" 자동기입  
☑ 아이템 파괴 간소화  
- `지금파괴` 문구를 자동으로 입력해줍니다.
<br>
<br>

![alt text](/_posts/coding/2026-01-27-dodo-expfilter/expfilter3.webp)

성능 최적화를 위해, 쐐기와 레이드에선 작동하지 않습니다.
<br>
<br>

## <span style="color:#0b89ff">■ </span> 설정법

![alt text](/_posts/coding/2026-01-27-dodo-deletenow/deletenow2.webp)

설정창 (`/dd`) 에서 기능을 활성화/비활성화 할 수 있습니다. (기본값 - 활성화)
<br>
<br>

## <span style="color:#0b89ff">■ </span> 애로사항

**<span style="color:#26beff">■ </span>** `예` 자동클릭

- 자동으로 `예`까지 클릭하려 했으나, 막혀버림 (ADDON_ACTION_BLOCKED).  
▶ "지금삭제" 자동기입 까지만 구현.
<br>
<br>

**<span style="color:#26beff">■ </span>** `tooltip` 앵커

```
GameTooltip:SetOwner(StaticPopup1, "ANCHOR_NONE")
GameTooltip:SetPoint("TOP", StaticPopup1, "BOTTOM", 0, -5)
```
- `tooltip`이 편집모드에서 지정된 위치에 자꾸 뜸.  
▶ 앵커 위치를 초기화하고 다시 설정
<br>
<br>

**<span style="color:#26beff">■ </span>** 설정창 체크박스 하위메뉴 구현

![alt text](/_posts/coding/2026-01-27-dodo-deletenow/deletenow4.webp)

```
local settingParentDeleteNow, initParentDeleteNow = Checkbox(OptionCategory, "deleteNowAutoFill", "\"지금파괴\" 자동기입", "아이템 파괴 확인 메시지를 자동으로 입력합니다.", true)
local settingChildDeleteNow, initChildDeleteNow = Checkbox(OptionCategory, "deleteNowHideEditbox", "아이템 파괴 간소화", "확인 메시지를 없애고 확인버튼만 남깁니다.", true)
if settingParentDeleteNow and settingChildDeleteNow then
    settingParentDeleteNow:SetValueChangedCallback(function(_, value)
        if value == false then
            settingChildDeleteNow:SetValue(false) -- 부모가 꺼지면 자식도 끔
        end
    end)
    initChildDeleteNow:SetParentInitializer(initParentDeleteNow, function()
        return settingParentDeleteNow:GetValue()
    end)
end
```

- 기본 설정창의 하위메뉴를 따라 만들어보고 싶었음.  
▶ 인터페이스 설장창 Lua에서 SetParentInitializer를 사용하여 구현. [Blizzard_SettingsDefinitions_Frame/Interface.lua](https://www.townlong-yak.com/framexml/live/Blizzard_SettingsDefinitions_Frame/Interface.lua#117)
<br>
<br>