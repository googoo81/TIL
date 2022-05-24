# js_data_type
<br>

## 자료형
 - true: 2진수의 1처럼 '참'과 '켜짐'을 의미함.
 - flase: 2진수의 0처럼 '거짓'과 '꺼짐'을 의미함.
 - null: '그냥'없음을 뜻함.
 - undefined: 설정은 되었으나 내용물이 비엇음.
<br><br>

### underfined와 null의 차이점
 - undefined = 박스만 만들어 놓은 상태
 - null = 박스만들고 아무것도 안넣고 포장함
<br><br><br><br><br><br>

## Aray

### Aray way
 - elemental 하나를 불러올때 0부터 센다.
 - 대괄호 안에 ',(쉼표)'로 만들고 싶은 변수들을 엮으면됨
 - ( ex) const daysOfWeek = ["mon", "tue", "wed", "thu", "fri", "sat"]; )
<br><br>

### add Aray 
 - (variable name).push("(elemental name)");
 - ( ex) daysOfWeek.push("sun"); )
<br><br>

### 목적
 - 하나의 variable 안에 데이터의 list를 가지는 것
 - 여러개의 elemental들을 한데 묶는 것
<br><br>

### Array Object
 - property를 가진 데이터를 저장해주며, { } 를 사용함
 - property를 추가 가능
<br><br>

#### Array Object 예시
 const player = {<br>
    name: "googoo",<br>
    point: "81",<br>
    fat: true,<br>
};<br><br>

- property 추가또는 값 변경 Object 바깥에서. 
