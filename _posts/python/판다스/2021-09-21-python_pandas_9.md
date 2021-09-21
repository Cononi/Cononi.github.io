---
title : "[pandas] 시리즈, 데이터프레임의 데이터 처리"
categories:
   - python
tags:
   - Pandas
   - 판다스 시작하기
   - 공부
date: 2021-09-21T23:43:20+09:00 #작성일자
last_modified_at: 2021-09-21 #업데이트날짜.
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
 * [pandas 실습자료 다운로드](https://github.com/easysIT/doit_pandas)
 
 
## ✅ <u>import</u>
	import pandas as ps
	import random

## 💡 <u>주요 내용</u> 
> 1. **dtype** : 데이터의 타입(자료형)을 알 수 있다.
>  
> 2. **to_datetime(컬럼(열), format='형식지정')** : pandas 라이브러리에서 지원하는 메서드로 바꿀 컬럼과 형식을 지정해서 날짜 형식으로 변경합니다. 
>  
> 3. **unpacking** : 여러변수에 각각 값을 할당할 수 있습니다.  
> ex ) A, B = (1, 2) 그러면 각각 A =1 , B = 2 가 됩니다.
>  
> 4. **random** : 랜덤관련 모듈이다. 여기에 대부분의 모듈이 들어있다.
>  
> 5. **seed(개수)** : 난수의 기준을 정해주는 메서드 입니다. 씨드는 특정 값을 기준으로 난수를 생성합니다. 시드기준으로 난수가 생성되기 때문에 동일한 입력을 주면 출력도 동일합니다.
> 
> 6. **shuffle** : 시리즈, 리스트등을 무작위로 섞어줍니다.
>  
> 7. **drop(칼럼, axis=?)** : 해당 데이터를 삭제합니다. axis값이 1이면 칼럼 0이면 행이 삭제 됩니다. 
## ✏️ <u>기억하자. </u>
> ## ✅ random
> 랜덤에 관련된 모든것은 대부분이 랜덤 모듈에 있습니다. 그러므로 무언가 해야한다면 꼭 랜덤이 필요합니다.
>   
> ## ✅ 타입 변경
> 판다스 라이브러리에는 데이터 타입을 바꾸는 여러 가지 방법이 있습니다.  
> 통계나 데이터분석등 여러가지 사항을 할때 미리 데이터 타입을 바꿔주면 훨씬 더 효율이 좋으며. 정확성도 좋아지고 시간도 좋아진다.
>   
> ## ✅ 언패킹
> 파이썬의 가장 큰 장점이다. 여러가지 변수에 각각의 값을 한번에 할당이 가능하다.
> 
## 💭 <u>오늘 나의 생각</u>
> 오늘도 좋은것을 알아간다. 생각하면 할수록 배울수록 활용도나 여러 접점들을 고려하니 확실히 다용성이 높아졌다.
  
## ❌ 실수 요인
없음.

## <u>📖 <u>실습 Code</u>
<script src="https://gist.github.com/Cononi/3867eb37caea3fed829f781bf4250925.js"></script>