  * 상위 항목: [컴퓨터 관련 정보](%EC%BB%B4%ED%93%A8%ED%84%B0%20%EA%B4%80%EB%A0%A8%20%EC%A0%95%EB%B3%B4.md)  

<del>[BDSM](BDSM.md)</del>  
<del>[DSBM](DSBM.md)</del>  
database management system. 줄여서 DBMS라고 부른다.

## Contents

    

1 개요

2 기능

3 특성

4 종류

5 한계

[[edit](http://rigvedawiki.net/r1/wiki.php/DBMS?action=edit&section=1)]

## 1 개요 ¶

[데이터베이스](%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%B2%A0%EC%9D%B4%EC%8A%A4.md)라는 데이터의
집합을 만들고, 저장 및 관리할 수 있는 기능들을 제공하는 응용프로그램이다. 즉,
[데이터](%EB%8D%B0%EC%9D%B4%ED%84%B0.md)의 관리에 특화된 프로그램이라고 생각하면 편하다.

  

널리 알려진 DBMS로는 [오라클](%EC%98%A4%EB%9D%BC%ED%81%B4.md)사의
[오라클](%EC%98%A4%EB%9D%BC%ED%81%B4.md)과 [MySQL](MySQL.md)`[1]`,
[IBM](IBM.md)사의 [INFORMIX](INFORMIX.md)와 [DB2](DB2.md),
[MS](MS.md)사의 [MS SQL SERVER](MS%20SQL%20SERVER.md),
[알티베이스](%EC%95%8C%ED%8B%B0%EB%B2%A0%EC%9D%B4%EC%8A%A4.md)의 [ALTIBASEHDB](ALTIBASE%20HDB.md),
[티베로](%ED%8B%B0%EB%A7%A5%EC%8A%A4%20%EC%86%8C%ED%94%84%ED%8A%B8.md)의
[티베로](%ED%8B%B0%EB%B2%A0%EB%A1%9C.md), [NHN](NHN.md)의
[Cubrid](Cubrid.md) 등이 있으며 그 외에도 다양한 상업용/오픈소스 제품들이 있다.

[[edit](http://rigvedawiki.net/r1/wiki.php/DBMS?action=edit&section=2)]

## 2 기능 ¶

  * 중복 제어 : 동일한 데이터가 여러 위치에 중복 저장되는 현상을 방지한다. 데이터가 중복되면, 저장 공간이 낭비되고 데이터의 [일관성](%EC%9D%BC%EA%B4%80%EC%84%B1.md)이 깨질 수 있다.
  * 접근 통제 : DBMS는 사용자마다 다양한 권한을 부여할 수 있으며, 권한에 따라 데이터에 대한 접근을 제어할 수 있다.
  * 인터페이스 제공 : DBMS는 사용자에게 [SQL](SQL.md) 및 [CLI](CLI.md),[GUI](GUI.md)등 다양한 인터페이스를 제공한다.
  * 관계 표현 : 서로 다른 데이터간의 다양한 관계를 표현할 수 있는 기능을 제공한다. 
  * [무결성](%EB%AC%B4%EA%B2%B0%EC%84%B1.md) 제약 조건 : [무결성](%EB%AC%B4%EA%B2%B0%EC%84%B1.md)에 관한 제약 조건을 정의/검사하는 기능을 제공한다. [데이터베이스](%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%B2%A0%EC%9D%B4%EC%8A%A4.md)는 반드시 [무결성](%EB%AC%B4%EA%B2%B0%EC%84%B1.md) 제약조건을 통과한 데이터만을 저장하고 있어야 한다.
  * [백업](%EB%B0%B1%EC%97%85.md)/[회복](%ED%9A%8C%EB%B3%B5.md) : 해당 항목 참고  

[[edit](http://rigvedawiki.net/r1/wiki.php/DBMS?action=edit&section=3)]

## 3 특성 ¶

보통 ACID라고 줄여 말한다.  

  * 원자성(Atomicity) : 하나의 트랜잭션은 원자적Atomically으로 수행되어야 한다. 즉 트랜잭션 전체가 수행되거나 아예 수행되지 않아야 하며 [중간은 없다.](N.EX.T.md)
  * 일관성(Consistency) : 트랜잭션이 완료된 이후에도 데이터베이스에는 결함이 없어야 한다.
  * 고립성(Isolation) : 어떠한 트랜잭션은 동시에 수행되는 다른 트랜잭션에 영향을 끼치지 말아야 한다.
  * 영속성(Durability) : 성공적으로 완료된 트랜잭션은 영원히 반영되어야 한다.  

[[edit](http://rigvedawiki.net/r1/wiki.php/DBMS?action=edit&section=4)]

## 4 종류 ¶

  * [dBASE](dBASE.md)
  * [오라클](%EC%98%A4%EB%9D%BC%ED%81%B4#s-7.md) : DBMS 시장의 지배자. 가장 앞선 기술과 안정성을 가지고 있다는 사실에 이의를 달 사람은 없을 지도... <del>그리고 그거 팔아서 벌어들인 돈으로 [SUN](SUN.md)을 인수했다.</del>
  * [MySQL](MySQL.md) : **한때 [오라클](%EC%98%A4%EB%9D%BC%ED%81%B4.md)의 대항마**로 군림한데다 <del>물론 오라클에게 먹힌 이후로는... 그래도 인수 전 못지않게 쌩쌩하게 돌아간다</del> 실질적으로 공짜로 쓰이는 녀석이라 많이 애용하는 녀석이다.`[2]` 특히 [PHP](PHP.md)를 쓴다면 [필수요소](%ED%95%84%EC%88%98%EC%9A%94%EC%86%8C.md).  

    * [MariaDB](https://mariadb.org/) : MySQL이 오라클이 인수된 이후, MySQL의 기술진이 오라클을 나와서 만든 것. MySQL과 호환된다.
  * [MS SQL Server](MS%20SQL%20Server.md) : 마이크로소프트에서 만든 DBMS. 이 때문에 윈도우 서버와 궁합이 잘 맞는다. 주로 ASP, ASP.NET과 연동해서 사용한다.
  * [DB2](DB2.md) : [IBM](IBM.md)에서 만든 DBMS. 보통 사용하는 기업에 와서야 이런 DB가 있는지 알게 되는 우리나라에서는 듣보잡 수준에 머물러 있는 DBMS로 성능이나 기능에선 [오라클](%EC%98%A4%EB%9D%BC%ED%81%B4.md) 에게.. 가격에선 [MS SQL SERVER](MS%20SQL%20SERVER.md)에게 밀리고 있는 안습한 존재이지만, 금융권, 특히 은행권에서는 중요한 DBMS. Unix를 사용하는 금융권은 [오라클](%EC%98%A4%EB%9D%BC%ED%81%B4.md)이나 [INFORMIX](INFORMIX.md)를 사용하지만, IBM [메인프레임](%EB%A9%94%EC%9D%B8%ED%94%84%EB%A0%88%EC%9E%84.md)을 사용할 경우에는 보통 DB2를 선택하는 경우가 많다.`[3]`
  * [티베로](%ED%8B%B0%EB%B2%A0%EB%A1%9C.md) : 국산 소프트웨어 회사인 [티맥스소프트](%ED%8B%B0%EB%A7%A5%EC%8A%A4%EC%86%8C%ED%94%84%ED%8A%B8.md)에서 개발한 국산 DBMS로 [오라클](%EC%98%A4%EB%9D%BC%ED%81%B4.md)과 매우 유사한 아키텍쳐를 가졌다. 저가 시장에서 나름 바람을 기대했으나 모기업인 [티맥스소프트](%ED%8B%B0%EB%A7%A5%EC%8A%A4%EC%86%8C%ED%94%84%ED%8A%B8.md)가 힘든 상황이 되면서 같이 안습인 상황. 법인을 [티베로](%ED%8B%B0%EB%B2%A0%EB%A1%9C.md)로 분리하여 살길을 모색하는 듯.
  * [Cubrid](Cubrid.md) : [NHN](NHN.md)이 운용중이다. 
  * [INFORMIX](INFORMIX.md) : IBM에서 만드는 상용 DB이다.`[4]` 주로 그룹웨어 같은 엔터프라이즈 시장에서 쓰이고 있다.
  * [ALTIBASE HDB](ALTIBASE%20HDB.md) : 메인메모리 DBMS인 ALTIBASE를 시작으로, 최근 v6인 Zeta를 발표한 [알티베이스](%EC%95%8C%ED%8B%B0%EB%B2%A0%EC%9D%B4%EC%8A%A4.md)의 메인 제품. 본래는 기존의 DBMS보다 빠르다는 장점으로 메인메모리 DBMS를 주력으로 밀었으나 v4부터는 용량한계를 극복하기 위해 디스크를 함께 활용한 하이브리드 형태의 DBMS를 출시하고 제품명도 ALTIBASE HDB로 변경했다. [교육용 책도 발간했다](http://book.naver.com/bookdb/book_detail.nhn?bid=6761434)
  * [SQLite](SQLite.md) : SQL를 사용하여 DB를 파일로 저장하는 DBMS이다. 주로 소프트웨어에 내장하기 위하여 설계되었다. SQL 문법을 지원하기 때문에 사용이 편리하며, 파일 입출력을 구현하는 시간도 크게 단축하여 데이터 관리를 효율적으로 할 수 있다. [안드로이드](%EC%95%88%EB%93%9C%EB%A1%9C%EC%9D%B4%EB%93%9C.md) 나 [iOS](iOS.md)에서 DB엔진으로 사용한다.
  * XDM/RD : 히타치에서 제작한 상용 DB. 
  * AIM : 후지쯔에서 제작한 DBMS. 
  * [PostgreSQL](PostgreSQL.md) : 오픈소스 DBMS. 자세한 것은 항목참조.

[[edit](http://rigvedawiki.net/r1/wiki.php/DBMS?action=edit&section=5)]

## 5 한계 ¶

DBMS가 데이터를 관리하는 최선의 방법은 아니다. DBMS는 위의 기능을 만족해야 하기에, 필연적으로 많은 오버헤드가 발생한다.

  

때문에 [휴대폰](%ED%9C%B4%EB%8C%80%ED%8F%B0.md)등의
[임베디드](%EC%9E%84%EB%B2%A0%EB%94%94%EB%93%9C.md) 기기 같은 단순한
[데이터베이스](%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%B2%A0%EC%9D%B4%EC%8A%A4.md)(예를 들어
[전화번호부](%EC%A0%84%ED%99%94%EB%B2%88%ED%98%B8%EB%B6%80.md) 등)의 경우는 다중사용자나
[회복](%ED%9A%8C%EB%B3%B5.md) 기능등을 뺀 단순한 [DBMS](DBMS.md)등을 만들어 사용하기도 한다.

  

[실시간](%EC%8B%A4%EC%8B%9C%EA%B0%84.md) 데이터 처리가 필요한 경우(예를 들어 군용, 항공/우주용 등)에도
일반적으로 복잡한 기능을 제공하는 [DBMS](DBMS.md)가 적합하지 않다. 다만, 통신망, 금융권등에서의 실시간 데이터 처리
개념`[5]`에서는 [오라클](%EC%98%A4%EB%9D%BC%ED%81%B4.md)의
[타임스텐](%ED%83%80%EC%9E%84%EC%8A%A4%ED%85%90.md)이나
[알티베이스](%EC%95%8C%ED%8B%B0%EB%B2%A0%EC%9D%B4%EC%8A%A4.md)의 [알티베이스HDB](%EC%95%8C%ED%8B%B0%EB%B2%A0%EC%9D%B4%EC%8A%A4%20HDB.md)와 같은 MM
DBMS(Main Memory DBMS) 또는 In Memory DBMS`[6]` 제품을 실시간 데이터 처리가 요구되는 구간에 사용하고 이력
데이터와 같은 저장성이 중요시 되는 데이터는 back-end 구간에 전통적인 디스크 기반 DBMS를 사용하는 방식으로 시스템을 구성하기도
한다.`[7]`

  

[검색엔진](%EA%B2%80%EC%83%89%EC%97%94%EC%A7%84.md)등 극단적으로 데이터가 크며,
READ/WRITE간의 격차가 큰 경우에도 일반적인 [DBMS](DBMS.md)를 사용하지 않는다. 이러한 경우는 MM DBMS와
[No SQL](No%20SQL.md) 기술을 혼용하여 서비스를 구축한다. No SQL 기술이 응용된 사례가 페이스북의 쪽지 기능이다.

  

`\----`

  * `[1]` [2008년](2008%EB%85%84.md) 2월에 [SUN](SUN.md)에 인수되었다가 2년 뒤인 [2010년](2010%EB%85%84.md) 1월에 [오라클](%EC%98%A4%EB%9D%BC%ED%81%B4.md)에게 인수되었다.
  * `[2]` Sparc 서버군과 JAVA를 가졌지만 DBMS가 없던 [SUN](SUN.md)사가 인수했으나 썬 자체가 이후 오라클에 인수되었다.
  * `[3]` 애당초 IBM 메인프레임 시장을 겨냥해서 IBM이 직접 개발한 것이다.
  * `[4]` 원래 인포믹스라는 별도의 회사였으나 UNIX용 RDB가 약한 IBM이 인수했다.
  * `[5]` 예를 들자면 SMS 전송 시스템 또는 금융권에서 계좌 이체와 같은 실시간으로 처리되어야 하는 업무단위.
  * `[6]` 메모리에 데이터베이스의 모든 자료를 올려놓고 insert, update, select와 같은 연산을 처리한다. 당연히 엄청나게 빠르다! 다만, 갑작스런 시스템의 종료, 예를 들자면 전원이 갑자기 나가버린다던지, 와 같은 상황에서 최대한 데이터의 유실을 막을 수 있어야 한다. MMDBMS의 선택 기준은 이와같은 유사시 안정성이다. 물론 디스크 기반 DBMS도 마찬가지이지만 메모리에 자료를 몽땅 올려놓고 사용하는 것 자체가 디스크를 기반으로 작동하는 것 보다 안정성이 훨씬 더 떨어질 수 밖에 없다.
  * `[7]` 예를 들자면 SMS 전송 자체는 매우 빠르게 이루어져야 하므로 Main Memory를 사용하는 DBMS가 전송관련 자료처리를 담당하고 전송이 완료(길어봐야 24시간이다.)된 후 속도가 크게 중요하지 않은 이력을 남기는 작업은 디스크 기반 DBMS가 설치된 구간에서 이루어 지도록 Data Flow를 설계한다.

