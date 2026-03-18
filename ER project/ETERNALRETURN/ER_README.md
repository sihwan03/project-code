🎮 Eternal Return: User & Content Bridge Analysis

데이터로 푸는 게임의 재미: 초보 유저 리텐션 강화 및 메타 밸런스 최적화

📌 Project Overview

본 프로젝트는 이터널 리턴의 유저 플레이 로그를 분석하여 초기 이탈의 핵심 원인을 진단하고, 게임 콘텐츠의 밸런스 고착화 문제를 해결하기 위한 데이터 기반의 인사이트를 도출

단순한 데이터 요약을 넘어, 통계적 유의성 검정을 통해 실제 유저 경험을 개선할 수 있는 비즈니스 액션 플랜을 수립하는 데 집중

🛠 Tech Stack

Language: Python

Data Engineering: Pandas, NumPy, Pickle

Statistics: SciPy (Mann-Whitney U test, Shapiro-Wilk, Spearman Correlation)

Machine Learning: Scikit-learn (K-Means Clustering, Logistic Regression)

Visualization: Seaborn, Matplotlib, Sankey Diagram

📂 Repository Structure

👤 유저 행동 분석 (User Perspective)

ER_preprocessing_user.ipynb

유저 단위 지표(봇 노출도, MMR 변동 등) 생성 및 리텐션 라벨링 과정

ER_analysis_user.ipynb

Mann-Whitney U Test를 활용하여 리텐션 그룹 간의 유의미한 행동 차이를 증명

⚔️ 콘텐츠 밸런스 분석 (Content Perspective)

ER_preprocessing_content.ipynb

캐릭터 이름/역할 매핑 및 인게임 성능 지표 집계 과정

ER_analysis_content.ipynb

캐릭터 승률/픽률 및 이동 경로 분석을 통해 메타 밸런스 현황을 진단

🚀 Key Insights & Results

1️⃣ 유저 측면: '봇 노출도'와 리텐션의 상관관계

분석 결과, 이탈 유저 그룹은 잔존 유저 그룹에 비해 봇(AI)과의 대전 비중이 통계적으로 유의미하게 높음을 확인 (p-value < 0.05)

인사이트: 초반의 지나친 봇 매칭은 유저의 도전 욕구를 저하시켜 이탈을 가속화하는 원인이 됨을 규명

2️⃣ 콘텐츠 측면: 특정 캐릭터 및 경로의 메타 고착화

특정 캐릭터의 승률이 과도하게 높고, 특정 이동 경로의 이용률이 편중된 메타 고착화 현상을 데이터로 입증

인사이트: 플레이 다양성 부족은 중장기 리텐션 저해 요소로 작용하며, 이를 해결하기 위한 캐릭터 밸런싱 근거를 마련

📊 엄밀한 통계 검정 절차

데이터가 정규성을 만족하지 않는 게임 로그의 특성을 고려하여, T-test 대신 Mann-Whitney U Test를 최종 채택함으로써 분석 결과의 객관성과 신뢰도를 확보

💡 프로젝트 회고

데이터의 특성(비정규성)에 맞는 올바른 통계 기법을 선택하는 분석적 전문성을 획득 
특히 유저(User)와 콘텐츠(Content)라는 두 가지 축을 연결하여 게임 생태계 전체를 조망하고, 실제 서비스 지표(Retention)를 개선할 수 있는 논리적 구조를 경험

© 2026 배시환 Data Analysis Portfolio