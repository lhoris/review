## Chris Richardson Interview
### 영상 소스(자바 챔피언 크리스 리처드슨이 말하는 마이크로서비스 아키텍처 | 김용욱 | 마이크로서비스 아키텍처 구축 가이드)
https://youtu.be/8BJUrHNFACA?si=rbuFfcrPdu28QifA

### 영상에서 주목할 만한 내용이라고 언급
- 한국은 프로젝트 위주의 개발 스타일이 많은 것 같다.
- 서비스 간의 DB를 분리하지 않으면 MSA가 아니다. 모놀리스 단점에 MSA 단점을 추가하는 것이다.
- 서비스를 너무 작게 많이 만드는 것은 좋지 않다.
- MSA에 이벤트 소싱이 꼭 필요하진 않다.
- 빅뱅 전환은 완료까지 가치를 제공하지 못하고, 개발자에게 큰 스트레스를 준다.

### 내가 생각하는 킬링 포인트
- 마이크로서비스로 분리하는 것을 암흑에너지, 암흑물질로 표현
- ACID를 보상 트랜잭션 대체할 수 있냐는 질문의 대답 -> 현실세계가 작동하는 방식
- 스타벅스는 2단계 커밋을 사용하지 않는다.
  + https://www.enterpriseintegrationpatterns.com/docs/IEEE_Software_Design_2PC.pdf
    - 스타벅스는 당신이 커피를 받을 때까지 문을 잠그지 않습니다. 커피 구매를 ACID 트랜잭션에 비유한다면, 커피를 전부 마실 때까지 나가지 못하게 할 것입니다.
- 어셈블리지 소개: 마이크로서비스 아키텍처 정의 프로세스
- ChatGPT가 어셈블리지를 배워 마이크로서비스 아키텍처 정의를 할 수 있을까요? -> ChatGPT를 AI라고 불러야 하는지도 모르겠습니다. 본질적으로는 텍스트 생성 알고리즘이기 때문입니다.(사실 여부에 대한 논란의 여지가 끊임없을 것이다.) Copilot의 코드 생성 같은 개발자 지향 AI 도구라면 가능할 것 같은데 서비스를 정의하는 건 회의적이다.
- 주니어 개발자와 숙련된 개발자 사이에 큰 차이점: 추상화를 식별하는 능력
- 마이크로서비스 패턴 책 2판을 준비한다면? -> 쿠버네티스에 대한 장을 추가하려고 생각(쿠버네티스는 이제 개발자들에게 필수인듯), 테스트컨테이너에도 관심, 이벤트소싱에 대해선 관심이 적어짐(MSA의 핵심은 아니라고 판단)
- 요약: 상황에 따라 다르다
- 트러블슈팅에 JIRA이슈 재할당을 반복하는 끔직한 사례
  + Steve Yegge의 구글 플랫폼 비판
    - https://gist.github.com/chitchcock/1281611
    - https://channy.creation.net/articles/google-platforms-rant-stevey-yegge
    - https://subokim.wordpress.com/2011/11/01/amazon-story/
  + 구글을 떠나고 Grab에 합류한 이유(인터뷰에선 Uber라고 하는데 착각한 듯)
    - https://steve-yegge.medium.com/why-i-left-google-to-join-grab-86dfffc0be84