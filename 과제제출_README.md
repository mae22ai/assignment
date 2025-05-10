## 📌 한 번만 하면 되는 과정
### 1. 본인의 저장소로 fork 하기
- 팀의 원격 저장소를 개인별 원격 저장소에 복사하는 과정이라고 생각하면 돼.
- 지금은 mae22ai/assignment에 있지만, fork하면 neulbokim/assignment에서 확인할 수 있어!

### 2. fork한 저장소로 이동 후 저장소 주소를 복사하기
- 자기 개인별 원격 저장소를 개인별 로컬 저장소에 clone하기 위한 거야
- 내 repository에서 fork한 저장소를 확인해줘

### 3. fork한 저장소를 자신의 컴퓨터로 clone하고, 해당 폴더로 이동하기
- 2번에서 복사한 주소를 붙여 넣으면 돼
```
pwd #현재 디렉토리 위치 확인 (present working directory)
cd #디렉토리 변경 (change directory)
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
  
### 2. 과제를 완성한 후, `add`, `commit`, `push` 명령어로 본인의 원격 저장소에 push하기
```bash
git status #변경된 파일 확인
git add 과제1_김현서.ipynb # 진행한 과제 파일만 추가
git commit -m "김현서 과제1 제출" # 작업한 내용에 대해 기록
git push # 로컬 저장소 -> 원격 저장소로 Push
```

### 3. Pull Requests 하기
- PR 템플릿에 맞춰 과제 제출하기!
  
