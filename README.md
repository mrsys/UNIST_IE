# UNIST_IE

### 이 저장소(Repository)는 UNIST에서의 프로젝트들이 저장되어있습니다.
(기본적인 학사과정과 project가 영어로 진행되어 자료는 영문으로 되어있습니다.)

Contents
========

 * [금융공학 연구보조](#금융공학연구보조)
    * [1. AI를 이용한 생애주기별 질병 치료비 예측](#1.AI를이용한생애주기별질병치료비예측)
    * [2. BC카드 데이터를 이용한 분석 프로젝트](2.BC카드데이터를이용한분석프로젝트)   
 * 
 * [데이터 마이닝](#데이터마이닝)
 

## 금융공학 연구보조

자료는 2021.03.01 ~ 2021.08.31 (6개월) 기간동안 UNIST Financial Engineering Lab의 연구보조원을 하면서 수행한 업무의 일부입니다.

### 1. AI를 이용한 생애주기별 질병 치료비 예측
해당 프로젝트는 데이터 마이닝 연구실과 협업하여 <인공지능을 기반으로 생애주기 의료비 관리>라는 주제로 진행되었습니다. 
1) 환자의 개인 데이터를 국민건강보험공단으로부터 얻어 개인이 걸릴 수 있는 질병을 미리 예측
2) 그에 따른 비용은 얼마나 들지를 계산하기 위한 연구
3) 파이썬을 이용해 개인의 의료데이터와 질병데이터의 명세서를 다방면으로 시각화
4) 비용을 계산하기 위해 Tree계열의 (xgboost, randomforest 등)의 시도

##### 1) 제안서
+ AI 보급 확산 지원 사업 제안서입니다.
+ [사업 제안서](https://github.com/mrsys/UNIST_IE/blob/main/%5B%EA%B8%88%EC%9C%B5%EA%B3%B5%ED%95%99%20%EC%97%B0%EA%B5%AC%EB%B3%B4%EC%A1%B0%5D%20%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8/AI%EB%A5%BC%20%EC%9D%B4%EC%9A%A9%ED%95%9C%20%EC%83%9D%EC%95%A0%EC%A3%BC%EA%B8%B0%EB%B3%84%20%EC%A7%88%EB%B3%91%20%EC%B9%98%EB%A3%8C%EB%B9%84%20%EC%98%88%EC%B8%A1/%5B%EC%A0%9C%EC%95%88%EC%84%9C%5DAI%20%EB%B3%B4%EA%B8%89%ED%99%95%EC%82%B0%EC%A7%80%EC%9B%90%EC%82%AC%EC%97%85%20-%20%EC%9D%B8%EA%B3%B5%EC%A7%80%EB%8A%A5%20%EA%B8%B0%EB%B0%98%20%EC%83%9D%EC%95%A0%EC%A3%BC%EA%B8%B0%20%EC%9D%98%EB%A3%8C%EB%B9%84%20%EA%B4%80%EB%A6%AC(%EC%88%98%EC%A0%95%EA%B3%B5%EA%B0%9C%EC%9A%A9).pdf) (일부 수정 공개)

##### 2) 진행
+ 사용되어진 [데모 데이터](https://github.com/mrsys/UNIST_IE/tree/main/%5B%EA%B8%88%EC%9C%B5%EA%B3%B5%ED%95%99%20%EC%97%B0%EA%B5%AC%EB%B3%B4%EC%A1%B0%5D%20%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8/AI%EB%A5%BC%20%EC%9D%B4%EC%9A%A9%ED%95%9C%20%EC%83%9D%EC%95%A0%EC%A3%BC%EA%B8%B0%EB%B3%84%20%EC%A7%88%EB%B3%91%20%EC%B9%98%EB%A3%8C%EB%B9%84%20%EC%98%88%EC%B8%A1/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20%EC%A7%84%ED%96%89%EC%9D%98%20%EC%9D%BC%EB%B6%80%20%EC%9E%90%EB%A3%8C/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20%EB%B6%84%EC%84%9D%EC%9D%84%20%EC%9C%84%ED%95%9C%20%EB%8D%B0%EB%AA%A8%20%EB%8D%B0%EC%9D%B4%ED%84%B0)는 건강보험 심사평가원에서 환자의 질병 코드와 비용등의 자료가 들은 엑셀 파일입니다
+ 예시로 올려둔 코드 파일은 질병의 분포와 질병 치료비를 주로 파악하는 시기에 진행한 코드입니다.
+ [7월 2주차](https://github.com/mrsys/UNIST_IE/blob/main/%5B%EA%B8%88%EC%9C%B5%EA%B3%B5%ED%95%99%20%EC%97%B0%EA%B5%AC%EB%B3%B4%EC%A1%B0%5D%20%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8/AI%EB%A5%BC%20%EC%9D%B4%EC%9A%A9%ED%95%9C%20%EC%83%9D%EC%95%A0%EC%A3%BC%EA%B8%B0%EB%B3%84%20%EC%A7%88%EB%B3%91%20%EC%B9%98%EB%A3%8C%EB%B9%84%20%EC%98%88%EC%B8%A1/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20%EC%A7%84%ED%96%89%EC%9D%98%20%EC%9D%BC%EB%B6%80%20%EC%9E%90%EB%A3%8C/%5B7%EC%9B%94_2%EC%A3%BC%EC%B0%A8%5D_Price_prediction.ipynb)자료에는 질병 치료 횟수를 파악해 일반적으,로 자주 걸리는 질병의 치료비 모델을 만들고자 시도하였습니다.
+ [7월 3주차](https://github.com/mrsys/UNIST_IE/blob/main/%5B%EA%B8%88%EC%9C%B5%EA%B3%B5%ED%95%99%20%EC%97%B0%EA%B5%AC%EB%B3%B4%EC%A1%B0%5D%20%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8/AI%EB%A5%BC%20%EC%9D%B4%EC%9A%A9%ED%95%9C%20%EC%83%9D%EC%95%A0%EC%A3%BC%EA%B8%B0%EB%B3%84%20%EC%A7%88%EB%B3%91%20%EC%B9%98%EB%A3%8C%EB%B9%84%20%EC%98%88%EC%B8%A1/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20%EC%A7%84%ED%96%89%EC%9D%98%20%EC%9D%BC%EB%B6%80%20%EC%9E%90%EB%A3%8C/%5B7%EC%9B%94_3%EC%A3%BC%EC%B0%A8%5D_Price_prediction.ipynb)치료비의 빈도를 seaborn그래프를 통해 시각화하여 데이터 EDA를 하고자 하였습니다.

##### 3) 보고서
(1) 프로젝트 진행해 필요한 데이터도 직접 구하기 위해 조사하는 단계
(2)데이터를 통해 질병의 치료비를 분석하는 것과 유사한 사례의 논문들을 찾아 리뷰
+ 초기 3개월 진행 보고서 :  [보고서](https://github.com/mrsys/UNIST_IE/blob/main/%5B%EA%B8%88%EC%9C%B5%EA%B3%B5%ED%95%99%20%EC%97%B0%EA%B5%AC%EB%B3%B4%EC%A1%B0%5D%20%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8/AI%EB%A5%BC%20%EC%9D%B4%EC%9A%A9%ED%95%9C%20%EC%83%9D%EC%95%A0%EC%A3%BC%EA%B8%B0%EB%B3%84%20%EC%A7%88%EB%B3%91%20%EC%B9%98%EB%A3%8C%EB%B9%84%20%EC%98%88%EC%B8%A1/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20%EC%A7%84%ED%96%89%EC%9D%98%20%EC%9D%BC%EB%B6%80%20%EC%9E%90%EB%A3%8C/%5B2021-1%ED%95%99%EA%B8%B0%5DYoungseok_Song_Research%20Internship%20Report.pdf)

### 2. BC카드 데이터를 이용한 분석 프로젝트 

해당 프로젝트는 데이터 마이닝 연구실과 협업하여 <인공지능을 기반으로 생애주기 의료비 관리>라는 주제로 진행되었습니다. 
1) 환자의 개인 데이터를 국민건강보험공단으로부터 얻어 개인이 걸릴 수 있는 질병을 미리 예측
2) 그에 따른 비용은 얼마나 들지를 계산하기 위한 연구
3) 파이썬을 이용해 개인의 의료데이터와 질병데이터의 명세서를 다방면으로 시각화
4) 비용을 계산하기 위해 Tree계열의 (xgboost, randomforest 등)의 시도

##### 1) 제안서
+ AI 보급 확산 지원 사업 제안서입니다.
+ [사업 제안서](https://github.com/mrsys/UNIST_IE/blob/main/%5B%EA%B8%88%EC%9C%B5%EA%B3%B5%ED%95%99%20%EC%97%B0%EA%B5%AC%EB%B3%B4%EC%A1%B0%5D%20%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8/AI%EB%A5%BC%20%EC%9D%B4%EC%9A%A9%ED%95%9C%20%EC%83%9D%EC%95%A0%EC%A3%BC%EA%B8%B0%EB%B3%84%20%EC%A7%88%EB%B3%91%20%EC%B9%98%EB%A3%8C%EB%B9%84%20%EC%98%88%EC%B8%A1/%5B%EC%A0%9C%EC%95%88%EC%84%9C%5DAI%20%EB%B3%B4%EA%B8%89%ED%99%95%EC%82%B0%EC%A7%80%EC%9B%90%EC%82%AC%EC%97%85%20-%20%EC%9D%B8%EA%B3%B5%EC%A7%80%EB%8A%A5%20%EA%B8%B0%EB%B0%98%20%EC%83%9D%EC%95%A0%EC%A3%BC%EA%B8%B0%20%EC%9D%98%EB%A3%8C%EB%B9%84%20%EA%B4%80%EB%A6%AC(%EC%88%98%EC%A0%95%EA%B3%B5%EA%B0%9C%EC%9A%A9).pdf) (일부 수정 공개)

##### 2) 진행
+ 사용되어진 [데모 데이터](https://github.com/mrsys/UNIST_IE/tree/main/%5B%EA%B8%88%EC%9C%B5%EA%B3%B5%ED%95%99%20%EC%97%B0%EA%B5%AC%EB%B3%B4%EC%A1%B0%5D%20%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8/AI%EB%A5%BC%20%EC%9D%B4%EC%9A%A9%ED%95%9C%20%EC%83%9D%EC%95%A0%EC%A3%BC%EA%B8%B0%EB%B3%84%20%EC%A7%88%EB%B3%91%20%EC%B9%98%EB%A3%8C%EB%B9%84%20%EC%98%88%EC%B8%A1/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20%EC%A7%84%ED%96%89%EC%9D%98%20%EC%9D%BC%EB%B6%80%20%EC%9E%90%EB%A3%8C/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20%EB%B6%84%EC%84%9D%EC%9D%84%20%EC%9C%84%ED%95%9C%20%EB%8D%B0%EB%AA%A8%20%EB%8D%B0%EC%9D%B4%ED%84%B0)는 건강보험 심사평가원에서 환자의 질병 코드와 비용등의 자료가 들은 엑셀 파일입니다
+ 예시로 올려둔 코드 파일은 질병의 분포와 질병 치료비를 주로 파악하는 시기에 진행한 코드입니다.
+ [7월 2주차](https://github.com/mrsys/UNIST_IE/blob/main/%5B%EA%B8%88%EC%9C%B5%EA%B3%B5%ED%95%99%20%EC%97%B0%EA%B5%AC%EB%B3%B4%EC%A1%B0%5D%20%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8/AI%EB%A5%BC%20%EC%9D%B4%EC%9A%A9%ED%95%9C%20%EC%83%9D%EC%95%A0%EC%A3%BC%EA%B8%B0%EB%B3%84%20%EC%A7%88%EB%B3%91%20%EC%B9%98%EB%A3%8C%EB%B9%84%20%EC%98%88%EC%B8%A1/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20%EC%A7%84%ED%96%89%EC%9D%98%20%EC%9D%BC%EB%B6%80%20%EC%9E%90%EB%A3%8C/%5B7%EC%9B%94_2%EC%A3%BC%EC%B0%A8%5D_Price_prediction.ipynb)자료에는 질병 치료 횟수를 파악해 일반적으,로 자주 걸리는 질병의 치료비 모델을 만들고자 시도하였습니다.
+ [7월 3주차](https://github.com/mrsys/UNIST_IE/blob/main/%5B%EA%B8%88%EC%9C%B5%EA%B3%B5%ED%95%99%20%EC%97%B0%EA%B5%AC%EB%B3%B4%EC%A1%B0%5D%20%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8/AI%EB%A5%BC%20%EC%9D%B4%EC%9A%A9%ED%95%9C%20%EC%83%9D%EC%95%A0%EC%A3%BC%EA%B8%B0%EB%B3%84%20%EC%A7%88%EB%B3%91%20%EC%B9%98%EB%A3%8C%EB%B9%84%20%EC%98%88%EC%B8%A1/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20%EC%A7%84%ED%96%89%EC%9D%98%20%EC%9D%BC%EB%B6%80%20%EC%9E%90%EB%A3%8C/%5B7%EC%9B%94_3%EC%A3%BC%EC%B0%A8%5D_Price_prediction.ipynb)치료비의 빈도를 seaborn그래프를 통해 시각화하여 데이터 EDA를 하고자 하였습니다.

##### 3) 보고서
(1) 프로젝트 진행해 필요한 데이터도 직접 구하기 위해 조사하는 단계
(2)데이터를 통해 질병의 치료비를 분석하는 것과 유사한 사례의 논문들을 찾아 리뷰
+ 초기 3개월 진행 보고서 :  [보고서](https://github.com/mrsys/UNIST_IE/blob/main/%5B%EA%B8%88%EC%9C%B5%EA%B3%B5%ED%95%99%20%EC%97%B0%EA%B5%AC%EB%B3%B4%EC%A1%B0%5D%20%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8/AI%EB%A5%BC%20%EC%9D%B4%EC%9A%A9%ED%95%9C%20%EC%83%9D%EC%95%A0%EC%A3%BC%EA%B8%B0%EB%B3%84%20%EC%A7%88%EB%B3%91%20%EC%B9%98%EB%A3%8C%EB%B9%84%20%EC%98%88%EC%B8%A1/%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20%EC%A7%84%ED%96%89%EC%9D%98%20%EC%9D%BC%EB%B6%80%20%EC%9E%90%EB%A3%8C/%5B2021-1%ED%95%99%EA%B8%B0%5DYoungseok_Song_Research%20Internship%20Report.pdf)



### 데이터 마이닝
