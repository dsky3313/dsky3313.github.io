---
# bundle exec jekyll serve
search: true
toc_sticky: true # 목차가 옆에 따라올지
# last_modified_at: # 2021-10-09 수정날짜

# published : false
date: 2025-09-01
title: "hodo UI &#124; 와우 내부전쟁 3시즌"
categories: # 카테고리 설정
  - WOWinfo # Plater, Weakauras, WOWinfo, Github
tags:
  - [UI]
toc: true # 목차 사용할지
toc_label: hodoUI
header:
  teaser: "/assets/img/wow/wowinfo/2025-09-01-hodoui-tww-s3/2.webp"
---

**주의!** 반드시 백업!
{: .notice--warning}  

## <span style="color:#0b89ff">■</span> UI 다운로드
[hodoUI](#https://github.com/dsky3313/hodoUI/archive/refs/heads/main.zip){: .btn .btn--info} (GitHub)

다음과 같은 파일이 있습니다.
```
hodo UI
├─ 편집모드 코드
├─ Font
├─ Interface
└─ WTF
```

## <span style="color:#0b89ff">■</span> UI 설치

<span style="color:#26beff">[1]</span> 와우 종료.
<br>

![이미지 설명](/assets/img/wow/wowinfo/2025-09-01-hodoui-tww-s3/install1.webp)  
<span style="color:#26beff">[2]</span> `Font`, `Interface` 폴더는 와우 설치폴더 (Program Files\World of Warcraft\_retail_) 에 붙여넣기.
<br>

![이미지 설명](/assets/img/wow/wowinfo/2025-09-01-hodoui-tww-s3/install2.webp)  
<span style="color:#26beff">[3]</span> `WTF`는 WTF\Account\본인계정(숫자#)SavedVariables 에 붙여넣기.  
<br>

<span style="color:#26beff">[4]</span> 와우 접속 > 채팅창에 '/reflux switch hodo' 입력.
<br>

## <span style="color:#0b89ff">■</span> WOW UI 편집모드 코드  

![이미지 설명](/assets/img/wow/wowinfo/2025-09-01-hodoui-tww-s3/1.webp)
![이미지 설명](/assets/img/wow/wowinfo/2025-09-01-hodoui-tww-s3/2.webp)
```  
1 43 0 0 0 4 4 UIParent 0.0 -291.0 -1 ##$%%/&('%)$+$,$ 0 1 0 1 7 MainMenuBar 0.0 -5.0 -1 ##$%%/&''%(#,$ 0 2 0 7 7 UIParent 0.0 4.0 -1 ##$$%/&$'%(#,$ 0 3 0 8 8 UIParent -430.0 4.0 -1 ##$$%/&$'%(#,$ 0 4 0 8 8 UIParent -430.0 34.0 -1 ##$$%/&$'%(#,# 0 5 0 8 8 UIParent -430.0 64.0 -1 ##$$%/&$'%(#,# 0 6 0 8 8 UIParent -430.0 94.0 -1 ##$$%/&$'%(#,# 0 7 0 7 7 UIParent -340.7 230.5 -1 ##$$%/&%'%(#,# 0 10 0 6 0 MultiBarBottomRight 0.0 4.0 -1 ##$$&%'% 0 11 0 6 0 MultiBarBottomRight 0.0 4.0 -1 ##$$&''%,# 0 12 0 6 0 MultiBarBottomRight 0.0 4.0 -1 ##$$&''% 1 -1 0 7 1 MainMenuBar 0.0 50.0 -1 ##$#%% 2 -1 0 2 2 UIParent -2.0 -2.0 -1 ##$#%( 3 0 0 2 0 MainMenuBar 15.0 25.0 -1 $#3# 3 1 0 0 2 MainMenuBar -15.0 25.0 -1 %#3# 3 2 0 0 2 TargetFrame -15.0 0.0 -1 %#&$3# 3 3 0 0 0 UIParent 299.0 -481.0 -1 '$(#)#-k.1/#1#3# 3 4 0 0 0 UIParent 82.0 -488.0 -1 ,$-#.1/#0#1#2( 3 5 0 2 2 UIParent -302.0 -284.5 -1 &$*#3# 3 6 0 2 2 UIParent -302.0 -284.5 -1 -#.#/#4& 3 7 0 2 8 PlayerFrameBottomManagedFramesContainer -11.0 0.0 -1 3# 4 -1 0 1 1 UIParent 0.0 -45.0 -1 # 5 -1 0 5 3 PlayerFrame 60.0 0.0 -1 # 6 0 0 2 0 MinimapCluster 0.0 -10.0 -1 ##$#%#&-(()( 6 1 0 0 6 BuffFrame 0.0 -25.0 -1 ##$#%#'-(()( 7 -1 0 6 0 ChatFrame1 -25.0 0.0 -1 # 8 -1 0 6 6 UIParent 34.0 33.0 -1 #'$#%%&\ 9 -1 0 4 4 UIParent -162.0 -193.0 -1 # 10 -1 0 6 0 FocusFrame 20.0 0.0 -1 # 11 -1 0 8 8 UIParent -2.0 320.0 -1 # 12 -1 0 2 8 MinimapCluster 0.0 -30.0 -1 #*$#%# 13 -1 0 8 8 UIParent 0.0 0.0 -1 ##$#%&&& 14 -1 0 8 8 UIParent -300.0 0.0 -1 #$$#%# 15 0 0 1 1 UIParent 1.0 -4.0 -1 # 15 1 0 1 7 MainStatusTrackingBarContainer 0.0 -4.0 -1 # 16 -1 0 4 4 UIParent -1.0 -3.0 -1 #( 17 -1 0 1 7 EncounterBar 0.0 -4.0 -1 ## 18 -1 0 8 2 MultiBarBottomRight 1.0 3.0 -1 ## 19 -1 0 1 1 UIParent 0.0 -216.0 -1 ## 20 0 0 2 0 MainStatusTrackingBarContainer -4.0 0.0 -1 ##$7%$&('%(-($)#+$,$-$ 20 1 0 0 6 EssentialCooldownViewer 0.0 -4.0 -1 ##$*%$&('%(-($)#+$,$-$ 20 2 0 0 2 UtilityCooldownViewer 4.0 0.0 -1 ##$$%$&('((-($)#+$,$-$ 20 3 0 7 7 UIParent -560.0 882.0 -1 #$$$%#&('%(-($)#*#+#,$-$
```  
<br>
<span style="color:#26beff">■</span> 적용 방법

상단 코드 복사 후, **<span style="color:#26beff">편집모드</span>** > 
**<span style="color:#26beff">가져오기</span>** > 
**<span style="color:#26beff">코드 붙여넣기 (Ctrl+V)</span>** > 
이름 지정 후, **<span style="color:#26beff">가져오기</span>**
<br>
<br>

## <span style="color:#0b89ff">■</span> Font (폰트)

[폰트 적용법 및 미리보기](https://dsky3313.github.io/wowinfo/font/)
<br>
<br>

## <span style="color:#0b89ff">■</span> Interface (애드온)

```
├─ Interface
 ├─ AddOns          (애드온)
 ├─ Raidframe       (레이드프레임 텍스쳐)
 ├─ Targetingframe  (기본 체력바 텍스쳐)
 └─ Tooltips        (말풍선 택스쳐)
```
<br>
<span style="color:#26beff">■</span> 프로필 수동입력 애드온
- Cell & Cell_UnitFrames ([프로필](https://dsky3313.github.io/wowinfo/cell/))
- Details [프로필](https://dsky3313.github.io/wowinfo/details/)
- MRT ([프로필](https://dsky3313.github.io/wowinfo/mrt/))
- OmniCD [(프로필)](https://dsky3313.github.io/wowinfo/omnicd/)
- Plater ([프로필](https://dsky3313.github.io/plater/plater-profile-tww-s3/))
<br>

<span style="color:#26beff">■</span> 그 외 애드온
- AdvancedInterfaceOptions
- BigWigs & LittleWigs
- BlizzHUDTweaks
- CauseseDB
- GTFO
- GuildMicroButton
- Hekili
- HidingBar
- idTip
- Leatrix_Plus
- MythicDungeonTools ([내부전쟁 3시즌](https://dsky3313.github.io/wowinfo/mdt-tww-s3/))
- Prat-3.0
- SharedMedia
- SharedMedia_MyMedia
- SoftInteractHUD
- WeakAuras
<br>
<br>

## <span style="color:#0b89ff">■</span> 위크오라
- [전사 직업 위크오라](https://dsky3313.github.io/weakauras/weakauras-warriror/)
- [전사 주문반사](https://dsky3313.github.io/weakauras/weakauras-spellreflect/)
- [쐐기 타이머](https://dsky3313.github.io/weakauras/m+timer-tww-s3/)
- [전투부활 & 블러드](https://dsky3313.github.io/weakauras/weakauras-blood/)
- [쐐기 오토마커](https://dsky3313.github.io/weakauras/automarker-tww-s3/)
- [말풍선 텍스쳐 및 글꼴 크기](https://dsky3313.github.io/wowinfo/chatbubble/)
<br>
<br>


## <span style="color:#0b89ff">■</span> 아이콘 팩
![alt text](https://raw.githubusercontent.com/AcidWeb/Clean-Icons-Mechagnome-Edition/refs/heads/master/docs/Merge.png)

[**Clean Icons - Mechagnome Edition**](https://github.com/AcidWeb/Clean-Icons-Mechagnome-Edition/releases)

**<span style="color:#26beff">■</span>** 설치 방법

- 압축해제 > World of Warcraft\_retail_\Interface 안에 붙여넣기
<br>
<br>