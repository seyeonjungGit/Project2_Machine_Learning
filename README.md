# Project2_machine_learning
한 사람이 연간 50K (k = 1000, 즉, 50,000달러)이상을 버는가?


# 파일 설명

### 1. (1) EDA&모델탐색_Section2_Project_machine_learning
  - 전처리 & EDA 
  - 가설검증 : Chisquare, Pearson correlation
  - 여러가지 머신러닝 모델의 성능 측정 : logistic regression, Desicion Tree, RandomForest, XGboost, LightGBM, CatBoost
  - cross validation
  - 
### 2. (2) 모델선정_Section2_Project_machine_learning
  - 최종모델선정 : LightGBM
  - Feature Engneering : 특성중요도, 순열중요도를 고려한 Feature selection
  - 하이퍼파라미터 조절 : early stopping, Randomized Search CV
  - 최적임계값 설정
  - 
### 3. (3) 모델의 해석_Section2_Project_machine_learning
  - 부분의존도 그림(PDP)을 활용한 특성 기여도 해석
  - SHAP을 활용한 개별관측치로부터의 특성 기여도 해석
  - Confusion matrix 및 결론

**<< 첨부 : 데이터셋 설명  >>**
- age(나이) : continuous(연속적인 수치)

- workclass(직업분류; 고용주의 유형)
    - Private(개인사업)
    - Self-emp-not-inc(자영업-수입없음) 
    - Self-emp-inc(자영업-수입있음)
    - Federal-gov(연방정부)
    - Local-gov(지방정부)
    - State-gov(주 정부)
    - Without-pay(무급)
    - Never-worked(무직)
- fnlwgt(가중치? : 데이터셋 출처에 설명없음) : continuous.인구조사 대상자들이,  관측치가 나타내는 것으로 믿는 사람들의 수.

- education(학력) : Preschool(유치원) < 1st-4th < 5th-6th < 7th-8th < 9th < 10th < 11th < 12th < HS-grad(고졸) < Prof-school(전문학교) < Assoc-acdm < Assoc-voc < Some-college < Bachelors(학사) < Masters(석사) < Doctorate(박사)
    - Some-college(고등학교 졸업 후 대학 수준의 수업을 일부 들었지만 아직 학위를 취득하지 못한 상태)
    - HS-grad(High School Graduate;고졸)
    - Prof-school(Professional School;전문학교) 

- education-num(교육번호) : continuous.

- marital-status(결혼상태)
    - Never-married 미혼
    - Married-civ-spouse 기혼-시민-배우자
    - Married-AF-spouse기혼-공군-배우자
    - Married-spouse-absent 기혼-배우자-부재
    - Separated 별거
    - Divorced 이혼
    - Widowed 사별
    
- occupation 직업
    - Tech-support 기술지원
    - Craft-repair 공예수리
    - Other-service 기타서비스
    - Sales 판매
    - Exec-managerial 간부관리
    - Prof-specialty 전문직
    - Handlers-cleaners 핸들러-청소부
    - Machine-op-inspct 기계 작동 검사
    - Adm-clerical ADM-사무
    - Farming-fishing 농업-낚시
    - Transport-moving 운송-이사
    - Priv-house-serv
    - Protective-serv
    - Armed-Forces군대.

- relationship (가족관계)
    - Wife
    - Own-child 자녀
    - Husband
    - Not-in-family 가족 외
    - Other-relative 친척
    - Unmarried

- race(인종)
    - White
    - Asian-Pac-Islander
    - Amer-Indian-Eskimo
    - Other
    - Black

- sex: Female, Male.

- capital-gain 자본이득: continuous
- capital-loss 자본손실: continuous
- hours-per-week 주당시간: continuous
- native-country 출신국: United-States, Cambodia, England, Puerto-Rico, Canada, Germany, Outlying-US(Guam-USVI-etc), India, Japan, Greece, South, China, Cuba, Iran, Honduras, Philippines, Italy, Poland, Jamaica, Vietnam, Mexico, Portugal, Ireland, France, Dominican-Republic, Laos, Ecuador, Taiwan, Haiti, Columbia, Hungary, Guatemala, Nicaragua, Scotland, Thailand, Yugoslavia, El-Salvador, Trinadad&Tobago, Peru, Hong, Holand-Netherlands.
