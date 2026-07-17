---
# bundle exec jekyll serve
## <span style="color:#0b89ff">■ </span>생태지구 알다니
#**<span style="color:#26beff">■ </span>**123
search: true
lastmod: 2026-07-16 00:00:00
sitemap: 
    changefreq : weekly
    priority : 0.5

title: "행동단축바 &#124; dodo"
categories: # 카테고리 설정
  - dodo # Plater, Weakauras, WOWinfo, Achievement, dodo,
tags:
  - [dodo]
toc: true # 목차 사용할지
toc_label: 자원바
header:
  teaser: "/_posts/dodo/2026-01-27-dodo-browsegroup/dodoLogo-teaser.webp"
---

'**Claude**'로 제작했습니다. (한밤 12.0.7 기준)
{: .notice--warning}  

## <span style="color:#0b89ff">■ </span> 참고한 애드온

[ActionBarsEnhanced](https://www.curseforge.com/wow/addons/actionbarsenhanced) (CurseForge)  
[CDMButtonAuras](https://www.curseforge.com/wow/addons/cdmbuttonauras) (CurseForge)  
[ActionBar Interrupt Highlight](https://www.curseforge.com/wow/addons/actionbarinterrupthighlight) (CurseForge)  
<br>


## <span style="color:#0b89ff">■ </span> 다운로드 및 설치

[dodo](https://github.com/dsky3313/dodo/archive/refs/heads/main.zip){: .btn .btn--info} (GitHub)

압축 풀고,  

폴더명을 `dodo-main` > `dodo`로 변경 후, 애드온 폴더에 넣어주세요.
<br>

## <span style="color:#0b89ff">■ </span> 설명

![alt text](/_posts/dodo/2026-07-18-dodo-actionbar/actionbar3.webp)  

블리자드 행동단축바에 기능을 추가합니다.
<br>
<br>

![alt text](/_posts/dodo/2026-07-18-dodo-actionbar/actionbar2.webp)  

편집모드에서 모듈 활성화/비활성화하고, 각 바별로 개별 설정할 수 있습니다.

명령어 : `/ed`
<br>
<br>

클릭 시, 각 기능 설명으로 이동합니다.

- [아이콘 색상](#-아이콘-색상)
- [아이콘 간격](#-아이콘-간격)
- [단축키 / 매크로 텍스트](#-단축키--매크로-텍스트)
- [차단 오버레이](#-차단-오버레이)
- [강화효과 오버레이](#-강화효과-오버레이)
- [물약 오버레이](#-물약-오버레이)
<br>
<br>

## <span style="color:#0b89ff">■ </span> 아이콘 색상

상태에 따라 아이콘의 색상을 변경합니다.

<!-- 이미지: 색상 비교 (기본 vs dodo) -->

| 상태 | 효과 |
|------|------|
| 사거리 밖 | 파란색 |
| 마나 부족 | 빨간색 |
| 쿨다운 & 사용불가 | 회색 |

<br>
<br>

## <span style="color:#0b89ff">■ </span> 아이콘 간격

![alt text](/_posts/dodo/2026-07-18-dodo-actionbar/iconpadding.webp)  

블리자드 편집모드에선 최소값이 2까지밖에 지원하지 않아서, -5까지 간격을 줄일 수 있게 만들었습니다.
<br>
<br>

## <span style="color:#0b89ff">■ </span> 단축키 / 매크로 텍스트

![alt text](/_posts/dodo/2026-07-18-dodo-actionbar/text.webp)  

단축키 텍스트, 매크로 이름을 바별로 숨길 수 있습니다.
<br>
<br>

## <span style="color:#0b89ff">■ </span> 차단 오버레이

![alt text](/_posts/dodo/2026-07-18-dodo-actionbar/interrupt.webp)  

대상 또는 주시대상이 스킬을 시전할 때, 차단 스킬 버튼에 오버레이와 남은시간을 표시합니다.

우선순위 : 주시대상 > 대상
<br>
<br>

## <span style="color:#0b89ff">■ </span> 강화효과 오버레이

![alt text](/_posts/dodo/2026-07-18-dodo-actionbar/actionbar1.webp)  

버프가 걸린 스킬의 남은 시간, 스택을 오버레이로 표시합니다.

재사용 대기시간을 켜고, 강화효과를 추적해야 활성화 됩니다.

일부 직업 특화 매핑이 포함돼 있습니다.

| 버프 | 연결 스킬 |
|------|----------|
| 집행자의 정밀함 | 필사의 일격 (무기 전사) |
| 격노 | 광란 (분노 전사) |
| 소용돌이 연마 | 소용돌이 (분노 전사) |

<br>

![alt text](/_posts/dodo/2026-07-18-dodo-actionbar/cdmAdd.webp)  

`\dodo\Module\Actionbar\OverlayCDM.lua`에서 수동으로 추가할 수 있습니다.
<br>
<br>


## <span style="color:#0b89ff">■ </span> 물약 오버레이

전투중, 물약을 사용가능하면 오버레이를 표시해줍니다.
<br>
<br>