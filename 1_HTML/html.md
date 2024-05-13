# HTML
HTML은 웹 컨텐츠의 의미와 구조를 정의할 때 사용되는 기본적인 개념이며, 웹을 이루는 가장 기초적인 구성 요소이다. <br>
웹 안에서 서로를 연결할 수 있는 링크(Hypertext)들을 구성(Markup)허는 언어(Language)라는 뜻! <br>
💡우리가 보는 웹 컨텐츠 = HTML(구조) + CSS(디자인) + Javascript(동작/기능) <br> 

그럼 어떻게 웹 컨텐츠를 구성한다는걸까? <br> 
HTML은 각 웹 컨텐츠 요소(element)들을 Tag라는 것을 통해 구체화시킨다. <br> 
Tag는 `<head></head>`, `<body></body>`, `<p></p>` 등등이 있고 <br> 
외에도 많은 종류가 있으니 자세한 의미와 용법은 [MDN공식문서](https://developer.mozilla.org/ko/docs/Web/HTML/Element)를 추천한다. <br> <br> 
Tag는 기본적으로 여는태그, 내용(content), 닫는태그 의 형태로 구성된다.
```html
<p>p태그는 paragraph, 즉 하나의 문단을 만들 때 쓰입니다.</p>
```
하지만, 모든 예외가 있는법! 닫는 태그가 없는 태그들도 있다. <br> 
`<br>` `<img>` `<meta>` `<link>` `<input>` `<hr>`의 경우에는 닫는 태그 없이 아래의 예시와 같이 사용한다. <br>
```html
<img src="이미지경로.jpg">
<input value="">
```
이처럼 내부 값인 content가 따로 없고 태그 자체의 속성(attribute)으로 값을 받아 사용하기에 닫는 태그가 불필요하다. <br><br><br>


## 블록요소(Block level) vs 인라인요소(Inline level)

HTML의 요소는 기본적으로 블록요소, 인라인요소 두가지로 나뉜다. <br>
💡실제로 화면에 요소들을 배치할 떄 중요한 개념이니 잘 익혀두자!
- <b>블록요소(Block level)</b><br>
말 그대로 웹 페이지에 하나의 블록으로서 존재한다. 블록이기에 가로 한줄을 꽉 채워 한자리를 차지하고, 때문에 block 요소의 이전요소와 다음요소는 줄바꿈이 일어난다. 하나의 덩어리 개념으로 웹 페이지 내의 구조를 잡을 때 사용한다. 큰 덩어리이기에 인라인요소 안에 존재할 수 없고, 블록 요소가 인라인요소를 품을 수 있는 더 큰 개념이라고 생각하면 된다. <br>
![Group 12 (2)](https://github.com/oching-choi/study-book/assets/102008712/4d707831-00ef-4953-bdeb-b6fccd0ccfa9)

- <b>인라인요소 (Inline level)</b><br>
하나의 문장, 단어 같은 작은 단위이다. 블록 요소 처럼 가로 한줄을 차지하지않고 해당 요소의 content 길이만큼만의 크기를 갖는다. 따라서 줄이 바뀌지않고 한 줄에 나란히 붙어 존재한다. 실제로 화면 구성시에 인라인 요소는 하나의 구조를 구성하는 블록 요소안에 담겨 있는 것이 안정적이라 `블록요소>인라인요소` 의 형태를 권장한다. <br>
![Group 11](https://github.com/oching-choi/study-book/assets/102008712/6eb63003-d120-4c1b-a389-ef746765fd33)<br><br><br>



## HTML 문서 
```html
<!doctype html>
<html>
  <head>
    <meta charset="utf-8" />
    <title>My test page</title>
  </head>
  <body>
  </body>
</html>
```
html 거의 기본 템플릿처럼 이러한 구조를 갖는다. <br>
만약 vscode와 같은 컴파일 프로그램을 사용한다면 `!+엔터`만 쳐도 자동완성처럼 위와 같은 HTML 구성을 갖춘다. <br>
- `<!DOCTYPE html>`
해당 문서가 HTML 문서라는 것을 공표하는 역할을 한다.
- `<html></html>`
html요소. 페이지 전체를 감싸며 root요소라고도 한다. 문서의 고유 언어를 설정하는 lang 속성을 포함한다.
- `<head></head>`
head요소. 웹 사이트 방문자에게는 보이지않는 웹 컨텐츠 외의 영역이다. 검색 결과에 표시되길 원하는 설명이나 해당 사이트를 위한 각종 선언들을 포함하는 역할을 한다.
- `<meta charset="utf-8">` 
웹 페이지의 언어 인코딩 방식을 utf-8로 정하겠다는 의미이다. 인코딩이란 HTML파일을 웹브라우저에서 표시될 수 있도록 변환하는 처리작업이다. 위 태그가 없으면 한글, 특수문자 들이 깨져서 나올 수 있다.<br>
![image 1](https://github.com/oching-choi/study-book/assets/102008712/5636dd44-d575-4251-8e2f-4456f79926a9)
- `<meta name="viewport" content="width=device-width">` 뷰포트를 지정하는건데, 우리말로 뷰포트는 보임창. 즉 화면상의 화상 표시 영역을 뜻한다. 



 



 
