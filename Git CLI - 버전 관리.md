## Git CLI - 버전 관리

#### 버전 생성

* **Working Tree**
  * 파일을 수정하는 곳

* **Staging Area**
  * 버전을 만드려고 하는 파일들
* **Repository**
  * 만들어진 버전



#### Git 버전 생성 및 확인

* `nano` make file

* `cat` 파일 내용 확인

* `git init`  Initialize repository

* `.git`  git repository

* `git status` working tree status
* `git add .` Working tree의 모든 파일을 Staging Area로 업로드 *add to staging area*

* `git commit -m [message]` Staging Area의 파일을 repository로 올리기 *create version*

* `git log` show version 

* `q` exit

* `git log --stat` 각 로그에 대해 자세한 변경 사항 설명

* `git diff` 이전 버전과 현재 작업한 내용의 변경 사항 확인 

* `git log -p` 각 버전의 자세한 변경사항 확인



#### 시간이동

* `git checkout [commit ID]` 버전을 만든 시점으로 이동

* `git checkout master` 현재 시점으로 이동



#### Add 되어 있는 파일만 commit 하기

* `git commit -am [message]`



#### 기본 에디터 변경

* `git config --global core.editor "[에디터 이름]"` 
  * nano, vi, vim 등



#### 버전 삭제

* `git reset --hard [commit ID]` 특정 버전이 되겠다.
  * `--hard` 수정하고 있던 것도 지우고 특정 버전으로 이동



#### 버전 되돌리기(버전을 삭제하지 않고, 되돌리는 것)

* `git revert [commit ID]` commit ID가 의미하는 버전에서 **진행된 사항**을 되돌리겠다. 
  * 즉, R3로 돌아가기 위해서는 R4를 Revert 해야함
  * 또한, 충돌을 방지하기 위해 역순으로 모두 Revert 해야함



#### 파일 선택

`.gitignore` 무시할 파일의 이름을 적어서 작성

`tag` commitID 대신 이름을 붙여서 이동할 수 있도록