---
# bundle exec jekyll serve
## <span style="color:#0b89ff">■ </span>생태지구 알다니
#**<span style="color:#26beff">■ </span>**123
search: true
lastmod: 2026-07-19 00:00:00
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
  teaser: "/_posts/dodo/2026-07-19-dodo-minimap/2.webp"
---

'**Claude**'로 제작했습니다. (한밤 12.0.7 기준)
{: .notice--warning}  

## <span style="color:#0b89ff">■ </span> 참고한 애드온

[Leatrix Plus](https://www.curseforge.com/wow/addons/leatrix-plus) (CurseForge)  
[Simple FPS Ping](https://www.curseforge.com/wow/addons/simple-fps-ping) (CurseForge)  
[HidingBar](https://www.curseforge.com/wow/addons/hidingbar) (CurseForge)  
<br>
<br>

## <span style="color:#0b89ff">■ </span> 다운로드 및 설치

[dodo](https://github.com/dsky3313/dodo/archive/refs/heads/main.zip){: .btn .btn--info} (GitHub)

압축 풀고,  

폴더명을 `dodo-main` > `dodo`로 변경 후, 애드온 폴더에 넣어주세요.
<br>
<br>

## <span style="color:#0b89ff">■ </span> 설명

![alt text](/_posts/dodo/2026-07-19-dodo-minimap/1.webp)  

미니맵에 기능을 추가합니다.

편집모드에서 모듈 활성화/비활성화하고, 미니맵 프레임을 선택해서 세부 설정할 수 있습니다.

- 설정 : 편집모드 (명령어 `/ed` 혹은 `/ㄷㅇ`) > 인터페이스 > ☑ **미니맵**  
<br>
<br>

### <span style="color:#0b89ff">■ </span> 사각형 미니맵

![alt text](/_posts/dodo/2026-07-19-dodo-minimap/2.webp)  

원형 미니맵을 사각형으로 바꿉니다.
<br>
<br>

### <span style="color:#0b89ff">■ </span> FPS / MS 표시

미니맵 좌측 상단에 FPS와 레이턴시(MS)를 표시합니다.

수치에 따라 색상이 바뀝니다.

| 수치 | FPS 기준 | MS 기준 |
|------|----------|---------|
| 초록 | 60 이상 | 100 이하 |
| 노랑 | 30~59 | 101~200 |
| 빨강 | 30 미만 | 200 초과 |

<br>

### <span style="color:#0b89ff">■ </span> 좌표 표시

미니맵 우측 상단에 현재 플레이어 위치 좌표를 표시합니다.

인스턴스 안에서는 숨겨지고, 필드에서만 표시됩니다.

월드맵을 열면 플레이어 좌표와 마우스 커서 좌표를 함께 표시합니다.
<br>
<br>

### <span style="color:#0b89ff">■ </span> 줌 초기화

미니맵 줌을 변경 후, 일정 시간 뒤에 자동으로 초기화합니다.
<br>
<br>

### <span style="color:#0b89ff">■ </span> 애드온 아이콘 모음

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