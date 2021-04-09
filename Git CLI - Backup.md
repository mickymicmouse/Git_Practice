## Backup

#### Git hosting

* **github** , **gitlab** 등등 존재



#### 원격 저장소 생성

0. [Github](https://github.com) 접속

1. New Repository 선택
2. Directory 이름 선택
3. private/public 선택
4. Create Repository 선택



#### 저장소 연결 종류

* HTTP : 보안 X
* SSH : 보안 O



#### 원격 저장소 연결

* `git remote add origin [원격 저장소 주소]` 



#### Local -> Remote 

1. `git push --set-upstream origin master`  origin이 master라는 branch로 업로드
   
* `--set-upstream` 이후 git push의 기본 저장소를 origin master로 고정
   
2. github의 아이디와 비밀번호 입력

   ```
   Username for '깃 주소' = [Github ID]
   userpassword for '깃 주소' = [Github Password]
   ```



#### Remote -> Local (복제)

`git clone [깃 주소]` 



#### Remote -> Local (받아오기)

`git pull`



#### Git 커밋 메시지 변경하기

1. `git log`로 이력 확인
2. `git rebase -i HEAD~[원하는 커밋순서]`로 editor 접속
3. `pick` 을 `reword`로 변경하게 되면 해당 커밋메시지를 변경할 수 있는 editor로 접속
4. 커밋메시지 변경 후 저장



#### push 한 커밋 메시지 변경하기

1. Git 커밋 메시지 변경하기를 진행
2. git push --force [~~origin main~~ 브런치 이름]

