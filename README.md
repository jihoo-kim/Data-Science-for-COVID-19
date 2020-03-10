# Coronavirus-Dataset
- **코로나바이러스감염증-19 (COVID-19)** 국내 확진자 정보를 데이터 분석에 용이하도록 CSV 파일로 재가공하였습니다.
1. patient 데이터셋: 7513명의 확진자에 대한 정보 (2020년 3월 10일 0시 기준)  
2. route 데이터셋: 확진자들의 이동 경로에 대한 정보
3. time 데이터셋: 일자별 검사 결과 및 현황 정보
4. trend 데이터셋: 일자별 코로나 관련 키워드 검색량 정보 (네이버 기준)
  
- 아직 확인되지 않은 정보는 추후에 업데이트할 예정입니다.
- kaggle Data에도 공개되어 있습니다. [Coronavirus-Dataset](https://www.kaggle.com/kimjihoo/coronavirusdataset) 

***

**Dataset License**: [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)

***

### 1. patient 데이터셋 정보
- ***id***: 확진자의 id (n번째 확진자) 
- ***sex***: 성별
- ***birth_year***: 출생 연도
- ***country***: 국적
  - *Korea*: 대한민국
  - *China*: 중국
  - *Mongolia*: 몽골
- ***region***: 주 활동 지역 (광역시/도 단위)
  - *capital area*: 수도권 (서울특별시/인천광역시/경기도)
  - *filtered at airport*: 공항 검역 이후 활동하지 않은 경우
  - *Busan*: 부산광역시
  - *Daegu*: 대구광역시
  - *Daejeon*: 대전광역시
  - *Gwangju*: 광주광역시
  - *Ulsan*: 울산광역시
  - *Gangwon-do*: 강원도
  - *Chungcheongbuk-do*: 충청북도
  - *Chungcheongnam-do*: 충청남도
  - *Jeollabuk-do*: 전라북도
  - *Jeollanam-do*: 전라남도
  - *Gyeongsangbuk-do*: 경상북도
  - *Gyeongsangnam-do*: 경상남도
  - *Jeju-do*: 제주도
- ***disease***: 기저 질환 여부
  - *0*: 없음
  - *1*: 있음
- ***group***: 특정 집단 관련
  - *Shincheonji Church*: 신천지 관련
  - *Cheongdo Daenam Hospital*: 청도대남병원 관련
  - *Eunpyeong St. Mary's Hospital*: 은평성모병원 관련
  - *Onchun Church*: 온천 교회 관련
  - *Myungsung Church*: 명성 교회 관련
  - *Pilgrimage*: 이스라엘 성지순례 관련
- ***infection_reason***: 감염 경로
  - *visit to ooo*: 감염 위험 나라/도시 방문
  - *contact with patient*: 국내 확진자와 접촉
  - *contact with patient in ooo*: 해외 확진자와 접촉
  - *residence in Wuhan*: 중국 우한 거주
  - *pilgrimage to Israel*: 이스라엘 성지순례
- ***infection_order***: 감염 차수 (n차 감염)
- ***infected_by***: 해당 확진자의 감염원 id
- ***contact_number***: 접촉자 수
- ***confirmed_date***: 확진 일자
- ***released_date***: 퇴원 일자 (격리 해제 일자)
- ***deceased_date***: 사망 일자
- ***state***: 상태
  - *isolated*: 입원 (격리)
  - *released*: 퇴원 (격리 해제)
  - *deceased*: 사망

***

### 2. route 데이터셋 정보
- ***id***: 확진자의 id (n번째 확진자) 
- ***date***: 일자
- ***province***: 특별시/광역시/도
- ***city***: 시/군/구
- ***visit***: 방문한 장소 (종류)
  - *airport*: 공항
  - *hospital_isolated*: 격리된 병원
  - *hospital*: 대형급 병원 또는 보건소
  - *clinic*: 의원급 병원 
  - *hotel*: 호텔
  - *store*: 소형 가게
  - *market*: 대형 마트
  - *restaurant*: 식당
  - *cafe*: 카페 
  - *company*: 회사
  - *bus_terminal*: 버스 터미널
  - *train_station*: 기차역
  - *movie_theater*: 영화관
  - *hair_salon*: 미용실
  - *church*: 교회
  - *etc*: 기타 방문 장소 
- ***latitude***: 위도
- ***longitude***: 경도

***

### 3. time 데이터셋 정보
- ***date***: 일자
- ***test***: 누적 검사 수 (진행 중인 검사 포함)
- ***negative***: 누적 음성 결과 수
- ***confirmed***: 누적 양성 결과 수 (확진)
- ***released***: 누적 격리 해제 수
- ***deceased***: 누적 사망 수
- ***Seoul***: 누적 확진자 수 in 서울 
- ***Busan***: 누적 확진자 수 in 부산
- ***Daegu***: 누적 확진자 수 in 대구
- ***Incheon***: 누적 확진자 수 in 인천
- ***Gwangju***: 누적 확진자 수 in 광주 
- ***Daejeon***: 누적 확진자 수 in 대전
- ***Ulsan***: 누적 확진자 수 in 울산
- ***Sejong***: 누적 확진자 수 in 세종
- ***Gyeonggi-do***: 누적 확진자 수 in 경기도
- ***Gangwon-do***: 누적 확진자 수 in 강원도
- ***Chungcheongbuk-do***: 누적 확진자 수 in 충청북도
- ***Chungcheongnam-do***: 누적 확진자 수 in 충청남도
- ***Jeollabuk-do***: 누적 확진자 수 in 전라북도
- ***Jeollanam-do***: 누적 확진자 수 in 전라남도
- ***Gyeongsangbuk-do***: 누적 확진자 수 in 경상북도
- ***Gyeongsangnam-do***: 누적 확진자 수 in 경상남도
- ***Jeju-do***: 누적 확진자 수 in 제주도

***

### 4. trend 데이터셋 정보
- ***date***: 일자
- ***cold***: '감기' 검색량
- ***flu***: '독감' 검색량
- ***pneumonia***: '폐렴' 검색량
- ***coronavirus***: '코로나바이러스' 검색량

***

### 참고 사이트
- [질병관리본부 공식 홈페이지](http://www.cdc.go.kr/) (정부)
- [코로나바이러스감염증-19 공식 홈페이지](http://ncov.mohw.go.kr/) (정부) 
- [코로나맵](https://coronamap.site/) (민간)
- [코로나19(COVID-19) 실시간 상황판](https://wuhanvirus.kr/) (민간)
- [대한민국의 코로나바이러스감염증-19 유행](https://ko.wikipedia.org/wiki/%EB%8C%80%ED%95%9C%EB%AF%BC%EA%B5%AD%EC%9D%98_%EC%BD%94%EB%A1%9C%EB%82%98%EB%B0%94%EC%9D%B4%EB%9F%AC%EC%8A%A4%EA%B0%90%EC%97%BC%EC%A6%9D-19_%EC%9C%A0%ED%96%89) (위키피디아)
- [코로나바이러스감염증-19/경과/대한민국 확진자 현황](https://namu.wiki/w/%EC%BD%94%EB%A1%9C%EB%82%98%EB%B0%94%EC%9D%B4%EB%9F%AC%EC%8A%A4%EA%B0%90%EC%97%BC%EC%A6%9D-19/%EA%B2%BD%EA%B3%BC/%EB%8C%80%ED%95%9C%EB%AF%BC%EA%B5%AD%20%ED%99%95%EC%A7%84%EC%9E%90%20%ED%98%84%ED%99%A9) (나무위키)
