## 📌 한 번만 하면 되는 과정
### 1. Git bash 설정
- git bash를 다운받은 후에 먼저 git bash와 인터넷의 gitHub를 연결시켜줘야 해.
- 연결하는 방법은 다음과 같아.
```bash
git config --global user.name "본인 아이디"
git config --global user.email "본인 이메일"
```
ex)
```bash
git config --global user.name "neulbokim"
git config --global user.email "twinsister1@naver.com"
```

### 2. 본인의 저장소로 fork 하기
- 팀의 원격 저장소를 개인별 원격 저장소에 복사하는 과정이라고 생각하면 돼.
- 지금은 mae22ai/assignment에 있지만, fork하면 neulbokim/assignment에서 확인할 수 있어!
- mae22ai/assignment에서 fork를 눌러주면 돼.

### 3. fork한 저장소로 이동 후 저장소 주소를 복사하기
- 자기 개인별 원격 저장소를 개인별 로컬 저장소에 clone하기 위한 거야
- 내 repository에서 fork한 저장소를 확인해줘

### 4. fork한 저장소를 자신의 컴퓨터로 clone하고, 해당 폴더로 이동하기
- 3번에서 복사한 주소를 붙여 넣으면 돼
```
pwd #현재 디렉토리 위치 확인(present working directory)
cd #디렉토리 변경(change directory)
git clone <https://github.com/{본인 아이디}/{레포지토리 이름}.git>
```
여기서 `cd`는 `change directory` 즉 현재 내가 있는 디렉토리(폴더) 위치를 {레포지토리 이름} 폴더로 옮기겠다는 뜻이야
즉 예를 들면
```
cd /Users/hyeonseokim_macbookpro/Desktop/서강대학교/2025/2025년\ 1학기/AI인문융합LAB/repos
git clone https://github.com/neulbokim/assignment.git
```
이렇게 하면 내가 관리하고 싶은 'repos'라는 디렉토리에서 관리할 수 있게 돼!!

## 📌 과제 제출 때마다 하는 과정
### 1. 본인 개인별 원격 저장소의 레포지토리에 들어가서 레포지토리 동기화하기
-  neulbokim/mae22ai/assignment 에 들어가서 `Sync-fork`=> `Update branch`누르기
  
### 2. 과제를 완성하고 ctrl+s 눌러서 모두 저장한 후, `add`, `commit`, `push` 명령어로 본인의 원격 저장소에 push하기
```bash
# 변경된 파일 확인
git status 


# add 방법 (1) 진행한 과제 파일 여러 개 나열해서 추가
git add 01_시작하기_김현서.ipynb 02_변수_김현서.ipynb 03_문자열_김현서.ipynb
# add 방법 (2) 진행한 과제 파일 하나씩 add하기
git add 01_시작하기_김현서.ipynb
git add 02_변수_김현서.ipynb
git add 03_문자열_김현서.ipynb
# add 방법 (3) 본인 디렉토리 전체 add하기
git add neulbokim/


# commit 하기: 작업한 내용에 대해 기록
git commit -m "[001-050] 김현서 과제 제출"


# push하기: 로컬 저장소 -> 원격 저장소로 Push
git push
```

### 3. Pull Requests 하기
- `pull request` 를 보낼 때 아래의 양식 지켜서 보내기!
  ```
  pr 제목: [001-050] 김현서 과제 제출
  내용: 해당 과제를 하면서 어려웠던 점이나 새로 알게 된 점 간단히 정리
  ```
  ex)
  ```
  [001-050] 김현서 과제 제출

  파이썬 시작하기, 파이썬 변수, 파이썬 문자열 과제를 진행함.
  split 부분이 어려웠음.
  replace 메서드를 익숙하게 써야 할 것 같음.

  질문
  002 print 기초에서 '가 있는 경우에 큰 따옴표로 감싸는 것 말고도 다른 방법으로 처리할 수 있나요?
  
  ```
  
