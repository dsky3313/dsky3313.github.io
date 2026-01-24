---
# bundle exec jekyll serve
search: true
# last_modified_at: # 2021-10-09 수정날짜

# published : false
date: 2025-09-01
title: "hodo UI &#124; 와우 내부전쟁 3시즌"
categories: # 카테고리 설정
  - UI # Plater, Weakauras, WOWinfo, Github
toc: true # 목차 사용할지
toc_label: hodoUI
header:
  teaser: "/assets/img/wow/wowinfo/2025-09-01-hodoui-tww-s3/2.webp"
---

**주의!** 반드시 백업!
{: .notice--warning}  

## <span style="color:#0b89ff">■</span> UI 다운로드
[hodoUI](https://github.com/dsky3313/hodoUI/archive/refs/heads/main.zip){: .btn .btn--info} (GitHub)

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

[▶ 폰트 적용법 및 미리보기](https://dsky3313.github.io/wowinfo/font/)
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


## <span style="color:#0b89ff">■</span> ElvUI 프로필
```
!E1!T3ZYYjoww(Tml6D4oKecmoxmra24eIWgCd4kRS7OWLaUyuBHeT0fNPRfvmlNiM)IztVCwnrmFpZ26NyoN7lDL0vpWPZOYP7CJFiDFCUN3V4Ys7LlwoFJh1BLxCc(3hi0HF(aj2NeUMGpGe6TkGSC1s6Y50DXepA(NsYmEk5Z0RJI3dJB(DdND5Wj6dF(F7ijHEz0(dbekzZ0WGxwoy58p5VHUB5exhRLZ3gfctfaIyssYN8EH)KPhPb(HKLZNE)IBgpz4Y5r4Es9O(rHlNpA6SX)5Ptw0)MLZ3r8FChD5eCXs2f9PBiptcGDbw1DrHrX5H)yYHJI1zrUL9hgoBX4lXfTiuj3g7oUQdGTdUGE)cGpO5XEWlEKesI9cWx4T9Pl3b4iaLSHS2FVxWnKWhX1WIHKosMdaXrgnjzThSgtS(JTzNb)nKHXXrXxh7TNHtxffEmz6Q)kzn1)zYDrj(COV)9lMYH850xGvy(8r9VA6huyqVJ0OzKdE(XlN)(7hFZvaSCm2BLFGp9L5YnTda3WgDlj8O6zxa0zVGN8dFCeXBddqg4T(PnXrhqY5QiknA)DEHaEhHpXR26bh1OaofWdWwWRwEDNUDS7CExhlNl61X9CNLBpRdUNL(M4YEdGCIKybgmnsqI6AbivVnBIcropVy6EGeJabIlraoX)xiCggJ8AWchefrNffWODjmkZaV4faV(XyyG36hIKq)ek(wgUE7XGaqOcoIhbKr4C(o4aV)G3AaXTCsBfBtBxlMGu4opqkAZDpF4wGlZ7rscI(cIE0pCp)b4)dSo4VE8OFWMbEHpHG06OJHGyxEEuGlCpJ9VMxvu6sTGMqgscQIycKr3oo2oDTT6Ebqx601cjjTzKXsEtCzVb2GNj78xhqMdABghUXFThnkMJb7ccBhI9F2Js6d8Qm5d)1Cr3e5iOfzf6d86JqQ9QISUk26EC6pBrjOigQmJPuOa(jvJgFxT7MzpRCskgoU6cMkXeG9jW8Skm2YHk9HkoLuFAGzWrTCLoc56Hy05798dwfT5LYwR1rrbBI(uyn4lniRSJbJ8vuHRxa9UOprIbbVmsH5f)ep(sK589XEBq95ioVWkIa9Xeqt17dI(eUKhtiSzHJUGIk8NpY(zm(tgqk4eN55V5dEXHOyDQ(Abv4X7pSHngQuDQs0JzVmII6(Rxgn7RaZTGYcA)vRIjpJSHzglxwX2k)YR0cH0tgs7acdbrRzg8q9zOvIPFi9zAlhE0jje6FokAVMXnMLvugKj3SXF7w)1hdOmgLppD7wygm0MYm25lN)I85NzZvOqbEWT(KGnzMLL2iH)(GY02GPlwm92BgE9cgvew4WnC2c1CDu7OT(mNn(9Jwi5NZmHZC02nhUNmCT7WizG56yVTubrwFFmdJsOJgdQlZplBDOtB(4Ue4LKmsOoif6C1WGD1XGc9DcByow8)DF0ZeUlDddEU)GhaDBlMEhctTGhC)478Ib5IwYNz36m3ETzd((RFazOBFlUcPZQWuCBDwB0W6cV4hjkrtXS4eO0jj(FNlUOLdQ9FqusYaMLrDIz(XZEwxRoW8GJ8nGnyMc7uildu1YQ1z9aMR)CuiPp3lgfGOFMLWsBRw2UD1pZG3VzG)cOlThB3YTnGuLN7lb5epqnwniGZCC71Yf0Oo)hsTX1490158w2cKNxy6Mzct44OiNCke)N1rFoVvBRoiUojbpsXrbzNHbe5z2T6yb49)uQBRPWftEldWXFcaF9y)avFJ2Ax4VNeBRDGYXMINjWfbnQLDt5q5saUvlbad22gqz9dYZlxcWGoZLcmonayaUFqbKkCJ8slCetreSaH5A5Ge)(58JnpQohKkMCBa5bS6xTG5v(V9F9)8B)h)7)2F))UztgbDhy2dMmCrZ5v5c6Gp2BP9huUab4iFR2a3tF4PEOpz6C1LY90(IUWp6CoNemEG3JNeQSvxBjBX51QySd4q18zyOeyiBNY(y3sTn2DQueY5cqjxBKfn6WLWlifuOucx45krI7c8EbMMxcDvE1Wg2rRwTX4DUHST4PQuvXUTai893Ec8aT72oJaE7Qpnx0JPgjH(bp66D5u2xflQTdkr2wHmUoATsluJivDqRmDa5ZHpdVBreGgRq5QT954XADC0kD1eLk5dOT7hZIApjVfmdyb2QNMgMA1eLYK5wdy4K1KqTCjoUUCScs86hqIZyaUrmaO1eg1WOhc1qv621QvNE5yXRfQptb2tZee4PYkDNwGMvB30cSPFUIkuTCNJDB5iDQ3KKlCkgqGau4b5CWGAH6uDFUBwQEtvrWWIU2kvSHpzG0vM0u3wOlBxPYNur(gJBPLlQYutHHtnQ)UqIlB3e4c9)0voJovrovoODdX7zsdDvTZ59A5GMwwabdt9p0y8fkN0vX)0Uw2IZb9KGnVtsdNRDxMZJhHahAgZJt72mvx)W0Xxo8Yr9xunC50UlB43rQYGFxBWOaIHIFChWiE5Ui)1Kfrp(iM1SQKB60r5kx3QhPn6yUaxAvR5DxNoYrFr9dgZ2l6)DJ9uHHvC61rPd7eIXWfrwoikLBB3eUQ4XVD3luBg4K4l1k1DMt3ZB1Th67Bon8Li15ybAUUIS6ezLSrhCe6XAaMJz3KLzPqyS07yjeftVmW4NjPNZLP9QQmMKCaudHt7tEXR8c3WQ7a)pT7kw22IF7Q)Yo4)CGraeV2w)1UIh6i(DhXVNlZZRD6yBlswcaLJd3gzo1RjhiR99cOVWYfvszj3XrTSFGNf5Zr7Kyo9fmil0ZrmMZXOJbd8Hd(kjmur(FHdGyzDrXU)6XWNgJPzDqP5AMg7fMCGrdz72bFmavT8YAXZSB4gwA5EjjtkKM7J(8(SxaMEdroHEuMPpEMnABkPGYurRJTvzyxKofIxmeLD86DtdVmikHK5qy6Oh(Kirz9YsRsZdgogj(XYfZ2si5fzzVU((BUrrC4Zbz8XArH4)fVCGFI1w5CSQRJ9oiq3uKMks09gUeh(N7II9)f0vGa9to7u9r9CybMq)OwU24J4h1ZcLc(WXQ)MsOZjeWVuWROPFkKLWlSQol2bVExuWg(MGRuXjwbkxoHuwBdY2Ooa)16hyN0zwCn3795paOXerIyvyodRCzC05rEgoQfW4N(PuhNx(XHY9OOF4AG0)JCkMbMG6Wt5OLsIplLHhd9PBzfveZlnZvXPH3gDmHCfMxFrk0fqFBKPFJ)wFrwg7Fd8JbbG4ilp8ILlHVu8IuPxdGvGj0CS05jmwC4BkCEIXk3WQp3JXrFIU7hfzxvl9OfOf65ogEPhdXDxKpIdeg0ZtaCW6FdEE(PLt6ukxXHyFaTZsTO8026d7aHz2FDhGoIc9cAD5Lc7Jsy(JGfZPFyIyDtRsR0EhIv24NGOiw4sSIsmqtBgyLIXfRQiwEC6ocy1yhRMfuQ36Dy68xeb6Jy0uw(SFyRqhfVcaB2eqUmWF9tSDKzNddsJPGru7uuXfOAN61pCJQOfmUK5Shdg0hE147VLx9ew5ueVGP7k7MYmpnIx0vQS6liyYyaU546NEbuK(Webpy2JXi(XtZMrMf)VeiM(7cHP)UaW3YZcJyLX5NYMI(Iwr(RaG4V9LrYYduslhKYT1oBT2uq(Ds0xwqN)46HCg2)Dap4AWk6zNkSJ9AXWz1c8wky3odSp6UVaCoN3tc6)0V(Z)V)B)N)6p)xepE9Xy0VG3bkoJPGr(JKt4yXLuR5qLLGiegUlMaIkYo7i9m4TkjkELOPi(WS(3D3WRW5ikhVdQ6rikYJywklIga4UKSpks0Sg79d7hCyNhV4Eixnp8AMknodUu3BgGivx6fMRnP4SHZMxCkSgB9zKhYgK4iIJxxo6vSnQ(yXOKUsOw2fnMfZLWkwarMAuH6TK3hhD8q(kFLR6Fk0UnN96szPxzfAvu0vwbyP6amMzItZ4rdTwCgo73Cldx5do2heG0LwybdyXHZcw6uSqeAu1yzA4JH9jB3ryBLh9lg2bcnN9yWbkm9nmyyI1jDQXZNW8N(5gx(epkUOctwSADkewk2Pzcj0jtrr9MFYZzjaybEHP4j1Ca1KxszrxITjsd9NT6TkN4KJKNRXuDMAEFqlZH9yn8DrDGQ2Va7QH1mFOslVSuB)NZW2MTuYPQh7LttGAC9yCvh3Zeuzoll4gVYpMSwRM5pW5nn5IcaWOc(10XfqEcmN4KW2mqxzcjJtmz8nJRUpjT9ZOgC7XG4EjSN575MUsgEi8nYCGRajfRWZG3MxanRRFsEimxvFLKOYtPm9siSWZIciJLTdrIwVfLJHq5TwbXwHcXlWwy44Ei2YgHxnAXsXDzsmDXXyAaHPi61AYmwCyZcDcPYC9cHjxqCW2pDV3JaQCvoUxQmiKC6LAoTxfSGaBL20wfu(NrXKsxpt8UzboKxBjisblbxGYeUxfOWKOq5FxUMFDC7S(3YA4QcUVVQHoOuGjvhVSFLhv4HEogwvAiYAy1klDvI66vgMBRFafDgE0WBU767Vrh7KvwQGMMvg00OpHIkwYQfjtR9kiJn3xTADpRoVWYVa8XRC2jx(ZuUzP3yTAnCjCOSyTjR4pIf)bvmQjrJXmQfF8aTztqTply98gOX6cX06AlMwNUIP1rKXaWc6txQ1OCQjzNRx5k4GOYRtNu))Ww1aZtXIOrS8RWAwUg4q4LmMwtCeilBZ8U4WZhKlqQk7ovQvCv5AfpuzyGFjXtx0(Vet2lxRSL1LiqS8WHFsIRzjvGSrZwdd5NAskDL6yyL2DG5cL0Jm1GlmwCeqSG)RqKGCv5VZJ1WI8ab)jtDlN840UJjV7BQ(DLcCRYudvPo5qDDYz1cQ7Jy2U7hFJddAlXPwGhJ9k)T(8ER0VSm5yGbvf1J13k(UMIT19In1N1I(ZQ5l2xQ)SoL5pRDBJM409dRkJCF1DVfOiVHE3Q7tBvEILsXRYNmnpXsjvzPafDtoLGB2Hz8atR0D3VuFCBKtpAH409npyYxHNZWSqvbjf(4ujcepv6scRfWBkvcDnQXqZ3g91VSKU()NtDP5egliN1d6GDjejFMx4MZ25D4aS7jjFnH(sZrzzoui47zfJblCUK1xy9UN1BFM7ZMQ(uXxgPDKelX5PAKeOb3Vl3yQOE7lYe5NEmvvhUF9H4viaUsd9spyWIAMPNusSEBDZSHoG1y3SYhK5PKYpZ(oP7hwwdTaMWOsTxzWPNCWILvjnvf3n5ah2nnLw(TFpJL0CGygcxQMOonf6yCHqhxLl0XAhv5bZAmQtzmMPrDkJdLQJTYhlPt6hexNoUVUyj1dhQOZgRkngjUIp2NI6cgAermzkjILh66msI5KCivZ)gPBx3CrUI1QVTvh2d7Jr(xLWEEZDutO27nikQmDxqjXrPxK4tjkQgvlaD3tYg1uHOQOFp2PxDStFzzXUMclKswleXKXcm8nuyuUV24EyMrXbBkP(zPrLv1yZfNmt5An4Js(sWQ6qhPBkolZLCB(hmFSZ94DGlZnKVg65EDkMkK3Ru2Pm9QswoY6lfz6cAYzJcki01eMrbb1qXeXYi(GaWnPXOYS4RXq0zPH6gY3WJhga09ztVzywrBZ4K25K94s5PYZvl1vu8UcfifZXLJoYolzQqaDG63OWGxqBl8wrwNNQgPFn7dDKSjoSURwE1LGT5BZub8Le1rdd4LkR9NXkaQFUtXELQV8e1qvxW2ngrP7xQHGFnMxhbUJwLhxO36ELP)83ZMNS8qOFt6zYIMh0cPFqrBcPDStzM8szEQTZlp1MRSrCivBYiL(4ALvM1yNB(8b4eVMPby1jfn637cnn9GnTl0(EVR(TucG)h9ExT2cn)gL03kBxB92J1pCBe)c(sBZ5xcsnpKDHkWfX(HpXnYZXdU26Qe(62NN1hiX3e99zd7KZTmRbv6AqVsphPwdRj351IZAuU0pDNc0Y)pfnScXrIF2St3ORV5(Xx9WG7V(65pmDYdxnK9NLy8VC)VY1LcuJUVL2JhAjtlffQjqUHWTw(H0ClsRk1FvxlpKlGtjrVcQZA8Rpf0ACdNyYOry6h1yEKry0ZUOjA0)AiY6PHc9dsL26Nleg0ZLRtJmq)AkOsnE(BBP76Vwu3niiamW(txKmNh7fKl1LNQYHDH4xbb1s7AX21jFwLATsf)tdlvkAspXuB4QRE31jxkifRw7CAaByNS30Mt)lkrpn364)qLq7tSTGEZtTDpjVX3Mz2(nUP3BAQT)k2wqMBgiL)mvKrnJgRpHKB3OiVBSl2LCzuUM)zZFH8KWuiGak3yj)HR0Q2j)j3Ee)q8g4tyL488oMae0WdhyyRpVBAJ5iAuNI3Hde21KOHEYL7vYdR0QQA9D(RayFHfCdsLXpXVabDqbWxTWpSbEpF1VUJB7l66cXn3PJvx7Z7I3IRU8lWxZVjUS3qlSp1EauEHDB)j9vJ(IZ16)ybEdDH6sTlS2ZT666c)Ot3296y54QaB(0k59ur0uYRmuAkx6cHfdUQ)9E(HYhRKAWNNX3cb)F(lryfaBOlU54HLQoRovsQAkn3XWgJzP5cBn3Dhn)AwL5PP9zlI(S)9Jp7rw0wP3cS48nxntkNlpMFH8Y2m8siNkZMsye37ywgUy(QlEWi2TgYGYcPMFpIQIlvE5MDfS2YhIuxMRpmFCWDwDZUv5WqEn8DjnCH1tmnoIfQgTyn7kpNdQyXkK3ihIlgLIRN5fq3pJMCeoDasDlbkwSRXGG2WB)Q3J3SiSfMhXGR4p0SquybnPif(ppMMpHFwWVyEVLZwh(PkGFpAR5PXEV1XLChQWflNrO4n4elCSi6t4n0HrUg2kNarCot6lTAPvBFjwA1VDVXR1i1ennSeXIlvbWSxixxt3GfWAHEiM6kD6Dde6FE0wy9HN)No6XUStxKR2hQZS6uWFeUMzUylu70h1CbmD6zplSbJIQCfAmR(ZjbBXqprunqc7zMewle)6OO5TmxlHclitjeQxp5Oi)zv8CfzWkH0yGiQtams6O6XYmn8sPo5k0BgFX3jz)otYwVdXx6elGSyBGSWU7vkamVocrTAd7AcnvcbJD)PdVr7sux9FsVxOLsh5afdjT6nGQQsxqTSWnNmwPkXIu0TbVeDKMZ4q5ao7iNxlmYd05RRfrtKHmBehzTjJ5Q8PaVPQjmG4YSxVn0Dh3gilxL8iRNFEp4GAkQkpdcLtCkXDLMJr(cOvnqXzfoL8fJQ)grXjqfUJqntgkJFnxRmuHkUY0qAIrRmjPIRrjyG8UIAzePOIHBL443TeReFD0qu0crrkC9QmkySOHCTVvMjmBB6vqZmqGAMWVrozGK)nT(K)jWrmYF7OpMJTXuYE2We3Z3PyCgFDMW4kEcGxYZZ8kJb(I06Z)oP(3zsDyeR9wuQbk5BDmrsln(gQieywXb0Ib25BBI7)e4xqUpBtOYv3Vtu(DMOauHVYHZuAiTFjP2ZQuct98oVnP7ZqwknqckHyzIyukJQozKQ(Y4B4N9PIRb)f15ZBtywQGGrZvf3Fb)cDILL4uaaVwNf3pYWMf7L)91ciL5FxjazoPX0DpH6X)o6yz(yq7j))rAncUbUCD(J6HVtd3MbSrtv6Fl9PxcguWSmTJ8GL0zglke96KvnkXvOzc2KXt)xL6tTqM(cKbnGQRv8Vu52tviT6SyWkVc2Oihc8OKY(qeMw1UpgD8x)5(XKF9Nhq8os93Em4FHz0KFptJZhVGYzHOX4SXlDF2bYpeVH6zLAAOQKs7FHcAjY(SDSVIekslWuRClBDxvwcPXTwIpvvFoZx8JPeORgpV)GBgELPdS5vx20mDZQNbMRxamTeaP)PzWwUxMX8SlkNFgV62ZEknTrY3X3dK4JnKbNle85u1ucxKx4C3U971Jo1wVI2)rMBNjei(InjzhfvIF3mt8XIquGg2yLhi9pgngpJP4f72vwjykVlNexj6wsSd2xMm(I9jjLDmyaloaT7uDBh(vQa(DJ8ImGb21FERktdZQ5KaGPKSbLFQVm)uEhfctC)b512)Fy07(d3(R)mG69tOrXVi0IJ98hIrhXFkUSJNmFr)jxoepGFC4n3G)Ew)XxH)M)fPm8hdVD6c2iM3)J4VUCu)jtgYg7D9NT4JI4c9KFN0kobaGl6umYgWGB0N1((CEW0Fy4d8VhwWV5IXc(Y)UEiPqPDYvUE)qSkRpdItSVuD44zEDGzDL6m5LlLLKTGxV9zKd4343ReJv1riZhn(QHGMXrWl8d)b8RLKbcNSqwBvVNwjPpTgvSfqgTmg58GfEpY(KumG1tIZb9CbbQVuKzTLncpAx5bx3Z1Q752TDB72TDxNlSeFBrJSaTbga3lWwo5cRZ7WIBJ1GiL9M4YEdYV695BamCc(5aZIX7hHL5EC6xFfcyJB0FM2xs4g68nGeVk6ZJ0z46O4ZZjrIF5d4Tkzs0anBzABfGwWpAAbBFuHjtjW8VhpqJelF37qBw(bK39UDrBI()(d
```
엘브를 사용하진 않지만 전에 만들던거 백업
<br>
<br>


## <span style="color:#0b89ff">■</span> 아이콘 팩
![alt text](https://raw.githubusercontent.com/AcidWeb/Clean-Icons-Mechagnome-Edition/refs/heads/master/docs/Merge.png)

[**Clean Icons - Mechagnome Edition**](https://github.com/AcidWeb/Clean-Icons-Mechagnome-Edition/releases)

**<span style="color:#26beff">■</span>** 설치 방법

- 압축해제 > World of Warcraft\_retail_\Interface 안에 붙여넣기
<br>
<br>