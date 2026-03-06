# ⚡ 실시간 알림 연동형 전력 모니터링 & 예측 기반 관리 시스템
> **2025 AI 해커톤 (숙명여대 AI센터 x 대웅재단) - 공장 전력 절감 시스템**

## 📝 프로젝트 소개
공장의 과거 전력 사용량 데이터를 기반으로 시계열 예측 AI를 구축하고, 예측치 대비 부하가 급증(이상치)할 경우 관리자에게 실시간 Slack 알림을 전송하는 비용 절감 및 이상 감지 통합 솔루션입니다.

## ⚙️ 기술 스택 (Tech Stack)
* **Language & Modeling:** Python, XGBoost, Prophet, SARIMA, LightGBM
* **Data Processing:** Pandas, NumPy, Scikit-learn
* **Service:** Slack API, (Dashboard 연동)

## 🚀 핵심 기능 (Key Features)
1. **전력 사용량 단기 예측 및 이상 탐지**
   * 다양한 외부 변수(요일, 주말 등)와 과거 전력 패턴(Lag, 이동평균)을 반영하여 향후 단기 전력 사용량 정밀 예측.
2. **5가지 시계열 모델 성능 비교 (MAPE, SMAPE 기준)**
   * 단일 모델(Prophet, SARIMA, LGBM, XGBoost)과 앙상블 모델의 성능을 교차 검증하여 최적 모델 도출.
3. **실시간 알림 파이프라인 (Team Contribution)**
   * 예측값을 초과하는 이상 징후 발생 시, 즉각적으로 Slack 메시지를 발송하여 공장 관리자가 즉시 조치할 수 있도록 구현.

## 🙋‍♀️ 나의 기여도 (My Contribution)
* **팀 빌딩 주도:** 비즈니스 목표 달성을 위한 개발 및 기획 파트 팀원 모집
* **데이터 전처리 (EDA):** 결측치 제거, 시간 리샘플링, 파생변수(Lag 1/7, 3일/7일 이동평균 등) 생성
* **AI 모델링 주도:** 5가지 알고리즘 벤치마킹 수행 및 최종 모델(XGBoost) 평가/선정 (비즈니스 성격에 맞춰 평가지표 MAPE, SMAPE 채택)
