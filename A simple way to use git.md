## A simple way to use git 
### 1. pull
- git pull로 Remote RP에 있는 내용 Local에 update
- ※ pull 과정없이 push할 경우 local에 있는 내용이 덮어지면서 Remote RP에 있는 내용이 없어질 수 있음. 

### 2. Add
- git status -> 현재 상태 확인
-     1. Clean -> 현재 워킹 디렉토리가 Clean한 상태

-     2. Red -> 보통 Untracked  files일 경우가 대부분으로 tracked 상태로 변환시켜 줌( git add . or git add "파일명")  

-     3. Green-> Tracked  file이므로 commit을 할 수 있는 상태

- git reset HEAD [File명]- > add 취소

### 3. Commit
- git commit -m "Memo"


### 4. Push
git push origin main 


### +α 
- Clone<br>
git clone "RP URL"

- Commit 이력 확인 <br>
git log
