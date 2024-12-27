# Gwangingu_bigdata

## 프로젝트 목표 및 설명
광진구에 대해서 2024년에 현황과 사회문제에 대해서 공공데이터 및 민간데이터를 다방면으로 분석하여 체감도 높은 정책 아이디어를 발굴하고, 데이터 분석에 기반을 두어 공익적 아이디어를 제안하는 문화를 확산하는 것이 목표입니다. 저희는 이 프로젝트의 주제를 광진구 쓰레기통의 실태조사와 함께 최적의 쓰레기통의 장소을 어디로 하면 좋을지 예상외 되는 곳을 탐색하는 것을 주제로 프로젝트를 하였습니다.

## 프로젝트 과정
**전처리 이후 분석 파이프라인**

1. 전처리한 데이터를 활용하여 회귀분석 진행(독립변수=버스 정류장 수, 지하철역 수, 생활인구 수, 집객시설 수/종속변수=쓰레기통 수)
2. 종속변수에 유의미한 영향을 미치는 변수 선정 후 해당 변수들을 활용하여 군집분석 실시(ex. 버스 정류장 수와 집객시설 수가 쓰레기통 수에 유의한 영향을 미친다면, 두 가지 변수를 가지고 군집분석 진행)
3. 군집화 결과에 따라 우선적으로 쓰레기통을 설치할 행정동 선정(ex. 광장동, 화양동, 군자동 선정, 이 군집의 경우 버스정류장과 집객시설 수 비중이 둘 다 높았음)
4. 선정된 행정동을 바탕으로 좌표에 기반한 세부 분석 진행(태블로와 거리뷰 활용)

4-1 쓰레기통에 영향을 미치는 변수들을 시각화(ex. 버스 정류장 위치와 집객시설 위치를 시각화)

4-2 쓰레기통 위치를 시각화한 후, 각 쓰레기통 위치를 기점으로 반경을 설정하여 각 쓰레기통이 담당할 수 있는 면적을 시각화

(여기서 반경은 서울시 면적을 서울시 쓰레기통 개수로 나눈 값을 사용,  추후 변경 가능)

4-3 쓰레기통이 담당하지 못하는 구역에 대해 거리뷰를 활용하여 쓰레기통 설치 솔루션 제안(ex. 광장동의 경우 버스 정류장 비중이 높았기에 컵 수거함 설치 고려, 화양동은 집객시설 수가 많았기에 적재 용량이 큰 쓰레기통을 설치하는 것이 적절)

우리의 Task
1. 쓰레기통을 설치할 입지 선정

> 행정동으로 분류된 데이터
상권분석데이터 : 집객시설수
생활인구데이터 : 유동인구를 대체
버스, 지하철 정류장 수
> 
1. 구체적인 쓰레기통 위치 선정

> 위치가 포함된 데이터
가로쓰레기통 데이터
지하철역
버스정류장
공원
> 

+차후 인허가 데이터를 추가

## 프로젝트 결과
ex) 버스 - 생활인구 연관 군집 결과 시각화<br>

ex) 지하철 - 생활인구 연관 군집 결과 시각화<br>
