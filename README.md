**<분만 감시 장치(CTG)를 이용한 태아 건강 상태 분류>**


**연구 동기**

퇴행성 관절염(Osteoarthritis)은 뼈의 과증식, 윤활액 염증, 연골하 경화증, 관절 사이 좁아짐 등을 동반하는, 관절연골에서 발생하는 모든 퇴행성 질환을 일컫는다.
퇴행성 관절염은 전 세계 약 3억 명이 앓고 있는 흔한 노인성 질병 중 하나이며, 기대수명이 증가함에 따라 유병률과 발생률이 크게 늘고 있다.
이에 대한 진단은 병력 청취와 X-ray 검진을 통해 이루어지지만, 초기 관절염을 진단하기 어렵다는 단점이 있다.
뼈와 같이 큰 조직의 구조만을 감별할 수 있는 X-ray의 특성상 cartilage나 meniscus와 같은 연부조직의 구조를 파악하는 데는 기술적 한계가 있다.
그러나 PET이나 Bone scan과 같은 핵의학 영상은 다른 영상의학 기기보다 민감도가 훨씬 뛰어난데,
병변의 생리학적 변화로 인한 방사성 표지자의 흡수 변화를 통해 병변의 위치를 알아내기 때문에 이러한 문제를 극복할 수 있다.


**연구 목적**
CTG(CardioTocogram) 데이터를 활용하여 태아의 건강 상태(fetal_health)를 3단계*로 예측하는 분류 모델을 개발하여
분만 전 태아의 건강 상태를 평가하여 적절한 치료를 제공하고,
바쁜 의료 환경에서 의료 사고가 발생할 위험을 줄이고자 한다.


**Data Set**

2126명의 CTG 데이터 (https://www.kaggle.com/datasets/andrewmvd/fetal-health-classification/data)

22개의 정보로 구성
 - Baseline value: 태아 심박수
 - Acceleration: 심박수가 증가하는 횟수
 - Abnormal short term variability: 비정상적인 단기 변화
 - Mean value of short term variabiltiy: 단기 변화의 평균값
 - Percentage of time with abnormal long term variabiltiy: 비정상적인 장기 변화가 전체 측정시간에서 차지하는 비율
 - Fetal health: 1(normal), 2(suspect), 3(pathological)
 - 외 17개 정보


**연구 기간**

2024.07.24 - 2024.07.26


**연구 결과**
Accuracy 기준 DNN(0.923), Random forest(0.951), Gradient Boosting(0.967), XGBoost(0.960)로 Gradient boosting이 가장 정확했음.
