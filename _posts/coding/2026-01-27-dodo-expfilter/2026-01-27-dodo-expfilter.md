---
# bundle exec jekyll serve
## <span style="color:#0b89ff">■ </span>생태지구 알다니
#**<span style="color:#26beff">■ </span>**123
search: true
lastmod: 2026-01-27 00:00:00
sitemap: 
    changefreq : weekly
    priority : 0.5

title: "경매장 '현행 확장팩 전용' 자동 설정 &#124; 와우 한밤 애드온"
categories: # 카테고리 설정
  - Coding # Plater, Weakauras, WOWinfo, Achievement, Coding,
tags:
  - [Lua]
toc: true # 목차 사용할지
toc_label: 함수와 변수
header:
  teaser: "/_posts/coding/2026-01-27-dodo-browsegroup/dodoLogo-teaser.webp"
---

'**Gemini**'로 제작했습니다. (한밤 12.0.0 기준)
{: .notice--warning}  

## <span style="color:#0b89ff">■ </span> 원본 위크오라

[경매장 "현행 확장팩 전용" 자동 설정 위크오라](https://www.inven.co.kr/board/wow/17/39328) (와우 인벤)
<br>

## <span style="color:#0b89ff">■ </span> 다운로드

[dodo](https://github.com/dsky3313/dodo/archive/refs/heads/main.zip){: .btn .btn--info} (GitHub)
<br>

## <span style="color:#0b89ff">■ </span> 설명

![alt text](/_posts/coding/2026-01-27-dodo-expfilter/expfilter1.webp)

경매장 / 주문제작 창에서 자동으로 "현행 확장팩 전용"을 활성화 합니다.

소한밤 업뎃으로 내부전쟁은 구확팩이 되어서, 지금 당장은 비활성화 하는것을 추천드립니다.
<br>
<br>

![alt text](/_posts/coding/2026-01-27-dodo-expfilter/expfilter3.webp)

성능 최적화를 위해, 쐐기와 레이드에선 작동하지 않습니다.
<br>
<br>

## <span style="color:#0b89ff">■ </span> 설정법

![alt text](/_posts/coding/2026-01-27-dodo-expfilter/expfilter2.webp)

설정창 (`/dd`) 에서 기능을 활성화/비활성화 할 수 있습니다. (기본값 - 활성화)
<br>
<br>

## <span style="color:#0b89ff">■ </span> 애로사항

**<span style="color:#26beff">■ </span>** 경매장, 주문제작 창 `HookScript` 오류

```
elseif event == "ADDON_LOADED" and arg1 == "Blizzard_AuctionHouseUI" then
    if AuctionHouseFrame and AuctionHouseFrame.SearchBar then
        AuctionHouseFrame.SearchBar:HookScript("OnShow", function()
            C_Timer.After(0, checkAuctionFilter)
        end)
        initFilterFrame:UnregisterEvent("ADDON_LOADED")
    end

elseif event == "AUCTION_HOUSE_SHOW" then
    checkAuctionFilter()
```

- `ADDON_LOADED` 와 `C_Timer.After(0, checkAuctionFilter)`를 추가하여,  
확실하게 Hook 할 수 있게 수정.
<br>
<br>

**<span style="color:#26beff">■ </span>** DB 저장 안됨
```
dodoDB = dodoDB or {}
local isEnabled = (dodoDB.useAuctionFilter ~= false) -- 기본값 true
```
- DB값 초기화, DB 기본값 추가.
<br>
<br>

**<span style="color:#26beff">■ </span>** 옵션 (체크박스) 추가
```
function ns.expfilter()
    checkAuctionFilter()
    checkCraftFilter()
end
```
- 나눠진 함수를 하나로 통합해서 체크박스 등록.
<br>
<br>