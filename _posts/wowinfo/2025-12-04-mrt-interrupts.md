---
# bundle exec jekyll serve
## <span style="color:#0b89ff">■ </span>생태지구 알다니
#**<span style="color:#26beff">■ </span>** 123
search: true
# last_modified_at: # 2021-10-09 수정날짜

title: "차단순서 배정 &#124; MRT"
categories: # 카테고리 설정
  - WOWinfo # Plater, Weakauras, WOWinfo, Achievement, Github,
tags:
  - [tag1, tag2]
toc: true # 목차 사용할지
toc_label: 차단순서 배정
header:
  teaser: "/ssets/img/wow/wowinfo/2025-12-04-mrt-interrupts/1.webp"
---

**<span style="color:#26beff">■ </span>**유튜브 질문댓글

![이미지 설명](/assets/img/wow/wowinfo/2025-12-04-mrt-interrupts/1.webp)

어느날, 한분이 유튜브 댓글로 질문을 주셨다.

사용한 애드온 : **<span style="color:#26beff">Method Raid Tools</span>** ([커스포지 링크](https://www.curseforge.com/wow/addons/method-raid-tools))
<br>

## <span style="color:#0b89ff">■ </span>MRT를 이용한 차단순서 배정

![이미지 설명](/assets/img/wow/wowinfo/2025-12-04-mrt-interrupts/2.webp)

/mrt > interrutps 에서 설정할 수 있습니다.

1. Profile : **<span style="color:#26beff">Shared</span>**  / 사용 **<span style="color:#26beff">체크</span>**  ✅  
2. 차단 할 몹의 **<span style="color:#26beff">NPCID</span>**를 입력합니다.  
   1넴 부관의 NPCID (211289)를 입력하면 테너 듀얼말이라고 인식합니다.  
3. 차단할 주문의 **<span style="color:#26beff">SpellID</span>**를 입력합니다.  
   화염구 (424421)를 입력합니다.  
4. 차단 로테이션을 돌릴 **<span style="color:#26beff">횟수</span>**를 입력합니다.  
   근거리 3로테이션을 돌릴 예정이므로, 3을 입력해줍니다.  
5. 차단을 담당할 **<span style="color:#26beff">Shared</span>**캐릭터명을 선택해줍니다.  
6. **<span style="color:#26beff">징표</span>**를 설정하면 해당 징표가 찍힌 몹에게서만 작동합니다. (아래 잠수부 참고)  
   듀얼말은 따로 징 설정을 하지 않으므로, 패스.  
7. **<span style="color:#26beff">차단 순서</span>**를 배정해줍니다.   
   Hodododo (1) > 근거리 1 (2) > 근거리 2 (3) 순으로 차단을 돌립니다.  
<br>
<br>

## <span style="color:#0b89ff">■ </span>MRT 차단 코드

아래 코드를 복사해서, 8번 import에 붙여넣으면 설정을 복사할 수 있습니다.
```
EXRTIRRU1ZqUmYqdnYclJZeJmXeJmuzJ1slTu2J8tbmuzdvw5323mEDllvzJuw5xTR99MPVMx3FlVA7741nV03o1TOSXkdu7MBQXggNjgBI5wyMYORB4SbQ)eZjPulQKKtm3sloFW60ydnXsZIZeZSWmJneSoXIna0fP8BABcVEZB9nDTM3mxqcyOYVU1D86fS032tpazBcmxOHkBexgAMPMyOjXzSXwyGbgJPFblMVrW9HgRmGp
```
<br>
<br>

## <span style="color:#0b89ff">■ </span>MRT 차단 외형설정

![이미지 설명](/assets/img/wow/wowinfo/2025-12-04-mrt-interrupts/3.webp)

**<span style="color:#26beff">Cast number</span>**과 **<span style="color:#26beff">Kicker name</span>** 은 본인이 보기 편한 크기로 설정.  

Font는 **<span style="color:#26beff">2002.ttf</span>**로 설정해야, 한글이 깨지지 않고 출력됩니다.
<br>
<br>

## <span style="color:#0b89ff">■ </span>예시 영상

{% include video id="0fkufq2pvow?start=506" provider="youtube" %} <!--유튜브-->