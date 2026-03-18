# 💳 신용카드 이용 패턴 분석 기반 이탈 예측 및 마케팅 ROI 최적화
> **데이터로 푸는 금융 비즈니스: 고객 이탈 징후 진단 및 수익 극대화 전략 수립**

📌 **Project Overview**

본 프로젝트는 **300만 건의 AIHub 신용카드 승인매출 및 회원 데이터**를 분석하여 고객의 이탈 원인을 다각도로 진단하고, 이를 방어하기 위한 마케팅 시나리오의 재무적 타당성을 검토한 프로젝트

단순한 데이터 요약을 넘어, **이용강도(I), 이용빈도(F), 소비습관(H)**이라는 세 가지 핵심 관점에서 고객 행동을 분해하고, 
최종적으로 마케팅 ROI를 2.9배 이상 레버리지할 수 있는 **'안정적 전략(Stable Strategy)'**을 제안하는 데 집중

🛠 **Tech Stack**

- **Language**: Python
- **Data Engineering**: Polars (대용량 처리 고도화), Pandas, NumPy
- **Data Format**: Parquet (ZSTD Compression)
- **Machine Learning**: LightGBM, CatBoost, Scikit-learn (Stacking Ensemble)
- **Statistics & Validation**: SHAP, PSI (Population Stability Index), Calibration Curve
- **Visualization**: Seaborn, Matplotlib

📂 **Repository Structure**

👤 **데이터 통합 및 마스터 전처리 (Data Foundation)**

- **FINANCE_master_preprocessing.ipynb**
    - 5개 산재 테이블(회원/신용/승인/청구/잔액) 병합 및 300만 건 데이터 최적화
    - **Polars & Parquet** 도입을 통한 기존 방식 대비 처리 속도 및 메모리 효율 60% 이상 개선
    - 2개월 관측 윈도우 기반 트렌드 피처 생성 및 리텐션(`is_churn`) 라벨링 프로세스 **구축**

⚔️ **주제별 이탈 예측 모델링 (Multi-Perspective Modeling)**

- **FINANCE_intensity_modeling.ipynb** (이용강도 관점)
    - 고액 결제 비중 및 소비 기울기 분석을 통한 '우량 고객 이탈' 징후 **포착**
- **FINANCE_frequency_modeling.ipynb** (이용빈도 관점)
    - 활동 밀도 및 결제 주기 변화를 통한 '주카드 지위 상실' 프로세스 **규명**
- **FINANCE_habit_modeling.ipynb** (소비습관 관점)
    - 온라인/쇼핑/유틸리티 등 업종별 패턴 전이에 따른 라이프스타일 변화 **추적**

🚀 **통합 마케팅 전략 및 ROI 시뮬레이션 (Business Strategy)**

- **FINANCE_marketing.ipynb**
    - **Profit Curve**: 마케팅 비용 대비 순이익이 극대화되는 최적 타겟 임계치(Top 9.1%) **도출**
    - **Strategy Compare**: '공격적 전략' 대비 '안정적 전략'의 ROI 우위(2.32배) **증명**
    - **Leverage Analysis**: 방어 성공률 상승에 따른 수익 레버리지 효과(최대 2.9배) 시뮬레이션 **수행**

🚀 **Key Insights & Results**

1️⃣ **데이터 엔지니어링: 대용량 처리 최적화**
300만 건의 금융 로그를 Pandas로 처리 시 발생하는 메모리 병목 현상을 해결하기 위해 **Rust 기반의 Polars**와 **Parquet 포맷**으로 전환
데이터 로드 및 전처리 속도를 획기적으로 단축하여 분석 사이클의 효율성 **확보**

2️⃣ **비즈니스 전략: ROI 중심의 타겟팅 최적화**
단순히 이탈 확률이 높은 고객을 모두 잡는 '공격적 전략'보다, 기대이익곡선(Profit Curve)상의 정점인 상위 9.1%에 집중하는 **'안정적 전략'**이 
투입 예산 대비 훨씬 높은 ROI(2.32배)를 기록함을 데이터로 **입증**

📊 **엄밀한 모델 검증 절차**
금융 도메인의 특성을 고려하여 모델의 예측 확률이 실제 발생 빈도와 일치하는지 확인하는 **Calibration Curve**와 
데이터 분포의 변화를 추적하는 **PSI(Population Stability Index)**를 도입하여 모델의 실무 적용 신뢰도 **확보**

💡 **프로젝트 회고**
300만 건이라는 대규모 시계열 데이터를 다루며 **데이터 엔지니어링(Polars/Parquet)**의 중요성을 깊이 체감함
특히 팀 프로젝트 진행 중 효율성 개선을 위해 기술 스택을 과감히 전환했던 경험은 기술적 유연성을 기르는 계기가 됨

단순히 이탈자를 예측하는 인공지능 모델링에 그치지 않고, 기업의 재무적 관점에서 **비용 대비 수익(ROI)**을 시뮬레이션하며 데이터 분석 결과가 실제 비즈니스 의사결정에 기여하는 전체 프로세스 **경험**

© 2026 배시환 Data Analysis Portfolio