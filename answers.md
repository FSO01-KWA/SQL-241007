# SQL Day 28 Assignment - Answers

**문제 1**  
SQL은 데이터베이스를 관리하고 조작하기 위한 표준 언어로, 데이터를 저장하고 조회, 수정, 삭제하는 데 사용됨. 

**문제 2**  
대표적인 RDBMS는 MySQL, PostgreSQL, Oracle임. 

**문제 3**  
SQL은 구조화된 데이터와 정해진 스키마 사용, NoSQL은 유연한 스키마와 비정형 데이터 지원함. SQL은 복잡한 쿼리에 강하고, NoSQL은 수평 확장이 용이함. 

**문제 4**  
d) DROP - DROP은 데이터베이스 객체를 삭제하는 명령어로, 기본 데이터 조작 언어(DML) 명령어에 해당되지 않음.

**문제 5**  
SELECT 문에서 모든 컬럼을 조회하려면 와일드카드 `*`를 사용함. 

**문제 6**  
특정 조건에 맞는 데이터를 조회할 때는 `WHERE` 절을 사용함. 

**문제 7**  
AND는 모든 조건이 참일 때, OR는 하나 이상의 조건이 참일 때, NOT은 조건의 부정을 나타냄. 

**문제 8**  
LIKE 연산자는 패턴 매칭을 위해 사용되며, `김%`는 '김'으로 시작하는 모든 값을 조회함. 

**문제 9**  
BETWEEN 연산자는 범위를 지정하여 조회할 때 사용되며, 예: `WHERE age BETWEEN 17 AND 19;`

**문제 10**  
INSERT 문으로 여러 행을 삽입할 때는 VALUES 절에 여러 값을 쉼표로 구분하여 나열함. 예: `INSERT INTO students (name, age, grade) VALUES ('김철수', 17, 'A'), ('김영희', 18, 'B');`

**문제 11**  
UPDATE 문은 조건 없이 실행 시 모든 행에 적용되므로, 항상 WHERE 절을 사용하여 특정 조건에만 적용하도록 해야 함. 

**문제 12**  
DELETE는 특정 조건의 데이터를 삭제하고, TRUNCATE는 테이블의 모든 데이터를 즉시 삭제하며 롤백이 불가함. 

**문제 13**  
GROUP BY 절은 데이터를 그룹화하여 집계함수를 사용하는 데 사용됨. 예: `SELECT grade, COUNT(*) AS '학생 수' FROM students GROUP BY grade;`

**문제 14**  
INNER JOIN은 양쪽 테이블에서 조건에 맞는 데이터만 반환하고, LEFT JOIN은 왼쪽 테이블의 모든 데이터와 오른쪽 테이블의 일치하는 데이터를 반환함. 

**문제 15**  
서브쿼리는 쿼리 내에 포함된 쿼리로, 예: `WHERE age > (SELECT AVG(age) FROM students);`와 같이 사용함. 

**문제 16**  
윈도우 함수는 행 순서에 따라 계산을 수행하며, 예로 RANK() 함수가 있음.

**문제 17**  
PRIMARY KEY는 고유한 식별자 역할을 하고, FOREIGN KEY는 다른 테이블의 기본 키를 참조하여 관계를 유지함. 

**문제 18**  
트랜잭션은 원자성, 일관성, 격리성, 내구성을 가지며, ACID 원칙을 따름.

**문제 19**  
사용자 계정을 생성하고 권한을 부여하려면 `CREATE USER`와 `GRANT` 명령어를 사용함. 예: `CREATE USER 'username'@'localhost' IDENTIFIED BY 'password';`

**문제 20**  
인덱스는 조회 성능을 향상시키지만, 데이터 삽입 및 수정 시 오버헤드가 발생할 수 있음.
