# 함수형 프로그래밍
함수형 프로그래밍에 대해 설명하기 앞서..

> 잠시 당신이 나무꾼이라고 가정해보자. 당신은 숲에서 가장 좋은 도끼를 가지고 있고, 그래서 가장 일 잘하는 나무꾼이다. <br />
  그런데 어느 날 누가 나타나서 나무를 자르는 새로운 패러다임인 전기톱을 알리고 다닌다. <br />
  이 사람이 무척 설득력이 있어서 당신은 사용하는 방법도 모르면서 전기톱을 사게 된다. <br />
  당신은 여태껏 했던 방식대로 시동을 걸지도 않고 전기톱으로 나무를 마구 두들겨댄다. <br />
  곧 당신은 이 새로운 전기톱은 일시적인 유행일 뿐이라고 단정하고 다시 도끼를 쓰기 시작한다. <br />
  그때 누군가 나타나서 전기톱의 시동 거는 법을 가르쳐 준다. <br />
  _- 닐포드, "함수형 사고"_


 <br /> <br />

## 특징

### 순수 함수
함수형 프로그래밍에서는 입력 값에 대해 항상 동일한 출력 값을 반환하는 순수 함수를 사용한다. <br />
함수가 외부 상태에 의존하지 않고, 외부 상태를 변경하지 않는 함수이다. <br />
이러한 함수는 부작용이 없어 예측 가능하며 테스트하기 쉽다. <br />

 <br />

### 불변성
데이터 구조를 변경할 수 없도록 설계하여 상태 변경을 피하고, 새로운 데이터 구조를 생성하는 방식으로 작업한다. <br />
이는 병렬 처리와 예측 가능한 코드 동작을 촉진하며, 버그를 줄일 수 있다. <br />

 <br />

### 고계 함수
함수를 값으로 취급하고, 다른 함수에 전달하거나 함수에서 반환할 수 있는 고계 함수를 사용한다. <br />
이는 코드의 재사용성을 높이고, 추상화 수준을 높여준다. <br />

 <br />

### 함수 합성
두 개 이상의 함수를 조합하여 새로운 함수를 만드는 것을 지향한다. <br />
이를 통해 코드를 간결하게 유지하고, 각각의 작은 함수들로 구성된 모듈화된 코드를 작성할 수 있다. <br />

 <br />

### 선언형 프로그래밍
함수형 프로그래밍은 어떻게 어떤 일을 달성할 것인지를 설명하는 선언적인 스타일을 취한다. <br />
이는 명령형 프로그래밍에서 사용되는 명령어의 순서와 상태 변경에 대한 접근과는 대조적이라고 할 수 있다. <br />

 <br />

### 데이터 불변성
함수형 프로그래밍에서는 데이터를 변경할 수 없도록 설계한다. <br />
새로운 데이터를 만들어내거나 변형시키는 방식으로 작업한다. <br />

 <br />

## 장점
함수형 프로그래밍은 주로 수학적인 개념과 결합되어 있고, 특히 람다 대수와 같은 이론적 기반을 기반으로 한다. <br />
함수형 프로그래밍은 병렬 처리 및 분산 시스템과 같은 현대적인 컴퓨팅 환경에서 특히 중요하다. <br />
또한 코드의 안정성과 유지보수성을 향상시킬 수 있다. <br />

## 정리
**JS는 함수형 프로그래밍을 지향하는 언어이다.**

