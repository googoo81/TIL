# 패스트캠퍼스 스타벅스 예제 후기

### <a href="https://github.com/googoo81/Fastcampus_STARBUCKS_Clone">코드</a>
<br>

## 글을 시작하기에 앞서
제가 문제 해결해 가며 클론코딩한게 아닌 강의를 따라한 점이라 저의 다른 회고록이랑은 다소 차이가 있을 것 같습니다. <br>
코드 소개와 느낀점을 위주로 글을 작성해 나갈테니 양해의 말씀 구합니다. <br>
많이 부족한 글이지만 이번에도 읽어주셔 감사하다는 말씀 올립니다! <br>
<br><br>

## 진행 날짜 <br>
`` 2022.09.07 ~ 2022.09.20 ``

<br><br>

## Code & library 소개 <br>

### 오픈 그래프 (Open Graph)

```
 og:type: 페이지의 유형(E.g, website, video.movie) 
 og:site_name: 속한 사이트의 이름 
 og:title: 페이지의 이름(제목) 
 og:description: 페이지의 간단한 설명 
 og:image: 페이지의 대표 이미지 주소(URL) 
 og:url: 페이지 주소(URL) 
```

웹페이지가 소셜 미디어로 공유되었을때 보이게 되는 정보를 설정합니다. <br>
- 슬랙 (Slack) ↓ <br>
![slack](https://user-images.githubusercontent.com/101445027/191243063-df9c9d3b-a5e4-4b87-9069-bedd4857e383.jpg)
- 카카오톡 (Kakao Talk) ↓ <br>
![kakao_og_example](https://user-images.githubusercontent.com/101445027/191243483-71bbf2d8-9dcf-4525-a778-edf3edc5d79d.jpg)

<br><br>

### 파비콘(Favicon, favorite icon)

웹페이지를 나타내는 아이콘, 웹페이지의 로고를 설정합니다. <br>
대부분의 경우 루트 경로에 `favicon.ico` 파일을 위치하면 자동으로 로딩하기 때문에 `<link />` 를 작성할 필요가 없습니다. <br>

> 단, 파비콘 이미지는 루트 경로에 있어야 합니다. <br>

<br><br>

### GSAP & ScrollToPlugin
<a href="https://greensock.com/gsap/">GSAP</a>은 자바스크립트로 제어하는 타임라인 기반의 애니메이션 라이브러리입니다. <br>
<a href="https://greensock.com/scrolltoplugin/">ScrollToPlugin</a>은 스크롤 애니메이션을 지원하는 GSAP 플러그인입니다. <br>
```
<script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.5.1/gsap.min.js" integrity="sha512-IQLehpLoVS4fNzl7IfH8Iowfm5+RiMGtHykgZJl9AWMgqx0AmJ6cRWcB+GaGVtIsnC4voMfm8f2vwtY+6oPjpQ==" crossorigin="anonymous"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/gsap/3.5.1/ScrollToPlugin.min.js" integrity="sha512-nTHzMQK7lwWt8nL4KF6DhwLHluv6dVq/hNnj2PBN0xMl2KaMm1PM02csx57mmToPAodHmPsipoERRNn4pG7f+Q==" crossorigin="anonymous"></script>
```

<br><br>

### Swiper
<a href="https://swiperjs.com/">Swiper</a>는 하드웨어 전환과 여러 기본 동작들을 갖춘 현대적 슬라이드 라이브러리입니다. <br>
> 강의를 따라 Swiper 6버전을 사용해 코딩을 진행했습니다!

<br><br>

### Youtube API
<a href="https://developers.google.com/youtube/iframe_api_reference?hl=ko">IFrame Player API</a>를 사용하여 유튜브의 영상을 가져와 활용할 수 있습니다. <br>
```
<!-- in HEAD -->
<script defer src="./js/youtube.js"></script>

<!-- in BODY -->
<div id="player"></div>
```

<br><br>

### ScrollMagic
<a href="https://github.com/janpaepke/ScrollMagic">ScrollMagic</a>은 스크롤과 요소의 상호 작용을 위해 사용하는 자바스크립트 라이브러리입니다. <br>
대표적으로 어떤 요소가 현재 화면에 보이는 상태인지를 확인할 때 사용할 수 있습니다. <br> 
```
<script src="https://cdnjs.cloudflare.com/ajax/libs/ScrollMagic/2.0.8/ScrollMagic.min.js"></script>
```

<br><br>

### Lodash
<a href="https://lodash.com/">Lodash</a>는 다양한 유틸리티 기능을 제공해주는 자바스크립트 라이브러리입니다. <br>

<br><br>

## 글을 마무리 하면서

### 느낀점

이 때까지 내가 어떤 방식으로 코드를 작성해 왔고 어떤 문제가 있었는지 객관적으로 알 수 있었던 기회가 된 것 같다. <br>
여러 태그의 효율적인 활용법과 자바 스크립트를 체험해 볼 수 있는 좋은 기회가 됐다. <br>
사실 전에 <a href="https://github.com/googoo81/Instagram_Clone_Coding">인스타그램 클론코딩</a>했었던게 확실히 나사가 빠져있는 코드라는걸 느끼게 된 것 같다. <br>
결과적으로 나 자신을 돌아볼 수 있었던 기회가 된 것 같아 좋고, <br> 
성장할 수 있는 계기 또한 된 것 같아 ~~강의 비용이 아깝지가 않구나ㅋ~~ 좋은 경험을 했다고 생각한다. <br>
_(+ 자바 스크립트 개꿀잼)_

<br><br>

### 앞으로 개선해야 할 점
class, id 선택자를 조금더 효율적이게 활용해야겠다. <br>
이미지와 css, js파일을 따로 만들어서 조금더 관리를 수월하게 할 수 있도록 해야겠다. <br>
다른 사람이 내 코드를 보았을때 조금더 이해하기 쉽도록 주석 등을 사용하거나 섹션별로 정리하여 가독성을 높이도록하자. <br>

<br>

#### 앞으로 내 코드를 보여줬을때 부끄럽지 않은 먿찐 개발자가 되도록하자!
