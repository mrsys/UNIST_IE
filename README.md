# UNIST_IE

이 저장소(Repository)는 UNIST에서의 프로젝트들이 저장되어있습니다.
(기본적인 학사과정과 project가 영어로 진행되어 자료는 영문으로 되어있습니다.)

목차
========

 1) 금융공학 연구보조
    1. AI를 이용한 생애주기별 질병 치료비 예측
    2. BC카드 데이터를 이용한 분석 프로젝트   
  
 2) 데이터 마이닝
 

## 1) 금융공학 연구보조

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

해당 프로젝트는 BC카드의 실제 사용 내역 데이터를 이용하여 유의미한 분석을 해
보는 프로젝트 또한 진행하였습니다. 
1) BC카드에서 제공한 개인의 가맹점 결제기록 데이터 전처리
2) feature가 매우 다양해를 autoencoder를 통해 차원을 축소
3) N2D clustering 기법을 적용하여 군집화
4) 클러스터간의 특징, 월별 특징, transition matrix을 보며 의미도출

##### 1) 진행
+ 1. 업종의 소분류 되어진 자료를 묶어서 재분류 및 전처리 : [1. 전처리.ipynb ](https://github.com/mrsys/UNIST_IE/blob/main/%5B%EA%B8%88%EC%9C%B5%EA%B3%B5%ED%95%99%20%EC%97%B0%EA%B5%AC%EB%B3%B4%EC%A1%B0%5D%20%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8/BC%EC%B9%B4%EB%93%9C%20%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%A5%BC%20%EC%9D%B4%EC%9A%A9%ED%95%9C%20%EB%B6%84%EC%84%9D%20%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8/python%20code/1.%20%EC%A0%84%EC%B2%98%EB%A6%AC.ipynb) 
+ 2. 2019년 4월 부터 2020년 4월까지의 결제 데이터이므로 전부 합쳐서 전처리 적용
 : [2.월별 데이터 합치기.ipynb](https://github.com/mrsys/UNIST_IE/blob/main/%5B%EA%B8%88%EC%9C%B5%EA%B3%B5%ED%95%99%20%EC%97%B0%EA%B5%AC%EB%B3%B4%EC%A1%B0%5D%20%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8/BC%EC%B9%B4%EB%93%9C%20%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%A5%BC%20%EC%9D%B4%EC%9A%A9%ED%95%9C%20%EB%B6%84%EC%84%9D%20%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8/python%20code/2.%20%EC%9B%94%EB%B3%84%20%EB%8D%B0%EC%9D%B4%ED%84%B0%20%ED%95%A9%EC%B9%98%EA%B8%B0.ipynb)
+ 3. Autoencoder를 거치고 GMM을 이용하여 clustering하였다. 그리고 cluster별로 어떤 업종이 많은지 (어떤 구매 유형을 띄는지)와 transition matrix를 통해 구매이동 분석 :  [3. 클러스터링.ipynb](https://github.com/mrsys/UNIST_IE/blob/main/%5B%EA%B8%88%EC%9C%B5%EA%B3%B5%ED%95%99%20%EC%97%B0%EA%B5%AC%EB%B3%B4%EC%A1%B0%5D%20%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8/BC%EC%B9%B4%EB%93%9C%20%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%A5%BC%20%EC%9D%B4%EC%9A%A9%ED%95%9C%20%EB%B6%84%EC%84%9D%20%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8/python%20code/3.%20%ED%81%B4%EB%9F%AC%EC%8A%A4%ED%84%B0%EB%A7%81.ipynb)
+ 4. 2019년 1월부터 2020년 4월까지 클러스터 비중과 양이 얼마나 변하였는지를 관찰하여 코로나 전후로 소비 패턴에서 유의미한 변화를 결과로 도출 [4. 월별분석_클러스터.ipynb](https://github.com/mrsys/UNIST_IE/blob/main/%5B%EA%B8%88%EC%9C%B5%EA%B3%B5%ED%95%99%20%EC%97%B0%EA%B5%AC%EB%B3%B4%EC%A1%B0%5D%20%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8/BC%EC%B9%B4%EB%93%9C%20%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%A5%BC%20%EC%9D%B4%EC%9A%A9%ED%95%9C%20%EB%B6%84%EC%84%9D%20%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8/python%20code/4.%20%EC%9B%94%EB%B3%84%EB%B6%84%EC%84%9D_%ED%81%B4%EB%9F%AC%EC%8A%A4%ED%84%B0.ipynb)


##### 2) 관련 문서
+ 프로젝트 진행 후 발표 자료 : [BC카드 데이터를 이용한 분석 프로젝트.pdf](https://github.com/mrsys/UNIST_IE/blob/main/%5B%EA%B8%88%EC%9C%B5%EA%B3%B5%ED%95%99%20%EC%97%B0%EA%B5%AC%EB%B3%B4%EC%A1%B0%5D%20%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8/BC%EC%B9%B4%EB%93%9C%20%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%A5%BC%20%EC%9D%B4%EC%9A%A9%ED%95%9C%20%EB%B6%84%EC%84%9D%20%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8/BC%EC%B9%B4%EB%93%9C%20%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%A5%BC%20%EC%9D%B4%EC%9A%A9%ED%95%9C%20%EB%B6%84%EC%84%9D%20%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8.pdf)
+ 참고한 논문 : [N2d(not too) deep clustering via clustering the local manifold of an autoencoded embedding.pdf](https://github.com/mrsys/UNIST_IE/blob/main/%5B%EA%B8%88%EC%9C%B5%EA%B3%B5%ED%95%99%20%EC%97%B0%EA%B5%AC%EB%B3%B4%EC%A1%B0%5D%20%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8/BC%EC%B9%B4%EB%93%9C%20%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%A5%BC%20%EC%9D%B4%EC%9A%A9%ED%95%9C%20%EB%B6%84%EC%84%9D%20%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8/python%20code/N2d(not%20too)%20deep%20clustering%20via%20clustering%20the%20local%20manifold%20of%20an%20autoencoded%20embedding.pdf)

### 2) 데이터 마이닝
Kaggle에서 진행 되었던 타이타닉 생존자 예측 Task를 Final project로 진행하였습니다.
머신러닝 입문시기에 접했던 project로 당시에는 많은 배움을 얻을 수 있었습니다.
+ Project Guideline : [IE30301_Term Project_Guideline.pdf](https://github.com/mrsys/UNIST_IE/blob/main/%5B%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%A7%88%EC%9D%B4%EB%8B%9D%5D%20Final%20Project%20-%20%ED%83%80%EC%9D%B4%ED%83%80%EB%8B%89%20%EC%83%9D%EC%A1%B4%EC%9E%90%20%EC%98%88%EC%B8%A1/%EC%A3%BC%EC%96%B4%EC%A7%84%20%EB%AC%B8%EC%A0%9C%20%EC%9E%90%EB%A3%8C/IE30301_Term%20Project_Guideline.pdf)
* Final project : [20151640_FinalProject_SongYoungSeok.ipynb](https://github.com/mrsys/UNIST_IE/blob/main/%5B%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%A7%88%EC%9D%B4%EB%8B%9D%5D%20Final%20Project%20-%20%ED%83%80%EC%9D%B4%ED%83%80%EB%8B%89%20%EC%83%9D%EC%A1%B4%EC%9E%90%20%EC%98%88%EC%B8%A1/20151640_FinalProject_SongYoungSeok.ipynb)
* Report : [20151640_FinalReport_SongYoungSeok.docx](https://github.com/mrsys/UNIST_IE/blob/main/%5B%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%A7%88%EC%9D%B4%EB%8B%9D%5D%20Final%20Project%20-%20%ED%83%80%EC%9D%B4%ED%83%80%EB%8B%89%20%EC%83%9D%EC%A1%B4%EC%9E%90%20%EC%98%88%EC%B8%A1/~%24151640_FinalReport_SongYoungSeok.docx)
