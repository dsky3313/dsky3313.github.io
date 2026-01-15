---
# bundle exec jekyll serve
## <span style="color:#0b89ff">■ </span>생태지구 알다니
#**<span style="color:#26beff">■ </span>**123
search: true
# last_modified_at: # 2021-10-09 수정날짜

title: "함수와 변수 &#124; 와우 API"
categories: # 카테고리 설정
  - Coding # Plater, Weakauras, WOWinfo, Achievement, Coding,
tags:
  - [lua]
toc: true # 목차 사용할지
toc_label: 함수와 변수
header:
  teaser: ""
---

## <span style="color:#0b89ff">■ </span> 전역변수와 지역변수

변수란? 데이터 **<span style="color:#26beff">값</span>**에 이름을 붙여주는 것.

Lua에선 변수 선언시 기본적으로 전역변수 (Global Variable),  

`local`을 앞에 붙이면 지역변수 (Local Variable)이 된다.

|구분|전역변수 (Global Variable)|지역변수 (Local Variable)|
|:---|:---|:---|
|선언 방법|키워드 없이 선언|키워드 `local` 사용|
|유효범위|프로그램 어디서든 접근가능|선언된 블록(function, if, for 등)|
|속도|느림|빠름|
|안전성|이름 충돌 가능|좁은 범위에서만 사용하여 충돌 가능성 낮음|

<br>
<br>

## <span style="color:#0b89ff">■ </span> 함수

함수란? 데이터 **<span style="color:#26beff">동작</span>**에 이름을 붙여주는 것.
<br>
<br>

## <span style="color:#0b89ff">■ </span> 예시 매크로

```
/run local m=WorldMapFrame:GetMapID() local p=C_Map.GetPlayerMapPosition(m,"player") local n=C_Map.GetMapInfo(m).name print(format("[지도] %s (#%d)", n, m)) if p then print(format("[위치] %.2f, %.2f", p.x*100, p.y*100)) end
```
MapID와 내 좌표를 계산해서 출력하는 매크로이다.

보기 쉽게 가공하면,

```
/run 
local m = WorldMapFrame:GetMapID()
local p = C_Map.GetPlayerMapPosition(m, "player")
local n = C_Map.GetMapInfo(m).name

print(format("[지도] %s (#%d)", n, m))

if p then
    print(format("[위치] %.2f, %.2f", p.x*100, p.y*100))
end
```
<br>

`WorldMapFrame:GetMapID()`, `C_Map.GetPlayerMapPosition(m, "player")`, `C_Map.GetMapInfo(m).name` 에  

각각 `m`, `p`, `n` 이라는 변수를 할당했다.

이쟈부터 니 이름은 p여~

그리고 `format` 함수로 문장을 가공한 뒤, `print` 함수로 출력했다.


### **<span style="color:#26beff">■ </span>**format("[지도] %s (#%d)", n, m)
- %s : **String(문자)**이 들어갈 자리 (n)
- %d : **Digit(정수)**가 들어갈 자리 (m)
       나중에 TomTom애드온과 함께쓰기 위해 앞에 #을 붙였다.
- n : 지역 이름 `C_Map.GetMapInfo(m).name`
- m : 지도 번호 `WorldMapFrame:GetMapID()`

현재 위치 (혹은 보고있는 지도의 위치)의 이름과, MapID를 출력.
<br>

### **<span style="color:#26beff">■ </span>**if p then print(format("[위치] %.2f, %.2f", p.x*100, p.y*100))
- p : 좌표 데이터 `C_Map.GetPlayerMapPosition(m, "player")`
- %.2f : 소수점 2자리
- p.x*100 : p X값 X 100
- p.y*100 : p Y값 X 100

if then ... end 를 사용하여, 만약 좌표값이 있다면 소수점 2자리까지 출력한다.
<br>
<br>

![alt text](/assets/img/coding/lua/2026-01-15-function_local/1.webp)

결과물 스크린샷