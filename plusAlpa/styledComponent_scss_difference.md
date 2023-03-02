# SCSS와 styled components 차이

<br><br>

## SCSS
 코드의 재활용성을 올리고, 가독성을 올리는 등 CSS의 단점을 보완하고 개발의 효율을 올리기 위한 것
 
 <br>

### 장점
```
 · CSS보다 심플한 표기법, CSS를 구조화하여 표현함 
 · Nesting, Mixin, selector등의 기능을 활용하여 CSS유지보수 편의성을 향상시킴
```

<br>

### 단점
```
 · 전처리기를 위한 도구가 필요함
 · 다시 컴파일 하는데 시간이 걸림
 · class명을 일일히 정해주어야 됨
```

<br>

### 특징

#### 변수 
```
$color: #d9d9d9;
$borderRadius: 10px;

div {
background: $color;
border-radius: $borderRadius;
}
```
이런식으로 특이한 변수 선언이 가능해짐

#### 중첩 
셀렉터를 중첩하거나 속성을 중첩시켜 상위 요소를 참조하는 것이 가능해짐
HTML 태그 자체에서 속성 값을 줄일 수 있어 HTML 코드 가독성도 상승됨

<br><br>

## Styled-component
 컴포넌트 기반으로 CSS를 작성할 수 있게 도와주는 라이브러리

<br>

### 장점
```
 · Scss라이브러리 설치 없이 Scss 문법을 사용할 수 있음
 · 자유로운 CSS 커스텀 컴포넌트를 만들 수 있음
 · 컴포넌트의 props를 참조할 수 있으며, props의 값에 따라 스타일을 다르게 코딩 할 수 있음
```

<br>

### 단점
```
 · 빠른 페이지 로드에 분리함
```

<br>

### 특징
#### Automatic critical Css
 - style component는 화면에 컴포넌트가 렌더링 되었는지 추적해 컴포넌트에 대한 스타일을 자동 삽입함
 - 코드를 적절히 분배해 놓으면 최소한의 코드만으로 화면이 띄워질 수 있음

#### No class name bugs
 - styled-component는 스스로 className을 생성하기 때문에 className의 중복이나 오타로 인한 버그를 줄여줌

#### Easier deletion of CSS
 - Styled Component는 모든 스타일 속성이 특정 컴포넌트와 연결되어 있기 때문에, <br>
   만약 컴포넌트를 더 이상 사용하지 않아 삭제할 경우 이에 대한 스타일 속성도 함께 삭제됨

#### Simple dynamic styling
 - className을 일일이 수동으로 관리할 필요 없이 React의 props나 전역 속성을 기반으로 컴포넌트에 스타일 속성을 부여하기 때문에 간단하고 직관적임

#### Painless maintenance
 - 컴포넌트에 스타일을 상속하는 속성을 찾아 다른 CSS 파일들을 검색하지 않아도 되기 때문에 코드의 크기가 커지더라도 유지보수가 어렵지 않음

#### Automatic vendor prefixing
 - 개별 컴포넌트마다 기존의 CSS를 이용하여 스타일 속성을 정의하면 될 뿐이다. 이외의 것들은 Styled Component가 알아서 처리해 줌

<br><br>

## 차이점 정리

<br>

### SCSS
 - css in css 문법으로 js 파일과는 분리되어 있음
 - 어떤 컴포넌트의 상태값이 변하더라도 반응하기 쉽지 않음
 - 브라우저에 보이지 않은 컴포넌트까지 읽기 때문에 불필요한 컴파일 과정이 추가됨

<br>

### styled components
 - css in js 방식으로 컴포넌트가 렌더링 될 때만 해당 스타일 정보를 읽음
동적인 이벤트가 많은 사이트라면 컴포넌트가 자주 렌더링 될 때 그만큼 스타일 정보도 다시 읽어와야 됨

<br><br>

## 정리
#### styled components는 컴포넌트 단위로 개발하기 때문에 react와 잘 어울리는 것 같다!!
