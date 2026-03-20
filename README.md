# Car Price Prediction (DACON)

중고차 데이터를 기반으로 차량 가격을 예측하는 머신러닝 프로젝트
다음을 참고하십시오
https://dacon.io/competitions/official/236114/overview/description 

## Overview
- Task: 자동차 가격 회귀 예측
- Data: DACON 중고차 거래 데이터
- Target: 가격(price)

## Data Processing
- 이상치 제거 (연식, 주행거리 등)
- 연식(feature) 생성
- 범주형 처리 (Label Encoding / CatBoost 자동 처리)
- Train/Test = 8:2 분할 :contentReference[oaicite:0]{index=0}

## Model
- RandomForestRegressor
- XGBoost / LightGBM / CatBoost 비교
- 최종: CatBoost 및 Ensemble 사용 :contentReference[oaicite:1]{index=1}

## Results
- Local MAE: ~5.7  
- DACON MAE: ~5.78 :contentReference[oaicite:2]{index=2}

## Key Idea
- 이상치 제거 + feature engineering이 성능에 큰 영향
- CatBoost → 범주형 데이터 처리에 효과적

## From this project
- 저의 첫 AI 프로젝트입니다.
