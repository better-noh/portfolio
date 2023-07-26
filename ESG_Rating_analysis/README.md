## ESG 평가등급이 기업가치 측정 지표로 적절한지 분석
__분석기간 :__ 22.10.19. - 22.10.24. (6일)

- 분석인원 : 5인팀
- 활용 데이터 :

  |이름|설명|Method|Source|
  |:---:|:---|:---:|:---|
  |KCGS ESG Rating|한국ESG기준원 ESG등급 데이터</br>- 기간 : 2011년~2018년|Web Scraping|[KRX 정보데이터시스템](http://data.krx.co.kr/contents/MDC/HARD/hardController/MDCHARD050.cmd#none)|
  |KRX KOSPI 200 Index Components|KRX KOSPI 200 지수 구성종목 정보</br>- 기간 : 2010-06-30~2018-06-31</br>- 매년 06월 말일과 12월 말일에 대한 데이터|Download|[KRX 정보데이터시스템](http://data.krx.co.kr/contents/MDC/MDI/mdiLoader/index.cmd?menuId=MDC0201010106)|
  |KRX KOSPI 200 Index Components</br>Stock Price|한국ESG기준원 ESG등급 데이터</br>- 기간 : 2011년~2018년|API|[FinanceDataReader](https://github.com/financedata-org/FinanceDataReader)|
  |DART corpCode|금융감독원 고유번호|API|[금융감독원 고유번호](https://opendart.fss.or.kr/guide/detail.do?apiGrpCd=DS001&apiId=2019018)|
  |DART company|금융감독원 공시정보 기업개황|API|[금융감독원 공시정보 기업개황](https://opendart.fss.or.kr/guide/detail.do?apiGrpCd=DS001&apiId=2019002)|
  |FSC FinaStatInfo|금융위원회 기업재무정보 (요약재무제표)</br>- 기간 : 2011년~2018년|API|[금융위원회 기업 재무정보](https://www.data.go.kr/tcs/dss/selectApiDataDetailView.do?publicDataPk=15043459)|
  |KRX KOSPI 200 Index Price|한국거래소 KOSPI 200 지수 가격 데이터</br>- 기간 : 2011년~2018년|Download|[KRX 정보데이터시스템](http://data.krx.co.kr/contents/MDC/MDI/mdiLoader/index.cmd?menuId=MDC0201010105)|
  |KRX KOSPI 200 ESG Index Price|한국거래소 KOSPI 200 ESG 지수 가격 데이터</br>- 기간 : 2010-06-31~2022-06-31|Download|[KRX 정보데이터시스템](http://data.krx.co.kr/contents/MDC/MDI/mdiLoader/index.cmd?menuId=MDC0201010105)|

  - 표본
     - 2011년~2018년 KOSPI200 지수에 구성된 적이 있는 종목(기업)이면서
     - KCGS에서 ESG등급 평가된 적이 있는 종목
- 사용기술 : pandas, numpy, seaborn, matplotlib, beautifulsoup

__개요 :__ 

다양한 연구를 통해 ESG가 기업의 지속가능성 및 장기적인 가치 창출을 평가하는 중요한
기준이 된다고 보고되고 있습니다. 다른 평가 지표와의 비교를 통해 ESG 평가 등급이 기업
가치 측정 지표로서의 가치가 있는지 분석했습니다.
- ESG등급 관련 선행 연구 확인
- ESG등급과 주가지수, 개별종목의 주가, 재무제표 분석

__담당역할 :__

- ESG등급 데이터 스크래핑
- ESG등급별 개별종목 시각화
- 연도별 ESG등급과 주가 관계 분
