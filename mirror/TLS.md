  * 관련 문서: [컴퓨터 관련 정보](%EC%BB%B4%ED%93%A8%ED%84%B0%20%EA%B4%80%EB%A0%A8%20%EC%A0%95%EB%B3%B4.md)
  * [스타크래프트 2](%EC%8A%A4%ED%83%80%ED%81%AC%EB%9E%98%ED%94%84%ED%8A%B8%202.md) 대회를 찾는다면 [SSL](Starcraft%202%20StarLeague.md) 항목으로.

![https.png](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/SSL/https.png)

[PNG image (45.35 KB)]

  
[인터넷 익스플로러](%EC%9D%B8%ED%84%B0%EB%84%B7%20%EC%9D%B5%EC%8A%A4%ED%94%8C%EB%A1%9C%EB%9F%AC.md), [모질라 파이어폭스](%EB%AA%A8%EC%A7%88%EB%9D%BC%20%ED%8C%8C%EC%9D%B4%EC%96%B4%ED%8F%AD%EC%8A%A4.md), [크롬](%ED%81%AC%EB%A1%AC%28%EC%9B%B9%20%EB%B8%8C%EB%9D%BC%EC%9A%B0%EC%A0%80%29.md)에서 [구글](%EA%B5%AC%EA%B8%80.md)에
TLS 연결을 한 모습. <del>파폭은 구글 같은 거 모른다</del>

Transport Layer Security

## Contents

    

1. 개요 
2. 작동 방법 
3. HTTPS 
4. 문제점 
5. 검증된 CA(인증 기관)들 
    

5.1. 미국

5.2. 이스라엘

5.3. 일본

5.4. 한국

6. NSA는 그런거 알 바 아닙니다? 
7. 관련항목 

[[edit](http://rigvedawiki.net/r1/wiki.php/TLS?action=edit&section=1)]

## 1. 개요 ¶

인터넷에서의 정보를 암호화해서 송수신하는 [프로토콜](%ED%94%84%EB%A1%9C%ED%86%A0%EC%BD%9C.md).
[넷스케이프](%EB%84%B7%EC%8A%A4%EC%BC%80%EC%9D%B4%ED%94%84.md) 커뮤니케이션스사가 개발한
SSL(Secure Sockets Layer)에서 기반한 기술로, 국제 인터넷 표준화 기구에서 표준으로 인정받은 프로토콜이다. 표준에 명시된
정식 명칭은 TLS지만 아직도 SSL이라는 용어가 많이 사용되고 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/TLS?action=edit&section=2)]

## 2. 작동 방법 ¶

인터넷을 사용한 통신에서 보안을 확보하려면 두 통신 당사자가 서로가 신뢰할 수 있는 자임을 확인할 수 있어야 하며, 서로간의 통신 내용이
제3자에 의해 도청되는 것을 방지해야 한다. 따라서 서로 자신을 신뢰할 수 있음을 알리기 위해 전자 서명이 포함된 인증서를 사용하며, 도청을
방지하기 위해 통신 내용을 암호화한다. 이러한 통신 규약을 묶어 정리한 것이 바로 TLS. 주요 웹브라우저 주소창에 자물쇠 아이콘이 뜨는
것으로 TLS의 적용 여부를 확인할 수 있다.

  

예를 들어 인터넷 뱅킹을 하기 위해 은행의 사이트에 방문했을 때, 고객은 그 사이트가 정말 은행의 사이트가 맞는지 아니면 해커가 만든 가짜
[피싱](%ED%94%BC%EC%8B%B1.md) 사이트인지 확인할 수 있어야 하며, 은행 역시 자신의 서비스를 이용하고자 하는 자가
해당 고객이 맞는지 아니면 신원을 도용한 다른 자인지 확인할 수 있어야 한다. 그리고 은행과 고객 간의 통신 내용이 다른 해커에게 도청되지
않도록 내용을 숨겨야 한다. 이럴 때 바로 은행과 고객 간에 TLS를 사용한 연결을 맺어 안전하게 통신을 할 수 있다.

  

구체적으로 서로의 신원을 확인하기 위해 핸드셰이크(Handshake) 과정을 거치며, 다음과 같다.

  

1\. 먼저 클라이언트에서 서버에 ClientHello 메시지를 보낸다. 여기에는 클라이언트에서 가능한 TLS 버전, 세션 식별자, 암호
설정 등의 정보가 포함된다.  

2\. 클라이언트의 메시지를 받은 서버는 ServerHello 메시지를 클라이언트에게 보낸다. 여기에는 ClientHello 메시지의 정보
중 서버에서 사용하기로 선택한 TLS 버전, 세션 식별자, 암호 설정 등의 정보가 포함된다.  

3\. 서버가 클라이언트에 Certificate 메시지를 보낸다. 여기에는 서버의 인증서가 들어간다. 이 인증서는 별도의 인증 기관에서
발급받은 것이며, 서버가 신뢰할 수 있는 자임을 인증한다. 전송이 끝나면 ServerHelloDone 메시지를 보내 끝났음을 알린다.  

4\. 클라이언트는 서버에서 받은 인증서를 검증한다. 인증서의 유효 기간이 만료되지 않았는지, 그 인증서가 해당 서버에게 발급된 인증서가
맞는지 등을 확인한다. 인증서를 신뢰할 수 있다고 판단하였다면 다음 단계로 넘어간다.  

5\. 클라이언트는 임의의 pre-master secret을 생성한 뒤, 서버가 보낸 인증서에 포함된 공개 키를 사용해 암호화한다. 이렇게
암호화된 pre-master secret을 ClientKeyExchange 메시지에 포함시켜 서버에 전송한다.  

6\. 서버는 전송받은 정보를 복호화하여 pre-master secret을 알아낸 뒤, 이 정보를 사용해 master secret을
생성한다. 그 뒤 master secret에서 세션 키를 생성해내며, 이 세션 키는 앞으로 서버와 클라이언트 간의 통신을 암호화하는데 사용할
것이다. 물론 클라이언트 역시 자신이 만들어낸 pre-master secret을 알고 있으므로, 같은 과정을 거쳐 세션 키를 스스로 만들 수
있다.  

7\. 이제 서버와 클라이언트는 각자 동일한 세션 키를 가지고 있으며, 이를 사용해 대칭 키 암호를 사용하는 통신을 할 수 있다. 따라서
우선 서로에게 ChangeCipherSpec 메시지를 보내 앞으로의 모든 통신 내용은 세션 키를 사용해 암호화해 보낼 것을 알려준 뒤,
Finished 메시지를 보내 각자의 핸드셰이킹 과정이 끝났음을 알린다.  

8\. 이제 서버와 클라이언트 간에 보안 통신이 구성된다.

  
경우에 따라 클라이언트에서 서버의 인증서를 요구하는 것 뿐만 아니라 서버에서 클라이언트의 인증서를 요구하기도 한다.

  

쉽게 요약해서, 먼저 서로가 어떤 TLS 버전을 사용 가능한지를 확인하고, 인증서를 사용해 서로를 믿을 수 있는지 확인한 뒤, 서로간의
통신에 쓸 암호를 교환하는 것이다. 그 다음부터는 서로 교환한 암호를 사용해 제3자가 도청할 수 없는 암호화된 통신을 하면 된다.

  

대신 일반 통신에 비해 [크고아름다운](%ED%81%AC%EA%B3%A0%20%EC%95%84%EB%A6%84%EB%8B%A4%EC%9A%B4.md)
[패킷](%ED%8C%A8%ED%82%B7.md)을 사용하는 암호화 통신인 만큼 속도상의 손해가 발생하게 된다.
[플래시](%EC%96%B4%EB%8F%84%EB%B9%84%20%ED%94%8C%EB%9E%98%EC%8B%9C.md)나 큰 이미지가
많은 사이트에서 TLS를 쓰는 것은 그야말로 [헬게이트](%ED%97%AC%EA%B2%8C%EC%9D%B4%ED%8A%B8.md).
사실 이것을 간과할 수 없는 게, HTTPS로 연결된 페이지에서 한 개라도 구성 요소 중 HTTP로 로드하는 것이 있다면 [웹브라우저](%EC%9B%B9%20%EB%B8%8C%EB%9D%BC%EC%9A%B0%EC%A0%80.md)가 "[네 컴퓨터의 통신이암호화 안된 요소에 침식당하기 시작해서 위험해](%EB%82%B4%ED%98%84%EC%8B%A4%EA%B3%BC%EC%98%A8%EB%9D%BC%EC%9D%B8%EA%B2%8C%EC%9E%84%EC%9D%B4%EB%9F%AC%EB%B8%8C%EC%BD%94%EB%AF%B8%EB%94%94%EC%97%90%EC%B9%A8%EC%8B%9D%EB%8B%B9%ED%95%98%EA%B8%B0%EC%8B%9C%EC%9E%91%ED%95%B4%EC%84%9C%EC%9C%84%ED%97%98%ED%95%B4.md)"라면서 **보안 경고를 뿜어대기
때문이다**.`[1]` 웹상의 모든 요소를 암호화해야 하기 때문인지, 외국 홈페이지는 화려하게 치장하기에 열을 올리는 국내 페이지에 비해
깔끔한(나쁘게 말하면 수수한) 편이다.`[2]`

  

[[edit](http://rigvedawiki.net/r1/wiki.php/TLS?action=edit&section=3)]

## 3. HTTPS ¶

TLS를 사용해 암호화된 연결을 하는 HTTP를 HTTPS라고 하며, 당연히 웹사이트 주소 역시 HTTP가 아닌 HTTPS로 시작된다. 기본
포트는 443번을 쓴다.

  

흔히 TLS와 HTTPS를 혼동하는 경우가 많은데, 둘은 유사하긴 하지만 엄연히 다른 개념임을 알아두자. TLS는 다양한 종류의 보안 통신을
하기 위한 프로토콜이며, HTTPS는 TLS 위에 HTTP 프로토콜을 얹어 보안된 HTTP 통신을 하는 프로토콜이다. 다시 말해 TLS는
HTTP뿐만이 아니라 [FTP](FTP.md), [SMTP](SMTP.md)와 같은 여타 프로토콜까지 포함하며, HTTPS는
TLS와 HTTP가 조합된 프로토콜만을 가리킨다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/TLS?action=edit&section=4)]

## 4. 문제점 ¶

다시 한 번 말하지만, TLS에서 서버 및 클라이언트의 신원을 확인하는 데는 인증서가 사용되며, 인증서의 신뢰성은 인증서를 발급해 준 인증
기관에 의해 결정된다. 인증 기관이 신뢰 가능한 인증서만을 발급해 줬다면 문제가 없지만, 만약 제대로 확인되지 않은 인증서를 발급한다면 더
이상 그 인증서를 신뢰할 수가 없을 것이다. **[그런데 그것이 실제로 일어났습니다](%EA%B7%B8%EB%9F%B0%EB%8D%B0%20%EA%B7%B8%EA%B2%83%EC%9D%B4%20%EC%8B%A4%EC%A0%9C%EB%A1%9C%20%EC%9D%BC%EC%96%B4%EB%82%AC%EC%8A%B5%EB%8B%88%EB%8B%A4.md)**.

  

몇몇 인증 기관에서 보안 수준이 매우 낮은 Domain Validation 인증서를 발급하기 시작한 것이다. 이러한 인증서는 오직 발급을
요청한 자가 그 도메인의 소유자가 맞는지만을 인증하기 때문에 사실상 발급 비용만 내면 아무나 인증서를 받을 수 있다. 심지어 해커가 피싱용
도메인 www.rigvedavviki.net`[3]`을 만든 뒤, 인증 기관에 Domain Validation 인증서를 요청하면 그대로
발급된다! 도메인을 소유한 자와 인증서를 신청한 자가 동일한 사람(=해커)이기 때문. 하지만 이 피싱 사이트에 접속한 대부분의 사용자들은
HTTPS 연결이 되었기 때문에 보안이 지켜질 것이라 생각하며 속게 된다.

  

![evc.png](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/SSL/evc.png)

[PNG image (70.18 KB)]

  
이러한 문제를 해결하기 위해 나온 것이 EV-SSL이다. EV-SSL은 **공신력 있는** 인증 기관에서 더욱 엄격한 심사 기준으로 발급한
Extended Validation 인증서를 사용하여 보안을 강화한 프로토콜이다. 주요 웹브라우저를 사용해 Extended
Validation 인증서를 쓰는 웹사이트에 접속하면 위와 같이 주소창에 특유의 녹색 표시가 생기며 EV-SSL 연결이 되었음을 알려 준다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/TLS?action=edit&section=5)]

## 5. 검증된 CA(인증 기관)들 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/TLS?action=edit&section=6)]

### 5.1. 미국 ¶

  * [Comodo Group](http://www.comodo.com/) : [한국SC은행](%ED%95%9C%EA%B5%ADSC%EC%9D%80%ED%96%89.md)이 여기서 발행한 인증서를 사용한다.
  * [Geo Trust](https://www.geotrust.com/)
  * [Go Daddy](http://www.godaddy.com/) : 레이싱 모델과 회사 사장이 나와서 광고하는 그 사이트다(...).
  * [Thawte](http://www.thawte.com/) : VeriSign과 함께 CA의 할아버지뻘 되는 아주 오래된 회사. 창립자가 회사를 VeriSign에 팔고 자기는 우주여행(...)을 다녀왔고 우분투를 만드는 캐노니컬을 창립했다.
  * [VeriSign](http://www.verisign.com/) : 세계 100대 은행 중 97개 은행이 사용할 정도로 유명한 회사이다. 한국의 [오픈뱅킹](%EC%98%A4%ED%94%88%EB%B1%85%ED%82%B9.md)도 대부분 이 회사의 인증서를 사용한다.  

[[edit](http://rigvedawiki.net/r1/wiki.php/TLS?action=edit&section=7)]

### 5.2. 이스라엘 ¶

  * [StartCom StartSSL](http://startssl.com/) : Class 1 인증서를 **무료로 준다**. (입력 실수나 개인키 분실로 인한 해당 계정의 인증 취소는 수수료를 요구함)  

[[edit](http://rigvedawiki.net/r1/wiki.php/TLS?action=edit&section=8)]

### 5.3. 일본 ¶

  * [VeriSign Japan](https://www.verisign.co.jp) : 베리사인의 일본법인이다.
  * [SECOM Trust Systems](https://www.secomtrust.net/service/pfw/index.html)
  * [cybertrust](https://www.cybertrust.ne.jp/)  

[[edit](http://rigvedawiki.net/r1/wiki.php/TLS?action=edit&section=9)]

### 5.4. 한국 ¶

원래는 국내 최상위 기관인 [KISA](%ED%95%9C%EA%B5%AD%EC%9D%B8%ED%84%B0%EB%84%B7%EC%A7%84%ED%9D%A5%EC%9B%90.md)가 관련 비표준기술 공인인증 이권을 이유로 일부러 10년 넘게 계속해서 웹트러스트 인증을 받지
않았기 때문에 존재 가치가 무의미했다.`[4]` 그러나 보안 이슈가 수면 위로 올라오고, 국가단위의 인증서이면서도 웹트러스트 인증이 없는
코믹한 실상을 더 이상 숨길 수 없게 되어 <del>비판 측 논리의 선제방어/면피용으로</del> 2014년에 웹트러스트 인증을 받았다.
([관련 트라비아](https://www.google.co.kr/?gws_rd=ssl#newwindow=1&q=firefox+kisa))

  

  * [한국전자인증](http://www.crosscert.com/)
  * [애니서트](https://www.anycert.co.kr/aboutus/vision/)
  * [써트코리아](https://www.certkorea.co.kr)
  * [한비로](https://www.comodossl.co.kr) : 코모도의 한국 내 공식 프리미엄 파트너.  

[[edit](http://rigvedawiki.net/r1/wiki.php/TLS?action=edit&section=10)]

## 6. NSA는 그런거 알 바 아닙니다? ¶

[NSA](NSA.md)는 조직 내에서 자체적인 학회를 열 정도의 인재풀과 자금력을 가지고 있어 암/복호화 및 감청에 관해 외부와
10년 이상의 격차를 가지고 있다고 알려져 있다. TLS는 벌써 2010년부터 뚫어서 죄다 훔쳐봤다고 하며, 차기 암호화 표준안에다 직접
마스터키 뒷구멍이 있는 암호표준을 넣기 위해 개입한다고 전해진다. [#1](http://www.zdnet.com/article/has-
the-nsa-broken-ssl-tls-
aes/)[#2](http://blog.cryptographyengineering.com/2013/12/how-does-nsa-break-
ssl.html)

  

[[edit](http://rigvedawiki.net/r1/wiki.php/TLS?action=edit&section=11)]

## 7. 관련항목 ¶

  * [오픈뱅킹](%EC%98%A4%ED%94%88%EB%B1%85%ED%82%B9.md)
  * [ActiveX](ActiveX.md)
  * [공인인증서](%EA%B3%B5%EC%9D%B8%EC%9D%B8%EC%A6%9D%EC%84%9C.md)
  * [해킹](%ED%95%B4%ED%82%B9.md)
  * [크래킹](%ED%81%AC%EB%9E%98%ED%82%B9.md)
  * [전기통신금융사기](%EC%A0%84%EA%B8%B0%ED%86%B5%EC%8B%A0%EA%B8%88%EC%9C%B5%EC%82%AC%EA%B8%B0.md)
  * [인터넷뱅킹](%EC%9D%B8%ED%84%B0%EB%84%B7%EB%B1%85%ED%82%B9.md)
  * [하트블리드 사태](%ED%95%98%ED%8A%B8%EB%B8%94%EB%A6%AC%EB%93%9C%20%EC%82%AC%ED%83%9C.md)  

`\----`

  * `[1]` 암호화 페이지를 거의 다뤄보지 않은 초보 웹 관리자가 여기서 [삽질](%EC%82%BD%EC%A7%88.md)하는 경우도 많다.
  * `[2]` 다만 [2010년대](2010%EB%85%84%EB%8C%80.md)의 [웹표준](%EC%9B%B9%ED%91%9C%EC%A4%80.md) 바람으로 일부나마 국내 웹 페이지가 TLS로 갈아타고 있는 상황이고, 거기에 맞게 디자인을 최적화하고 있기는 하다.
  * `[3]` rigvedawiki에서 w를 v 2개로 바꾼 것. 자세히 보지 않는 한 속기 쉽다.
  * `[4]` 사실 KISA는 좀 억울한 게 공인인증사업은 KISA의 수익사업이 아니다. 즉 남의 이권싸움에 낑겨서 높으신 분들이 하라는 대로 했는데 욕은 KISA가 먹은 셈.

