# 상품 분류를 해보자🛒

Classifying preduct categories using Kakao Arena data

## 1. 문제 정의
**상품의 이미지 정보를 가지고 상품을 대분류로 나눠보자!**   
☑️ 원래 상품에는 대/중/소/세 4가지 분류가 있지만, 이 프로젝트에서는 대분류만 나눠본다!  
☑️ 상품 정보는 상품명, 브랜드,  제조사 등 다양하지만, 이 프로젝트에서는 이미지 정보만 가지고 분류한다!  
<br>
## 2. 데이터
[카카오 아레나](https://arena.kakao.com/c/5) '쇼핑몰 상품 카테고리 분류'에서 제공해주는 데이터셋

- 데이터 크기 : 1,000,000개
- feature :  상품명, 이미지, 브랜드 ...  
<br>
## 3. 모델
**DNN**를 사용한다!  

☑️ Hyperparameter
| Hyperparameter | My Model | 
| :---------- | :---------------------------------------------- |
| # input neurons | 2048(img_feat의 colums) | 
| # hidden layers | 1 |
| # neurons per hidden layer | 100 |
| # output neurons | 57(대분류 갯수) |
| output layer activation | Softmax(1개의 class에만 할당될 수 있어서!) |
| Loss function | Cross entropy(Classification 문제라서!) |  
<br>
## 4. 라이브러리
#### 
    keras  
    pandas  
    numpy  
    matplotlib  
    ...
<br>

## 5. 라이센스
This software is licensed under the **Apache 2** license