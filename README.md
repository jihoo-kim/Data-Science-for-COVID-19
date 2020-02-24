# Coronavirus-Dataset
[질병관리본부(KCDC) 공식 홈페이지](http://www.cdc.go.kr/)에서 제공하는 **코로나바이러스감염증-19 (COVID-19)** 국내 확진자 정보를 데이터 분석에 용이하도록 CSV 파일로 재가공하였습니다.

### 데이터셋 정보
833명의 확진자에 대한 정보 (2020년 2월 24일 기준)
- *id*: 확진자의 id (n번째 확진자) 
- *sex*: 성별
- *birth_year*: 출생 연도
- *country*: 국적
- *region*: 주 활동 지역 (광역시/도 단위)
  - *capital area*: 수도권(서울특별시 및 경기도)
- *infection_reason*: 감염 경로
- *infection_order*: 감염 차수 (n차 감염)
- *contact_number*: 접촉자 수
- *confirmed_date*: 확진 일자
- *released_date*: 격리 해제 일자
- *state*: 상태
  - *isolated*: 격리(입원)
  - *released*: 격리 해제(퇴원)
  - *dead*: 사망
  
