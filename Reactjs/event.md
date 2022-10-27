# 이벤트
## React에서의 이벤트 처리
### html과의 차이점
 - React 이벤트 이름은 소문자 대신 camelCase를 사용함
 - JSX에 문자열 대신 함수를 전달함

html에서는 아래와 같이 이벤트를 넣었다면,
```
<button onclick="activateButton()">클릭하셍</button>
```
React에서는 이벤트이름을 `onClick`, `onSubmit` 등과 같이 camelCase로 설정한다는 차이점이 있다. <br>
event handler는 JSX 표기인 { }를 사용하여 연결함 <br>
```
<button onClick={activateButton}>클릭하셍</button>
```

### 주의할 점
DOM 요소에만 이벤트 설정이 가능합니다. <br>
`div`, `button`, `input`, `form`, `span` 등의 DOM 요소에는 이벤트 설정이 가능하지만, <br>
리액트의 컴포넌트에는 불가능하다. <br>
예를 들면 위와 같이 button이라는 DOM 요소에 이벤트를 설정했는데, <br>
아래처럼 <Component>라는 리액트 컴포넌트에는 onClick을 달아서 우리가 의도한대로 이벤트가 실행되지 않는다. <br>
그냥 color, name과 같은 props를 전달해주는 것에 불과함 <br>
```
function App() {
  const sayHi = function () {
    alert('Hello');
  }
  return (
    <>
      <Component onClick={sayHi} name="송현우" nickname="송송" />
    </>
  );
}
```
  
### 이벤트 핸들러 네이밍
 - Props의 경우 : 보통 `onClick`과 같이 `on`접두사를 지정함.
 - Function Names의 경우: 보통 `handleClick`과 같이 `handle`접두사를 지정합니다. <br>
   이 두 경우를 함께 사용한 결과 코드는 이런 패턴을 가진다. <br>
   `<Component onClick={handleClick}/>` <br>
