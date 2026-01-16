# regression-analysis-student-performance
Regression analysis project analyzing factors affecting student exam performance using OLS, variable selection, and Ridge regression

본 프로젝트는 회귀분석 수업에서 수행한 분석 과제로,  
학생들의 시험 성적(Exam_Score)에 영향을 미치는 다양한 요인들을  
통계적 회귀 모델을 통해 분석하는 것을 목표로 한다.

---

## 📌 Project Overview
- **Objective**  
  학생의 학습 습관, 심리적 요인, 가정 및 학교 환경 변수가  
  시험 성적에 어떠한 영향을 미치는지 분석

- **Dataset**  
  Kaggle - *Student Performance Factors*  
  - Observations: 6,607 students  
  - Original variables: 20  
  - Variables after preprocessing: 27  

- **Target Variable**  
  - `Exam_Score`

---

## 🧪 Methodology

### 1. Data Analysis
- Confirmatory Data Analysis (CDA)
- Exploratory Data Analysis (EDA)
- Missing value handling (mode imputation)
- One-hot encoding for categorical variables
- Multicollinearity prevention via dummy variable reduction

### 2. Regression Modeling
- Ordinary Least Squares (OLS)
- Multicollinearity diagnosis using VIF
- Variable selection  
  - Forward Selection  
  - Backward Elimination  
  - Stepwise Selection (BIC 기준)

### 3. Model Improvement
- Ridge Regression to handle multicollinearity
- Hyperparameter tuning using RidgeCV
- Standardization with StandardScaler

### 4. Diagnostics & Assumptions
- Residual Q-Q plot
- Fitted vs residual plot
- Influence point detection using Cook’s Distance
- Separate analysis for high-score student group

---

## 📊 Key Findings
- 가정 환경 및 교육 자원 접근성이 시험 성적에 가장 큰 영향
- 학습 태도(Hours_Studied, Attendance)는 핵심 예측 변수
- 단순 변수 제거만으로는 다중공선성 해결이 어려움
- Ridge Regression이 회귀계수의 안정성을 크게 개선
- 고득점 학생 집단은 일반 학생과 다른 성취 패턴을 보임

---
