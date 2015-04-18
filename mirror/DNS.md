## Contents

    

1. 개요 
2. 기술적 설명 
    

2.1. Authoritative answer

2.2. Non-authoritative answer

3. 서버 목록 
4. 기타 
5. 관련 용어 
6. 관련 문서 

[[edit](http://rigvedawiki.net/r1/wiki.php/DNS?action=edit&section=1)]

## 1. 개요 ¶

**Domain Name System**`[1]`

  

[IP](IP.md) 네트워크에서 사용하는 시스템이다. 우리가 인터넷을 편리하게 쓰게 해주는 것으로, 영문/한글 주소를 IP
네트워크에서 찾아갈 수 있는 [IP](IP.md)로 변환해 준다. 만약 DNS가 없다면 [리그베다위키](%EB%A6%AC%EA%B7%B8%EB%B2%A0%EB%8B%A4%20%EC%9C%84%ED%82%A4.md)에 접속하기 위해
<http://108.162.202.52/r1/wiki.php> `[2]`으로 접속을 해야한다. 모든 웹 사이트 주소를 도메인 대신 아이피로
외운다고 생각하면 머리 아파진다. <del>하지만 실제로 이렇게 하는 사람들이 꽤 많다고 한다.</del>

  

이 DNS를 운영하는 서버를 네임서버(Name Server)라고 한다. 서버 구축에 대한 지식이 있으면 어렵지 않게 구성하는 것이 가능하다.
규모가 있는 사이트의 경우에는 네임서버를 자체 운영하는 경우가 많다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/DNS?action=edit&section=2)]

## 2. 기술적 설명 ¶

DNS는 도메인 이름과 IP 주소를 서로 변환하는 역할을 한다.

  

Forward Zone(도메인 이름 → IP)과 Reverse Zone(IP → 도메인 이름)을 가진다. 주로 Forward Zone에는
도메인을 구성하는 호스트에 대한 정보를, Reverse Zone에는 DNS 서버 [자기 자신에 대한정보](%EC%9E%AC%EA%B7%80%ED%95%A8%EC%88%98.md)를 기록한다.

  

DNS 서버에 질의하면 돌아오는 응답은 Authoritative answer와 Non-authoritative answer로 나뉜다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/DNS?action=edit&section=3)]

### 2.1. Authoritative answer ¶

DNS 서버가 질의받은 도메인 또는 IP 주소의 레코드를 Forward Zone, Reverse Zone 모두 가지고 있을 경우에 하는
응답이다. 여러 호스트로 구성되어 있는 도메인의 네임서버에 도메인을 구성하고 있는 호스트의 주소를 직접 질의할 때 얻을 수 있다.  

순서

질의자

응답자

종류

쿼리의 내용

1

클라이언트

ns1.daum.net `[3]`

질의

"[www.daum.net](Daum.md)"

2

ns1.daum.net에서 자신의 레코드를 확인 **(성공)**

3

클라이언트

ns1.daum.net

응답

"[www.daum.net](Daum.md)"의 IP 주소

[[edit](http://rigvedawiki.net/r1/wiki.php/DNS?action=edit&section=4)]

### 2.2. Non-authoritative answer ¶

DNS 서버가 질의받은 도메인 또는 IP 주소의 레코드를 Forward Zone, Reverse Zone 중 하나 이상 가지고 있지 않을
경우에 하는 응답이다. 도메인의 네임 서버에 해당 도메인을 구성하지 않은 호스트, 즉 외부 서버의 주소를 질의했을 때 받을 수 있는
응답이다.  
가정집에서 DNS 서버에 질의할 때 받게 되는 응답이 바로 이것이다.  

순서

질의자

응답자

종류

쿼리의 내용

1

클라이언트

[ISP](%EC%9D%B8%ED%84%B0%EB%84%B7%20%EC%84%9C%EB%B9%84%EC%8A%A4%20%EC%A0%9C%EA%B3%B5%EC%82%AC%EC%97%85%EC%9E%90.md) `[4]`

질의

"[www.daum.net](Daum.md)"

2

ISP의 DNS 서버에서 자신의 레코드를 확인 **(실패)**

3

ISP

**.**`[5]`
질의

net DNS 서버의 도메인 이름

4

응답

net DNS 서버의 IP 주소

5

ISP

net

질의

daum.net DNS 서버의 도메인 이름

6

응답

daum.net DNS 서버의 IP 주소

7

ISP

daum.net

질의

"[www.daum.net](Daum.md)"

8

응답

"[www.daum.net](Daum.md)"의 IP 주소

9

클라이언트

ISP

응답

"[www.daum.net](Daum.md)"의 IP 주소

[[edit](http://rigvedawiki.net/r1/wiki.php/DNS?action=edit&section=5)]

## 3. 서버 목록 ¶

**경고! DNS 설정을 변경할 경우 인터넷이 작동하지 않을 수 있습니다.** 신뢰할 수 없는 DNS 서버는 **비정상적 인터넷 작동, 피싱, 해킹의 위험**이 있습니다. 따라서 신뢰할 수 있는 DNS 서버만 이용하시기 바랍니다.  
또한 일부 DNS 서버의 경우 **유해매체 및 악성코드 필터링 기능이 있어 특정 사이트 접속에 장애가 생길 수도 있습니다.**

이 항목에는 피해 방지를 위해 신뢰할 수 있는 DNS 서버만 기록하시기 바랍니다. 기록 전 질의에 응답하는지 여부를 반드시 먼저 확인하세요.

  

운영주체 서버이름

기본주소

보조주소

기타

[KT DNS](KT.md)

168.126.63.1  
(kns.kornet.net)

168.126.63.2  
(kns2.kornet.net)

열린주소창이 작동한다.

[SK Broadband](SK%EB%B8%8C%EB%A1%9C%EB%93%9C%EB%B0%B4%EB%93%9C.md)

210.220.163.82

219.250.36.130

[LG U+](LG%20U+.md)

164.124.101.2

203.248.252.2

[Google Public DNS](%EA%B5%AC%EA%B8%80.md)

8.8.8.8

8.8.4.4

[홈페이지](https://developers.google.com/speed/public-dns)

OpenDNS

208.67.222.222

208.67.220.220

[홈페이지](https://www.opendns.com/opendns-ip-addresses)

[Comodo Secure DNS](Comodo.md)

8.26.56.26

8.20.247.20

[홈페이지](http://www.comodo.com/secure-dns/index.html)

[Norton ConnectSafe](%EB%85%B8%ED%84%B4.md)`[6]`

199.85.126.10

199.85.127.10

보안 (멀웨어, 피싱 방지)`[7]`

199.85.126.20

199.85.127.20

보안 + 성인용 컨텐츠 차단`[8]`

199.85.126.30

199.85.127.30

보안 + 성인용·불건전한 컨텐츠 차단`[9]`

[[edit](http://rigvedawiki.net/r1/wiki.php/DNS?action=edit&section=6)]

## 4. 기타 ¶

일반적으로 집에서 사용하는 컴퓨터는 통신사(ISP)에서 기본적으로 제공하는 DNS 주소를 사용하도록 설정되어 있다. 그러나 학교 등에서
전용선을 통해 인터넷에 연결하는 컴퓨터는 별도의 DNS 설정이 되어있는 것이 보통이다. 인터넷 응답 속도 향상을 위하여 DNS 설정을 따로
하기도
한다.[#](http://circlash.tistory.com/277)[#](http://circlash.tistory.com/376)

  

종종 인터넷에서 볼 수 있는 ‘[유튜브](%EC%9C%A0%ED%8A%9C%EB%B8%8C.md) 속도 개선법’과 같은 팁 또한 대부분
DNS 서버를 바꾸는 것이다. 다만 이 중 해외 DNS를 이용하는 방법은 적용하면 오히려 국내 홈페이지의 로딩 속도가 느려질 수 있는
부작용이 있으므로 주의해야 한다.

  

DNS 서버가 털리면 [엉뚱한 곳으로 리다이렉트되는
사고](http://star.fnnews.com/news/index.html?no=24233)가 터지거나, [인터넷이 먹통이되어버린다](%EC%9D%B8%ED%84%B0%EB%84%B7%20%EB%8C%80%EB%9E%80.md). 단 이런 경우는 먹통이
되지 않은 다른 DNS서버를 사용하면 해결된다. 만에 하나 모든 DNS서버가 터지더라도 사용자가 IP를 외우고 다닌다면 이런 상황에서도
웹서핑을 할 수 있다.

  

과거 [대한민국](%EB%8C%80%ED%95%9C%EB%AF%BC%EA%B5%AD.md) 정부에서는 DNS를 이용해서
[warning.or.kr](warning.or.kr.md)을 띄웠었다. 국내 [ISP](ISP.md)들이 돌리는 DNS서버에
차단하고 싶은 특정 주소를 입력하면 [warning.or.kr](warning.or.kr.md)로 자동 리다이렉트 되는 식이였다.
하지만 결국 이 방법은 국내 [ISP](ISP.md)들의 DNS 서버를 안쓰면 해결되는 일이므로, 실효성 논란과 국내기업 역차별 문제가
불거졌다. 그래서 지금은 아예 [IP](IP.md)를 차단하는 방법을 주로 쓰고있다. 그렇다고 DNS 차단이 없어진것은 아니고, 아직
국내 [ISP](ISP.md) DNS 한정으로 병행되고 있기 때문에, <del>그럴 일은 없겠지만</del>해외 인터넷 망에서 국내
[ISP](ISP.md)의 DNS를 쓰면 전세계 어디서든 [warning.or.kr](warning.or.kr.md)를 만날 수
있다.

  

.GEEK, [.onion](Tor#s-2.md) 같은 특이한 주소를 연결해 주는 서버나 보안업체에서 제공하는 DNS 서버도 있다.
후자의 경우 악성코드, 유해매체 차단 등의 기능이 들어가기도 한다.

  

DNS 서버의 벤치마킹 프로그램으로 namebench라는 프로그램 있다. [사용법과 다운로드](http://clien.career.co.kr
/cs2/bbs/board.php?bo_table=lecture&wr_id=84500)

  

[[edit](http://rigvedawiki.net/r1/wiki.php/DNS?action=edit&section=7)]

## 5. 관련 용어 ¶

  * [IP](IP.md)
  * [ISP](%EC%9D%B8%ED%84%B0%EB%84%B7%20%EC%84%9C%EB%B9%84%EC%8A%A4%20%EC%A0%9C%EA%B3%B5%EC%82%AC%EC%97%85%EC%9E%90.md)
  * [도메인](%EB%8F%84%EB%A9%94%EC%9D%B8.md)
  * [인터넷](%EC%9D%B8%ED%84%B0%EB%84%B7.md)
  * [웹 브라우저](%EC%9B%B9%20%EB%B8%8C%EB%9D%BC%EC%9A%B0%EC%A0%80.md)  

[[edit](http://rigvedawiki.net/r1/wiki.php/DNS?action=edit&section=8)]

## 6. 관련 문서 ¶

  * [DNS 스푸핑](DNS%20%EC%8A%A4%ED%91%B8%ED%95%91.md)
  * <del>[warning.or.kr](warning.or.kr.md)</del>
  * [인터넷 대란](%EC%9D%B8%ED%84%B0%EB%84%B7%20%EB%8C%80%EB%9E%80.md)

`\----`

  * `[1]` "DNS"는 시스템을 의미하고, 이 시스템을 운영하는 서버가 "DNS서버"이다.
  * `[2]` 2015년 2월 기준. ISP 정책으로 링크가 올바로 작동하진 않는다.
  * `[3]` [daum.net](Daum.md)의 DNS 서버 (보조: ns2.daum.net)
  * `[4]` [ISP](%EC%9D%B8%ED%84%B0%EB%84%B7%20%EC%84%9C%EB%B9%84%EC%8A%A4%20%EC%A0%9C%EA%B3%B5%EC%82%AC%EC%97%85%EC%9E%90.md)[(통신사)](%ED%86%B5%EC%8B%A0%ED%9A%8C%EC%82%AC.md)의 DNS 서버를 이용한다고 가정한다.
  * `[5]` 루트 DNS 서버를 **.**으로 표시한다.
  * `[6]` 등급별로 필터링 기능이 있다. [안내 페이지 ](https://dns.norton.com/dnsweb/huConfigurePc.do)
  * `[7]` A - Security (malware, phishing sites and scam sites)
  * `[8]` B - Security + Pornography
  * `[9]` C - Security + Pornography + Non-Family Friendly

