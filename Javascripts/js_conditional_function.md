# js_conditional_function <br><br>

## 조건문<br><br>

### prompt<br>

#### 특징<br>
 - 사용자에게 창을 띄어 값을 받음
 - typeof라는 키워드를 쓰면 type를 볼 수 있음, prompt();에서 숫자를 입력해도 string이라고 뜸. string이 디폴트이기 때문임
 - ex)
    const age = prompt("how old are you?"); <br>
    console.log(typeof age); <br>
 - 한 type로 받아서 다른 type로 바꾸는 작업을 해야함( ex) "15" -> 15 )<br>

#### 단점
 - 사용시 답을 할때까지 코드에 실행을 멈춤
 - 매우 오래된 방법임 
 - 예쁘지 않음 
 - css로 못 바꿈<br>

### parseInt<br>

#### 의미
 - string을 number로 변환해주는 함수임<br>

#### 특징
 - 숫자로 변환이 되어야 비교가 가능함 <br>
  ( ex) console.log(typeof "15", typeof parseInt("15")); -> string number )
 - ( 특) "숫자"가 아닌게 입력되면 변환불가) [NaN(nat a number)] )<br>


### isNaN <br>

#### 의미
 - 입력받은 것이 NaN인지 판별하는 방법
 - ex)<br>
  const age= parseInt(prompt (“How old are you?”));<br>
  console.log(isNaN(age));<br>
  const age= parseInt(prompt (“How old are you?”));<br>
  console.log(isNaN(age));<br>
 - 글자 입력시 ture, 숫자 입력시 false가 출력됨 <br>

#### condition은 boolean(true , false)으로 판별가능해야 함 <br>
