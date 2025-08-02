---
search: true
toc: true # 목차 사용할지
toc_sticky: true # 목차가 옆에 따라올지

date: 2025-08-01
last_modified_at: # 2021-10-09 수정날짜

title: "와우 내부전쟁 파티탈퇴 매크로"
excerpt: "와우 내부전쟁 파티탈퇴 매크로"

categories: # 카테고리 설정
  - WOW Data
# tags:
#   - [tag1, tag2]

permalink: /wowdata/party-leave-macro

# toc_label: 포스팅 목차 # 목차 제목
---

## 와우 내부전쟁 파티탈퇴 매크로

![이미지 설명](/assets/img/wow/wowdata/2025-08-01-partyleave/1.webp)

```  
/run C_PartyInfo.InviteUnit("일리단");C_Timer.After(0.1,function()C_PartyInfo.LeaveParty()end)
```  

탈것, 형변, 애완동물 등을 수집할 때 유용한 파티탈퇴 매크로입니다.  

특히 구 확장팩의 공격대나 던전은 길이가 길고 입구로 바로 보내주지 않는 경우도 있어

이 매크로가 매우 유용합니다.

## 파티탈퇴 매크로 사용 모습

![이미지 설명](/assets/img/wow/wowdata/2025-08-01-partyleave/2.webp)

매크로 실행 시, `일리단` 이라는 플레이어를 파티에 초대하고 플레이어는 파티탈퇴를 실행합니다.

![이미지 설명](/assets/img/wow/wowdata/2025-08-01-partyleave/3.webp)

잠시 뒤, 알림창이 뜨며 인스턴스 밖으로 나가게 됩니다.

[수집가의 은혜](https://www.wowhead.com/ko/guide/world-events/collectors-bounty-guide-mounts-rewards) 같은 이벤트 기간에 사용하기 유용합니다.