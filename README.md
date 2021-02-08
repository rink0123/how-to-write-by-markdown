# README 작성을 위한 Markdown 활용법
```
개인적으로 쓸만한 것만 추려서 정리하였습니다.
```
### Header(`<h1> ~ <h6>`)
* format : `# 문자`
* 제목을 만들려면 #제목 텍스트 앞에 1 ~ 6 개의 기호를 추가합니다. 사용하는 수에 #따라 제목의 크기가 결정됩니다.
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

### Styling text(`<b>`, `<i>`, `<del>`)
| Style | Syntax | Tag | Example | Output |
|---|---|---|---|---|
| Bold | `**Text**` or `__Text__` | `<b>Bold</b>` | `**Bold**` | **bold** |
| Italic | `*Text*` or `_Text_` | `<i>Italic</i>` | `*Italic*` | *Italic* |
| Strikethrough | `~~Text~~` | `<del>Strikethrough</del>` | `~~Strikethrough~~` | ~~Strikethrough~~ |
| Bold and nested italic | `**Text**` and `_Text_` | `<b>This text is<i> extremely </i>important</b>` | `**This text is _extremely_ important**` | **This text is _extremely_ important** |
| All bold and italic | `***Text***` | `<b><i>All bold and italic</i></b>` | `***All bold and italic***` | ***All bold and italic*** |

***

### Lists
* 띄어쓰기 3번을 주면 새로운 [ ol | ul ], li tag가 해당 li tag의 하위 태그로 종속된다.
* 하위 태그로의 적용 단계는 3단계가 끝이다.
* Markup 언어와 똑같이 혼합해서 사용하는 것도 가능하다.

#### Unordered(`<ul>`)
* format : [ * | + | - ] 문자
* 현재까지는 어떤 번호를 입력해도 순서는 내림차순으로 정의된다.
```
* <ul type="disc"> - 검정 원형 점
   + <ul type="circle"> - 흰 원형 점
      - <ul type="square"> - 검정 사각형 점
```
* `<ul type="disc">` - 검정 원형 점
   + `<ul type="circle">` - 흰 원형 점
      - `<ul type="square">` - 검정 사각형 점
   
#### Ordered(`<ol>`)
* format : 숫자. 문자
* 현재까지는 어떤 번호를 입력해도 순서는 내림차순으로 정의된다.
```
1. <ol type="1"> - 숫자(기본값)
   1. <ol type="i"> - 소문자 로마 숫자
      1. <ol type="a"> - 소문자 알파벳
```
1. `<ol type="1">` - 숫자(기본값)
   1. `<ol type="i">` - 소문자 로마 숫자
      1. `<ol type="a">` - 소문자 알파벳

***

### Images(`<img>`)
* format : `![Alt Text](url "Alt title")`
* `![Alt Text](url "Alt title")` 에서 "Alt title"을 제외한 나머지는 필수이다.
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

### Links(`<a>`)
* format : `url - automatic!`, `[Alt](http://github.com)`
```
url
[a tag text](url)
```
http://github.com   
[GitHub](http://github.com)

***

### Blockquotes(`<blockquote>`)
* format : `> 문자`
* 다른 Markdown 요소를 포함할 수 있다.
```
> This is a first blockqute.
>	> This is a second blockqute.
>	>	> This is a third blockqute.
```
> This is a first blockqute.
>	> This is a second blockqute.
>	>	> This is a third blockqute.

***

### Inline code(`<code>`)
* format : '문자'
* 역 따옴표이니 작은 따옴표랑 헤깔리면 안 된다.
```
I think you should use an `<addr>` element here instead.
```
I think you should use an `<addr>` element here instead.

***

### Syntax highlighting(`<pre>`)
* format : ` ```문자``` `, (띄어쓰기 4개)문자(띄어쓰기 4개)
<pre><code> 
```
javascript
function fancyAlert(arg) {
  if(arg) {
    $.facebox({div:'#foo'})
  }
}
```
</code></pre>

```
javascript
function fancyAlert(arg) {
  if(arg) {
    $.facebox({div:'#foo'})
  }
}
```

***

### Ignoring Markdown formatting(Escape)
* format : `\Markdown language`
```
Let's rename \*our-new-project\* to \*our-old-project\*.
```
Let's rename \*our-new-project\* to \*our-old-project\*.
