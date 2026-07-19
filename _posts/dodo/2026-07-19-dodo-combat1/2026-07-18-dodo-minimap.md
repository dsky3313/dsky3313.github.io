---
# bundle exec jekyll serve
## <span style="color:#0b89ff">■ </span>생태지구 알다니
#**<span style="color:#26beff">■ </span>**123
search: true
lastmod: 2026-07-18 00:00:00
sitemap: 
    changefreq : weekly
    priority : 0.5

title: "미니맵 &#124; dodo"
categories: # 카테고리 설정
  - dodo # Plater, Weakauras, WOWinfo, Achievement, dodo,
tags:
  - [dodo]
toc: true # 목차 사용할지
toc_label: 미니맵
header:
  teaser: "/_posts/dodo/2026-07-18-dodo-minimap/minimap.webp"
---

'**Claude**'로 제작했습니다. (한밤 12.0.7 기준)
{: .notice--warning}  

## <span style="color:#0b89ff">■ </span> 참고한 애드온

[Leatrix Plus](https://www.curseforge.com/wow/addons/leatrix-plus) (CurseForge)  
[Simple FPS Ping](https://www.curseforge.com/wow/addons/simple-fps-ping) (CurseForge)  
[HidingBar](https://www.curseforge.com/wow/addons/hidingbar) (CurseForge)  
<br>


## <span style="color:#0b89ff">■ </span> 다운로드 및 설치

[dodo](https://github.com/dsky3313/dodo/archive/refs/heads/main.zip){: .btn .btn--info} (GitHub)

압축 풀고,  

폴더명을 `dodo-main` > `dodo`로 변경 후, 애드온 폴더에 넣어주세요.
<br>

## <span style="color:#0b89ff">■ </span> 설명

![alt text](/_posts/dodo/2026-07-18-dodo-minimap/minimap.webp)  

미니맵에 기능을 추가합니다.

편집모드에서 모듈 활성화/비활성화하고, 미니맵 프레임을 선택해서 세부 설정할 수 있습니다.

명령어 : `/ed`
<br>
<br>

클릭 시, 각 기능 설명으로 이동합니다.

- [사각형 미니맵](#-사각형-미니맵)
- [FPS / MS 표시](#-fps--ms-표시)
- [좌표 표시](#-좌표-표시)
- [줌 초기화](#-줌-초기화)
- [애드온 아이콘 모음](#-애드온-아이콘-모음)
<br>
<br>

## <span style="color:#0b89ff">■ </span> 사각형 미니맵

![alt text](/_posts/dodo/2026-07-18-dodo-minimap/square.webp)  

미니맵을 원형에서 사각형으로 바꿉니다.

순정 테두리를 숨기고, 행동단축바 스타일의 9슬라이스 테두리를 새로 적용합니다.
<br>
<br>

## <span style="color:#0b89ff">■ </span> FPS / MS 표시

![alt text](/_posts/dodo/2026-07-18-dodo-minimap/fps.webp)  

미니맵 아래에 FPS와 레이턴시(MS)를 표시합니다.

수치에 따라 색상이 바뀝니다.

| 수치 | FPS 기준 | MS 기준 |
|------|----------|---------|
| 초록 | 60 이상 | 100 이하 |
| 노랑 | 30~59 | 101~200 |
| 빨강 | 30 미만 | 200 초과 |

인스턴스 안에서는 2초마다, 바깥에서는 1초마다 갱신됩니다.
<br>
<br>

## <span style="color:#0b89ff">■ </span> 좌표 표시

![alt text](/_posts/dodo/2026-07-18-dodo-minimap/coord.webp)  

미니맵 아래에 현재 플레이어 위치 좌표를 표시합니다.

인스턴스 안에서는 숨겨지고, 필드에서만 표시됩니다.

월드맵을 열면 플레이어 좌표와 마우스 커서 좌표를 함께 표시합니다.
<br>
<br>

## <span style="color:#0b89ff">■ </span> 줌 초기화

지역을 이동하면 미니맵 줌을 자동으로 최소값(0)으로 초기화합니다.

초기화 시 짧은 사운드가 재생됩니다.

레이드·쐐기돌 던전 안에서는 초기화하지 않습니다.
<br>
<br>

## <span style="color:#0b89ff">■ </span> 애드온 아이콘 모음

![alt text](/_posts/dodo/2026-07-18-dodo-minimap/iconaddons.webp)  

미니맵 주변에 흩어진 애드온 아이콘들을 미니맵 아래에 한 줄로 정렬합니다.

`\dodo\Module\Minimap\IconAddons.lua`의 `Config.sortOrder` 테이블에서 표시 순서를 지정하고, `Config.hideSet` 테이블에서 완전히 숨길 애드온을 등록할 수 있습니다.

기본 정렬 순서:

| 순서 | 애드온 |
|------|--------|
| 1 | 확장팩 랜딩 페이지 버튼 |
| 2 | SimpleAddonManager |
| 3 | NotEvenClose |
| 4 | SimulationCraft |
| ... | 기타 |

기본 숨김: RaiderIO
<br>
<br>
