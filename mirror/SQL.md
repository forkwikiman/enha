## Contents

    

1. 샌 카를로스 공항 
2. Structured Query Language 
    

2.1. 소개

2.2. 구문 설명

[[edit](http://rigvedawiki.net/r1/wiki.php/SQL?action=edit&section=1)]

## 1. 샌 카를로스 공항 ¶

  * 상위 항목 : [세계의 공항 목록](%EC%84%B8%EA%B3%84%EC%9D%98%20%EA%B3%B5%ED%95%AD%20%EB%AA%A9%EB%A1%9D.md)

![http://upload.wikimedia.org/wikipedia/commons/thumb/8/82/Kluft-photo-San-
Carlos-Airport-Oct-2008-Img_1915.jpg/1280px-Kluft-photo-San-Carlos-Airport-Oct
-2008-Img_1915.jpg](http://upload.wikimedia.org/wikipedia/commons/thumb/8/82
/Kluft-photo-San-Carlos-Airport-Oct-2008-Img_1915.jpg/1280px-Kluft-photo-San-
Carlos-Airport-Oct-2008-Img_1915.jpg)

[[JPG external
image]](http://upload.wikimedia.org/wikipedia/commons/thumb/8/82/Kluft-photo-
San-Carlos-Airport-Oct-2008-Img_1915.jpg/1280px-Kluft-photo-San-Carlos-
Airport-Oct-2008-Img_1915.jpg)

  
San Carlos Airport  

  * IATA: SQL
  * ICAO: KSQL  

[미국](%EB%AF%B8%EA%B5%AD.md)
[샌프란시스코](%EC%83%8C%ED%94%84%EB%9E%80%EC%8B%9C%EC%8A%A4%EC%BD%94.md) 광역권의
San Carlos에 소재한 공항.`[1]` 경비행기가 잔뜩 <del>주차</del>주기되어 있고 카페 하나 덜렁 서있는 평범한 미국 지방
공항이다.

  

위에서 보다시피 IATA 코드가 **SQL**인데 바로 옆에
**[오라클](%EC%98%A4%EB%9D%BC%ED%81%B4#s-7.md)** 본사가 있다! 다만 이것은 순전히 우연에 의한
것으로, 오라클이 창립되기 한참 전부터 사용된 코드. 우연치고는 절묘하다만.

  

샌프란시스코 광역권과 [LA](LA.md)광역권을 월정액으로 무제한 왕래할 수 있는 Surf Air의 첫 노선이기도 하다. 실리콘
밸리의 북쪽 끝인데다 고속도로(US 101)가 바로 옆인 교통상의 이점을 살린 듯.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/SQL?action=edit&section=2)]

## 2. Structured Query Language ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/SQL?action=edit&section=3)]

### 2.1. 소개 ¶

SQL; Structured Query Language  
에스큐엘, 혹은 시퀄이라고 읽는다. 구조적 데이터 질의 언어.
[데이터베이스](%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%B2%A0%EC%9D%B4%EC%8A%A4.md)에서 자료를
처리하는 용도로 쓰인다.

  

어느 데이터베이스에서나 기본으로 제공하기 때문에 배워두면 여러 곳에서 쓸데가 많다.  
그러나 DBMS 밴더에 따라 사용하는 SQL에는 다소 차이가 있다. 그래서 [ANSI](ANSI.md) SQL이라고 하는 표준
SQL구문이 있으나 DBMS 시장을 독식하고 있는 오라클이 잘 지키지 않아서 현실은 시궁창. 일반적으로 사용하는 데이터베이스는
RDBS(관계형 데이터베이스)이며, RDBS에서 데이터 처리는 RDBS용 데이터 모음인 테이블`[2]`을 기준으로 이루어지기 때문에 SQL
역시 테이블을 염두에 두고 읽으면 이해하기 쉽다.

  

아래 구문 설명 및 예제는 공통적으로 대문자는 키워드, 소문자는 이름이나 값 등 변수를 의미하고, 주로 사용되는 WHERE 옵션은 중괄호로
표기한다`[3]`.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/SQL?action=edit&section=4)]

### 2.2. 구문 설명 ¶

  * INSERT : 데이터를 입력하는 구문. 형식은 다음과 같다.
INSERT INTO table(field1, field2, ...) VALUES (value1, value2, ...);  
table에 field1=value1, field2=value2, ...와 같은 속성값을 가지는 항목을 새로 생성하여 삽입한다. 만약
테이블에 입력될 값이 문자라면 반드시 ** '' **으로 문자열 (String)임을 표시해 주어야 탈이 없다. 이는 UPDATE 구문에서도
마찬가지.

  

  * UPDATE : 데이터를 수정하는 구문. 
UPDATE FROM table SET field1=value1, field2=value2, {WHERE 조건};  
table의 field1에 value1, field2에 value2, ... 로 변경한다. WHERE 절이 없을 경우 테이블의 모든 항목이
바뀌므로, 대개 WHERE절과 함께 사용하여 범위를 한정해 준다.  
ex) UPDATE FROM document SET title='무제' WHERE author='무명씨';  
작성자가 '무명씨'인 모든 문서의 제목을 '무제'로 바꾸는 명령.

  

  * DELETE : 데이터를 삭제하는 구문.
DELETE FROM table {WHERE 조건};  
말 그대로 데이터를 삭제하는 구문이다. 조건절이 없을 경우 테이블의 모든 데이터를 비우게 되므로`[4]`, 대개 조건절과 함께 사용된다.

  

  * SELECT : 데이터를 읽어오는 구문.
SELECT field1, field2, ... FROM table {WHERE 조건};  
서비스시 가장 빈번하게 사용되는 구문이다. 테이블에서 지정된 값을 가져오는 구문이며, 모든 값을 가져오기 위해 으레 field 부분을
생략하고 *로 표기하기도 한다`[5]`.

  

ex) SELECT * FROM document WHERE author='무명씨';  
작성자가 '무명씨'인 모든 문서의 모든 항목를 가져오는 구문.

  

SELECT title FROM document WHERE date > to_date('2011/09/01', 'yyyy/mm/dd/');  
2011년 9월 1일 이후로 작성된 모든 문서의 제목을 가져오는 구문(to_date 함수는 문자열을 시간 데이터로 바꾸는 함수로 오라클
한정).

  

SELECT * FROM document WHERE no between 1 and 10;  
1부터 10의 번호를 가지는 document 테이블 내의 모든 항목을 가져오는 구문.

  

SELECT * FROM document WHERE author in ('무명씨','홍길동');  
작성자가 무명씨, 홍길동인 문서의 모든 항목을 가져오는 구문.

  

SELECT * FROM document WHERE author like '김*';  
작성자가 김으로 시작되는 문서의 모든 항목을 가져오는 구문.

  

실제 업무에서는 여러 쿼리를 조합하거나 테이블을 UNION, INTERSECTION, JOIN 등으로 가공하여 사용하는 경우가 많으므로
쿼리가 매우 복잡해진다.  
ex)  
SELECT document FROM (  

SELECT document, COUNT(document) cnt  
FROM rel_document_keyword  
WHERE keyword IN(  

SELECT id FROM keyword WHERE keyword IN ('key1', 'key2', 'key3', 'key4')

) GROUP BY document

) WHERE cnt=4;

  

  * DROP : 개체 삭제
DROP TABLE table_name;

  

데이터베이스 내의 개체를 삭제해 버린다. 즉, 테이블 내의 데이터 뿐만 아니라 구조까지 모조리 날려버리는 궁극의 명령어이다. 실수로 사용중인
DB 내에서는 쓰지 않기를 바란다. 만약 이 명령어로 회사의 데이터를 날려먹었을 경우... 상사에게 깨지거나 회사에서 해고당하는 정도로
끝나면 다행으로, 고소장이 날아오는 경우도 많다고 한다.

  

  * UNION, JOIN : 둘 이상의 테이블을 결합
(SELECT * FROM `table_a`) UNION (SELECT * FROM `table_b`);  
SELECT a.*, b.* FROM `table_a` a LEFT OUTER JOIN `table_b` b;

  

둘 이상의 테이블을 묶어서 가져온다. UNION의 경우는 아래쪽에 붙이고, JOIN은 옆에 붙인다는 차이점이 있다. UNION의 경우
ALL, JOIN의 경우 FULL, INNER, OUTER, LEFT, RIGHT 등 보조적인 명령어를 사용하여 원하는 대로 조합할 수
있다.  
한편 UNION은 테이블의 열 개수가 다르면 에러를 뱉어내고(...), JOIN은 열 이름이 같은 게 있을 경우 애로사항이 꽃핀다는 단점이
있다.  
**SQL 주입(SQL injection)**이라는 [해킹](%ED%95%B4%ED%82%B9.md) 기법에서 악용될 수 있다. 테이블 정보를 알고 있다면 이를 이용해서 **DB상에 있는 회원 정보를 빼올 수 있으므로** 로그인 폼에서는 이를 제대로 필터링해야만 한다. **[꼭 해라 두 번 해라](%EA%BC%AD%20%ED%95%B4%EB%9D%BC%20%EB%91%90%20%EB%B2%88%20%ED%95%B4%EB%9D%BC.md).**

`\----`

  * `[1]` 실제 위치는 Redwood Shores에 더 가깝다.
  * `[2]` 단일 주제에 대해 행과 열로 이루어진 데이터 집합이다. 주로 행은 데이터 원소(entity)이며 열은 데이터 원소가 가지는 속성값으로 표현된다. 표나 엑셀 시트 하나를 생각하면 이해하기 쉬운데 예를 들어 '고객'이라는 테이블이 있다고 가정하면 고객 한명은 ID, 이름, 주소, 전화번호 등의 값을 가진다. 각각의 고객은 하나의 열을 차지하여 첫번째 열에는 고객의 ID가, 두번째 열에는 고객의 이름이, 세번째 열에는 고객의 주소가...와 같이 지정되어 저장된다. 테이블에서 열의 순서는 중요하지 않으며 입출력시 열의 이름을 정확하게 지정하여 준다.
  * `[3]` 물론 옵션은 WHERE 말고도 GROUP BY, COUNT 등 목적에 따라 여러가지 있을 수 있으나 구문 설명을 위해 WHERE절을 사용하지 않을 수 없으므로 WHERE절만 표기한다. 다른 옵션에 대해서는 [추가바람](%EC%B6%94%EA%B0%80%EB%B0%94%EB%9E%8C.md).
  * `[4]` 데이터를 통째로 비우는 명령으로 TRUNCATE가 있는데, 조건절 없이 사용되는 DELETE 구문과 TRUNCATE 구문은 실행방식이 약간 다르다. 이를테면, TRUNCATE 구문은 테이블을 마치 갓 생성한 것처럼 최적화를 시켜 주지만(자동증가값 초기화, 테이블 오버헤드 초기화 등), DELETE 구문은 그렇지 못하다.
  * `[5]` 이 경우 프로그램 레벨에서 필드값의 순서를 알고 있어야 하므로 그다지 권장되는 방법은 아니다.

