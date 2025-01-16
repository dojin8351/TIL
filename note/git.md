# git 필기

## **git 계정 설정시 최초 1회**

- github은 전역으로 관리 `--global`
    - 정말 최초 1회
- gitlab은 지역으로 관리 `--local`
    - 레포를 만들때마다 최초 1회

---

- gitlab
    - `$ git config --local user.email '[나의 github email]'`:
        - git 작업하는 폴더에만 gitlab email 설정
        - `$ git config --local user.email`
    - `$ git config --local user.username '[내 github username]'` :
        - git 작업하는 폴더에만 gitlab username 설정
        - `$ git config --local user.username`

---

- github
    - `$ git config --global user.email '[나의 github email]'`:
        - 내 로컬 컴퓨터 전역에 github email 설정
        - `$ git config --global user.email`
    - `$ git config --global user.name '[내 github username]'` :
        - 내 로컬 컴퓨터 전역에 github username 설정
        - `$ git config --global user.name`

## **git으로 폴더를 앞으로 관리할때 최초 1회**

- `$ git init` : git 시작하기, 이 특정 폴더를 git으로 관리할거야!
    - `$ git remote add origin [github repo 주소]` :
    - remote 등록
    - 레포지토리 이름 등록
- `$ git remote -v`

## **git으로 작업할때 빈번하게**

- `$ git status` :
    - git 으로 관리되고 있는 폴더의 현황 조회
    - commit 전단계까지만 확인 가능!
- `$ git add` : git 에게 tracking을 요청
    - `.git` 이 있는 최상단에서 해야만 한다. 🍗
    - staging area 에 올려줘!
        1. `$ git add [파일이름1.확장자]`
        2. `$ git add [파일이름1.확장자] [파일이름2.확장자]`
            - 띄어쓰기가 포함된 파일이다! -> `'` / `"`따옴표로 감싸준다
        3. `$ git add .` : 전체를 다 올려줘
- `$ git commit -m '[커밋 메시지]'` :
    - staging area에 올린 컨텐츠에 커밋 메시지 남기기
    - 커밋 메시지
        - 명령조로 작성한다.
- `$ git log`
    - 커밋 남긴 후에만 확인 가능.
    - 커밋 메시지 확인
    - `$ git log --oneline`
- `$ git push origin master` : github에 파일 모두 올리기
- `$ git pull origin master` : github에 있는 파일 내려받기
    - 폴더 생성
    - 폴더에 들어가서 `$ git init`
    - 폴더 안에서 `$ git remote`
- `$ git clone [나의 github repo 주소]` :
    - 폴더를 만들지 않고도 바로 내려받을 수 있다.
    - A가 A꺼를 clone 받았다. -> `add` `commit` `push`
    - B가 A꺼를 clone 받았다. -> `pull request` == B의 코드를 A의 레포에 반영하고 싶을 때

## git branch

- intro

  master (통로 == 브랜치)

  origin (별명)

  브랜치 → 새로운 통로 만들기


- 브랜치 시작하기
    - `$ git branch` : 나의 현재 브랜치 현황
        - `*` 너가 지금 있는 브랜치 (초록색으로 표현됨)
    - `$ git branch [브랜치 이름]` : 브랜치 생성
        - 아무런 응답이 없다
        - 이미 있는 브랜치는 생성 새로 불가
    - `$ git switch [브랜치 이름]`/ `$ git checkout [브랜치 이름]` : 해당 브랜치로 이동
        - 브랜치 현황에 있는 브랜치로만 이동 가능


## git merge

e.g. Branch 1 → Branch 2

- Branch 1에 있는 파일들을
    1. `add` `commit`
    2. Branch2로 이동
    - `$ git merge [merge하고 싶은 브랜치 이름]`

## pull request

github에서 브랜치를 merge할 때 사용하는 일종의 명령

## fork

다른 사람 저장소 가져오기