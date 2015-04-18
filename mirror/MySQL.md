![http://upload.wikimedia.org/wikipedia/en/thumb/6/62/MySQL.svg/200px-
MySQL.svg.png](http://upload.wikimedia.org/wikipedia/en/thumb/6/62/MySQL.svg
/200px-MySQL.svg.png)

[[PNG external
image]](http://upload.wikimedia.org/wikipedia/en/thumb/6/62/MySQL.svg/200px-
MySQL.svg.png)

[홈페이지](http://www.mysql.com/)

## Contents

    

1. 개요 
2. 라이선스 
3. 이용 현황 
4. 버전 
5. MariaDB 

[[edit](http://rigvedawiki.net/r1/wiki.php/MySQL?action=edit&section=1)]

# 1. 개요 ¶

[DBMS](DBMS.md)의 한 종류.  
제작사는 "MySQL AB"로, MySQL을 만든 제작자들이 설립한 회사이다. 이 회사는 [SUN](SUN.md)에 10억 달러에
인수되었는데, 이후 [오라클](%EC%98%A4%EB%9D%BC%ED%81%B4.md)이 썬을 72억달러에 인수하면서 같이 넘어갔다.
따라서 MySQL의 실질적인 소유주는 오라클인데, 이 회사가 자체 상용 DB를 가지고 있고, 프로그램이 버전업이 될수록 더욱 복잡해지고
있으며, 오픈소스에 대해 호의적이지 않기 때문에 MySQL 사용자들 사이에서도 불안감이 커지고 있다. 그래서 [오픈소스](%EC%98%A4%ED%94%88%20%EC%86%8C%EC%8A%A4.md) 진영에서 MySQL을 모태로
[MariaDB](https://mariadb.org/)라는 DBMS를 만들었다.`[1]`

  

[[edit](http://rigvedawiki.net/r1/wiki.php/MySQL?action=edit&section=2)]

# 2. 라이선스 ¶

라이선스는 제품 종류에 따라 [GPL](GPL.md)과 자체적인 라이선스 두 가지가 적용된다. 이 때문에
[오픈소스](%EC%98%A4%ED%94%88%EC%86%8C%EC%8A%A4.md) DB의 범주에 들어가기도 한다.

  

제품 종류는 무료와 유료로 나뉘는데, 무료 버전은 커뮤니티 에디션(Community Edition)이라는 이름이고, 나머지는 전부 유료이다.
유료 버전 가격은 2000~10000달러 사이이다. 무료 버전은 라이센스를 [GPL](GPL.md)을 적용하고 소스를 공개하는데, 유료
버전은 자체 상용 라이센스로 소스를 수정해도 공개하지 않아도 된다. 대신 유료 버전은 고객 지원을 빵빵하게 해주지만, 무료 버전은 [그런 거없다](%EA%B7%B8%EB%9F%B0%20%EA%B1%B0%20%EC%97%86%EB%8B%A4.md).

  

참고로 [오픈소스](%EC%98%A4%ED%94%88%EC%86%8C%EC%8A%A4.md)의 경우 이런 방식의 유료화가
많다.`[2]` 기업에서 중요한 것은 돈이 들더라도 문제가 생겼을 때 빠르게 해결할 수 있어야 하는데, 오픈소스는 그런 면에서 기업에
메리트가 없다.`[3]` 또, 오픈소스 진영에서는 수익금이 들어와야 서버 유지 같은 돈이 드는 곳에 투자를 할 수 있다. 이렇게 기업
입장에서는 일반적인 상용 버전보다 돈은 적게 들면서 사후지원이 되고, 오픈소스 그룹 입장에서는 스폰서 등을 받지 않아도 수익수단이 생겨서
좋은 Win-Win 전략이 고객지원에 대한 요금부과이다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/MySQL?action=edit&section=3)]

# 3. 이용 현황 ¶

점유율은 상당히 높다. 설치형 블로그나 게시판 등등 상당수의 CMS(컨텐츠 관리 시스템)가 MySQL을 지원한다. 한국에서는
[제로보드](%EC%A0%9C%EB%A1%9C%EB%B3%B4%EB%93%9C.md),
[그누보드](%EA%B7%B8%EB%88%84%EB%B3%B4%EB%93%9C.md)가 이걸 지원하면서 폭발적으로 점유율을 높혔다.
세계적으로도 [미디어위키](%EB%AF%B8%EB%94%94%EC%96%B4%EC%9C%84%ED%82%A4.md)나
[드루팔](%EB%93%9C%EB%A3%A8%ED%8C%94.md),
[워드프레스](%EC%9B%8C%EB%93%9C%ED%94%84%EB%A0%88%EC%8A%A4.md),
[phpBB](phpBB.md)등의 유명한 웹 프로그램에서 사용되고 있다. 전통적으로
[리눅스](%EB%A6%AC%EB%88%85%EC%8A%A4.md)에 설치하는 APM 패키지(Apache+PHP+MySQL)에 기본
포함될 정도로 인기가 있다. 물론 [윈도우](%EC%9C%88%EB%8F%84%EC%9A%B0.md)용도 나온다.

  

하지만 오라클에 넘어간 이후로 기업들은 급히 MySQL에서 발을 빼고 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/MySQL?action=edit&section=4)]

# 4. 버전 ¶

1995년 5월 23일에 첫 버전이 출시되었고, 2014년 4월 현재 5.6.17 버전이 최신이다. 5.7 버전은 베타로 출시되어 있는 중.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/MySQL?action=edit&section=5)]

# 5. MariaDB ¶

<https://mariadb.org/>

  

MySQL이 오라클로 넘어간뒤, 불확실한 라이선스 문제를 해결하려고 나온 오픈소스 DBMS. 2013년 현재 기능적으로 MySQL과
동일하며, 성능은 더 낫다(고 주장한다). 오라클로 인수된 뒤 MySQL 기능추가가 제대로 이뤄지지 않고 있었다고.

  

MySQL AB 출신 개발자들이 따로 나와 개발 중인 오픈소스 DBMS. MariaDB에서 먼저 구현된 기능이 MySQL에도 반영 되기도
한다는 듯.

  

[GPL](GPL.md) v2 라이선스이다.

`\----`

  * `[1]` 리눅스 페도라와 오픈수세는 mySQL을 버리고 MariaDB를 장착한다. [기사1](http://www.clien.net/cs2/bbs/board.php?bo_table=news&wr_id=1572468) [기사2](http://www.clien.net/cs2/bbs/board.php?bo_table=news&wr_id=1572452) [애플](%EC%95%A0%ED%94%8C%28%EA%B8%B0%EC%97%85%29.md)은 [OS X](OS%20X.md) 서버 버젼에서 MySQL을 버리고 [PostgreSQL](PostgreSQL.md)을 채용했다. 
  * `[2]` [리눅스](%EB%A6%AC%EB%88%85%EC%8A%A4.md), 오픈오피스, 각종 [서버](%EC%84%9C%EB%B2%84.md) 관련 프로그램 등등
  * `[3]` 물론 오픈소스 커뮤니티에서 지지고 볶고 하면 답이 나오지만, 시간이 돈인 기업에서 그런 짓을 하겠는가?

