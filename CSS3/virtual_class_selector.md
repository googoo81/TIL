# 가상 클래스 선택자
## 가상 선택자
CSS에는 가상 요소(:pseudo-element)와 가상 클래스(:pseudo-class)가 있다. <br>
이것들을 사용해서 html 문서의 수정 없이 CSS만으로 디자인적 요소를 추가할 수 있다. <br>
효과로 html 문서에 쓸데없는 태그를 사용하여 화면 리더기 등에 쓸데없는 정보가 읽히게하거나, <br>
불필요한 클래스를 남발해 코드 가독성을 낮추지 않게 한다. <br>

<br><br>
  
## 앵커 가상 클래스
앵커 가상 클래스는 화면의 특정 요소에 커서가 향했을 때 특정 디자인을 입혀주거나, 
어떤 요소에 `동적인 스타일`을 입혀준다.

앵커 가상 클래스에서 가장 자주 쓰이는 패턴이다. :link는 아직 방문하지 않은 링크를 나타낸다. 
다음을 사용해서 아직 방문하지 않은 링크를 파란색으로, 
방문한 링크는 밑줄 없이 보라색으로 표현할 수 있다.
```
      a:link {
        color: blue;
    }
    a:visited {
        color:purple;
        text-decoration: none;
    }
```
사용자의 행동에 영향을 받는 앵커 가상 클래스 ↓
```
      a:hover {
        color: red;
    }
    a:active {
        color: gray;
    }
    a:focus {
        color: yellow;
    }
```
  
### 뜻
 - :hover : 사용자가 해당 요소에 커서를 가져다 댔을 때
 - :active : 요소가 활성화 되었거나 클릭 되었을 때
 - :focus : 해당 요소에 키보드 포커스가 맞춰졌을 때
 
<br><br><br>
  
## 순서에 따른 가상 클래스
가상 클래스의 장점 중 하나는 오직 CSS를 주기 위해 클래스를 추가할 필요가 없다는 것이다.

 - :first-child : li 중 첫번쩨 요소에 해당 CSS를 적용한다.
 - :last-child : li 중 마지막에 해당 CSS를 적용한다.
 - :nth-child(n) : li 중 n번쩨 요소에 해당 CSS를 적용한다.
```
    ol li:first-child {
        border-top: none;
    }

    ol li:last-child {
        border-top: none;
    }

    ol li:nth-child(2) {
        border-top: none;
    }
 ```
 
 <br><br><br>

## 가상 요소
가상 클래스가 실제로 존재하는 요소에 클래스 추가 없이 디자인을 입히기 위한 것이라면, <br> 
가상 요소는 아예 실제로 존재하지 않는 요소를 만들게 해준다. <br>
```
    선택자::가상요소 { property: value; }
```
- ::first-line : 해당 가상 요소는 텍스트의 첫번째 줄에만 특정 스타일을 입혀준다. <br>
  문장의 첫 줄은 상위 요소의 크기나 브라우저의 크기에 따라 달라질 수 있으니 주의하자.
```
    p::first-line {
        color: #ff0000;
        font-variant: small-caps;
    }
```
- ::first-letter : 이 요소는 텍스트의 첫 문자에 특정 스타일을 입혀준다. 
  미디엄 글 맨 상단에 있는 이런 스타일을 입힐 때 좋다.
```
    p::first-letter {
        color: #ff0000;
        font-size: xx-large;
    }
```

<br><br><br>

## ::before 과 ::after 요소
이 요소들은 생성된 콘텐츠의 내부에 삽입된다. <br>
이 요소는 특정 요소를 풍부하게 하는데 좋다. <br>
보통 이미지나 글, 그라데이션 등을 삽입하는 경우가 많다. <br>
```
    h1::before {
        content: 'hello';
    }
    h1::after {
        content: url("images/marker-right.gif");
    }
```
