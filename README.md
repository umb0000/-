🧠 흡연 여부 예측 모델 구축기 (기계학습 프로젝트)

팀원: 5명
기간: 2024-1학기 기계학습 수업 최종 프로젝트

📊 데이터 출처 및 설명
DACON 흡연 여부 예측 AI 해커톤

다양한 생체지표 포함 (중성지방, 혈청 크레아티닌, 고/저밀도 지단백 등)

🔍 데이터 전처리 & EDA
이상치 처리: Z-score, IQR, UCL/LCL 방식 활용

피처 제거: 다중공선성 문제 해결 위해 BMI, 콜레스테롤 제거

스케일링: MinMaxScaler, StandardScaler 사용

🧪 사용 모델 및 성능 비교
단일 모델: LightGBM, XGBoost, CatBoost, SVM, DNN, Logistic Regression 등

해석 도구: SHAP 활용 → 키, 헤모글로빈, 중성지방 등이 흡연과 큰 관련

🔗 앙상블 모델 성능 (Logistic Regression + Random Forest + XGBoost)
정확도: 0.78

정밀도: 0.73

재현율: 0.86

ROC AUC: 0.87
→ 단일 모델보다 높은 예측 성능

🧭 결론 및 한계
키 변수의 영향이 컸지만, 성별 데이터 부재로 왜곡 가능성

PCA, 변수 제거, 하이퍼파라미터 튜닝 노력에도 성능 아쉬움

학습 시간이 오래 걸려 최적값 탐색에 제약
