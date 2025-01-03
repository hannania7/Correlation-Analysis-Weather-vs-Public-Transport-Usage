
📊 주제

기상 데이터와 대중교통 이용량 상관분석


📌 프로젝트 목표

기상 데이터(기온, 강수량, 풍속, 습도, 적설량)와 대중교통 이용량의 관계를 분석

피어슨 상관계수 및 T-검정을 활용하여 변수 간 관계 파악

출퇴근 시간과 비출퇴근 시간에 따른 승객 수 및 기상 데이터의 차이 비교


📥 수집한 데이터

서울버스 일별 시간대별 승하차 인원.csv

출처: 서울특별시 빅데이터 캠퍼스

데이터: 버스 시간대별 승하차 인원

서울철도 일별 시간대별 승하차 인원.csv

출처: 서울특별시 빅데이터 캠퍼스

데이터: 지하철 시간대별 승하차 인원

OBS_ASOS_TIM_20250104050402.csv

출처: 기상자료개방포털

데이터: 시간대별 기온, 강수량, 풍속, 습도, 적설량


📈 사용한 분석 기법

상관분석 (Pearson Correlation): 기상 변수와 대중교통 이용량 간의 관계 분석

T-검정 (T-Test): 출퇴근 시간과 비출퇴근 시간 간 기상 데이터 차이 비교

데이터 시각화: Seaborn 및 Matplotlib를 활용한 히트맵 시각화


📦 데이터 전처리

데이터 통합: 버스 및 철도 데이터를 병합하여 승차시간구분, 승하차총승객수 기준으로 정리

시간대 변환: 시간 데이터를 정수형으로 변환 (06시 -> 6)

기상 데이터 결합: 시간대 기준으로 기상 데이터와 대중교통 데이터를 병합


📌 결론 및 인사이트

기온이 높을 수록 대중교통 이용량이 증가한다.

습도가 높을 수록 대중교통 이용량이 감소한다.

바람이 많이 불수록 대중교통 이용량이 증가한다.

강수량, 적설량으로는 대중교통 이용량의 추세는 알 수가 없다.

출퇴근 시간과 비출퇴근 시간 간 기상 데이터 차이는 유의미하지 않았음
