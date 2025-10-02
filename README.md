🚦 Pedestrian Behavior Classification (Intel Geti 기반)
📌 개요

Intel Geti 플랫폼을 활용하여 횡단보도 보행자의 걷기/달리기 행동을 인식하는 AI 모델을 개발.
영상·이미지 데이터를 학습시켜 보행자의 행동을 자동으로 분류하며, 교통 신호 제어 및 보행자 안전 확보에 적용 가능.

주제: 횡단보도 보행자의 걷기 vs 달리기 행동 인식

Intel 7기 AI mini project 발표_이호빈

목적: 보행자의 안전을 높이고 교통 신호 체계에 적용 가능한 인공지능 학습

방법: 영상/이미지 데이터를 기반으로 행동 Classification 모델 학습 → 보행자의 행동을 자동 구분

📂 Dataset

형식: Intel Geti 기반 이미지/영상 데이터셋

라벨링 클래스:

Walking (걷기)

Running (달리기)

문제점:

빠른 걷기 vs 느린 달리기 경계가 모호 → 라벨링 기준 차이 발생

화질 저하 및 불균형 데이터셋에서 정확도 감소

Intel 7기 AI mini project 발표_이호빈

🧠 모델

모델 타입: Classification (Image-based)

Custom Model: Intel Geti 훈련 환경에서 학습

평가 결과:

데이터 다양성 부족 시 정확도 저하

단순 환경에서는 90% 이상 정확도 확보 가능

인사이트: AI 성능은 알고리즘 자체보다 데이터 품질과 다양성에 크게 의존

Intel 7기 AI mini project 발표_이호빈

⚙️ 설치 및 실행
1. 환경 설정
# 의존성 설치
pip install -r requirements.txt

2. 실행 예시
# Classification 실행
python3 run_behavior_classification.py --model best.engine --input sample_video.mp4

📊 결과

정확도: 모델/데이터셋 구성에 따라 편차 있음

테스트 결과: 걷기 vs 달리기 대부분 잘 분류하나, 경계 상황(빠른 걷기, 느린 달리기)에서 혼동 발생

Intel 7기 AI mini project 발표_이호빈

🔍 아쉬운 점 & 개선 방향

현실적인 도로 환경 데이터 확보 어려움 → 다양한 상황(멈춤, 자전거, 휴대폰 사용 등) 확장 필요

영상 화질이 낮거나 과도하게 많은 데이터가 혼재 시 성능 저하 발생

실제 교통 신호 제어 연계 시 실시간성·안정성 확보 필요

Intel 7기 AI mini project 발표_이호빈
