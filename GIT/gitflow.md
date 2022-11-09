# Git Flow
### Git으로 개발할 때 거의 표준과 같이 사용되는 방법론임.
- Git Flow는 기능이아닌 서로간의 약속인 방법론 입니다 

- master : 초기 커밋
- develop : master branch 병합 
- feature : develop branch의 서브 branch > 기능들을 구현한뒤 develop branch에서 병합
- release : 배포를 위해서 master branch로 가서 QA(품질검사)함.
- hotfix : 배포뒤 오류등을 긴급 수정한다