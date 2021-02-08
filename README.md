참고 URL   
[GitHub Guide - Mastering Markdown](https://guides.github.com/features/mastering-markdown/)   
[GitHub Docs - Writing on GitHub](https://docs.github.com/en/github/writing-on-github)   
[GitHub - 마크다운 markdown 작성법](https://gist.github.com/ihoneymon/652be052a0727ad59601#1-%EB%A7%88%ED%81%AC%EB%8B%A4%EC%9A%B4%EC%97%90-%EA%B4%80%ED%95%98%EC%97%AC)   
   
# README 작성을 위한 Markdown 활용법
```
개인적으로 쓸만한 것만 추려서 정리하였습니다.
```
### Header(`<h1> ~ <h6>`)
* format : `# Text`
* 제목을 만들려면 #제목 텍스트 앞에 1 ~ 6 개의 기호를 추가합니다. 사용하는 수에 #따라 제목의 크기가 결정된다.
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

### Horizontal Line(`<hr/>`)
* format : `* * *` or `***` or `- - -` or `---`
* `*` or `-`가 3개 이상 있어야 수평선임을 인식한다.
```
* * *
***
- - -
---
```
* * *
***
- - -
---

***

### Line Break(`<br/>`)
* format : 띄어쓰기 3번
* 문장 끝에 띄어쓰기 3번 또는 새 줄에 띄어쓰기 3번을 쓰면 줄바꿈된다.
```
줄 바꿈을 하기 위해서는 문장 마지막에서 3칸이상을 띄어쓰기해야 한다.___ // 띄어쓰기
이렇게
___ // 띄어쓰기
또는
___ // 띄어쓰기
이렇게
```
줄 바꿈을 하기 위해서는 문장 마지막에서 3칸이상을 띄어쓰기해야 한다.   이렇게
   
또는
   
이렇게

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

### Links
* Autumatic Link, External Link는 흔히 보는 링크 연결이다.
* Internal Link는 주로 목차로 쓰인다.
* `()` : Header로 링크, 띄어쓰기 => `-`로 대체, 대소문자 구문X. 규칙 어길 시 일반 글자로 인식.
* Header에 특수 문자가 있을 경우, 특수 문자를 제외한 Text를 넣으면 된다. (ex. Images(`<img>`) => imagesimg)
* Interpreter로 실행되기에 Internal Link를 목차로 사용하려면 최상단에 두어야 한다. Internal Link가 선언된 위 Header를 인식하지 못한다.
   
| Style | Syntax | Tag | Example | Output |
|---|---|---|---|---|
| Autumatic Link | `url` | `<a href="[url]" target="_self">url</a>` | `http://github.com` | http://github.com |
| External Link | `url` or `[Text](url)` | `<a href="[url]" target="_self">Text</a>` | `[GitHub](http://github.com)` | [GitHub](http://github.com) |
| Internal Link | `[Text](#Header)` | `<a id="#Header"(or name="#Header")>Header</a>` | `[Inline code](#Inline code)` | [Images(`<img>`)](#imagesimg) |

***

### Lists
* 띄어쓰기 3번을 주면 새로운 `<ol>` or `<ul>`가 해당 `<li>`의 하위 태그로 종속된다.
* 하위 태그로의 적용 단계는 3단계가 끝이다.
* Markup 언어와 똑같이 혼합해서 사용하는 것도 가능하다.

#### Unordered(`<ul>`)
* format : `*` or `+` or `-` Text
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
* format : 숫자. Text
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

### Blockquotes(`<blockquote>`)
* format : `>` Text
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

### code(`<code>`, `<pre>`)
* format : \`Text\` or \`\`\`Text\`\`\`
* 역 따옴표이니 작은 따옴표랑 헤깔리면 안 된다.
<pre><code>
```
I think you should use an \`<addr>\` element here instead.
```
</code></pre>
I think you should use an `<addr>` element here instead.

***

### Ignoring Markdown formatting(Escape)
* format : `\Markdown language`
```
Let's rename \*our-new-project\* to \*our-old-project\*.
```
Let's rename \*our-new-project\* to \*our-old-project\*.

***

### Tables(`<table>`)
* format : `|` and `-`, 왼쪽 정렬=`:---`, 가운데 정렬=`:---:`, 오른쪽 정렬=`---:`
* 단어 목록을 조합하고 하이픈 `-`(첫 번째 행)으로 나눈 다음 각 열을 `|`(파이프)로 구분하여 표를 만들 수 있다.
* `-`을 3개 이상 넣어야 행으로 인식한다.
```
| First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |
```
| First Header  | Second Header |
| ------------- | ------------- |
| Content Cell  | Content Cell  |
| Content Cell  | Content Cell  |
   
```
| Left-aligned | Center-aligned | Right-aligned |
| :---         |     :---:      |          ---: |
| git status   | git status     | git status    |
| git diff     | git diff       | git diff      |
```
| Left-aligned | Center-aligned | Right-aligned |
| :---         |     :---:      |          ---: |
| git status   | git status     | git status    |
| git diff     | git diff       | git diff      |
