# README 작성을 위한 Markdown 활용법
### Header(```<h1> ~ <h6>```)
* format : ```# 문자```
```
# h1 tag - 문서 제목
## h2 tag - 문서 부제목
### h3 tag
#### h4 tag
##### h5 tag
###### h6 tag
```
# h1 tag - 문서 제목
## h2 tag - 문서 부제목
### h3 tag
#### h4 tag
##### h5 tag
###### h6 tag

***

### Emphasis(```<i>, <b>```)
* format : 글자 기울기=```[ * | _ ]문자[ * | _ ]```, 글자 굵기=```[ ** | __ ]문자[ ** | __ ]```
* 문장 중간에 사용할 경우에는 띄어쓰기를 사용하는 것이 좋다.   
```
*i tag*
_i tag_
**b tag**
__b tag__
```
*i tag*   
_i tag_   
**b tag**   
__b tag__   
_문장 중간에 사용할 경우에는 **띄어쓰기** 를 사용하는 것이 좋다._

***

### Lists
* 띄어쓰기 3번을 주면 새로운 [ ol | ul ], li tag가 해당 li tag의 하위 태그로 종속된다.
* 하위 태그로의 적용 단계는 3단계가 끝이다.
* Markup 언어와 똑같이 혼합해서 사용하는 것도 가능하다.

#### Unordered(```<ul>```)
* format : [ * | + | - ] 문자
* 현재까지는 어떤 번호를 입력해도 순서는 내림차순으로 정의된다.
```
* <ul type="disc"> - 검정 원형 점
   + <ul type="circle"> - 흰 원형 점
      - <ul type="square"> - 검정 사각형 점
```
* ```<ul type="disc">``` - 검정 원형 점
   + ```<ul type="circle">``` - 흰 원형 점
      - ```<ul type="square">``` - 검정 사각형 점
   
#### Ordered(```<ol>```)
* format : 숫자. 문자
* 현재까지는 어떤 번호를 입력해도 순서는 내림차순으로 정의된다.
```
1. <ol type="1"> - 숫자(기본값)
   1. <ol type="i"> - 소문자 로마 숫자
      1. <ol type="a"> - 소문자 알파벳
```
1. ```<ol type="1">``` - 숫자(기본값)
   1. ```<ol type="i">``` - 소문자 로마 숫자
      1. ```<ol type="a">``` - 소문자 알파벳

***

### Images(```<img>```)
* format : ```![Alt Text](url "Alt title")```
* Markdown 언어에서는 이미지 크기 조정이 안되니 Markup 언어를 사용해야 한다.
```
![이주빈 증명사진](https://img.hankyung.com/photo/201904/01.19372617.1.jpg)
![이주빈 증명사진](https://img.hankyung.com/photo/201904/01.19372617.1.jpg "이주빈 증명사진")
<img src="https://img.hankyung.com/photo/201904/01.19372617.1.jpg" width="480px" alt="이주빈 증명사진" title="이주빈 증명사진"/>
```
![이주빈 증명사진](https://img.hankyung.com/photo/201904/01.19372617.1.jpg)
![이주빈 증명사진](https://img.hankyung.com/photo/201904/01.19372617.1.jpg "이주빈 증명사진")
<img src="https://img.hankyung.com/photo/201904/01.19372617.1.jpg" width="240px" alt="이주빈 증명사진" title="이주빈 증명사진"/>

***

### Links
* format : 
