---
# bundle exec jekyll serve
search: true
#toc: true # 목차 사용할지
toc_sticky: true # 목차가 옆에 따라올지
last_modified_at: # 2021-10-09 수정날짜
#excerpt: "와우 내부전쟁 탈것 매크로"
# tags:
#   - [tag1, tag2]
# permalink: /wow-data/riding-macro

date: 2025-08-07
title: "전사 매크로 &#124; 와우 내부전쟁 3시즌"
tags:
   - [전사, 매크로]

categories: # 카테고리 설정
  - WOWinfo
header:
  teaser: "/assets/img/wow/wowinfo/2025-08-07-wowinfo-macro-warrior/1.webp"
---
![alt text](/assets/img/wow/wowinfo/2025-08-07-wowinfo-macro-warrior/1.webp){: .align-center}

내부전쟁 3시즌 전사 매크로
{: .text-center}

## <span style="color:#0b89ff">■</span> 주시 차단
```
#showtooltip 들이치기
/시전 [@focus,harm][harm]들이치기
```
주시대상 차단하는 매크로입니다.  

## <span style="color:#0b89ff">■</span> 투신 (쿨기)
```
#showtooltip 투신
/시전 투신
/시전 천둥의 포효
/사용 13
/사용 꿈결속 증강의 룬  
/사용 절제된 물약​
```
투신, 쿨기, 장신구, 물약 다 묶어놨습니다.  

## <span style="color:#0b89ff">■</span> 원버튼 태세 전환
```  
#showtooltip
/시전 [form:2]방어 태세;[spec:1/3]전투 태세;광폭 태세​
```  
[ 방어 태세 ] ↔ [전투 태세 ], [광폭 태세 ] 스위칭해줍니다.  

## <span style="color:#0b89ff">■</span> 원버튼 돌진, 연전연승 매크로
```
#showtooltip
/시전 [@target,help]가로막기;[@target,harm]돌진;돌진
/시전 [harm]연전연승;[help,dead,combat]그럴싸하게 현실적인 전력선;[help,dead,nocombat]노움 군용칼;[help,nodead,nocombat]방직천 붕대;연전연승
```

- 아군 대상으로 [ **가로막기** ], 적군 대상으로 [ **돌진** ] 
- 적군 대상으로 [ **연전연승** ]
- 전투중일 때 죽은 아군 대상 ▶ **그럴싸하게 현실적인 전력선** (기공 전투부활 소모템)
- 비전투중일 때 죽은 아군 대상 ▶ **노움 군용칼** (기공 부활템)
- 비전투중일 때 살아있는 아군 대상 ▶ **방직천 붕대** (치유 소모템)  

## <span style="color:#0b89ff">■</span> 천포 ↔ 용창
```
#showtooltip
/시전 [known:천둥의 포효]천둥의 포효;용사의 창
```
특성창에서 천둥의 포효를 배웠으면 [ **<span style="color:#26beff">천둥의 포효</span>** ], 그렇지 않으면 [ **<span style="color:#26beff">용사의 창</span>** ]