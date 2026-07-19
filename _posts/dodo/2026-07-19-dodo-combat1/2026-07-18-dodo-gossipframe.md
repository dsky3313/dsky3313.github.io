---
# bundle exec jekyll serve
## <span style="color:#0b89ff">■ </span>생태지구 알다니
#**<span style="color:#26beff">■ </span>**123
search: true
lastmod: 2026-07-18 00:00:00
sitemap: 
    changefreq : weekly
    priority : 0.5

title: "NPC 대화창 &#124; dodo"
categories: # 카테고리 설정
  - dodo # Plater, Weakauras, WOWinfo, Achievement, dodo,
tags:
  - [dodo]
toc: true # 목차 사용할지
toc_label: NPC 대화창
header:
  teaser: "/_posts/dodo/2026-07-18-dodo-gossipframe/gossip.webp"
---

'**Claude**'로 제작했습니다. (한밤 12.0.7 기준)
{: .notice--warning}  

## <span style="color:#0b89ff">■ </span> 참고한 애드온

[ExwindTools](https://www.curseforge.com/wow/addons/exwindtools) (CurseForge)  
[MKS_Helper](https://www.curseforge.com/wow/addons/mks-helper) (CurseForge)  
<br>


## <span style="color:#0b89ff">■ </span> 다운로드 및 설치

[dodo](https://github.com/dsky3313/dodo/archive/refs/heads/main.zip){: .btn .btn--info} (GitHub)

압축 풀고,  

폴더명을 `dodo-main` > `dodo`로 변경 후, 애드온 폴더에 넣어주세요.
<br>

## <span style="color:#0b89ff">■ </span> 설명

NPC 대화창에 기능을 추가합니다.

설정 경로 : `/dd` → 인터페이스 → NPC 대화
<br>
<br>

클릭 시, 각 기능 설명으로 이동합니다.

- [자동 선택](#-자동-선택)
- [린도르미 현재돌](#-린도르미-현재돌)
- [ID 표시](#-id-표시)
<br>
<br>

## <span style="color:#0b89ff">■ </span> 자동 선택

![alt text](/_posts/dodo/2026-07-18-dodo-gossipframe/autoselect.webp)  

사전 설정된 NPC 대화 선택지를 자동으로 클릭합니다.

주로 M+ 던전 진입 전 버프 NPC 대화에 활용됩니다.

기본 포함된 자동 선택 목록:

| NPC | 내용 |
|-----|------|
| 사론 포로구출 | 버프 선택지 |
| 알게타르 대학 | 버프 선택지 |
| 공결탑 제나스 | 버프 선택지 |
| 마이사라 동굴 | 버프 선택지 |
| 한여름 불꽃축제 | 아훈 소환 |

`\dodo\Module\GossipFrame\SelectAuto.lua`의 `PRESET_IDS` 테이블에 ID를 추가해서 직접 등록할 수 있습니다.
<br>
<br>

## <span style="color:#0b89ff">■ </span> 린도르미 현재돌

![alt text](/_posts/dodo/2026-07-18-dodo-gossipframe/lindormi.webp)  

쐐기돌 교환 NPC인 린도르미와 대화할 때, 대화창 상단에 현재 보유 중인 쐐기돌 정보를 표시합니다.

쐐기돌을 교환하면 정보가 자동으로 갱신됩니다.
<br>
<br>

## <span style="color:#0b89ff">■ </span> ID 표시

![alt text](/_posts/dodo/2026-07-18-dodo-gossipframe/id.webp)  

NPC 대화창의 선택지와 퀘스트 항목에 ID를 회색으로 표시합니다.

자동 선택 기능에 새 NPC를 등록할 때 ID를 확인하는 용도로 활용할 수 있습니다.
<br>
<br>
