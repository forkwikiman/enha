  * [두문자어](%EB%91%90%EB%AC%B8%EC%9E%90%EC%96%B4.md)

## Contents

    

1. 개요 

[[edit](http://rigvedawiki.net/r1/wiki.php/JSP?action=edit&section=1)]

## 1. 개요 ¶

[자바](%EC%9E%90%EB%B0%94#s-2.md)를 사용한 서버측 코드가 들어가 있는 웹페이지. 같은 카테고리로는
**[PHP](PHP.md)**, [ASP](ASP.md)가 있다.
[확장자](%ED%99%95%EC%9E%A5%EC%9E%90.md)는 당연히 .jsp를 사용.  
ASP와 마찬가지로 `<% ... %>`로 이루어진 스크립트 영역이 있으며, 실행시에
`javax.servlet.http.HttpServlet` 클래스를 상속받은 자바 소스코드로 변환된 다음 컴파일되어 실행된다.`[1]`  
이 JSP 파일을 Servlet 클래스로 변환하고 실행시켜 주는 역할을 하는 프로그램이 Servlet Container. 대표적으로 오픈소스
서블릿 컨테이너인 [톰캣](%ED%86%B0%EC%BA%A3.md)이 있다.

  

서블릿 컨테이너도 [자바](%EC%9E%90%EB%B0%94#s-2.md) 프로그램이며, [자바 가상머신](%EC%9E%90%EB%B0%94%20%EA%B0%80%EC%83%81%20%EB%A8%B8%EC%8B%A0.md) 위에서
실행된다. 따라서 대부분의 [운영체제](%EC%9A%B4%EC%98%81%EC%B2%B4%EC%A0%9C.md)에서 소스코드 변경이나
재 컴파일 없이 실행시킬 수 있고, 특히 [유닉스](%EC%9C%A0%EB%8B%89%EC%8A%A4.md)계열과 궁합이 잘 맞는다.

  

하나의 JSP페이지가 하나의 자바 클래스이기 때문에 모든 자바 라이브러리를 끌어다 쓸 수 있다.

  

중-소규모 사이트에서 주로 쓰이는 [PHP](PHP.md)와는 달리 주로 대규모 기업용 시스템 구축에 사용된다. 이런 경우에는 보통
단순한 서블릿 컨테이너가 아닌, WAS(Web Application Server)라는 프로그램이 동원된다. WAS는 JSP의 실행 뿐만
아니라 DB 커넥션 풀, 메시징 시스템, 로드밸런싱 등등 화려한 기능들로 무장하고 있고 덕분에 매우 비싸다.`[2]`  
이쪽 업계의 최고봉은 [BEA](BEA.md)의 WebLogic이었지만 지금은
[오라클](%EC%98%A4%EB%9D%BC%ED%81%B4.md)에 인수된 상태(...)

  

PHP를 지원하는 호스팅 업체는 많이 널려있지만 JSP를 호스팅해주는 업체는 찾기가 쉽지 않다.  
하지만 대인배 [구글](%EA%B5%AC%EA%B8%80.md)의 App Engine이 Java를 지원하니 이쪽을 이용해 보도록 하자.
게다가 공짜다!  
<https://developers.google.com/appengine/docs/java/gettingstarted/usingjsps?hl
=ko>

`\----`

  * `[1]` JSP 페이지를 만들지 않고 직접 서블릿 클래스를 작성하여 컴파일 한 다음 실행하는것도 가능하며 현업에서도 이런 방식이 많이 쓰인다.
  * `[2]` 오픈소스 WAS도 존재한다. [글래스피시](https://glassfish.java.net/), [wildfly](http://www.wildfly.org/) 등.

