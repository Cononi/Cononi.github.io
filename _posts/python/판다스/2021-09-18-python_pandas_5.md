---
title : "[pandas] 나만의 데이터로 시리즈,데이터프레임 데이터 이해하기!"
categories:
   - python
tags:
   - Pandas
   - 판다스 시작하기
   - 공부
date: 2021-09-18T11:47:41+09:00 #작성일자
last_modified_at: 2021-09-18 #업데이트날짜.
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

## 💡 <u>주요 내용</u> 
> 1. **Series** : 시리즈 메서드에 리스트를 전달하면 시리즈 데이터가 생성됩니다. 
>   
> 2. **DataFrame()** : 데이터프레임 클래스에 딕셔너리를 전달하면 데이터프레임 클래스가 만들어집니다.
>   
> 3. **OrderedDict()** : 딕셔너리는 데이터의 순서를 보장해주지 않습니다. 하지만 그런것을 보안해주는게 있습니다. 바로 순서를 보장하면서 딕셔너리를 전달할 수 있는 OrderedDict 클래스를 사용해야 합니다.

## ✏️ <u>기억하자. </u>
> ## ✅ Series
> 시리즈는 메서드에 데이터를 전달하면서 시리즈 데이터가 생성된다.  
> 그리고 시리즈는 데이터를 생성할때 인덱스를 자동으로 부여해 0부터 시작하게 된다.  
> 인덱스를 특정 문장으로 바꿀 수 있는데 그때 활용하는것이  
> 시리즈내에 있는 index=[''] 인자다.  
> 리스트형식으로 리스트 값을 전달하면 자연스럽게 부여된다.  
> 인덱스 문장데이터, 시리즈데이터가 따로 있는 파일이 있다고 하면  
> 파일을 불러들여 시리즈 데이터에 인덱스를 부여해주면 된다.  
> 이러한 방식을 통해 내가 원하는 가공된 데이터를 만들수 있다. 
>   
> ####시리즈  데이터
> 
> | 0  |  banana| 
> |:--:|:--:|
> | 1     |  42
>   
> ####시리즈 인덱스 변경후
> 
> |Person     |    Wes McKinney
> |:--:|:--:|
>| Who    |   Creator of Pandas
>  
> ## ✅ DataFrame
> 데이터프레임 클래스는 딕셔너리를 통해 인자값을 전달해주면 자동으로 데이터프레임 클래스가
> 만들어진다. 그리고 인자 전달에 따라 자동으로 인덱스도 생성 된다.  
> 데이터 프레임도 인덱스를 문장으로 바꿀 수 있으며, 컬럼순서도 바꿀수 있다.
> 
> #### 데이터 프레임
> | Name   | Occupation  |      Born   |     Died Age
> |:--:|:--:|:--:|:--:|
> |0|  Rosaline Franklin      Chemist | 1920-07-25  |1958-04-16  37
> |1  |   William Gosset Statistician|  1876-06-13 | 1937-10-16  61
> 
>#### 데이터 프레임 인덱스 및 컬럼순서 변경
>
> | Name   | Occupation  |      Born   |     Died Age
> |:--:|:--:|:--:|:--:|
> |Rosaline Franklin|  Rosaline Franklin      Chemist | 1920-07-25  |1958-04-16  37
> |William Gosset |   William Gosset Statistician|  1876-06-13 | 1937-10-16  61
>  
> ## ✅ collections 라이브러리에 OrderedDict 클래스
> 딕셔너리를 순서를 보장하지 않습니다. 하지만 collections 라이브러리의  OrderedDict 클래스를 이용하면 딕셔너리에 선수를 보장할 수 있게 됩니다. 그렇게 데이터프레임으로 만들면 데이터의 순서를 유지하면서 데이터프레임 생성이 가능해집니다. 

## 💭 <u>오늘 나의 생각</u>
> 간단한 그래프를 그려봤는데 그렇게 어려운건 없는거 같다.  
> 물론 뭐 지금 처음 해봐서 그렇겠지만 간간하게 plot(x,y) 행열에 데이터를
> 넣어주면 빠르게 내가 원하는 정보가 나온다는 것이다.  
> 종합적으로 생각해보면 데이터를 시각화하는건 어렵지 않다는걸 알 수있다.  
> 그럼 무엇이 어려운가? 고민해봤더니 역시 전처리,정제과정등이 어려운거 같다.
  
## ❌ 실수 요인
없음.

## <u>📖 <u>실습 Code</u>
<script src="https://gist.github.com/Cononi/e7659b6f0a60f9b46ded543008b6fb98.js"></script>