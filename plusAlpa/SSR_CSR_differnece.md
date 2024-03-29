# SSR과 CSR 

## SSR의 정의 및 설명

<br>

### Server Side Rendering의 약자이다.
 - 서버에서 렌더링 준비를 끝마친 상태로 클라이언트에 전달하는 방식.
  
<br>
  
### 예시
 - 유저가 웹사이트에 요청을 보냄 ↓
 - 서버가 즉시 랜더링이 가능한 html 파일을 만듬 <br>
   (클라이언트에 전달되는 순간, 이미 렌더링 준비가 되어있기 때문에 html은 즉시 렌더링 됨, 그러나 사이트는 조작불가{js가 읽히기 전}) ↓
 - 클라이언트가 자바스크립트를 다운 <br>
   (다운 받아지고 있는 사이에 유저는 컨텐츠는 볼 수 있지만 사이트를 조작 할 수는 없음. 클라이언트는 이때 사용자 조작을 기억하고 있음) ↓ 
 - 브라우저가 js 프레임워크를 실행 <br>
   (js까지 성공적으로 컴파일 되었기 때문에 기억하고 있던 사용자 조작이 실행되고 이제 웹 페이지는 상호작용 가능해짐)
   
<br>

### 정리
서버에서 이미 '렌더 가능한' 상태로 클라이언트에 전달되기 때문에, JS가 다운로드 되는 동안 사용자는 무언가를 보고 있을 수 있음

<br><br>

## CSR의 정의 및 설명

<br>

### Client Side Rendering의 약자이다.
 - SSR과 달리 렌더링이 클라이언트 쪽에서 일어남 <br>
   (서버는 요청을 받으면 클라이언트에 html과 js를 보내준다. 클라이언트는 그것을 받아 렌더링을 시작함)

<br>

### 예시
 - 유저가 웹사이트에 요청을 보냄 ↓
 - CDN이 html 파일과 js로 접근할 수 있는 링크를 클라이언트를 보낸다. <br>
   (CDN : aws의 cloudflare를 생각하면 됨. 엔드 유저의 요청에 '물리적'으로 가까운 서버에서 요청에 응답하는 방식) ↓
 - 클라이언트는 html과 js를 다운로드 받음 <br>
   (이때 SSR과 달리 유저는 아무것도 볼 수 없음) ↓
 - 다운이 완료된 js가 실행, 데이터를 위한 api가 호출됨
   (이때 유저들은 placeholder를 보게됨) ↓
 - 서버가 api로부터의 요청에 응답 ↓
 - api로부터 받아온 data를 placeholder 자리에 넣어준뒤 페이지는 상호작용이 가능해짐 ↓

<br>

### 정리  
- 서버에서 처리 없이 클라이언트로 보내주기 때문에 자바스립트가 모두 다운로드 되고 실행이 끝나기 전까지 사용자는 볼 수 있는게 없음

<br><br>

## 각각의 차이점

<br>

### 페이지 로딩 시간
첫 페이지를 로딩한 후, 사이트의 다른 곳으로 이동하는 식의 동작을 가정하면,
CSR은 이미 첫 페이지 로딩할 때 나머지 부분을 구성하는 코드를 받아왔기 때문에 빠르다.
반면, SSR은 첫 페이지를 로딩한 과정을 정확하게 다시 실행한다. 그래서 더 느리다.

<br>

### 서버 자원 사용
SSR이 서버 자원을 더 많이 사용한다. 매번 서버에 요청을 하기 때문

<br><br>

## 최종 정리

<br>

### SSR을 사용해야 할 때
 - 네트워크가 느릴 때
 - 검색 엔진 최적화가 필요할 때
 - 최초 로딩이 빨라야하는 사이트를 개발할 때
 - 사이트 상호작용이 적을 때

<br>

### CSR을 사용해야 할 때
 - 네트워크가 빠를 때
 - 서버 성능이 안 좋을 때
 - 유저에게 보여줘야 하는 데이터가 많을 때
 - 내용이 전반적으로 가벼울 때
