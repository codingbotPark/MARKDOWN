# MarkDown

## 역사
[위키백과<마크다운역사>](https://ko.wikipedia.org/wiki/%EB%A7%88%ED%81%AC%EB%8B%A4%EC%9A%B4#%EC%97%AD%EC%82%AC)   
2004년 존 그루버가 문법면에서 에런 스위츠와 협약을 통해 마크다운 언어를 만들었으며, 사람들이 읽고 쓰기 쉬운 플레인 텍스트 포맷을 사용하여 쓸 수 있으면서 구조적으로 XHTML / HTML 으로 선택적 변환이 가능하게 하는 것이 목표이다 


<br>

## 마크다운
HTML (Hyper Text `Mark up` Language) <=> `Mark Down`   
**HTML에서 제공되는 다양한 화법보다 더 쉽고 빠르게 글을 작성 가능**  

### 장점
* 문법이 쉽다
* 관리가 쉽다
* 지원 가능한 플랫폼과 프로그램이 다양하다   
### 단점
* 표준이 없어서 사용자마다 문법이 상이할 수 있다   
(표준화된 문법이 없다 = 사용자마다 다르게 이해해서 사용)
* 모든 HTML마크업을 대신하지 못한다   
(HTML으로 변환되는 모든 HTML태그를 지원하지 못한다)


<br>

## 마크다운 사용
메모장부터  전용 에디터까지 많은 곳에서 활용 가능, 문법이 쉬워서 꼭 전용 에디터를 사용할 필요는 없지만 전용 에디터를 사용하여 하이라이트 효과 사용가능, 마크다운 문법을 지원하는 모든 곳에서 사용가능 
  
(VScode에서 미리보기를 활용해 마크다운이 표현되는 것을 볼 수 있다)

<br>
<br>
<br>
<br>
<br>

# 마크다운문법
## 제목

### 제목 앞에 #을 사용한다

<br>   

\# = \<h1>   
\## = \<h2>   
\### = \<h3>   
\#### = \<h4>   
\##### = \<h5>   
\###### = \<h6>

<br>
<br>
<br>

## 강조

아래의 형식대로 문자를 감싼다

<br>   

형태 | **강조** | *이텔릭체* | ~~취소선~~ | <u>언더라인</u>
 --- | --- | --- | --- | --- 
HTML | \<strong> | \<em> | \<del> | \<u>
MD | ** 또는 __ | * 또는 _ | ~~ | \<u>(html형식)

<br>

##### +조합해서 사용
##### 예) **_이텔릭체와 강조_** =  \**\_이텔릭체와 강조_**

<br>

##### +색상변경(html과 같음)
##### 예) <u style = "color : green">초록색</u> = \<u style = "color : green">초록색\</u>

<br>
<br>
<br>

## 목록

### 순서가 있는 목록
1. 문장 앞에 1. , 1. , 1. ... 을 쓴다
1. 자동으로 순서가 붙는다
1. 이 방법은 목록을 수정할 때 편리할 수 있다
---
1. 또는
2. 문장앞에 1. , 2. , 3. ... 을 쓴다

<br>

### 순서가 없는 목록
- 문장 앞에 ' - ' 을 쓴다
* 또는 문장 앞에 ' * ' 을 쓴다
+ 또는 문장 앞에 ' + ' 을 쓴다

<br>
<br>
<br>

## 링크

### \[text](주소url) 의 형식

<br>

[구글](https://www.google.co.kr/) = \[구글](https://www.google.co.kr/)   
[네이버](https://www.naver.com/) = \[네이버](https://www.naver.com/)   
[깃허브](https://github.com/) = \[깃허브](https://github.com/)

<br>

+참조링크 사용   
반복적으로 사용되는 주소를 참조링크로 대신할 수 있다   
예)[유튜브][유튜브 url] =

[유튜브 url]: https://www.youtube.com/

   

\[유튜브][유튜브 url]

\[유튜브 url]: https://www.youtube.com/

<br>

+target사용  
마크다운에서 target은 지원하지 않기때문에 target사용하려면 HTML방식으로 a 태그 작성   
예)<a href = "https://www.worksout.co.kr/front/main.do" target = "_blank">웍스아웃</a> = \<a href = "https://www.worksout.co.kr/front/main.do" target = "_blank">웍스아웃</a>

<br>
<br>
<br>

## 이미지

src = 주소   
alt = 대체 텍스트(이미지 이름)   

### \!\[alt](src) 의 형태

<br>

\!\[지구](https://www.solarsystemscope.com/textures/download/2k_earth_daymap.jpg)

=

![지구](https://www.solarsystemscope.com/textures/download/2k_earth_daymap.jpg)

<br>
<br>
<br>

## 코드강조

### 1번 옆에 \` (grave) 으로 `강조` 할 문장을 감싼다

<br>

### 블록(block) 코드강조

위의 \` (grave) 를 활용

<br>

### \``` 사용된 언어   
### 강조할 코드   
### \```

의 형태

<br>

\```C   
print("블록강조");   
\```   

=

```C
printf("블록강조");
```

\```python   
print("블록강조");   
\```   

=

```python
print("블록강조");
```

<br>
<br>
<br>

## 표
\- (hyphen / dash)   
\: (colons)   
\| (vertical bar)   
을 활용

<br>

### \| 왼쪽 | 오른쪽 | 중간
### \| --- | ---:|:---:
### \| left | right | midlle

의 형식   

 ---  = 글씨를 왼쪽으로 정렬   
:---: = 글씨를 중간으로 정렬   
 ---: = 글씨를 오른쪽으로 정렬   

<br>

단어 \| 뜻    
:---:\| ---   
table \| 탁자   
image \| 그림   

 =

 단어 | 뜻 
:---:| ---
table | 탁자
image | 그림

<br>
<br>
<br>

## 인용문

### 인용 할 문장앞에 > 을 사용한다

<br>

> 마크다운
>> 개요   
>> 제목   
>> 강조   
>> 목록   
>> 링크   
>> 이미지   
>> 코드강조   
>> 표   
>> 인용문   
>> 원시 HTML   
>> 수평선과 줄바꿈   

<br>
<br>
<br>

## 원시 HTML

### 마크다운은 '구조적으로 XHTML / HTML 으로 선택적 변환이 가능하게 하는 것' 이기 때문에 마크다운이 아닌 원시 HTML 문법을 사용할 수 있다

<br>

\<img src = "https://www.google.com/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png" alt = "구글" title = "구글" width=200px height = 100  >

=

<img src = "https://www.google.com/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png" alt = "구글" title = "구글" width=200px height = 100  >

<br>
<br>
<br>

## 수평선과 줄바꿈

### 줄바꿈 = \<br>

줄바꿈을 하기 위해 
줄바꿈을 쓰기 전 문장의 뒤에 **두 번 뛰우기**  
<br>
또는
<br>  
**\<br>** 을 사용할 수 있다

<br>

### 수평선 = \--- , *** , ___ = \<hr>

\---

=

---

<br>

\***

=

***

<br>

\___

=

___

<br>

\<hr>

=

<hr>
