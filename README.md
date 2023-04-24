수평선 (구분선, 수평선을 만들려면 - or * or _을 3개를 입력)

---

***

___


*기울기1*
_기울기2_




# 글자크기1
## 글자크기2
### 글자크기3
#### 글자크기4




# 소스코드블록
```c
for i in range(0,5):
   print(i)
```


# 코드블록2

하나

    둘(탭, 스페이스바로 이부분 회색 될 때까지 들여쓰기)

셋



# 링크걸기
[링크를걸겠습니다.](https://www.naver.com/)

# 순서없는목록

+ 목록1
  + 목록 1-1
    + 목록 1-1-1

* 목록1
  * 목록 1-1
    * 목록 1-1-1

- 목록1
  - 목록 1-1
    - 목록 1-1-1





# BlockQuote

> "알파코1기" - 올림
>> "알파코2기" - 올림
>>> "알파코3기" - 올림





# 숫자목록 출력
1. 하나
2. 둘
3. 셋





# 테이블 만들기

프로젝트목록 | 일자 | 사용기술 | 링크
------------|------|-------|-----|
이미지 생성 | 2021 | GAN | [GAN 프로젝트 링크](https://github.com/shiny0510/FewShot_GAN-Unet3D)
객체탐지 | 2022 | YOLO | [링크를걸겠습니다.](https://github.com/shiny0510/pycaret)




# 강조
**이 부분을 집중해주세요!** 감사합니다
__이 부분을 집중해주세요!__ 감사합니다


x

# 취소선
~~취소선~~


# 이미지 넣기 

<!-- tip) 이미지 크기 조절 -->
<!-- <img src="이미지 링크" width="너비 " height="높이"> -->
ex)
<img src="https://user-images.githubusercontent.com/31477658/85016059-f962aa80-b1a3-11ea-8c91-dacba2666b78.jpeg" width="700" height="370">

![텍스트](이미지 링크 주소) <br>
![CNN-Figure-02](https://user-images.githubusercontent.com/85111065/173890872-1592710c-4711-42a0-803c-6d37ebcd2b3e.png)


<img src="./APOD.jpg" width="300"> <br>

<img src="./APOD.jpg" width="100" height="100">



# 문자열 개행
방법1. 문장 마지막에 스페이스 두 번 이상 입력  
방법2. html <br> 태그를 사용 
방법2. html <br> 태그를 사용 


다음과 같이 체크박스를 표현 할 수 있습니다. 
* [x] 체크박스
* [ ] 빈 체크박스
* [ ] 빈 체크박스




<!-- 참고: https://shields.io/ -->

<!-- <img src="https://img.shields.io/badge/이름-색상코드?style=flat-square&logo=로고명&logoColor=로고색"/> -->

# Badge (뱃지)
기술 스택이나 사용 툴 등을 간결하게 표현하고 싶을 때
인스타, 블로그 등 다양한 바로가기 링크들을 깔끔하게 나타내고 싶을때
로고와 공식컬러를 포함한 예쁜 아이콘 뱃지

<img src="https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=white"/>


# 뱃지에 링크걸기

<!-- <a href="링크"><img src="위에있는뱃지코드"/></a>  -->

<a href="https://www.naver.com/"><img src="https://img.shields.io/badge/Velog-3DDC84?style=flat-square&logo=Blogger&logoColor=white"/></a>





# 실습 


# Test 모델을 이용한 Test 도출

* Github Url: https://github.com/shiny0510/FewShot_GAN-Unet3D (꼭! 하이퍼링크)

* requirement: pandas, numpy, torch, seaborn, matplotlib

1. 수행 기관:  부트캠프 (역할: Method 튜닝, 전처리, 팀장, 트러블 슈팅)

2. 데이터: 환자 데이터 10000개, 정상인 데이터 20만개

3. Method:  전처리: 이미지 Normalize + MixUp(Augmentation) + Denosing               
            모델: F-AnoGAN (Medical Image Analysis, 2019.05)
	         optimizer: Adam 
            loss: L1 loss
	<img src="https://user-images.githubusercontent.com/85111065/173891979-c4353c43-345f-4cec-8a4f-d818e00d97f5.png" width="500">

4. 결과: <br>

* Anomaly detection: <br>
	<img src="https://user-images.githubusercontent.com/85111065/173892034-27a00459-f7af-4ed7-877c-45baa59f2a10.png" width="500" >

* Acc: <br>
	<img src="https://user-images.githubusercontent.com/85111065/173892050-d0406ab4-e31b-43c1-bfa7-cd121428e1aa.png" width="500" >

* 프로젝트 수행 중 문제: 정상인 데이터에서도 미세한 Anomaly가 검출되어서, 환자로 분류하는 threshold를
    높혀줌으로써 정확히 분류될 수 있도록 조치하였으며, 데이터가 부족하여 오픈데이터를 다수 활용.

5. 참고: Schlegl, Thomas, et al. "f-AnoGAN: Fast unsupervised anomaly detection with generative 
    adversarial networks." Medical image analysis 54 (2019): 30-44.

