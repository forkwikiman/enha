**주의. 이 문서는 지속적으로 갱신되는 내용을 다룹니다.**  
  
이 문서와 하위 문서는 진행 상황에 따라서 갱신될 가능성이 높으며, 급보는 오보일 수 있습니다. 검증된 내용이 나타날 때마다 지속적으로
갱신하기를 권장합니다. 더 갱신될 전망이 없으면 이 틀을 떼어주시기 바랍니다. 창작물은 반전 요소가 포함될 수도 있으니 열람 시 주의해
주세요.

  

  * 이 항목은 [프로젝트 스파르탄](%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%20%EC%8A%A4%ED%8C%8C%EB%A5%B4%ED%83%84.md)으로도 들어올 수 있습니다.
  * 관련 항목: [웹 브라우저](%EC%9B%B9%20%EB%B8%8C%EB%9D%BC%EC%9A%B0%EC%A0%80.md), [인터넷 익스플로러](%EC%9D%B8%ED%84%B0%EB%84%B7%20%EC%9D%B5%EC%8A%A4%ED%94%8C%EB%A1%9C%EB%9F%AC.md), [Windows 10](Windows%2010.md)  

## Contents

    

1. 개요 
2. 상세 
    

2.1. 인터넷 익스플로러와의 관계

3. 공개 
4. 명칭 
5. 특징 
6. 기타 

[[edit](http://rigvedawiki.net/r1/wiki.php/Project%20Spartan?action=edit&secti
on=1)]

## 1. 개요 ¶

2015년 1월 21일에 발표된 [인터넷 익스플로러](%EC%9D%B8%ED%84%B0%EB%84%B7%20%EC%9D%B5%EC%8A%A4%ED%94%8C%EB%A1%9C%EB%9F%AC.md)를 대체하기 위해 만들어진 [마이크로소프트](%EB%A7%88%EC%9D%B4%ED%81%AC%EB%A1%9C%EC%86%8C%ED%94%84%ED%8A%B8.md)의 신형 [웹브라우저](%EC%9B%B9%20%EB%B8%8C%EB%9D%BC%EC%9A%B0%EC%A0%80.md). 윈도우 10부터 시작하여
마이크로소프트 및 마이크로소프트의 OS 제품군을 사용하는 모든 장치의 기본 브라우저로 사용될 예정이다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Project%20Spartan?action=edit&secti
on=2)]

## 2. 상세 ¶

"프로젝트 스파르탄"은 마이크로소프트가 현대 웹 디자인과의 호환성을 극대화하기 위해 기존 인터넷 익스플로러에 사용되던 렌더링 엔진인
트라이던트(mshtml.dll)를하위호환을 고려하지 않고 바닥부터 개조하여 만들어낸 렌더링 엔진인 EdgeHTML(edgehtml.dll)을
기반으로 만들어진 새로운 웹 브라우저다. [원문 및 설명](http://blogs.msdn.com/b/ie/archive/2015/03/24
/updates-from-the-project-spartan-developer-workshop.aspx) 이게 무슨 뜻이냐 하면...

  

![http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-w
eblogfiles/00-00-00-38-71-metablogapi/1273.Microsoft_2D00_engines_2D00_diagram
_5F00_660x327.png](http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-
blogs-components-weblogfiles/00-00-00-38-71-metablogapi/1273.Microsoft_2D00_en
gines_2D00_diagram_5F00_660x327.png)

[[PNG external image]](http://blogs.msdn.com/cfs-file.ashx/__key
/communityserver-blogs-components-weblogfiles/00-00-00-38-71-metablogapi/1273.
Microsoft_2D00_engines_2D00_diagram_5F00_660x327.png)

  

스파르탄은 인터넷 익스플로러가 아니다. 이름만 바꾼 IE12가 아니고, IE11의 개선판은 더더욱 아니다. 스파르탄의 개발 과정을 설명하던
IE 팀의 한 개발자는 스파르탄의 개발이 결정된 이후 십여년 만에 처음으로 트라이던트 엔진의 코드를 지우기 시작한 순간 개발진 전체가
숙연하게 바라보며 희열을 느꼈다는 발언을 했는데, 위의 짤을 보면 쉽게 이해할 수 있다. 인터넷 익스플로러 11은 IE11 뿐만 아니라
10, 9, 8, 7, 심지어 5.5까지 지원하기 위한 하위 호환 코드들을 그대로 가지고 있다. 하지만 스파르탄은 이 하위호환을 위한 코드를
전부 날려버리고, 심지어 바로 이전 브라우저인 IE11과의 호환을 위한 코드까지 남김없이 뜯어낸 뒤 웹킷 또는 게코와 비슷한 현대적인
방식으로 렌더링을 함으로써 웹 표준을 따라 최근 만들어진 사이트들을 표시할 때 깨지거나 오류가 나는 상황을 최소화하는 것을 목적으로 하고
있다.

  

이것은 곧 MS가 드디어 [ActiveX](ActiveX.md)를 버린 브라우저를 만들었다는 뜻이기도 하다. 사실 액티브X를 위시한
IE6 방식의 웹 사이트는 해외에서도 그 문제가 심각한데, 특히 기업용 웹페이지 및 소프트웨어가 IE6을 요구하는 경우가 많다고 하며, 이런
부분 때문에 MS가 함부로 IE6 코드나 액티브X를 버리지 못한 측면이 크다. IE9 이래로 인터넷 익스플로러는 이 시절의 익스플로러에
비하면 훨씬 더 나아졌고 상당 부분 웹 표준을 따라가고 있지만, 아직 렌더링의 기본적인 원리는 IE5.5 내지 6 시절을 따라가고 있어 종종
오류가 나기도 했고, 반대로 웹페이지 쪽에서 사용자의 브라우저를 IE로 인식하는 바람에 웹 표준을 지키는 IE10이나 11을 사용함에도
불구하고 IE7/8 방식으로 코드를 보내주면서 문제가 생기기도 했었다. 스파르탄은 이를 막기 위해 레거시 코드를 통째로 날리고, 현대적
기준에 완전히 맞아 떨어지도록 기존 엔진을 [마개조](%EB%A7%88%EA%B0%9C%EC%A1%B0.md)하여 최신의 방식으로만
코드를 받고 표시하는 것을 목표로 한다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Project%20Spartan?action=edit&secti
on=3)]

### 2.1. 인터넷 익스플로러와의 관계 ¶

앞서 살펴본 바와 같이 스파르탄은 [파이어폭스](%EB%AA%A8%EC%A7%88%EB%9D%BC%20%ED%8C%8C%EC%9D%B4%EC%96%B4%ED%8F%AD%EC%8A%A4.md)나 [크롬](%ED%81%AC%EB%A1%AC%28%EC%9B%B9%20%EB%B8%8C%EB%9D%BC%EC%9A%B0%EC%A0%80%29.md)과 같은 선상에 있는 완전히 새로운 브라우저이기 때문에,
[ActiveX](ActiveX.md)로 떡칠되어 있는 온라인 뱅킹이나 인강 등의 서비스를 전혀 사용할 수 없다. 그렇다면 MS는
호환성 문제를 어떻게 해결했을까?

  

![http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-blogs-components-w
eblogfiles/00-00-00-38-71-metablogapi/1273.Microsoft_2D00_engines_2D00_diagram
_5F00_660x327.png](http://blogs.msdn.com/cfs-file.ashx/__key/communityserver-
blogs-components-weblogfiles/00-00-00-38-71-metablogapi/1273.Microsoft_2D00_en
gines_2D00_diagram_5F00_660x327.png)

[[PNG external image]](http://blogs.msdn.com/cfs-file.ashx/__key
/communityserver-blogs-components-weblogfiles/00-00-00-38-71-metablogapi/1273.
Microsoft_2D00_engines_2D00_diagram_5F00_660x327.png)

  

MS는 원래 스파르탄을 두 개의 엔진으로 돌리려고 하고 있었다. 대부분의 사이트는 새로 만든 EdgeHTML 엔진으로 보여주되, IE 레거시
코드를 필요로 하는 사이트들은 한정적으로 IE11의 엔진을 사용하는 방식이었다. 하지만 이렇게 하면 스파르탄이 나온다고 해도 레거시 코드로
그대로 돌아가니까 낡은 사이트들의 운영자들이 사이트를 갈아엎을 생각을 하지 않게 될 수밖에 없었고, 자동으로 EdgeHTML과 MSHTML을
오가게 하는 데에도 문제가 있어서, 결국에는 위의 그림에서처럼 스파르탄은 IE와 완전히 분리되게 되었다.

  

때문에 스파르탄으로 인한 호환성 문제는 스파르탄과 별개로 IE11을 남겨두는 방식으로 상당히 간단하게 해결되었다. 아직 익스플로러의 구식
코드를 필요로 하는 사이트가 많고, 이런 사이트들이 많아질수록 호환성 구리다고 업그레이드 안할 사람들이 늘어나리라는 걸 MS가 모를리가 없기
때문에, 윈도우 10에서도 IE11은 여전히 있다. 이 IE11은 심지어 기존 [윈도우8.1](%EC%9C%88%EB%8F%84%EC%9A%B0%208.1.md)의 IE와 아무런 차이도 없다. 다만 윈도우 10의 기본
브라우저는 스파르탄이며, IE11은 어디까지나 레거시 프로그램으로서 시작 메뉴의 액세서리 폴더로 들어가야 사용할 수 있다고 한다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Project%20Spartan?action=edit&secti
on=4)]

## 3. 공개 ¶

2014년 12월부터 마이크로소프트가 [윈도우 10](%EC%9C%88%EB%8F%84%EC%9A%B0%2010.md)을 위해서 인터넷
익스플로러가 아닌 새로운 브라우저를 만들고 있다는 루머가 돌았고, 2015년 1월 21일 공개 직전에는 이미 거의 대부분의 내용이 루머로
알려진 상황이었다. <del>그리고 기자들은 [홀로렌즈](%ED%99%80%EB%A1%9C%EB%A0%8C%EC%A6%88.md)로
통수를 맞았지</del> 예상대로 윈도우 10 발표회에서 루머로 돌았던 스파르탄의 존재와 대부분의 특징들이 그대로 공개되으나, 이후
[테크니컬 프리뷰](Windows%2010/%ED%85%8C%ED%81%AC%EB%8B%88%EC%BB%AC%20%ED%94%84%EB%A6%AC%EB%B7%B0.md)를 통해 공개하겠다고 밝히면서 당장은 쓸 수 없게 되었다.

  

2015년 3월 30일에 테크니컬 프리뷰의 10049 빌드가 빠른 채널로 풀리면서 프로젝트 스파르탄이 처음으로 대중에 공개되었다. 발표회에서
밝혔던 필기 기능, 리딩 리스트 기능, 코타나 연동 등의 기능들이 전부 사용 가능한 상태로 풀렸다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Project%20Spartan?action=edit&secti
on=5)]

## 4. 명칭 ¶

이름의 유래는 [헤일로시리즈](%ED%97%A4%EC%9D%BC%EB%A1%9C%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md)의 [병사 양성 프로젝트](%EC%8A%A4%ED%8C%8C%EB%A5%B4%ED%83%84%28%ED%97%A4%EC%9D%BC%EB%A1%9C%20%EC%8B%9C%EB%A6%AC%EC%A6%88%29.md). 다만 확정되지않은 임시 명칭이다. 공개 이후 유출된 설문조사에 따르면
MS에서는 "인터넷 익스플로러 엣지" 또는 "엣지" 등의 이름을 고려하고 있었다고 하는데, 이러한 이름들은 유출을 알리는 기사들에 달리는
댓글 뿐만이 아니라 설문조사 자체에서도 그리 좋은 반응을 얻지 못했다. 결국 3월 들어서 인터넷 익스플로러라는 브랜드가 완전히 폐기되었고,
"마이크로소프트 (브라우저 이름)"의 형태가 가장 반응이 좋았다는 자체 조사 결과에 따라 곧 이름이 정해질 예정이다. 그러나 [같은게임](%ED%97%A4%EC%9D%BC%EB%A1%9C%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md)의 [모여캐](%EC%BD%94%ED%83%80%EB%82%98.md)의 이름을 따온 가칭이 공식 명칭으로 확정된 전례가 최근에 있어서,
현재로서는 마이크로소프트 스파르탄으로 이름이 정해질 가능성이 다분하다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Project%20Spartan?action=edit&secti
on=6)]

## 5. 특징 ¶

  * 웹페이지 저장 및 필기 기능  
웹페이지를 통째로 하드 드라이브, 원노트 또는 원드라이브에 저장하고 그 위에 서피스 프로 등의 장치에서 사용하는 펜으로 필기를 할 수 있는
기능이 있다. MS에서는 이 기능을 스파르탄의 주력 기능 중 하나로 밀고 있다.

  * 읽기 목록 및 읽기 모드  
읽기 목록 기능은 기존 윈도우에서도 별도의 앱으로 지원하고 있었고, 다른 OS들도 마찬가지였지만, 스파르탄은 이 기능을 브라우저 안으로 끌고
들어와서 언제든지 오프라인으로 저장해 읽을 수 있도록 한다. 한편 페이지를 저장하든 저장하지 않았든 이들을 읽기 모드로 볼 수도 있는데,
다른 브라우저에도 있는 읽기 모드지만 스파르탄은 여기에 다양한 옵션을 제공하며, 읽기 모드 상태로 저장하여 나중에 다시 볼 수도 있다.

  * [코타나](%EC%BD%94%ED%83%80%EB%82%98#s-2.md) 연동  
[윈도우폰 8.1](Windows%20Phone.md)에서 처음 등장한 코타나가 윈도우 10에 이어 스파르탄에도 손을 댄다. 스파르탄의
검색창에 "날씨" 등 간단한 키워드를 입력하면 코타나가 알아서 검색어를 인식하고 엔터를 누르기도 전에 원하는 정보들을 간략하게 보여주기도
하며, 특정한 단어나 문구를 선택하여 오른쪽 버튼을 누르면 (터치 화면에서는 길게 누르면) "코타나에게 물어보기"가 뜨면서 즉시 원하는
정보를 검색하도록 해 준다.

  * 앱으로의 분리를 통한 빠른 업데이트  
윈도우 코드에 묶여 있어서 보안 부문 이외의 업데이트가 느렸던 인터넷 익스플로러와는 달리 스파르탄은 윈도우 스토어를 통해서 업데이트되는
앱이다. 따라서 다양한 부문에서의 업데이트가 [파이어폭스](%EB%AA%A8%EC%A7%88%EB%9D%BC%20%ED%8C%8C%EC%9D%B4%EC%96%B4%ED%8F%AD%EC%8A%A4.md)나 [크롬](%ED%81%AC%EB%A1%AC%28%EC%9B%B9%20%EB%B8%8C%EB%9D%BC%EC%9A%B0%EC%A0%80%29.md) 만큼이나 빠르게 이루어질 수 있다.

  * 다양한 플랫폼에 최적화된 UI  
스파르탄은 MS의 모든 플랫폼에 사용될 예정이다. 데스크탑 뿐만이 아니라 스마트폰, [엑스박스원](%EC%97%91%EC%8A%A4%EB%B0%95%EC%8A%A4%20%EC%9B%90.md),
[홀로렌즈](%ED%99%80%EB%A1%9C%EB%A0%8C%EC%A6%88.md), [서피스 허브](%EB%A7%88%EC%9D%B4%ED%81%AC%EB%A1%9C%EC%86%8C%ED%94%84%ED%8A%B8%20%EC%84%9C%ED%94%BC%EC%8A%A4%20%ED%97%88%EB%B8%8C.md) 등이 전부 스파르탄을 사용하며, 플랫폼에 맞는 서로 다른 UI가 사용될 예정이다.

  * 확장 기능 지원 (예정)  
스파르탄은 [파이어폭스](%EB%AA%A8%EC%A7%88%EB%9D%BC%20%ED%8C%8C%EC%9D%B4%EC%96%B4%ED%8F%AD%EC%8A%A4.md)나 [크롬](%ED%81%AC%EB%A1%AC%28%EC%9B%B9%20%EB%B8%8C%EB%9D%BC%EC%9A%B0%EC%A0%80%29.md)과 같이 플러그인 및 확장기능을 지원할 예정이다. 하지만 현재로서 이 기능은 우선 순위가 조금
밀려 있으며, '나중에' 나온다고 하는 것으로 보아 윈도우 10이 RTM을 끊고 조금 시간이 지나서 추가될 예정이다.  

[[edit](http://rigvedawiki.net/r1/wiki.php/Project%20Spartan?action=edit&secti
on=7)]

## 6. 기타 ¶

  * [어도비](Adobe.md)가 스파르탄 및 EdgeHTML의 그래픽 부분에 손을 대고 있다고 한다. 어도비는 과거 [오픈소스](%EC%98%A4%ED%94%88%EC%86%8C%EC%8A%A4.md) 기획인 [웹키트](%EC%9B%B9%ED%82%A4%ED%8A%B8.md) 및 게코에도 상당 부분 기여를 한 바가 있고 [애플](%EC%95%A0%ED%94%8C.md) [OS X](OS%20X.md)가 자랑하는 데스크톱OS 최강의 2D 엔진 쿼츠 역시 어도비의 기술이 많이 사용되었다. MS의 브라우저에 손을 대는 것은 이번이 처음이라고 한다. 이걸 보고 최근에 MS가 .NET을 오픈소스로 전환한 것도 그렇고 혹시 [EdgeHTML도 오픈소스로 가는거 아니냐는 반응](http://blogs.msdn.com/b/ie/archive/2015/03/23/partnering-with-adobe-on-new-contributions-to-our-web-platform.aspx)도 심심찮게 나오고 있다.

