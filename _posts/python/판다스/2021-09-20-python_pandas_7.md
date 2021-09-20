---
title : "[pandas] 시리즈 다루기 - 응용"
categories:
   - python
tags:
   - Pandas
   - 판다스 시작하기
   - 공부
date: 2021-09-20T12:03:22+09:00 #작성일자
last_modified_at: 2021-09-20 #업데이트날짜.
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
> 1. **Series()** : 시리즈 메서드에 리스트를 전달하면 시리즈 데이터가 생성됩니다.
>  
> 2. **max()** : 최댓값을 반환 합니다.
>  
> 3. **mean()** : 평균값을 반환 합니다.
>  
> 4.  **불린추출** : 해당 데이터의 대괄호안에 조건식 비교식을 넣으면 True 데이터만 반환 한다.  ( 리스트로 True,False와 같은 참거짓 데이터로 전달시 True만 반환 )
> ex ) ages[age > 5] age가 5보다 큰 데이터만 반환함.
>  
> 5. **브로드캐스팅** : 모든 데이터에 대해 한번 연산하는것을 가르킵니다.
>  
> 6. **벡터** : 여러개의 데이터를 가지고 있는 공간을 의미 한다.
>  
> 7. **스칼라** : 단순 크기를 나타내는 데이터 입니다.
>  
> 8. **sort_index** : 인덱스를 정렬하는 메서드이며, ascending 인자로 False 전달하면 역순 정렬이 됩니다. 기본값은 True 입니다.
>  
## ✏️ <u>기억하자. </u>
> ## ✅ 시리즈와 불린 추출
> 데이터를 추출할때 보통 인덱스를 모르는 경우가 더 많습니다. 수많은 데이터에서
> 인덱스를 찾기란 쉽지 않기 때문입니다.  
> 그러므로 이럴때 사용하는게 불린추출입니다. 조건 비교식으로 원하는 특정 조건을 가진 데이터만을 추출하여 사용 가능합니다.
>  
> ## ✅ 시리즈와 브로드캐스팅(벡터와 스칼라)
> 모든 데이터에 대해 한 번에 연산을 모두 수행하는것을 브로드캐스팅이라고 합니다.  
> 그리고 그 여러개의 데이터를 가진것을 벡터,  
> 단순한 크기를 나타내는 데이터 한개를 스칼라라고 합니다.
> 
>   
## 💭 <u>오늘 나의 생각</u>
> 하나를 배워도 여러개를 배워가는 장이다. 왜 파이썬인가 했는데 불린연산으로 이해가 됐다.
  
## ❌ 실수 요인
없음.

## <u>📖 <u>실습 Code</u>
<script src="https://gist.github.com/Cononi/20bc4f57282d2aa6eaea09208fc56292.js"></script>