---
# bundle exec jekyll serve
## <span style="color:#0b89ff">■ </span>생태지구 알다니
#**<span style="color:#26beff">■ </span>**123
search: true
lastmod: 2026-01-27 00:00:00
sitemap: 
    changefreq : weekly
    priority : 0.5

title: "말풍선 & 글꼴변경 &#124; 와우 한밤 애드온"
categories: # 카테고리 설정
  - Coding # Plater, Weakauras, WOWinfo, Achievement, Coding,
tags:
  - [lua]
toc: true # 목차 사용할지
toc_label: 말풍선 & 글꼴
header:
  teaser: "/_posts/coding/dodoLogo-teaser.webp"
---

'**Gemini**'로 제작했습니다. (한밤 12.0.0 기준)
{: .notice--warning}  

## <span style="color:#0b89ff">■ </span> 원본 위크오라

[adjust Chat Bubble Font](https://wago.io/AMt_WQ2Zk) (Wago)
<br>

## <span style="color:#0b89ff">■ </span> 다운로드

[dodo](https://github.com/dsky3313/dodo/archive/refs/heads/main.zip){: .btn .btn--info} (GitHub)
<br>

## <span style="color:#0b89ff">■ </span> 설명

![alt text](/_posts/coding/2026-01-27-dodo-chatbubble/chatbubble1.webp)

말풍선 배경과 폰트를 변경합니다.

예전에 사용하던 말풍선 위크오라를 애드온으로 만들었습니다. ([링크](https://dsky3313.github.io/coding/dodo-chatbubble/))

[말풍선 텍스쳐 다운로드](https://downgit.github.io/#/home?url=https://github.com/dsky3313/hodoUI/tree/main/Interface/Tooltips){: .btn .btn--info} (GitHub)  

```
World of Warcraft
 └─ _retail_
  ├─ AddOns
  ├─ Raidframe
  ├─ Targetingframe
  └─ Tooltips        (말풍선 택스쳐)
    ├─ ChatBubble.blp
    └─ ChatBubbleVertical.blp
```
`Interface` 폴더 안에 `Tooltips` 폴더를 만들고
`ChatBubble.blp`, `ChatBubbleVertical.blp`를 넣어준 뒤, 와우 실행.
<br>
<br>

## <span style="color:#0b89ff">■ </span> 설정법

![alt text](/_posts/coding/2026-01-27-dodo-chatbubble/chatbubble2.webp)

설정창 (`/dd`) 에서 글꼴과 크기를 조절할 수 있습니다.

글꼴은 기본 글꼴 중에서 변경할 수 있고, 글꼴 추가는 아래 글을 참고해주세요.

[와우 글꼴 변경 및 추천 | 와우 내부전쟁 3시즌](https://dsky3313.github.io/wowinfo/font/)
<br>
<br>

## <span style="color:#0b89ff">■ </span> 추가예정

- `ChatBubble.blp`, `ChatBubbleVertical.blp`를 따로 넣지않고, 인게임 내에서 변경하기.