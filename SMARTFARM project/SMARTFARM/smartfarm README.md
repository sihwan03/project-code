🍅 Smart Farm Tomato BER Analysis

데이터 정밀 보정부터 13단계 통계적 원인 규명까지: 배꼽썩음과(BER) 예방 전략

📌 Project Overview

본 프로젝트는 스마트팜 4개 농가에서 수집된 환경 센서 데이터와 생육 데이터를 분석하여, 토마토 품질 저하의 주범인 **배꼽썩음과(Blossom-End Rot)**의 환경적 유발 인자를 규명

🛠 Tech Stack

Language: Python

Data Engineering: Pandas, NumPy

Statistical Analysis: SciPy (Shapiro, Levene, Mann-Whitney U, Kruskal-Wallis)

Machine Learning: Scikit-learn (Random Forest)

Visualization: Seaborn, Matplotlib, Tableau

📂 Repository Structure

1. 데이터 정밀 전처리 파이프라인 (Preprocessing)

Step 1-2: 데이터 로드 및 특정 농가('이삭줍는 알파고') 열 밀림 정밀 보정

Step 3-5: 센서 코드 한글 매핑 및 데이터 해상도 조정(일 단위 집계)

Step 6-8: 결측치 선형 보간, 데이터 병합 및 시계열 트렌드 파생 변수 생성

Step 9: 전처리 과정 종합 정리

2. 가설 검증 및 13단계 통계 분석 (Analysis)

Step 1-6: 기초 통계 진단, 상관분석(Spearman) 및 그룹 간 시각적 비교

Step 7-11: 통계적 의사결정 (정규성/등분산 검정 기반 비모수 검정 선택 과정)

Step 12-13: 머신러닝 기반 변수 중요도 검증 및 최종 결론 도출

🚀 Key Insights & Results

1️⃣ 데이터 무결성 확보

특정 농가의 시스템 오류(열 밀림)를 발견하고 수동 보정함으로써 분석 결과의 신뢰도를 높임

2️⃣ 통계적 분석의 엄밀함

데이터 분포의 비정규성을 입증하고, 이에 적합한 Mann-Whitney U Test를 채택하여 결과의 객관성 확보

3️⃣ 핵심 인자 규명

**배액 EC(전기전도도)**가 품질에 가장 큰 영향을 미침을 확인

고 EC 환경에서의 삼투압 상승이 칼슘(Ca) 흡수를 저해한다는 인과관계를 입증

💡 프로젝트 회고

데이터의 기술적 특성을 먼저 파악하여 최적의 분석 방법론을 선택하는 것이 실무 데이터 분석가의 핵심 역량임을 경험

© 2026 배시환 Data Analysis Portfolio