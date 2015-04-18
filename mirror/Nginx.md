![nginx.gif](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Nginx/nginx.gif)

[GIF image (524 Bytes)]

[공식사이트](http://nginx.org/)

2002년부터 [러시아](%EB%9F%AC%EC%8B%9C%EC%95%84.md)의
[프로그래머](%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%A8%B8.md) 이고르 시쇼브(Игорь
Сысоев)가 아파치 코딩하다 아파치의 C10K 문제`[1]`를 보고 이를 극복하면서 네이티브 Win32환경에도 돌아갈 무설치 웹 서버
프로그램에 대한 개발을 시작하여 2004년 [스푸트니크1호](%EC%8A%A4%ED%91%B8%ED%8A%B8%EB%8B%88%ED%81%AC#s-1.md) 발사일에 발표한
[오픈소스](%EC%98%A4%ED%94%88%EC%86%8C%EC%8A%A4.md)
[서버](%EC%84%9C%EB%B2%84.md) 프로그램. 현재 이고르 시쇼브와 그가 설립한 회사인 Nginx Inc.가 이
프로젝트를 운영중에 있다. 목표는 가벼우면서도 강력한 프로그램이라고... HTTP와 리버스 프록시, IMAP/POP3등의 서버를
구동가능하다.

이를 지칭할땐 엔진 X라고 부른다. (<del>E</del>**Ngin**<del>e</del>**X**)

구조적으로는 [아파치](%EC%95%84%ED%8C%8C%EC%B9%98#s-5.md)에서 사용하는 스레드/프로세스 기반 구조 대신
비동기 이벤트 기반 구조를 가진다. 이로 인해서 서버 부하시 성능 예측이 쉽다고... 덤으로 이로 인하여 10000개의 동시 접속을 하면 그
10000개에 드는 메모리 점유는 2.5MB다(....) 사용하는 리눅스 웹서버의 경우 LAMP([Linux](Linux.md) \+
Apache + [MySQL](MySQL.md) \+ [PHP](PHP.md) or
[Python](%ED%8C%8C%EC%9D%B4%EC%8D%AC#s-3.md) or [Perl](Perl.md))대신 LEMP를
쓴다. Nginx는 여러 서드파티 기능들(SSL, GeoIP등)을 모듈로 덧 붙이는 방식을 쓰고 있으며, 그래서 모듈을 쓰지 않을 경우
제외해 놓을 수 있다, 단, 소스 컴파일시 모듈을 추가하지 않으면, 그 이후에 추가가 안되지만...

Nginx를 사용하면서 conf 설정`[2]`을 바꿀때는 재시작 할필요 없이 reload를 하면 된다. 즉, 프로세스를 재시작 할 필요가
없다는 점이 있다.

넷크래프트의 2013년 1월 웹서버 조사에서, 조사한 사이트중 점유율 3위를 차지`[3]`하였으며,
[아마존닷컴](%EC%95%84%EB%A7%88%EC%A1%B4%EB%8B%B7%EC%BB%B4.md) 웹 서비스(AWS)에서는
44%이상의 점유율로 1위, 활동적인 웹 서버중 3위`[4]`를 차지했으며, 이 속도라면 잘 나가는 사이트쪽에선
[콩라인](%EC%BD%A9%EB%9D%BC%EC%9D%B8.md) 획득 가능할듯 보여진다.

현재 Nginx를 쓰는 유명한 곳으로는 [페이스북](%ED%8E%98%EC%9D%B4%EC%8A%A4%EB%B6%81.md),
[넷플릭스](%EB%84%B7%ED%94%8C%EB%A6%AD%EC%8A%A4.md),
[워드프레스닷컴](%EC%9B%8C%EB%93%9C%ED%94%84%EB%A0%88%EC%8A%A4.md), GitHub,
SoundCloud, Zynga, Sourceforge 등이 있으며, 한국에서는
[네이버](%EB%84%A4%EC%9D%B4%EB%B2%84.md) 첫페이지,
[백괴사전](%EB%B0%B1%EA%B4%B4%EC%82%AC%EC%A0%84.md), [엔하위키미러](%EC%97%94%ED%95%98%EC%9C%84%ED%82%A4%20%EB%AF%B8%EB%9F%AC.md),
[XpressEngine](XpressEngine.md) 공식 홈페이지 등이 있다고 한다. 그 외에
[카카오톡](%EC%B9%B4%EC%B9%B4%EC%98%A4%ED%86%A1.md) 공지사항 서버`[5]`,
translatewiki.net, Hostinger.kr`[6]` 에서도 사용한다.

![http://ivandarmawan.files.wordpress.com/2012/10/nginxwelcome.jpg](http://iva
ndarmawan.files.wordpress.com/2012/10/nginxwelcome.jpg)

[[JPG external
image]](http://ivandarmawan.files.wordpress.com/2012/10/nginxwelcome.jpg)

  
Nginx를 처음 깔면 환영 문구가 나오는데, 구식버전에서는 그냥 빈 화면에 Welcome to Nginx만 뜨고 땡이다. 근데 문제는 몇몇
[악성코드](%EC%95%85%EC%84%B1%EC%BD%94%EB%93%9C.md)들이 컴퓨터를 감염시켜 DNS를 변경, 사이트를
변경시키는데 하필이면 저 화면만 뜨는 서버로 이동시킨다는 것. 덕택에 Nginx도 악성코드 취급을 받아, 현재는 환영페이지를 저렇게
변경해놨다.

현재 카카오톡 PC버전은 이 nginx 서버를 사용하고 있다.

`\----`

  * `[1]` 1만개의 소켓을 열게 된다면 하드웨어가 충분한데도 불구하고 I/O 처리방식의 문제때문에 프로세스가 제대로 처리하지 못한다는 것 
  * `[2]` vhost는 '서버 블록'으로 불리며, 정 귀찮으면 nginx.conf에 필요한 줄을 왕창 넣으면 돌아는 간다. 
  * `[3]` 현재 전세계 웹서버중 55.7%는 아파치, 17.6%는 IIS, 12.07%가 Nginx 
  * `[4]` 아파치 59.04%, IIS 13.22%, Nginx 12.44% 
  * `[5]`

![1386549615670_Screenshot_2013-12-09-09-29-00.png](//rv.wkcdn.net/http://rigv
edawiki.net/r1/pds/Nginx/1386549615670_Screenshot_2013-12-09-09-29-00.png)

[PNG image (14 KB)]

  
하단 nginx에 주목.

  * `[6]`

![http://ghostcloud.96.lt/xe/files/attach/images/720/799/7288f503dafbc6c760dc5
08c2da6014b.PNG](http://ghostcloud.96.lt/xe/files/attach/images/720/799/7288f5
03dafbc6c760dc508c2da6014b.PNG)

[[PNG external image]](http://ghostcloud.96.lt/xe/files/attach/images/720/799/
7288f503dafbc6c760dc508c2da6014b.PNG)

