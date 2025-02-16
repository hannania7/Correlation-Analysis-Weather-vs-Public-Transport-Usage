📊 계절별 기상 데이터와 대중교통 이용량 상관 분석

프로젝트 개요

본 프로젝트는 서울시 버스 및 철도 대중교통 이용량과 기상 데이터를 분석하여 계절별로 대중교통 이용량과 기상 변수 간의 상관관계를 파악하는 것을 목표로 합니다. 이를 위해 다음과 같은 단계를 수행하였습니다.

📂 데이터 설명

사용 데이터:

서울버스 일별 시간대별 승하차 인원 데이터

서울철도 일별 시간대별 승하차 인원 데이터

기상 데이터 (OBS_ASOS_TIM)

출처:

서울특별시 열린데이터광장 (data.seoul.go.kr)

기상청 (data.kma.go.kr)

📈 데이터 전처리

데이터 불러오기: CSV 파일을 불러온 후, euc-kr 인코딩을 사용하여 로드

계절 분류: 날짜 데이터를 기준으로 봄, 여름, 가을, 겨울로 계절 분류

시간 변환: 승차시간구분 컬럼을 정수형으로 변환

데이터 결합: 버스와 철도 데이터를 하나의 데이터프레임으로 결합

결측치 제거 및 필터링: 결측치 제거 및 데이터 정제

📊 상관분석

계절별 기상 데이터와 대중교통 이용량 간의 상관관계를 분석하였습니다.

🌸 봄

**풍속(m/s)**만 상관계수 = 0.516, p-value = 0.017로 유의미한 양의 상관관계.

다른 변수들은 통계적으로 유의미하지 않음.

☀️ 여름

모든 기상 변수에서 통계적으로 유의미한 상관관계 없음.

🍂 가을

모든 기상 변수에서 통계적으로 유의미한 상관관계 없음.

❄️ 겨울

모든 기상 변수에서 통계적으로 유의미한 상관관계 없음.

✅ 결론: 봄의 풍속이 유일하게 대중교통 이용량과 유의미한 상관관계를 보였습니다.

📊 T-검정 (출퇴근 시간 vs 비출퇴근 시간)

출퇴근 시간과 비출퇴근 시간의 기상 데이터 차이를 검정한 결과, 모든 계절에서 p-value > 0.05로 유의미한 차이가 없음을 확인하였습니다.

📊 단순회귀분석 (봄 - 풍속 기준)

🌸 봄

풍속이 1m/s 증가할 때, 대중교통 이용량은 약 평균적으로 43.18% 증가하는 것으로 나타났습니다. ​

다른 변수는 유의미한 영향을 보이지 않음.

✅ 결론: 봄의 풍속이 대중교통 이용량에 유의미한 영향을 미치는 유일한 변수로 나타남.

📌 종합 결론

**풍속(m/s)**만 봄에 대중교통 이용량과 유의미한 양의 상관관계를 보임.

여름, 가을, 겨울에서는 모든 기상 변수가 유의미하지 않은 결과를 보임.

기온, 강수량, 적설량, 습도는 모든 계절에서 유의미하지 않은 상관관계.

