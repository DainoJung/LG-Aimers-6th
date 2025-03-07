# 임신 성공률 예측 AI

## 📌 프로젝트 개요
본 프로젝트는 난임 환자의 시술 데이터를 바탕으로 **임신 성공 여부를 예측**하는 AI 모델을 개발하는 데 목적이 있습니다.  
ROC-AUC 점수를 기준으로 모델을 평가하며, 최적의 예측 모델을 구축하는 것이 목표입니다.

## 📂 데이터 개요
본 프로젝트에서 사용한 데이터는 **LG Aimer 데이터 분석 해커톤**에서 제공한 데이터셋으로, 아래와 같은 구조를 가집니다.

- **train.csv**  
  - 256,351개의 샘플  
  - 67개의 컬럼 (난임 환자의 시술 데이터 포함)  
  - `임신 성공 여부 (1: 성공, 0: 실패)` 라벨 존재  

- **test.csv**  
  - 90,067개의 샘플  
  - 67개의 컬럼 (라벨 없음)  

- **sample_submission.csv**  
  - 제출을 위한 양식  
  - `ID` 및 `probability` (예측 확률)  

- **데이터 명세.xlsx**  
  - 데이터 컬럼 및 상세 설명 포함  

## 🔧 기술 스택
본 프로젝트에서는 다음과 같은 기술을 활용하여 데이터 분석 및 모델링을 수행하였습니다.

- **언어:** Python
- **라이브러리:** pandas, numpy, scikit-learn, matplotlib, seaborn
- **모델링:** 머신러닝 모델 (예: RandomForest, XGBoost, LightGBM 등)
- **성능 평가:** ROC-AUC  

## 🚀 프로젝트 진행 과정
1. **데이터 탐색 (EDA, Exploratory Data Analysis)**
   - 결측치 확인 및 전처리
   - 이상치 탐지 및 처리
   - 변수 중요도 분석

2. **특성 엔지니어링**
   - 카테고리형 변수 인코딩
   - 피처 스케일링
   - 파생 변수 생성

3. **모델 학습 및 평가**
   - 기본 모델 성능 비교
   - 최적의 모델 선택 및 하이퍼파라미터 튜닝
   - 최종 모델 평가 (ROC-AUC 점수 기준)

4. **예측 및 제출**
   - 최종 모델을 통해 test 데이터 예측
   - `sample_submission.csv` 형식에 맞춰 결과 저장 후 제출

## 📊 데이터 분석 결과
- 주요 변수 탐색 결과 및 시각화 추가 예정

## 📌 참고 사항
- 본 프로젝트는 **LG Aimer 데이터 분석 해커톤**을 기반으로 진행되었습니다.
- 프로젝트 진행 중 업데이트가 있을 수 있습니다.

## 📝 작성자
- **Dino** (데이터 분석 및 머신러닝 모델링)
