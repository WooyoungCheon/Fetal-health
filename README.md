## 분만 감시 장치(CTG)를 이용한 태아 건강 상태 분류

<h3>연구 목적</h3>

CTG(CardioTocogram) 데이터를 활용하여 태아의 건강 상태(fetal_health)를 3단계로 예측하는 분류 모델을 개발하여
분만 전 태아의 건강 상태를 평가하여 적절한 치료를 제공하고,
바쁜 의료 환경에서 의료 사고가 발생할 위험을 줄이고자 한다.


<h3>Data Set</h3>

2126명의 CTG 데이터 (fetal_health.csv)
(Reference: https://www.kaggle.com/datasets/andrewmvd/fetal-health-classification/data)

22개의 정보로 구성
 - Baseline value: 태아 심박수
 - Acceleration: 심박수가 증가하는 횟수
 - Abnormal short term variability: 비정상적인 단기 변화
 - Mean value of short term variabiltiy: 단기 변화의 평균값
 - Percentage of time with abnormal long term variabiltiy: 비정상적인 장기 변화가 전체 측정시간에서 차지하는 비율
 - Fetal health: 1(normal), 2(suspect), 3(pathological)
 - 외 17개 정보


<h3>연구 기간</h3>

2024.07.24 - 2024.07.26

<h3>팀 내 역할</h3>
이상치 확인, ML model(Random forest, Gradient boosting, XGBoost) 구성, 최종 발표

<h3>연구 결과</h3>

Accuracy 기준 DNN(0.923), Random forest(0.951), Gradient Boosting(0.967), XGBoost(0.960)로 Gradient boosting이 가장 정확했음.
