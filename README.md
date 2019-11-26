# Health-Care-Big-Data-Project

Overview
-------------------------------
* **Organization** : POSCO AI BIG DATA ACADEMY
* **Industry** : Health
* **Project Title** : 중증질환 위험도 예측 모델 개발 및 위험도 수준별 맞춤 의료 서비스 제공으로 헬스케어 시장 선점
* **Project Description** : 2016년 기준 건강검진 수검자의 기본정보(성, 연령대, 시도코드 등)와 검진내역(신장, 콜레스테롤, 혈색소 등) 데이터를 활용한 중증질환 발병 위험수준 예측 및 개선안 도출
* **Author(s)** : 박규동, [공은비](https://github.com/barha-star), 김규리, [김송일](https://github.com/camelia13), [박병수](https://github.com/Hinterhalter), [이수진](https://github.com/sooooojinlee)
* **Date** : 19/11/04 ~ 19/11/15  


Dataset
-------------------------------
 * **health_data.csv** : [국가건강검진정보](https://www.data.go.kr/dataset/15007122/fileData.do) 개인 건강검진 결과 데이터 100만 건 중 7만 건 랜덤 추출
 * **cell_img.csv** : 악성/양성종양 세포 MRI 이미지 데이터
 * **hospital_basic_info.csv** : 전국 시도별 병원 위치 정보 데이터
 * **hospital_medical_sub_spec.csv** : 병원 진료 과목 정보 데이터  


Timeline
-------------------------------
|date|day|note|
|:-----:|:-----:|:------|
|19/11/04|mon|헬스케어 비즈니스 상황 분석, 추진배경 작성|
|19/11/05|tue|현황 및 개선기회 작성|
|19/11/06|wed|데이터 셋 확인, 웹 구현 시작|
|19/11/07|thur|도메인 지식, 변수 파악, 파생변수 생성, 태블로 시각화|
|19/11/08|fri|변수 파악 및 탐색적 분석, 추진배경 재작성, 구글 API 병원 위치 정보 지도 시각화, 태블로 시각화, 암 진단 모델링|
|19/11/09|sat|탐색적 분석 및 인사이트 도출|
|19/11/10|sum|탐색적 분석 후 분석 방향에 대한 고민, 데이터셋 통합 시도|
|19/11/11|mon|HRA 발견, 심뇌혈관질환 위험도 계산, 대사증후군 모델링, 암 모델링(LR, DT, RF, GB, XGB)|  
|19/11/12|tue|심뇌혈관질환 위험도 계산, 대사증후군 모델링, 암 모델링, 카이제곱 검정으로 지역별 의료인프라 차이 확인|
|19/11/13|wed|카이제곱검정, PPT 구성|
|19/11/14|thur|최종 PPT 완성|
|19/11/15|fri|최종 발표|  


Notebooks and Analysis
-------------------------------
The project includes the following notebooks (data manipulation and analysis):  

* #### [Data Preprocessing](https://nbviewer.jupyter.org/gist/KimGyuLee/30aca84f405bb5ddc81a522b6fda84df)
* #### [Data Exploration](https://nbviewer.jupyter.org/gist/KimGyuLee/c370b6d1c85167bcd1cda85789603f05)
* #### [Modeling & Evaluating model performance (1)-대사증후군](https://nbviewer.jupyter.org/gist/KimGyuLee/6f8dbdd37f4b845f22272a6732236644)
* #### [Modeling & Evaluating model performance (2)-심혈관질환](https://nbviewer.jupyter.org/gist/KimGyuLee/325028ce0612728111bdb7641596e04b)
* #### [Modeling & Evaluating model performance (3)-암](https://nbviewer.jupyter.org/gist/KimGyuLee/c4b3a29ff479431cf69f809db372046e)
* #### [Web]()
* #### [Project Portfolio](https://nbviewer.jupyter.org/github/KimGyuLee/Health-Care-Big-Data-Project/blob/master/healthcare_project.pdf)

It is recommended to view the notebooks in the above order to avoid missing out on code explainations.

Tech
-------------------------------
The following technologies were used for this part of the project:

* Python 3
* iPython Notebooks: For interactive code development and result presentation.
* Pandas: Python package for data analysis.
* Matplotlib and Seaborn: Python 2D plotting library.

Reference
----------------------------------------------
|#|title|source|note|
|:----:|:-----|:-------|:------|
|1|[국가건강검진 건강위험평가 개선](#국가건강검진-건강위험평가-개선-참고-페이지)|질병관리본부|health_data 변수 전처리 참고, 심뇌혈관질환 위험도 계산|
|2|국가중점개방데이터 사용자 매뉴얼(ver4.0)|국민건강보험공단 빅데이터운영실|health_data 변수 파악|
|3|[대한진단검사학회](https://labtestsonline.kr/)|대한검사의학회|각 질병 진단 기준을 파악하여 파생변수 생성|
|4|[라이프시맨틱스](https://lifesemantics.kr/intro/company)|라이프시맨틱스|데이터 분석 후 개선안 수립 시 참조|
|5|[메트라이프](http://insu.greenpio.com/MetLife360health/)|메트라이프|데이터 분석 후 개선안 수립 시 참조|
|6|직장에서의 뇌·심혈관계질환 예방을 위한 발병위험도 평가 및 사후관리지침|한국산업안전보건공단|심뇌혈관질환 예측 모델을 만들기 위해 참고|
|7|[일반적으로 잘 알려져 있는 심혈관질환의 위험인자](https://www.circulation.or.kr:4443/bbs/index.php?code=int&category=&gubun=&page=1&number=6896&mode=view&keyfield=all&key=)|대한심장학회|중증질환의 주요 위험인자인 대사증후군 진단 기준 참고|  


Appendix
----------------------------------------------
#### 국가건강검진 건강위험평가 개선 참고 페이지  
**p.37~64** 예측 모형에 대한 설명  
**p.82** 기존 예측 모형  
**p.100** 생활습관 요인 정의  
**p.109** 수검여부에 따른 건강위험요인 변화여부 비교    
**p.127** (p.144, p.221) HRA 로직 수정 및 시범 적용  
**p.204** 서비스 예시  
**p.216** 결론 및 발전방향  
**p.219** 스마트 헬스케어 분야 활용  
**p.222** 변수 재정리  
**p.231** 건강위험요인 알아보기 평가기준  
**p.233** 로직계산 예시  
