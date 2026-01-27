---
# bundle exec jekyll serve
## <span style="color:#0b89ff">■ </span>생태지구 알다니
#**<span style="color:#26beff">■ </span>**123
search: true
# last_modified_at: # 2021-10-09 수정날짜

title: "애드온 로딩속도 최적화 &#124; 와우 API"
categories: # 카테고리 설정
  - Coding # Plater, Weakauras, WOWinfo, Achievement, Coding,
tags:
  - [lua]
toc: true # 목차 사용할지
toc_label: 애드온 로딩속도 최적화
header:
  teaser: "/assets/img/coding/github.webp"
---

## <span style="color:#0b89ff">■ </span> 이벤트 실행 순서

1. `ADDON_LOADED`
- 애드온 파일 및 설정값(SavedVariables) 로드 완료.
<br>

2. `PLAYER_LOGIN`
- 모든 애드온 로드 후.
- 게임접속, `/reload` 후 딱 한번 실행
<br>


3. `PLAYER_ENTERING_WORLD`
- 애드온 로드 -> 월드 데이터 로드 완료 직전.
- 지역이동 (인스입장, 포탈, 대륙이동) 할 떄마다 실행.
<br>
<br>

**<span style="color:#26beff">■ </span>** 최적화를 위해 무거운 코드는 `PLAYER_LOGIN`를 사용하고,  
&nbsp; &nbsp; &nbsp;`C_Timer.After` 등으로 작업 시간을 미룬다.


bundle exec jekyll serve <!--vsc에서 로컬 테스트-->