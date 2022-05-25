# Javascripts function and argument
<br>

## 함수
### 의미 
 - 어떠한 코드를 캡슐화 하여서 여러번 실행할 수 있게 해줌
 <br><br>

### 실행과 선언
 - 실행 : (함수명) (); <br>
    └  argument(인수)를 보내야 하는데 인수란 함수를 실행하는 동안 어떤 정보를 함수에게 보낼 수 있는 방법이다.
   
 - function 선언 : <br>
   function (함수명) () { <br>
   (실행코드) <br>
   } <br> 
   
### return
 - 함수를 통해 console이나 alert가 아니라 결과값을 받기 원할 때 사용한다
 - return안의 내용을 실행, 계산 후에 함수를 나가면서 값을 반환하는 역할을 한다.
   (비유: 빵반죽을 만들어 냉장고에 숙성시켜 놓은 것을 꺼내는 것)
   <br>
 
#### return 특징
 - function안에서 return과 추가작업을 입력하면return만 작업하고 추가 수행은 이뤄지지 않음.<br> 
   만약 return 앞에 기타작업이 있다면 이 작업은 수행된다. 즉, return"까지만" 수행됨
   <br>
   

#### player.points(); 라고 사용하지 않았다. 왜냐하면 player.points은 function이 아니기 때문임
<br>

### 특징
 - function sayHello( ){ <br>
   console.log("Hello!"); <br>
   }; <br><br>
   &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; ↓
   소괄호 안에 작성하는 것은 실행버튼을 누를 때마다 발생
 - function의 값은 function 안에서만 존재
   
 <br>

## 인수

### 의미
 - function을 실행하는 동안 어떤 정보를 function에 보낼 수 있는 방법 <br>

### 특징
 - 하나만 받을 수 있는게 아니라 여러개를 받을 수 있음
 - object 안에서 매개변수가 argument를 받는 방식<br>
   ex)<br>
   const player = {<br>
   name : function(Name) {<br>
   console.log("Your Name is " + Name + " 입니다.")<br>
   } ,<br>
   sayHello : function(Age) {<br>
   console.log("Your age is " + Age + " 입니다." )<br>
   }<br>
 <br><br><br><br><br><br>
