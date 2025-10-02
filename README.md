# 🚦 Pedestrian Behavior Classification (Intel Geti 기반)

## 📌 개요
Intel Geti 플랫폼을 활용하여 **횡단보도 보행자의 걷기/달리기 행동을 인식하는 AI 모델**을 개발.  
영상·이미지 데이터를 학습시켜 보행자의 행동을 자동 분류하며, 교통 신호 제어 및 보행자 안전 확보에 적용 가능.

| 구분 | 내용 |
|------|------|
| **주제** | 횡단보도 보행자의 걷기 vs 달리기 행동 인식 |
| **목적** | 보행자의 안전을 높이고 교통 신호 체계에 적용 가능한 인공지능 학습 |
| **방법** | 영상/이미지 데이터 기반 **Classification 모델** 학습 → 보행자의 행동을 자동 구분 |

---

## 📂 Dataset
- **형식**: Intel Geti 기반 이미지/영상 데이터셋  
- **라벨링 클래스**:  
  - 🟢 Walking (걷기)  
  - 🔴 Running (달리기)  

| 문제점 | 설명 |
|--------|------|
| **빠른 걷기 vs 느린 달리기** | 경계가 모호해 라벨링 기준 차이 발생 |
| **데이터 품질 문제** | 화질 저하 및 불균형 데이터셋에서 정확도 감소 |
<img width="1148" height="647" alt="image" src="https://github.com/user-attachments/assets/2022ff3f-217f-49fa-a0aa-dac7ffd78458" />

---

## 🧠 모델
- **타입**: Classification (Image-based)  
- **Custom Model**: Intel Geti 환경에서 직접 학습  

| 평가 지표 | 결과 |
|-----------|------|
| **정확도** | 단순 환경에서는 90% 이상 |
| **한계** | 데이터 다양성 부족 시 성능 저하 |
| **인사이트** | 모델 성능은 **데이터 품질과 다양성**에 크게 의존 |
<img width="1148" height="647" alt="image" src="https://github.com/user-attachments/assets/fc7e17ac-e732-4653-a574-55f769c7493b" />

---

# 📊 결과

걷기 vs 달리기 대부분 잘 분류

경계 상황(빠른 걷기 ↔ 느린 달리기)에서 혼동 발생

---
