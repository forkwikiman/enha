![jQuery.png](//z.enha.kr/http://rigvedawiki.net/r1/pds/jQuery.png)

[PNG image (13.9 KB)]

  
[공식 사이트](http://jquery.com/)  
[jQuery UI](http://jqueryui.com/)  
[jQuery Mobile](http://jquerymobile.com/)

**"write less, do more"**

**jQuery**는 HTML 속 클라이언트 사이드 스크립트 언어를 단순화 하도록 설계된 브라우저 호환성이 있는 [자바스크립트](%EC%9E%90%EB%B0%94%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8.md) [라이브러리](%EB%9D%BC%EC%9D%B4%EB%B8%8C%EB%9F%AC%EB%A6%AC.md)이다. [존 레식](%EC%A1%B4%20%EB%A0%88%EC%8B%9D.md)에 의해, 2006년 뉴욕 시 바캠프(Barcamp NYC)에서 공식으로 소개되었다. jQuery는 현재 가장 인기있는 자바스크립트 라이브러리이다. 거의 표준에 가까운 점유율을 자랑한다.([참고](http://w3techs.com/technologies/history_overview/javascript_library/all/y))

기능적으로야 더 좋은 라이브러리들도 많지만, jQuery가 순식간에 업계를 장악한 특장점은 바로 무지하게 쉽고 간편하다는 점이다.
'write less, do more'가 모토로서 비프로그래머인 웹디자이너들도 어렵지않게 이해할 수 있을 만큼 쉬운 편이다. DOM구조와
CSS에 대한 지식만 있다면 애니메이션 같은 건 바로 이해가 가능할 정도다. 실제로 저자인 존 레식은 프로그래머들의 칭찬보다 순수
웹디자이너들의 감사 인사가 더 특별한 기쁨이라고 한다.

jQuery는 [MIT](MIT.md) 라이선스와 GNU 일반 공중 사용 허가서 버전 2의 듀얼 라이선스를 가진 [자유 소프트웨어](/
wiki/%EC%9E%90%EC%9C%A0%20%EC%86%8C%ED%94%84%ED%8A%B8%EC%9B%A8%EC%96%B4)이다.
jQuery의 문법은 코드 보기, 문서 객체 모델 찾기, 애니메이션 만들기, 이벤트 제어, [Ajax](Ajax.md) 개발이 쉽도록
디자인 되었다. 또한, jQuery는 개발자가 [플러그인](%ED%94%8C%EB%9F%AC%EA%B7%B8%EC%9D%B8.md)을
개발할 수 있는 기능을 제공한다.

[마이크로소프트](%EB%A7%88%EC%9D%B4%ED%81%AC%EB%A1%9C%EC%86%8C%ED%94%84%ED%8A%B8.md)와 [노키아](%EB%85%B8%ED%82%A4%EC%95%84.md)는 자사
[플랫폼](%ED%94%8C%EB%9E%AB%ED%8F%BC.md)에 jQuery를 포함하는 계획을 발표한 바 있다. [마이크로소프트]
(/wiki/%EB%A7%88%EC%9D%B4%ED%81%AC%EB%A1%9C%EC%86%8C%ED%94%84%ED%8A%B8)는 [비주얼 스튜디오](%EB%B9%84%EC%A3%BC%EC%96%BC%20%EC%8A%A4%ED%8A%9C%EB%94%94%EC%98%A4.md)의 ASP.NET AJAX [프레임워크](%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8C%ED%81%AC.md)와
ASP.NET MVC 프레임워크에 적용했고, 노키아는 자사의 런타임 웹 위젯 개발 플랫폼에 통합하였다.

주요 웹 CMS나 위키위키에도 내장하는 경우가 많다.
[미디어위키](%EB%AF%B8%EB%94%94%EC%96%B4%EC%9C%84%ED%82%A4.md)에도 1.16 버전부터 사용되고
있고, [그누보드](%EA%B7%B8%EB%88%84%EB%B3%B4%EB%93%9C.md)나
[XpressEngine](XpressEngine.md)도 이게 기본으로 들어가 있다.

최근에는 jQuery Mobile이라는 물건도 개발하였는데, [iOS](iOS.md),
[안드로이드](%EC%95%88%EB%93%9C%EB%A1%9C%EC%9D%B4%EB%93%9C.md), [WindowsPhone](Windows%20Phone.md),
[블랙베리](%EB%B8%94%EB%9E%99%EB%B2%A0%EB%A6%AC.md),
[심비안](%EC%8B%AC%EB%B9%84%EC%95%88.md) 등 **웬만한 기기는 다 지원한다.**
[흠많무](%ED%9D%A0%EB%A7%8E%EB%AC%B4.md).

jQuery는 다음과 같은 기능을 갖고 있다.  

  * DOM 엘리먼트 선택
  * DOM 트래버설 및 수정(CSS 1-3 지원. 기본적인 XPath를 플러그인 형태로 지원)
  * 이벤트
  * CSS 조작`[1]`
  * 특수효과 및 애니메이션`[2]`
  * [Ajax](ajax#s-1.md)
  * 자바스크립트 플러그인을 통한 확장성
  * 유틸리티 - 브라우저 종류와 버전,`[3]` "each" 함수`[4]`
  * [JSON](JSON.md), [XML](XML.md) 파싱

`\----`

  * `[1]` 어디까지나 **브라우저가 지원하는 것까지만.** IE8 이하에서는 죽어라 border-radius 등을 줘도 안먹는다(...).
  * `[2]` 물론 좀 더 복잡한 애니메이션이 필요하다면 jQuery UI라는 확장기능을 사용해야 한다.
  * `[3]` [IE](IE.md), [모질라 파이어폭스](%EB%AA%A8%EC%A7%88%EB%9D%BC%20%ED%8C%8C%EC%9D%B4%EC%96%B4%ED%8F%AD%EC%8A%A4.md), [오페라](%EC%98%A4%ED%8E%98%EB%9D%BC%28%EC%9B%B9%20%EB%B8%8C%EB%9D%BC%EC%9A%B0%EC%A0%80%29.md), [웹키트](%EC%9B%B9%ED%82%A4%ED%8A%B8.md) 등을 판별할 수 있다. 다만 1.9 버전 이후부터 삭제되었다. 굳이 사용하고 싶다면 jQuery Migrate라는 것을 하나 더 불러와야 한다.
  * `[4]` 배열이나 객체 등의 집합에서 요소를 차례로 훑는다.

