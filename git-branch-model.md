# git-flow
(출처 : https://beomseok95.tistory.com/207)  

### git-flow 간단하게 살펴보기

Git-flow를 사용했을 때 작업을 어떻게 하는지 살펴보기 전에 먼저 Git-flow에 대해서 간단히 살펴보겠습니다.  
Git-flow에는 5가지 종류의 브랜치로 나누어지게 됩니다.  

항상 유지되는 메인 브랜치들(master, develop)과  

일정 기간 동안만 유지되는 보조 브랜치들(feature, release, hotfix)이 있습니다.   
  
1. master : 제품으로 출시될 수 있는 브랜치  
2. develop : 다음 출시 버전을 개발하는 브랜치  
3. feature : 기능을 개발하는 브랜치  
4. release : 이번 출시 버전을 준비하는 브랜치  
5. hotfix : 출시 버전에서 발생한 버그를 수정 하는 브랜치  
<img src="https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fk.kakaocdn.net%2Fdn%2F9zIJi%2FbtqxhK5q0Pi%2FIdKFE5wqKCq53qTYulzZxK%2Fimg.png">

### master 와 develop 브랜치
- master와 develop브랜치가 존재하고, develop브랜치는 master 브랜치에서 시작된 브랜치입니다.

### develop 브랜치
- develop브랜치에는 상시로 버그를 수정한 커밋들이 추가되게 됩니다.
- 새로운 기능을 추가하는 경우,  
develop 브랜치에서 시작하는  
feature브랜치를 생성합니다.

### Feature 브랜치
- 이 feature 브랜치에서 기능 추가 작업이 완료되었다면, develop 브랜치로 merge 합니다.
- 새로운 기능을 추가하는 경우 develop 브랜치에서 시작하는 feature브랜치를 생성합니다.

### release 브랜치
- develop 브랜치에서 이번 버전에 포함되는 모든 기능이 merge 되었다면,
QA를 위해 develop브랜치에서 release브랜치를 생성합니다.
- QA를 무사히 통과하게 되면
release 브랜치를 master 와 develop 브랜치로 merge 합니다.
- QA를 진행하면서 발생한 버그들은 모두 release 브랜치에 수정되게 됩니다.

마지막으로,  
출시된 master 브랜치에서 버전 태그를 추가합니다.

# 참고 링크  

- [성공적인 git branch 관리 Model](http://amazingguni.github.io/blog/2016/03/git-branch-%EA%B7%9C%EC%B9%99)
- [우린 git-flow를 사용하고 있어요](https://woowabros.github.io/experience/2017/10/30/baemin-mobile-git-branch-strategy.html)
- [git-flow Integration으로 git-flow 심플하게 운영하기](https://jojoldu.tistory.com/268)
- [git-flow cheatsheet](https://danielkummer.github.io/git-flow-cheatsheet/index.ko_KR.html)
