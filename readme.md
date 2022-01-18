# 다운로드 경로
## apache
https://drive.google.com/file/d/1utm1LjFk0G14WDxajD7sGaBEZNJTNUzz/view?usp=sharing
### 압축을 풀면 Apache24 폴더만 쓰면 된다. C:/으로 이동시켜준다(아래 그림).
### <br/>
## php
### php는 thread safe 버전으로 사용한다.
### 압축을 푼 후 C:/으로 이동시켜준다.
https://drive.google.com/file/d/19t4PixNse6dqT1jbehTJ8mYnQPxX4gX5/view?usp=sharing
![image](https://user-images.githubusercontent.com/62974484/149971655-7106efff-bbb1-45c8-a2c3-67d8d12a0ff4.png)
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
### <br/>
### 4. cmd 창에 아래 명령어를 실행하면 MySQL 서비스가 install된다.
### > mysqld.exe --install
### 5. 윈도우 검색 - 서비스를 검색해서 실행 -> MySQL을 실행하자.
### <br/>
### 6. root 비밀번호 설정
### cmd 창에서 MySQL을 실행한다.
### > mysql -u root -p 친 후 초기 임시 비번을 복붙한다.
### 비번 변경
### > alter user 'root'@'localhost' identified with mysql_native_password by 'root';
### 확인
### select host, user, plugin, authentication_string, password_last_changed from user;
### 하고 quit으로 나간 다음 재접속해보기
![image](https://user-images.githubusercontent.com/62974484/149970901-a463be2e-be2e-4299-829f-2189f55d6601.png)
### <br/><br/>
## php 설정
### 1. php.ini-developmen를 복사해서 php.ini로 이름 변경한다.
![image](https://user-images.githubusercontent.com/62974484/149972069-7c7807e4-1692-48f1-be2b-51fb3fb1a52f.png)
### 2. php.ini 설정
### ; 는 꼭 지우기
### extension_dir = "C:/php8/ext/"
### .
### extension=mbstring
### extension=mysqli
### extension=openssl
### extension=pdo_mysql
### 그 다음 C:/windows/로 옮겨준다.
### 원래 php8 폴더에 있던 것은 충돌이 날 수도 있다고 하니 삭제해준다.
![image](https://user-images.githubusercontent.com/62974484/149972040-3b38c78c-f04c-4ff1-83a7-cd9cbefad865.png)
