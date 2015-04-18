## 목차

    

1 개요

2 지원 운영체제

3 용도

4 사용례

5 관련 항목

## 1 개요 ¶

Privoxy는 [프록시 서버](%ED%94%84%EB%A1%9D%EC%8B%9C%20%EC%84%9C%EB%B2%84.md)
[소프트웨어](%EC%86%8C%ED%94%84%ED%8A%B8%EC%9B%A8%EC%96%B4.md)의 일종으로, 일반적인 프록시
서버와 달리 자신의 컴퓨터에 설치하여 사용하는 소프트웨어이다. 이 소프트웨어는 [오픈소스](%EC%98%A4%ED%94%88%20%EC%86%8C%EC%8A%A4.md) 라이센스 중 하나인
[GPL](GPL.md)을 따르고 있다. 공식 사이트는 <http://www.privoxy.org/>

## 2 지원 운영체제 ¶

공식 사이트에 따르면, 다음 운영체제를 지원한다고 한다. (출처:
<http://www.privoxy.org/faq/installation.html#WHICHOS>) 단, 소스코드를 받아 직접
[컴파일](%EC%BB%B4%ED%8C%8C%EC%9D%BC.md)을 해야 하는 운영체제도 있다. (예: 솔라리스)  

  * [윈도우즈](Microsoft%20Windows.md) \- 98, ME, 2000, XP, Vista, 7
  * [OS X](OS%20X.md) (10.4 이상)
  * [리눅스](%EB%A6%AC%EB%88%85%EC%8A%A4.md)
  * [OS/2](OS/2.md)
  * [하이쿠](%ED%95%98%EC%9D%B4%EC%BF%A0#s-2.md)
  * [DragonFlyBSD](DragonFlyBSD.md)
  * [FreeBSD](FreeBSD.md)
  * [NetBSD](NetBSD.md)
  * [OpenBSD](OpenBSD.md)
  * [솔라리스](%EC%86%94%EB%9D%BC%EB%A6%AC%EC%8A%A4#s-4.md)  

## 3 용도 ¶

자신의 컴퓨터에 설치하기 때문에 <del>[warning.or.kr](%EB%B0%A9%EC%86%A1%ED%86%B5%EC%8B%A0%EC%8B%AC%EC%9D%98%EC%9C%84%EC%9B%90%ED%9A%8C.md) 우회</del> [IP우회](IP%20%EC%9A%B0%ED%9A%8C.md)같은 효과는 전혀 없다. 하지만 프록시를 통해 주고받는 정보를 중간에서 가로채
조작할 수 있기 때문에 HTTP 헤더나 웹 사이트의 내용을 고칠 수 있다.

  

설정 파일(action 파일이나 filter 파일)을 고칠 때
[정규표현식](%EC%A0%95%EA%B7%9C%ED%91%9C%ED%98%84%EC%8B%9D.md)을 알아두면 수월하다.

## 4 사용례 ¶

Action 파일을 고쳐 어떤 사이트에 어떤 기능을 적용할지 설정할 수 있고, Filter 파일을 고쳐 웹 사이트의 내용을 어떻게 고칠지
설정할 수 있다.  

  

  * 웹 사이트 차단 - hosts파일 수정하여 광고를 차단하듯, 특정 URL을 차단하거나 다른 사이트로 가도록 할 수 있다. 광고 사이트나 [쇼크 사이트](%EC%87%BC%ED%81%AC%20%EC%82%AC%EC%9D%B4%ED%8A%B8.md)를 차단 하는데에 쓸 수 있다.  

    * 차단 임시 해제 - 필요하면 임시로 차단을 해제할 수도 있다. 물론 이 기능을 끌 수 있다. (컴파일 할 때 disable-force옵션을 주면된다.)  

  * [HTTP](HTTP.md) 헤더 조작 (단, [자바스크립트](%EC%9E%90%EB%B0%94%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8.md)로 원래의 유저 에이전트`[1]`나 리퍼러`[2]`를 알아낼 수 있다는 점에 주의할 것)  

    * [유저 에이전트](%EC%9C%A0%EC%A0%80%20%EC%97%90%EC%9D%B4%EC%A0%84%ED%8A%B8.md)(User Agent) 조작 - 자신이 사용하는 [운영체제](%EC%9A%B4%EC%98%81%EC%B2%B4%EC%A0%9C.md)나 [웹 브라우저](%EC%9B%B9%20%EB%B8%8C%EB%9D%BC%EC%9A%B0%EC%A0%80.md) 정보를 속일 수 있다.
    * [리퍼러](%EB%A6%AC%ED%8D%BC%EB%9F%AC.md)(Referer) 조작 - 외부 링크 차단`[3]`등을 우회할 수 있다.  

  * 웹 페이지 내용 조작 - 말 그대로 웹 페이지의 글자를 마음대로 고칠 수 있다. 단순한 단어 변경부터`[4]`, blink태그 때문에 깜박거리는 글자가 있으면 blink 태그를 없앨 수 있고, [팝업](%ED%8C%9D%EC%97%85.md)을 막거나, 광고 차단 등 폭넓게 활용할 수 있다.  

  * [쿠키](%EC%BF%A0%ED%82%A4#s-4.md) 차단 - 쿠키를 차단하여 특정 사이트의 로그인을 막을 수 있다.  

  * [GIF](GIF.md) 애니메이션([움짤](%EC%9B%80%EC%A7%A4.md))을 정지이미지로 변환할 수 있다.  

## 5 관련 항목 ¶

  * [오픈 소스](%EC%98%A4%ED%94%88%20%EC%86%8C%EC%8A%A4.md)
  * [프록시 서버](%ED%94%84%EB%A1%9D%EC%8B%9C%20%EC%84%9C%EB%B2%84.md)
  * [HTTP](HTTP.md)

`\----`

`[1]` navigator.userAgent  
`[2]` document.referrer  
`[3]` 예를 들어, [이글루스](%EC%9D%B4%EA%B8%80%EB%A3%A8%EC%8A%A4.md)에 링크한 이미지를 외부
사이트에서 보면 저품질화된 이미지가 뜨는데, 이 기능을 이용하면 원래 품질의 이미지를 볼 수 있다.  
`[4]` 예: [ActiveX](ActiveX.md)를 쓰레기로 치환할 수 있다. (...)

