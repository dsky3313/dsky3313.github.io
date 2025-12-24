---
# bundle exec jekyll serve
## <span style="color:#0b89ff">■ </span>생태지구 알다니
#**<span style="color:#26beff">■ </span>**123
search: true
# last_modified_at: # 2021-10-09 수정날짜

published : false
title: "매크로 만들기 &#124; 와우 내부전쟁 3시즌"
categories: # 카테고리 설정
  - WOWinfo # Plater, Weakauras, WOWinfo, Achievement, Github,
tags:
  - [매크로]
toc: true # 목차 사용할지
toc_label: 매크로 만들기
header:
  teaser: "/assets/img/wow/weakauras/2025-08-08-bigwig-timer/1.webp"
---

## <span style="color:#0b89ff">■ </span>매크로창 띄우기

ESC > 매크로설정 > 만들기 클릭

```
/dump C_Map.GetBestMapForUnit("player")
/run print("지도 mapID:",WorldMapFrame:GetMapID())
/script px,py=C_Map.GetPlayerMapPosition(C_Map.GetBestMapForUnit("player"),"player"):GetXY()
/script print(format ("현 위치:[%s]%.2f %.2f",GetZoneText(),px*100,py*100));
```

https://us.forums.blizzard.com/en/wow/t/how-do-i-find-out-zone-id/422066/8
https://us.forums.blizzard.com/en/wow/t/macro-for-coordinates/513149



**<span style="color:#26beff">■ </span>** 123
본문은 여기에...  
<br>
![이미지 설명](/)
![이미지 설명](/assets/img/wow/wowdata/partyleave/1.webp){: .align-center}
![이미지 설명](https://wow.zamimg.com/images/wow/icons/large/spell_nature_bloodlust.jpg){: width="30" height="30"} <!--블러드-->
![이미지 설명](https://wow.zamimg.com/images/wow/icons/large/ability_ambush.jpg){: width="30" height="30"} 패스 : 1넴 뒤 박스, 14번 앞 방울이, 막넴앞 시동자 2 마리 <!--패스--> 
![이미지 설명](https://wow.zamimg.com/images/wow/icons/large/ability_ambush.jpg){: width="30" height="30"} 저주 해제 : 드루이드, 마법사, 주술사
![이미지 설명](https://wow.zamimg.com/images/wow/icons/large/ability_ambush.jpg){: width="30" height="30"} 질병 해제 : 사제, 성기사, 수도사
![이미지 설명](https://wow.zamimg.com/images/wow/icons/large/ability_ambush.jpg){: width="30" height="30"} 마법 해제 : 사제, 흑마법사
![이미지 설명](https://wow.zamimg.com/images/wow/icons/large/ability_ambush.jpg){: width="30" height="30"} 독 해제 : 기원사, 드루이드, 성기사, 수도사

![이미지 설명](https://wow.zamimg.com/images/wow/icons/large/spell_nature_bloodlust.jpg){: width="30" height="30"} 
&nbsp;&nbsp;**블러드** : 입구 ▶ 7번 (1넴 뒤) ▶ 15번 (막넴 앞 중보)

{% include video id="유튜브영상id" provider="youtube" %}
<br>
<br>

## 코드
```
여기에 코드 복붙
```
&nbsp; 띄워쓰기
`일리단` <!--글자강조-->

## 링크
[링크](https://community.algolia.com/jekyll-algolia/options.html)

[hodoUI](https://github.com/dsky3313/hodoUI/archive/refs/heads/main.zip){: .btn .btn--info} (GitHub)

{% include video id="0fkufq2pvow?start=506" provider="youtube" %} <!--유튜브 start=뒤에 숫자 입력하면 원하는 곳부터 재생-->

**Notice:** This is an important info notice.
{: .notice--primary}  

**Notice:** This is an important info notice.
{: .notice--warning}  


**Notice:** This is an important info notice.
{: .notice--success}  

[Text](#link){: .btn .btn--info}

<span style="color:red"> ■ 글씨색 변경 </span>  
<span style="color:#0b89ff">■ </span>
**<span style="color:#26beff">할말</span>**

내부전쟁 3시즌 전사 매크로
{: .text-center}

|기본값|왼쪽 정렬|가운데 정렬|오른쪽 정렬|
|---|:---|:---:|---:|
|내용 1|내용 2|내용 3|내용 4|
|내용 5|내용 6|내용 7|내용 8|
|내용 9|내용 10|내용 11|내용 12|

✅

bundle exec jekyll serve <!--vsc에서 로컬 테스트-->