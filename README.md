# Project – ESG 등급 변화 분석을 통한 기업 특성 및 평가 체계 이해

## 📘 프로젝트 소개  
ESG(Environmental, Social, Governance) 등급 변화가 기업의 단기 주가에 미치는 영향을 실증적으로 검토하고,  
ESG 항목별 변화 특성, 기업 규모 및 산업군에 따른 평가의 구조적 차이를 분석함.

---

## 📈 ESG 등급 변화가 단기 주가에 미치는 영향 분석
- ESG 등급 발표일 전후의 1일 및 5일 종가 평균을 비교하는 **이벤트 스터디 방식** 활용  
- **Welch’s t-검정** 결과, 등급 상승/하락 간의 단기 주가 변화율에 **통계적으로 유의미한 차이 없음**

---

## 🧩 ESG 개별 항목(E, S, G)의 변화 특성과 기여도 분석
- 환경(E) 항목의 등급 **개선 비율이 가장 높음**
- 사회(S)는 편차가 크고 **등급 상승 기업보다 하락 기업 비율이 더 높음**
- **Random Forest 기반 Permutation Importance** 분석 결과:  
  → **지배구조(G)** 와 **사회(S)** 항목이 ESG 등급 결정에 **높은 기여도**

---

## 🏭 기업 규모 및 산업군에 따른 클러스터링 및 구조적 특성 분석
- E, S, G 항목 기반 **KMeans 클러스터링** 수행
- 클러스터 간 **시가총액 차이 통계적으로 유의미** (ANOVA, Kruskal–Wallis test)  
- ESG 등급이 높은 기업일수록 **시가총액이 크고 서비스/금융 업종 비중이 높음**
- ESG 등급이 낮은 클러스터에는 **제조업 중심 산업군**이 다수 포함됨

---

## 🛠️ 활용 기술 및 분석 방법

- **데이터 수집 및 전처리**  
  - Python 기반 웹 크롤링  
  - 한국ESG기준원 및 KRX 데이터 병합

- **통계 분석**  
  - Welch’s t-test  
  - ANOVA  
  - Kruskal–Wallis test

- **머신러닝 기법**  
  - Random Forest Regression (Permutation Importance)  
  - KMeans Clustering

- **시각화**  
  - Box plot  
  - Bar chart  
  - Cluster scatter plot

---

> 본 프로젝트는 ESG 평가가 기업 고유의 노력 외에도 구조적 요인(산업군, 규모 등)에 의해 영향을 받는다는 점을 보여주며, ESG 등급의 해석과 정책 설계에 있어 산업 맞춤형 접근의 필요성을 강조함.
