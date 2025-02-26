# LSTM 모델을 활용한 창원 지역구별 주택가격지수 예측 
> ## 개요:  다변량 시계열 데이터를 학습한 LSTM 모델을 활용하여 창원시 지역구별(의창구, 성산구, 마산합포구, 마산회원구, 진해구) 주택가격지수를 예측, 부동산시장 과열을 선제적으로 대응하는데 도움을 주는 프로그램을 제작한다.

* ## 독립변수
  * 기간: 2004-01-01 ~ 2020-12-01
  * 경남 소비자물가지수
  * 경남 가계대출금(2004 ~ 2007 데이터 누락)
  * 전국 건축허가면적
  * 전국 CD금리
  * 의창구 주택가격지수

    <img src="https://user-images.githubusercontent.com/32115744/111197112-6c993000-8601-11eb-870a-461ef22be5ba.png">
* ## 종속변수
  * 의창구 주택가격지수 
* ## 참고논문 
  * 전해정, 양혜선. (2019). 딥 러닝을 이용한 주택가격 예측에 관한 연구. 주거환경, 17(2), 37-49.
  * 이태형, 전명진. (2018). 딥러닝 모형을 활용한 서울 주택가격지수 예측에 관한 연구. 주택도시연구, 8(2), 39-56.
  * http://keras-ko.kr/, Keras Documemtation

* ## 변수선정 근거 
  * 주택가격지수
    * 주택가격지수는 국민은행에서 전국의 부동산 중개업자로부터 표본으로 추출된 표본 주택의 주택 매매가격을 조사하고 일정시점을(2015-12 = 100)을 기준시점으로 한 [라스파이레스산식](http://kostat.go.kr/incomeNcpi/cpi/cpi_cp/1/7/index.static)을 적용하여, 지역별, 주택유형별, 주택재고 구성비를 가중치 값으로 부여하여 산출한 지표를 말한다. 
* ## 기존 연구와의 차이점
  * 서울주택가격지수를 예측하는데 사용했던 국내 거시경제지표 데이터를 경남 도내에서 수집한 경제지표 데이터로 대체
* ## 진행상황
  * 의창구 주택가격지수를 활용한 단변량 시계열 LSTM모델 구성(최적화x)
  * <img src=" https://user-images.githubusercontent.com/32115744/111197453-d285b780-8601-11eb-9968-ff31eb14bef5.png">
  * <img src="https://user-images.githubusercontent.com/32115744/111197649-0f51ae80-8602-11eb-9b23-5624e1928fc8.png">



