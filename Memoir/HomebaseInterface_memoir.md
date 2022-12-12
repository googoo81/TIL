# Hi 일부 제작 및 중간발표 후기 <br>

### <a href="https://github.com/GSM-MSG/Hi-FrontEnd">코드</a>
<br>

## 시작하게 된 이유
 맛소금(MSG) 팀에서 인턴쉽 마무리로 팀원을 골라내기 위해서 선배들의 권유로 시작하게 되었다. <br>
 
<br>

## 어째서 'Hi' 였는가?
 현재 재학중인 학교에는 기숙사 자습을 온라인 웹으로 신청한다. <br>
 홈베이스 또한 신청해야 이용할 수 있는데, 오프라인으로 신청해야 한다. <br>
 "이것도 온라인으로 신청할 수 있게 만들어보자!" 하고, Hombase Interface 해서 약자를 따서 Hi를 제작하게 되었다 . <br>
 
<br>
 
## 진행 날짜
 `2022.11.07 ~ 2022.11.30`
 
<br>

## 멤버
 > 송현우 - PL <br>
 > Front-End <br>

 > 김희망 - PL <br>
 > Back-End <br>
 
 > 김대진 - PL, PM <br>
 > 정민석 <br>
 > Android <br>
 
 > 박준서 - PL <br>
 > 박건우 <br>
 > iOS <br>
 
 > 강민수 - PL <br>
 > Design <br>

<br>

## 문제 <br>

### 1. 이메일 형식
 로그인 화면이랑 회원가입 화면에 학교 이메일로만 기입되어야 하는데, <br>
 input 태그안에 내용물 작성을 제한하는 방법은 html에서 지원해주는 maxlength 길이 제한 밖에 없었다. <br>
 
### 2. 인증번호 숫자 확인
 인증번호 숫자 확인을 하는 모달창을 만드는데, 인증번호를 작성하는 input을 만드는데, <br>
 숫자가 작성되면 테두리가 노란색으로 바뀌어야하고, 비어 있다면 회색 테두리, 포커스 중일때는 테두리 없이 그림자가 생겨야한다. <br>
 그 중 2번째 3번째만 html과 css로 해결할 수 있었는데 1번째는 그렇지 않았다. <br>
 
<br><br>
 
## 해결 <br>

### 1. 이메일 형식
 input을 id로 js에 연결하여 정규식 확인을 통해 제한하였다. <br>
 ``` let reg_id = /[s][0-9][0-9][0][0-9][0-9]/; ``` <br>
 
### 2. 인증번호 숫자 확인
 인증번호 확인란이 4칸의 input으로 이루어져 있는데, <br>
 4칸 전부 각자의 변수를 할당해서 if문으로 숫자의 범위를 정해주어서 전부 if문에 돌아가서 조건에 맞으면 색을 빠꿔 주었다. <br>
 
<br><br> 

## 진행중 느낀점
 처음으로 하는 BE, AOS, iOS, Design의 많은 팀원들과 합을 맞춰보는 프로젝트였는데, <br>
 많은 인원의 프로젝트 팀원들과 합을 맞춰보는 과정이 힘들었던거 같다. <br>
 프로젝트를 진행하면서 PM을 바꾸는 등 여러가지 일이 있었는데, <br>
 다들 너무 열심히 해주어서 보람찬 프로젝트가 됐던거 같다. <br>
 
<br><br>
 
## 앞으로 배워야 할 점
 js의 명확한 한계를 느끼게된 계기가 된거 같다. 고로 리액트 같은 기술스택들을 열심히 배워야겠다. <br>
 BE, AOS, iOS, Design의 여러 팀원들과 진행하다 보니 서로의 진행 상황같은 상태등을 잘 살피는게 중요하다고 느꼈다. <br>
 서로의 상황을 잘 볼 수 있는 방법을 배우면 좋겠다고 느꼇다. <br>
 
 <br><br>
 
 ## 결과물 사진
 
![1](https://user-images.githubusercontent.com/101445027/207029228-a787bda0-c169-480d-82b9-0b489cbba0ec.PNG)
![2](https://user-images.githubusercontent.com/101445027/207029233-e634bf1c-7356-4c05-9a31-8549cd6b41ea.PNG)
![3](https://user-images.githubusercontent.com/101445027/207029241-2113df64-23d3-476e-afb3-ee7c0a07675f.PNG)
![4](https://user-images.githubusercontent.com/101445027/207029372-7fda00d4-2bfc-47e8-94a9-fa5edca2b261.PNG)
![5](https://user-images.githubusercontent.com/101445027/207029397-ddfd48a8-9287-4685-a8fc-f3246fc22495.PNG)
![6](https://user-images.githubusercontent.com/101445027/207029640-0f065c74-741f-4cfa-8a5b-dac80d7e471c.PNG)
