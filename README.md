# 하고 싶은 프로젝트 : 스마트폰의 위치 기능을 이용한 사용자의 행동분석 어플

1. 이 어플을 활용할 수 있는 용도
* 로나와 같은 치명적인 바이러스 감염자의 경로 및 행동분석
* 이트 어플같은 곳에 기능을 추가하여 남자(여자)친구의 위치뿐 아니라 행동도 알 수 있다.
* 죄자들에게 이 어플을 깔게 하여 전자팔찌 대신 사용할 수도 있다.
--------------
2. 생각 하게 된 계기 
현재 코로나가 유행하고 있고 이에 따라 좀 더 편하게 확진자의 경로를 알아낼 수 있는 어플이 있었으면 좋겠다는 생각에서 시작했다. 
또 이번 수업시간에 배울 DNN을 이용하면 사용자의 위치로 행동을 예측하여 평소 행동들을 예측할 수 있을 것 같아서 기획하게 되었다.
--------------
3. 프로젝트를 위해 구현해야 할 것들 
* 어플에서 몇 분 ~ 시간 간격으로 사용자의 위치 추출
* 추출한 자료를 서버 또는 핸드폰 어플안에서 processing하여 행동 예측
* 분석한 행동들을 누적시키면서 그 사람의 평소 행동분석(파악)
* 추출한 위치에서의 예측 결과  및 행동 분석 결과 표시

```plantuml
@startuml Diagram

User -> Server: give position data
Server -> Server: Using position data, process behavior information
Server -> User: send result information

@enduml
```
