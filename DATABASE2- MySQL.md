# [DATABASE2- MySQL]

## 수업소개
- Relational database
- 무료이면서, 오픈소스이고, 3대 데이터베이스 중에 하나인 MySQL의 입문 수업
- 수업구성
	- MySQL 소개
	- 서버, 스키마, 테이블 만드는 법
	- 테이블에 데이터를 입력하고, 출력하는 법
	- JOIN
	- 데이터베이스 클라이언트와 서버의 개념
	- MySQL Workbench 사용법


## 데이터베이스의 목적
- 스프레드시트 VS. 데이터베이스
- 데이터베이스는 컴퓨터 언어를 통해 제어 가능


## MySQL 설치
- https://www.mysql.com/products/community/
- 온라인으로 MySQL: codeanywhere.com
- bitnami로 대체
- 윈도우 + R


## MySQL의 구조
- 데이터는 표(table)에 저장이 된다.
- 데이터베이스(== 스키마): 연관되어 있는 표들을 묶어서 다른 것과 구분한다. 표를 그룹핑한 일종의 폴더
- 데이터베이스 서버: 위와 같은 데이터베이스(스키마)가 저장되어 있는 곳


## MySQL 서버 접속
- 데이터베이스는 자체적인 보안체제가 있기에 안전하게 보관 가능
- 권한 기능 존재: 여러 사람 등록해 놓을 수 있다.
- 읽기, 쓰기, 수정, 삭제 중 원하는 것을 가능하게 차등적으로 권한 줄 수 있다.
- -u:user
- -uroot: 관리자 권한, 중요한 일이 있을 때만 사용하는 것을 권장
- -p: 비밀번호 입력

> bin ./mysql -uroot -p
> //데이터베이스 서버라는 담장을 넘은 것


## MySQL 스키마(schema)의 사용
- mysql create database
> CREATE DATABASE 디비이름;
- mysql delete database
> DROP DATABASE 삭제하고자 하는 디비 이름;
- how to show database list in mysql
> SHOW DATABASES
- 어떤 데이터베이스를 사용하겠다
>USE 사용하고자 하는 디비이름;


## SQL과 테이블의 구조
- SQL: Structured Query Language
	- Structured(구조화 되었다): 관계형 데이터 베이스는 표의 형식으로 정리정돈
	- Query: 데이터 베이스에게 데이터 넣어줘, 읽어줘,,, 포괄적으로 디비에게 요청한다.
- table: 표
	- x축: 수평--> row, record, 행 --> 테이터 하나하나, 데이터 자체
	- y축: 수직--> colum, 열 --> 데이터의 타입, 구조
