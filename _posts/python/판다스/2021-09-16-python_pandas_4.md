---
title : "[pandas] 간단한 그래프 그리기"
categories:
   - python
tags:
   - Pandas
   - 판다스 시작하기
   - 공부
date: 2021-09-16T23:47:02+09:00 #작성일자
last_modified_at: 2021-09-16 #업데이트날짜.
#toc: true # 퀵메뉴 활성화
#toc_label: "안녕하세요" # 퀵메뉴 이름
#toc_sticky: true # 퀵메뉴 고정할것인지?
# other options
---

 > # 📜 <u>Mac, VS Code에서 작성되었습니다.</u> 
 > ## <u>📌 체크 사항</u> 
 * python 3.8.8 버전
 *  VS Code Extension 확인
	* Python, Pylance, Python Extension Pack, Python for VSCode
 	* 추가 포함 - Rainbow CSV, Visual Studio intelliCode
 *   pip 설치 확인
 	* pip(pip3) install pandas 설치. 
 	* pip(pip3) install matplotlib 설치.
 * [pandas 실습자료 다운로드](https://github.com/easysIT/doit_pandas)
 
 
## ✅ <u>import</u>
	import pandas as ps
	import matplotlib as plt

## 💡 <u>주요 내용</u> 
> 1. **read_csv** : csv파일을 데이터프레임 형식으로 불러옵니다.
>  * read_csv 메서드는 기본적으로 쉼표(,) 기준으로 열이 구분되어 있는 데이터를 불러옵니다.
> 그외 다른 구분으로 데이터를 불러오고 싶으면 sep 속성값으로 구분을 지정해주시면 됩니다.
> 그외에 기본적으로 첫행을 열이름으로 사용합니다.
> 2. **head()** : head() 메서드는 데이터프레임의 가장 앞에있는 5개의 행을 출력하므로 내가 불러온 데이터가 어떤 값을 가지고 있는지 알수 있습니다.
> 	* 반대 되는 값으로 tail() 메서드가 있습니다. 최하위 5개의 행을 출력합니다.
> 3. **type(데이터)** : type은 괄호() 안에 타입을 알고 싶은 데이터를 넣으면 어떤 타입인지 확인 가능합니다.
> 4. **groupby 메서드** : 특정 데이터를 기준으로 그룹화하여 새로운 데이터 프레임을 만듭니다. 
>   
> 5. **mean() 메서드** : 해당 데이터의 평균값을 구합니다.
>   
> 6. **plot(x,y) 메서드** : 메서드에 하나의 숫자 리스트를 입력함으로써 그래프가 그려집니다.
>   
> 7. **show()** : plot으로 그려진 그래프를 화면에 띄워 시각화 해줍니다.

## ✏️ <u>기억하자. </u>
> ## ✅ matplotlib 라이브러리
> matplotlib 라이브러리는 데이터를 그래프로 시각화 시켜주는 라이브러리다.
> 파이썬에서 가장 널리 쓰이는 그래프 그리는 라이브러리로 활용도가 아주 좋다.
> 한눈에 파악을 할 수 있고 내 입맛에 맞게 여러가지 그래프를 그릴 수 있다.
> 접근성이 아주 좋고 쉽고 간편하다는 큰 장점이 있다.

## 💭 <u>오늘 나의 생각</u>
> 간단한 그래프를 그려봤는데 그렇게 어려운건 없는거 같다.  
> 물론 뭐 지금 처음 해봐서 그렇겠지만 간간하게 plot(x,y) 행열에 데이터를
> 넣어주면 빠르게 내가 원하는 정보가 나온다는 것이다.  
> 종합적으로 생각해보면 데이터를 시각화하는건 어렵지 않다는걸 알 수있다.  
> 그럼 무엇이 어려운가? 고민해봤더니 역시 전처리,정제과정등이 어려운거 같다.
  
## ❌ 실수 요인
없음.

## <u>📖 <u>실습 Code</u>
<script src="https://gist.github.com/Cononi/3e3e102f7b1497bf9061e180b28e2446.js"></script>