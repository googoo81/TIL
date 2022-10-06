# JS함수

## 종류
 - 화살표 함수(Arrow function)
 - 함수 표현(Function expression)
 - 즉시 실행 함수(Immediately-invoked function)
 - 호이스팅(Hoisting)
 - 타이머 함수(Timmer function)
 - 콜백(Call back)

## 화살표 함수
 - JS의 기존 함수를 더욱 간소화 한 함수
 - `ex) const doubleArrow = x => ({ name: 'Herropy' })`


## 함수 표현(Function expression)
- 함수를 정의하고, 변수에 함수를 저장하고 실행하는 과정을 거치는 것. 

### 익명 함수 표현 (Anonymous function expression)
 - ex)
```
var x = function(y) {
   return y * y;
};
console.log(x(2)); 

// 결과 : 4
```

### 기명 함수 표현 (Named function expression)
 - ex)
```
var x = function square(y) {
   return y * y;
};
console.log(x(2)); 

// 결과 : 4
```

## 즉시 실행 함수 
 - 함수를 정의하고 바로 실행하여 이러한 과정을 거치지 않는 특징이 있습니다. 함수를 정의하자마자 바로 호출하는 함수

### 기본 형태
```
(function () {
    // statements
})()
```

## 호이스팅
 - 함수 선언부가 유효범위 최상단으로 끌어 올려지는 현상

## 타이머 함수

### 종류
 - setTimeout(함수, 시간): 일정 시간 후 함수 실행
 - setTimeInterval(함수, 시간): 시간 간격마다 함수 실행
 - clearTimeout(): 설정된 Timeout 함수를 종료
 - clearInterval(): 설정된 Interval 함수를 종료

## 콜백 
 - 함수의 인수로 사용되는 함수
 - `ex) setTimeout(함수, 시간)`
