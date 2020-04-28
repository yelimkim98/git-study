# 용어 정리

## 개요

- 명령어를 사용하는 `목적`과 어떤 작업을 수행하는지 `행위`를 작성한다.
- 필요에 따라 이미지 또는 링크 추가를 적극 권장한다.
- 명령어에 사용할 수 있는 옵션 (e.g. `--mixed`)중에서 자주 사용되는 것을 추가한다.
- 다른 사람이 정리하는 용어라도 추가하고 싶은 내용이 있다면 추가한다.
- 경우에 따라서 용어에 대한 부가설명이 길어질 수 있는데, 이 때에는 별도의 페이지로 분리한다.
- 리스트에 없는 용어 중에서 필요하다고 생각되는 용어가 있다면 새로 추가한다.
- 월요일, 화요일 팀이 문서를 정리한 후에는 하나로 합친 후 우아한테크위키에 기록할 예정이다.

# 명령어

## 기본

### git

### init

### add

### commit

- `-m`
- `--amend`

### push

- `-f`

### pull

### checkout

### branch

- 생성, 삭제

### clone

---

## 응용

### remote
- git remote : 연결된 remote 저장소들에 붙인 이름들 출력 (리모트 = 원격 맞나?)
```
$ git remote
origin
```
- git remote -v : 연결된 remote 저장소들 이름 & 원격저장소 링크 
```
$ git remote -v
origin httpsorigin  https://github.com/yelimkim98/jwp-chess.git (push)
```
- git remote add [리모트이름] [경로] : 새 리모트를 추가합니다. [경로]영역에는 URL이나 파일경로를 넣을수 있습니다.
```
[root@localhost test]# git remote add test https://github.com/yelimkim98/java-chess.git
[root@localhost test]# git remote -v
test	https://github.com/yelimkim98/java-chess.git (fetch)
test	https://github.com/yelimkim98/java-chess.git (push)
// push, fetch 왜 따로 생기는지 이런거 모르겠다..

```
### fetch
- git fetch 
### merge

### rebase

- squash, interactive mode
    - p, pick = use commit
    - r, reword = use commit, but edit the commit message
    - e, edit = use commit, but stop for amending
    - s, squash = use commit, but meld into previous commit
    - f, fixup = like "squash", but discard this commit's log message
    - x, exec = run command (the rest of the line) using shell

### reset

- `--soft`
- `--hard`
- `--mixed`

### HEAD

- pointer
- `~`
- `^`

### stash


### reflog

### cherry-pick

---

## 기타

### diff

### tag

### log

### revert

### status

### blame

### help

---

# 개념 용어

### version

### index

### local

- working directory
- staging area
- .git directory(repository)

### repository

- origin
- upstream

### master

### snapshot

### checksum(hash)

### blob

### stage

### unstage

### fast-forward

### .gitignore

### pull request

### issue

### contribute

### contributor

### fork


# 참고 링크

- [git | 기초](https://git-scm.com/book/ko/v2/%EC%8B%9C%EC%9E%91%ED%95%98%EA%B8%B0-Git-%EA%B8%B0%EC%B4%88)
- [git | reset 명확히 알고 가기](https://git-scm.com/book/ko/v2/Git-%EB%8F%84%EA%B5%AC-Reset-%EB%AA%85%ED%99%95%ED%9E%88-%EC%95%8C%EA%B3%A0-%EA%B0%80%EA%B8%B0)
- [git add -p 와 git commit -v 의 사용](https://blog.outsider.ne.kr/1247)
- [git guides: 용어 정리](https://optimalbi.com/git-guides-terminology/)
- [fetch | 원격 저장소](https://backlog.com/git-tutorial/kr/stepup/stepup3_2.html)
- [rebase로 병합하기 | 튜토리얼1: 브랜치를 사용해 보자](https://backlog.com/git-tutorial/kr/stepup/stepup2_8.html)
- [https://git-scm.com/book/ko/v2/Git-도구-히스토리-단장하기#_squashing](https://git-scm.com/book/ko/v2/Git-%EB%8F%84%EA%B5%AC-%ED%9E%88%EC%8A%A4%ED%86%A0%EB%A6%AC-%EB%8B%A8%EC%9E%A5%ED%95%98%EA%B8%B0#_squashing)
- [https://git-scm.com/docs/git-stash](https://git-scm.com/docs/git-stash)
- [https://suwoni-codelab.com/git/2018/04/06/Git-stash/](https://suwoni-codelab.com/git/2018/04/06/Git-stash/)
- [https://wit.nts-corp.com/2014/03/25/1153](https://wit.nts-corp.com/2014/03/25/1153)
- [https://git-scm.com/docs/git-commit](https://git-scm.com/docs/git-commit)
