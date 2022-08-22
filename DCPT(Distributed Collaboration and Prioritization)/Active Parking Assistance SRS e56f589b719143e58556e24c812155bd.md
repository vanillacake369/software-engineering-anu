# Active Parking Assistance SRS

# Contents

# 실제 APA 예시

## 1. 벤츠

[https://www.youtube.com/watch?v=0LP-0RaNMqo](https://www.youtube.com/watch?v=0LP-0RaNMqo)

## 2. 포드

[https://www.youtube.com/watch?v=_-owU4tFczk](https://www.youtube.com/watch?v=_-owU4tFczk)

## 3. 현대

[https://www.youtube.com/watch?v=2mhRwhJA4Gs](https://www.youtube.com/watch?v=2mhRwhJA4Gs)

## 4. 삼성

[https://www.youtube.com/watch?v=WwdY-IDvkCw](https://www.youtube.com/watch?v=WwdY-IDvkCw)

## 공통된 작동과정

공통된 모듈 작동은 다음과 같다

- 상시로 파킹 area를 찾을지, APA를 On할 지
- 왼쪽에서 찾을 지, 오른쪽에서 찾을 지 선택
    - 벤츠는 자동이다. UI-Friendly
- 적당한 주차 공간을 찾으면 벨소리를 울린다
- APA를 시작할 것인지 묻는다
- 핸들을 떼면 APA가 시작한다.
- 브레이크를 통해 속도 감속을 조절하며 스티어링 휠 제한권을 가져간 소프트웨어가 자동차를 후진추가 및 평행주차를 실시한다.
    - 이 때 화면에 후면범퍼에 카메라를 통해 달려있는 후진주차 장면을 보여준다.
    - 후진주차 장면에는 장애물간의 거리를 보여주는 레이더 행렬이 나타난다.
    - 전진주차 장면에는 전진 제어 중인 전면 범퍼에 달려있는 카메라를 통해 전진 장면을 보여준다.
- 주차 완료 시 완료된 화면과 함께 기어를 P단으로 진행한다.

## Limitation

- 20,30km/h 이하로 달려야만 APA가 작동하게끔 제한을 걸어두었다.
- 핸들을 떼야지만 실행될 수 있게끔 하였다. 이는 급작스런 스티어링 휠 조작으로 사용자의 팔에 부상을 입히지 않게끔 하기 위함이다.
- 기어와 가속,브레이크,핸들에 대한 책임은 운전자 본인에 있도록 걸어두었다. ~~(사고 나도 회사 책임이 아니다 이 말이다)~~
- 최근에는 어떠한 방식으로 주차를 할 지 디스플레이에 표시 한 뒤, 가능한 방식을 터치하여 사용자가 직접 주차방식을 선택할 수 있게 되어있다.
    - 왼쪽으로
        - 후진이냐
        - 평행이냐
    - 오른쪽으로
        - 후진이냐
        - 평행이냐
- 옆에 장애물이 없더라도 라인에 맞춰 주차가 가능하다. 이는 카메라를 통해 장애물 인식 또한 하지만, 바닥에 있는 선 또한 본다는 것을 의미한다.

# Functional Requirements

## Power

- on
- off

## Display

- HMI
- APA on/off 여부
- 주차가능공간 유무 표시
- 전진 시, 전면 카메라
- 후진 시, 후면 카메라
- 장애물 위치 파악
- 시스템에 의한 핸들 조절 각도 표시

## Assist

- 센서 감지에 따른 자동 브레이크(긴급 브레이크)
- 핸들 돌아가는 각도에 따른 경로 예측
- 영상처리로 각도 뎁스 측정

## Camera

- 주차 장소 탐색 시 사용
- 장애물 인식

---

# Requirements Suggestion

## 1차

### 지훈

### 정흠

### 하빈

## 최종

- show path
- obstacle detect auto break
- auto parking on/off
- search parking area
- auto parking
- control restriction

---

# Presentation

1. 초기 동기 및 목적 설명 & 기능 제시 및 각 기능 별 설명
2. 1차 투표 
    1. 팀원 별 각 기능에 대한 Importance / Difficulty 정한 이유 설명
    2. 어떻게 회의 진행하여 합의하였는지
3. 1차 기능사항 수정
4. 2차 투표
    1. 팀원 별 각 기능에 대한 Importance / Difficulty 정한 이유 설명
    2. 어떻게 회의 진행하여 합의하였는지
5. 3차 투표
    1. 팀원 별 각 기능에 대한 Importance / Difficulty 정한 이유 설명
    2. 어떻게 회의 진행하여 합의하였는지
6. 결론 및 향후 방향성 제시

---

# DCPT Q&A

## overlap은 뭐야?

> An item is placed in the overlap column when the area of consensus of the item does not entirely within a bin area fall (there is a tolerance adjustment that we have set very high for the screenshot examples to avoid a cluttered display).
> 

합의가 bin area fall에 있지 않는다면 overlap 열에 아이템이 속하게된다고 이해했는데 bin area fall이 무엇인지 모르겠습니다. overlap 열은 무엇을 뜻하는 것인가요?

소프트웨어공학에서의 prioritization 정의

> Within software engineering the definition of prioritization translates into choosing an ordered partition of the requirements with respect to the tradeoffs and constraints of the project. In spirit this is an application of the classic “divide, order, and conquer” paradigm. The goal is to
minimize overall risk (through reduced complexity) by identifying classifications and an ordering that maximize satisfaction over all the stakeholders.
> 

# Bin Model 선정 기준

> The stakeholders must determine the ordering of the bins with respect to an individual project. For example, a-priori why should an item placed in bin II have higher priority over an item placed in bin III? It should not unless we prefer importance to difficulty.
> 

*The stakeholders must determine the ordering of the bins with respect to an individual project* 이 무슨 말을 하는지 잘 모르겠습니다. bin의 순서를 결정해야한다니...여러 model 중 하나의 model을 선정하여 진행하는 것 아닌가요?

# 아래와 같이 이해한 게 맞나요?

Average Bin Model

`각 영역에 대한 기준치 baseline 그림`

> This model provides independent baselines for importance and difficulty. The base is set by the average value whereby there are an approximately equal number of items above and below the baseline.
> 

Ratio Bin Model

`우선순위 > 구현난이도`

`다른 영역은 분자와 분모에서 중요도와 난이도의 0-3 표준 편차(허용되는 부분) 값을 더하고 빼서 결정합니다.`

> The ratio bin model partitions the grid into regions based on baselines where importance over
difficulty is a constant. The baseline is set where importance / difficulty = (average importance) / (average difficulty). The baseline is set where importance / difficulty = (average importance) / (average difficulty). The other regions are determined by adding and subtracting a value of 0-3 standard deviations (fractions allowed) of the importance and difficulty from the numerator and denominator respectively.
> 

Diagonal Bin Model

`우선순위와 구현난이도의 우선순위가 exchangeable함. 기준치 간의 간극, 차(difference), 즉 우선순위-구현난이도`

`다른 베이스는 중요도와 난이도의 0-3 표준 편차의 합을 플러스 또는 마이너스한 값으로 설정된다.`

> This model assumes that importance and difficulty are exchangeable in which the importance minus the difficulty is constant. The baseline is where importance - difficulty = average importance - average difficulty. The other bases are set at this value plus or minus the sum of 0-3 standard deviations of the importance and difficulty.This model can be interpreted as Net Value
> 

+) Diagonal Bin Model 마지막 줄에서 *This model can be interpreted as Net Value*에서 말하는 Net Value가 무엇인지 모르겠습니다.

---

# SRS Report Reference

## SRS of APA

1. [http://cse.msu.edu/~evenson6/cse435-project1/APA SRS.pdf](http://cse.msu.edu/~evenson6/cse435-project1/APA%20SRS.pdf)
2. [https://www.cse.msu.edu/~schmi703/Documents/SRSDocumentv2.pdf](https://www.cse.msu.edu/~schmi703/Documents/SRSDocumentv2.pdf)
3. [https://student.cs.uwaterloo.ca/~cs445/Winter2022/SRSs/SRS_AS.pdf](https://student.cs.uwaterloo.ca/~cs445/Winter2022/SRSs/SRS_AS.pdf)

## Template/Form of SRS

[https://web.cs.dal.ca/~hawkey/3130/srs_template-ieee.doc](https://web.cs.dal.ca/~hawkey/3130/srs_template-ieee.doc)

## **Jung-won Park,Daniel Port,Barry Boehm, “Supporting Distributed Collaborative Prioritization for WinWin Requirements Capture and Negotiations”**

[https://www.researchgate.net/publication/2466378_Supporting_Distributed_Collaborative_Prioritization_for_WinWin_Requirements_Capture_and_Negotiations](https://www.researchgate.net/publication/2466378_Supporting_Distributed_Collaborative_Prioritization_for_WinWin_Requirements_Capture_and_Negotiations)