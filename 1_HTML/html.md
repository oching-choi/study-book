# HTML
HTML(Hypertext Markup Language)은 우리가 보는 웹페이지가 어떻게 구조화되어 있는지 알 수 있도록 하는 마크업 언어이다. <br>
웹을 이루는 가장 기초적인 구성 요소로, 웹 컨텐츠의 의미와 구조를 정의할 때 사용한다. <br>
💡웹 컨텐츠는 HTML(구조), CSS(디자인), Javascript(동작/기능)로 구성된다. <br><br>

HTML의 각 요소(element)를 표현할 떄 Tag를 사용하는데 Tag는 `<head></head>`, `<body></body>`, `<p></p>` 등등이 있다.<br> 
이 외에도 굉장히 많기에 각 Tag들의 자세한 의미와 용법은 [MDN공식문서](https://developer.mozilla.org/ko/docs/Web/HTML/Element)를 보는 것을 추천한다. <br> <br> 
Tag사용시에는 기본적으로 통용되는 형태가 있는데 여는태그`<태그명`, 내용(content), 닫는태그`/태그명>`로 구성된다. <br>
![image](https://github.com/oching-choi/study-book/assets/102008712/0539fb73-9710-4853-8971-e9cd528a9eeb)<br>
하지만, 모든 예외가 있는법! 닫는 태그가 없는 태그들이 있다. <br> 
`<br>` `<img>` `<meta>` `<link>` `<input>` `<hr>`의 경우에는 닫는 태그가 없으니 주의하자. <br>
 위의 태그들은 태그 내부 값인 content가 따로 없고 태그 자체의 속성(attribute)으로 값을 받아 사용한다. 
```html
<img src="이미지경로.jpg">
<input value="">
```
<br>

### 블록요소(Block level) vs 인라인요소(Inline level)
![image](https://github.com/oching-choi/study-book/assets/102008712/45ce2118-60bc-4c59-87d5-81f39d9ee7f5)
![image](https://github.com/oching-choi/study-book/assets/102008712/2a8b7091-1f40-4d75-af05-30b3a0fe02d1)

HTML의 요소는 기본적으로 블록요소, 인라인요소 두가지로 나뉜다. <br>
⭐️ 실제로 화면에 요소들을 배치할 떄 알아두어야 하니 꼭 기억하기!
- 블록요소(Block lever) : 말 그대로 웹 페이지에 하나의 블록으로서 존재한다. 블록이기에 가로 한줄을 꽉 채워 한자리 차지한다. 때문에 block 요소는 이전요소와 다음요소 사이에서 줄을 바꾼다. 때문에 블록요소는 하나의 덩어리 개념으로 웹 페이지 내의 구조를 잡을 때 사용한다. 큰 덩어리이기에 인라인요소 안에 존재할 수 없고, 블록 요소가 인라인요소를 품을 수 있는 더 큰 개념이라고 생각하면 된다.
- 인라인요소 (Inline level) : 하나의 문장, 단어 같은 작은 단위이다. 블록요소 처럼 가로 한줄을 차지하지않고 해당 요소의 content 길이만큼만의 크기를 갖는다. 따라서 줄이 바뀌지않고 같은 줄에 존재한다. 인라인 요소만 나와있는 것 보다 하나의 구조를 구성하는 블록 요소안에 담겨 있는 것이 안정적이라 권장한다. <br>

 
