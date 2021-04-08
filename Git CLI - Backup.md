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