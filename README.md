# Dataset
* 데이콘, 영화 리뷰 감성분석 경진대회 데이터셋

  * train.csv : 학습 데이터
    * id: 데이터의 id값
    * document: 리뷰 내용
    * label: 리뷰의 감성 종류


  * test.csv : 테스트 데이터
    * id: 데이터의 id값
    * document: 리뷰 내용

# Preprocess

* 특수문자 제거
* 띄어쓰기 (pykospacing)
* 형태소 분석 (Okt)

# Model
* tfidf + Logistic Regression
  * 특수문자 제거: 0.882 (Accuracy)
  * 띄어쓰기: 0.88
  * 형태소 분석: 0.88
* tfidf + Random Forest
  * 특수문자 제거: 0.843
  * 띄어쓰기: 0.847
  * 형태소 분석: 0.829
* tfidf + Support Vector Machine
  * 특수문자 제거: 0.885
  * 띄어쓰기: 0.885
  * 형태소 분석: 0.894
* tfidf + Naive Bayes
  * 특수문자 제거: 0.891
  * 띄어쓰기: 0.887
  * 형태소 분석: 0.889

# REFERENCE
* 데이콘, 영화 리뷰 감성분석 경진대회 - 박이삭님 코드공유

