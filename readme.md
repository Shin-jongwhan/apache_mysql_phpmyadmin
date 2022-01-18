# 다운로드 경로
## apache
https://drive.google.com/file/d/1utm1LjFk0G14WDxajD7sGaBEZNJTNUzz/view?usp=sharing
### 압축을 풀면 Apache24 폴더만 쓰면 된다.
### <br/>
## php
https://drive.google.com/file/d/19t4PixNse6dqT1jbehTJ8mYnQPxX4gX5/view?usp=sharing
### <br/>
## phpMyAdmin
https://drive.google.com/file/d/1Cefj_JesAbO5WOLboBFEqWcOwj1Ji_Cj/view?usp=sharing
### <br/>
## MySQL
https://dev.mysql.com/downloads/installer/
![image](https://user-images.githubusercontent.com/62974484/149966040-a41009c8-0251-45e7-96f6-ec9635797ca5.png)
### <br/><br/><br/>

# 설정
## MySQL
### 1. MySQL 폴더 안에 **my.ini** 파일을 하나 생성한 후 아래와 같이 작성한다.
###
![image](https://user-images.githubusercontent.com/62974484/149967279-c2402331-48f0-48ad-be44-dff418299a4e.png)
```
[mysqld]
basedir="C:/Program Files/MySQL/MySQL Server 8.0"
datadir="C:/Program Files/MySQL/MySQL Server 8.0/data"
```
### <br/>
### 2. MySQL 환경 변수를 설정해준다.
### 환경 변수 -> path -> MySQL 경로 입력 및 저장
![image](https://user-images.githubusercontent.com/62974484/149969013-9bc5c161-c88d-40d6-ae57-df3cf1ae6f45.png)
#### <br/>
### 3. cmd를 관리자 권한으로 실행
### 아래 명령어를 치면 mysql 폴더 안에 data 폴더가 생성된다.
### > mysqld.exe --initialize
![image](https://user-images.githubusercontent.com/62974484/149969470-840984cc-7862-45ef-a278-e03845fa6911.png)
### <br/>
### 컴퓨터 id인 파일명을 가진 파일에서 root 계정의 초기 임시 비밀번호를 확인할 수 있다.
![image](https://user-images.githubusercontent.com/62974484/149969540-9f25bfaf-71fe-433c-86ed-0000141a1837.png)


