![http://www.unix-experience.fr/wp-content/uploads/2012/08/postgresql-logo-
624x227.png](http://z1.enha.kr/http://www.unix-experience.fr/wp-
content/uploads/2012/08/postgresql-logo-624x227.png)

[[PNG external image]](http://www.unix-experience.fr/wp-
content/uploads/2012/08/postgresql-logo-624x227.png)

  
<http://www.postgresql.org/>

[오픈소스](%EC%98%A4%ED%94%88%EC%86%8C%EC%8A%A4%20%EC%86%8C%ED%94%84%ED%8A%B8%EC%9B%A8%EC%96%B4.md) RDBMS. 라이센스는 처음에는 BSD였으나 언제부터인가 MIT 비스무리한 독자적 라이센스를 따르기
시작했다.

점유율은, [대한민국](%EB%8C%80%ED%95%9C%EB%AF%BC%EA%B5%AD.md)을 포함해 전세계적으로
[MySQL](MySQL.md)에 밀리지만 유독 [일본](%EC%9D%BC%EB%B3%B8.md)에서는 왠지 MySQL보다도
점유율이 높다(그렇다고 MySQL의 점유율이 낮은 건 아니다). 실제로 일본 관공서에서는 상용이라면
[오라쿠루](%EC%98%A4%EB%9D%BC%ED%81%B4.md) 무료라면 포스구레... 이런 경향이 있다고도. 나이먹은
일본엔지니어들은 옛날부터 지금까지 주로쓰던 PostgreSQL을 고수하며 최근에 썬마이크로시스템을
[오라클](%EC%98%A4%EB%9D%BC%ED%81%B4.md)이 집어삼키면서 MySQL 소유권도 넘어갔는데 젊은 층에서는 그로
인해 "이거 언젠가 mysql은 개발 중단될 지도?" 하는 불안감이 있어서 일본에서는 아직도 잘 나가는 편이라고 한다.

현재 OS X Lion Server 버젼에서는 MySQL이 퇴출(?)되고, PostgreSQL이 자리잡게 되었는데, 이는 MySQL이
오라클에 넘어가면서 저작권 분쟁 방지를 위한 방책이라 한다. 또한 양 DB간 migration이 어렵지 않기 때문에 상당수의 상용/비상용
프로그램 중 MySQL 사용 프로그램들이 PostgreSQL로 넘어가고 있다.

현재 사용자들:

  * Yahoo!: 유저 사용형태 분석에 관한 자료를 저장하는 데 쓰이고 있다. 물론, 다루는 용량이 엄청나게 큰 지라(2 페타바이트 정도라 한다) 많이 고쳐서 사용하고 있다고 하는 중.
  * MySpace: 데이타 저장에 쓰이고 있다. Yahoo! 처럼 마개조해서 사용하고 있지는 않다.
  * OpenStreetMap
  * Afilias: .org 나 .info 도메인 저장에 쓰인다.
  * Sony Online: 멀티플레이 게임용 데이타베이스로 쓰인다. 위에 언급되었듯이 일본 기업임을 상기.
  * BASF: 웹 쇼핑 데이타베이스 관리.
  * hi5.com
  * reddit.com
  * Skype: 중앙 데이타베이스로 사용된다.
  * Sun xVM
  * MusicBrainz: 온라인 음악 백과사전 데이타 수록용으로 쓰인다.
  * International Space Station: 현재 우주 정거장 그거 맞다. 천체 관측 자료를 저장하여 지상에서 분석할 때 사용한다.
  * MyYearbook
  * Heroku: 클라우드 서비스용 데이타베이스로 사용된다. 의외로 일본 회사가 아니다.
  * ZOHO ManageEngine: OpManager, SDP 등의 MySQL을 신버전부터 PostgreSQL로 변경. 
  * [KT](KT.md): 공개SW 도입을 위한 시범 사업 추진 건으로 CentOS, JBoss EAP 등과 함께 도입되었다.  

이렇듯이 일본 외에도 생각보다 많은 사용자를 가지고 있다.

