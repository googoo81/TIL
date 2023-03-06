# React Router

<br><br>

## '라우팅'이란?
사용자가 요청한 URL에 따라 해당 URL에 맞는 페이지를 보여주는 것이다.

<br><br>

## 리액트 라우터
사용자가 입력한 주소를 감지하는 역할을 하며, 여러 환경에서 동작할 수 있도록 여러 종유의 라우터 컴포넌트를 제공한다.

<br>

### BrowserRouter
HTML5를 지원하는 브라우저의 주소를 감지 한다.

<br>

### HashRouter
해시 주소를 감지 한다.

<br><br>

## 설치

<br>

#### - npm
```
npm install react-router-dom
```
#### - yarn
```
yarn add react-router-dom
```

<br><br>

## 사용예시

<br>

### ex) App.js
```
import React, { Component } from 'react';
import { BrowserRouter, Routes, Route } from 'react-router-dom';
import Header from './Header';
import Main from './Main';
import Footer from './Footer';

const App = () => {
	return (
		<div className='App'>
			<Header />
			<Main />
			<Footer />
		</div>
	);
}

export default App;
```

<br>

### ex) Header.js
```
import React from 'react';

function Header(props) {
    return (
		<>
			<h1>머갈통</h1>
		</>
    );
}

export default Header;
```

### ex) Main.js
```
import React from 'react';
const Main = (props) => {
	return (
		<>
			<h2>메인티비</h2>
		</>
	);
};

export default Main;
```

<br>

### ex) Footer.js
```
import React from 'react';

const Product = (props) => {
    return (
        <>
            <h2>발바닥!</h2>
        </>
    );
}

export default Footer;
```
