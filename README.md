# Health-Care-Big-Data-Project 
#### Data : 19/11/04 ~ 19/11/15
#### POSCO AI BIG DATA ACADEMY
#### Author : 박규동, [공은비](github.com/eunbikong), 김규리, 김송일, 박병수, [이수진](github.com/sooooojinlee)
#### Title : 중증질환 위험도 예측 모델 개발 및 위험도 수준을 고려한 맞춤 서비스 제공으로 헬스케어 시장 선점
#### Data set
* health_data.csv : [국가건강검진]()개인 건강검진 결과 데이터 중 7만 건 랜덤추출
* cell_img.csv : 악성/양성종양 세포 MRI 이미지 데이터
* hospital_basic_info.csv : 
* hospital_medical_sub_spec.csv :

##### Reference
|제목|출처|비고|
|-----|-------|------|
|[국가건강검진 건강위험평가 개선](#국가건강검진-참고-페이지)|질병관리본부|health_data 변수 전처리 참고, 심뇌혈관질환 위험도 계산|
|국가중점 개방데이터(건강검진정보) 사용자 매뉴얼(ver 4.0)|국민건강보험공단 빅데이터운영실|변수 파악|
|[대한진단검사학회](https://labtestsonline.kr/)|대한검사의학회|각 질병 진단 기준을 파악하여 파생변수 생성|
|[라이프시맨틱스](https://lifesemantics.kr/intro/company)|데이터 분석 후 개선안 수립 시 참조|
|[메트라이프](http://insu.greenpio.com/MetLife360health/)|데이터 분석 후 개선안 수립 시 참조|
|직장에서의 뇌·심혈관계질환 예방을 위한 발병위험도 평가 및 사후관리지침|한국산업안전보건공단|심뇌혈관질환 예측 모델을 만들기 위해 참고|
|[일반적으로 잘 알려져 있는 심혈관질환의 위험인자](https://www.circulation.or.kr:4443/bbs/index.php?code=int&category=&gubun=&page=1&number=6896&mode=view&keyfield=all&key=)|대한심장학회|중증질환의 주요 위험인자인 대사증후군 진단 기준 참고|

### 국가건강검진 참고 페이지
p.37~64 예측 모형에 대한 설명  
p.82 기존 예측 모형  
p.100 생활습관 요인 정의  
p.109 수검여부에 따른 건강위험요인 변화여부 비교    
p.127 (p.144, p.221) HRA 로직 수정 및 시범 적용  
p.204 서비스 예시  
p.216 결론 및 발전방향  
p.219 스마트 헬스케어 분야 활용  
p.222 변수 재정리  
p.231 건강위험요인 알아보기 평가기준  
p.233 로직계산 예시  
