# README 작성을 위한 Markdown 활용법
### Header(제목)
* 사용법 : ```# 문자```
* #의 갯수에 따라 h1~h6까지 지원.
```
# h1 tag
## h2 tag
### h3 tag
#### h4 tag
##### h5 tag
###### h6 tag
```
# h1 tag
## h2 tag
### h3 tag
#### h4 tag
##### h5 tag
###### h6 tag

***

### Emphasis(강조)
* 사용법 : ```[* | _]문자[* | _]```, ```[** | __]문자[** | __]```
* ```*``` 또는 ```_```의 갯수가 1개냐 2개냐에 따라 글자 기울기 또는 글자 굵기로 나뉨.
* 문장 중간에 사용할 경우에는 띄어쓰기를 사용하는 것이 좋다.   
```
*i tag*
_i tag_
**b tag**
__b tag__
```
_You **can** combine them_

***

### Lists(목록)
* 띄어쓰기 3번을 주면 새로운 ol, li tag가 해당 li tag의 하위 태그로 종속된다.
* 하위 태그로의 적용 단계는 3단계가 끝이다.

#### Unordered(미순차, 점)
* 사용법 : [* | + | -]. 문자
* 현재까지는 어떤 번호를 입력해도 순서는 내림차순으로 정의된다.
```
1. ol, li tag - 일반숫자
   1. ol, li tag - 로마숫자
      1. ol, li tag - 알파벳
```
1. ol, li tag - 일반숫자
   1. ol, li tag - 로마숫자
      1. ol, li tag - 알파벳
   
#### Ordered(순차, 숫자)
* 사용법 : 숫자. 문자
* 현재까지는 어떤 번호를 입력해도 순서는 내림차순으로 정의된다.
```
1. ol, li tag - 일반숫자
   1. ol, li tag - 로마숫자
      1. ol, li tag - 알파벳
```
1. ol, li tag - 일반숫자
   1. ol, li tag - 로마숫자
      1. ol, li tag - 알파벳
