---
title : "[pandas] 시리즈 다루기 - 기초"
categories:
   - python
tags:
   - Pandas
   - 판다스 시작하기
   - 공부
date: 2021-09-19T17:21:21+09:00 #작성일자
last_modified_at: 2021-09-19 #업데이트날짜.
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
> 1. **DataFrame()** : 데이터프레임 클래스에 딕셔너리를 전달하면 데이터프레임 클래스가 만들어집니다.
>   
> 2. **loc** : 행 단위로 데이터를 추출할때 씁니다. loc 속성은 인덱스를 기준으로 행 데이터를 추출합니다. loc 속성으로 인덱스를 전달하면 행 데이터를 추출할 수 있습니다. 그리고 인덱스에 없는 번호를 전달하면 오류가 발생하니 주의가 필요합니다. list와 같은 인덱스 계열과 같습니다.
>   
> 3. **index** : 시리즈의 인덱스를 불러옵니다.
>  
> 4. **values** : 시리지의 데이터를 불러옵니다.
>  
> 5. **keys()** : index와 마찬가지로 해당 시리즈의 인덱스를 불러옵니다.
>    
> 6. **astype** : 해당 데이터의 타입을 바꿔줍니다.
>  
> 7. **mean()** : 산술 평균값을 반환합니다.
>   
> 8. **min()** : 최솟값을 반환 합니다.
>   
> 9. **max()** : 최댓값을 반환 합니다.
>   
> 10. **std()** : 표준편차를 반환 합니다.
## ✏️ <u>기억하자. </u>
> ## ✅ 데이터 프레임 Series 선택
> 시리즈를 선택하려면 loc 속성에 인덱스를 지정하면 됩니다.  
> 지정 방법은 데이터네임.loc['인덱스번호or이름'] 입니다.
>  
> ## ✅ index, values, keys 활용
>   
> | 이름   | 분류  |   사용법   | 응용
> |:--:|:--:|:--:|:--:|
> | index |  속성  | 알고자하는 시리즈데이터에 .index 로 사용  | .index[0] 과같이 인덱스 번호 부여시 해당 인덱스의 데이터 값 반환
> | values |  속성 |  알고자하는 시리즈데이터에 .values 로 사용 | .values[0] 과같이 인덱스 번호 부여시 해당 인덱스의 데이터 값 반환
> | keys() |  메서드 |  알고자하는 시리즈데이터에 .keys 로 사용 | .keys()[0] 과같이 인덱스 번호 부여시 해당 인덱스의 데이터 값 반환
>   
> ## ✅ 시리즈 메서드 정리
> | 시리즈 메서드명 | 설명 |
> |:---:|:---:|
> |append|2개 이상의 시리즈 연결
> |describe| 요약통계량 계산
> |drop_duplicates|중복값이 없는 시리즈 반환
> |equals| 시리즈에 해당 값을 가진 요소가 있는지 확인
> |get_values| 시리즈 값 구하기(values 속성과 동일)
> |isin| 시리즈에 포함된 값이 있는지 확인
> |min| 최솟값 반환
> |max| 최댓값 반환
> |mean| 산술 평균 반환
> |median| 중간값 반환
> |replace| 특정 값을 가진 시리즈 값을 교체
> |sample| 시리즈에서 임의의 값을 반환
> |sort-values| 값을 정렬
> |to-frame| 시리즈를 데이터프레임으로 변환
>   
## 💭 <u>오늘 나의 생각</u>
> 응용법도 다양하다보니 헷갈리게 만드는거 같다.  
> 전체적으로 한번에 많은걸 보여주려고 하다보니 응용도가 떨어질거 같은게 마음에 걸린다.
  
## ❌ 실수 요인
없음.

## <u>📖 <u>실습 Code</u>
<script src="https://gist.github.com/Cononi/a4e5d02dfe39fc7a7ac0642811cb3c55.js"></script>