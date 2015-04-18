  * [컴퓨터 관련 정보](%EC%BB%B4%ED%93%A8%ED%84%B0%20%EA%B4%80%EB%A0%A8%20%EC%A0%95%EB%B3%B4.md)  

이 항목은 [위지위그](%EC%9C%84%EC%A7%80%EC%9C%84%EA%B7%B8.md),
[위지윅](%EC%9C%84%EC%A7%80%EC%9C%85.md)으로도 들어올 수 있습니다.

  

![msword.png](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/WYSIWYG/msword.png)

[PNG image (32.13 KB)]

  
대표적인 WYSIWYG
[워드프로세서](%EC%9B%8C%EB%93%9C%ED%94%84%EB%A1%9C%EC%84%B8%EC%84%9C.md)인
[Microsoft Word](Microsoft%20Word.md).

## Contents

    

1. 개요 
2. 종류 
    

2.1. [워드프로세서](%EC%9B%8C%EB%93%9C%ED%94%84%EB%A1%9C%EC%84%B8%EC%84%9C.md)

2.2. [그래픽 툴](%EA%B7%B8%EB%9E%98%ED%94%BD%20%ED%88%B4.md)

2.3. [앱개발](%ED%86%B5%ED%95%A9%20%EA%B0%9C%EB%B0%9C%20%ED%99%98%EA%B2%BD.md)

2.4. [웹](%EC%9B%B9.md) 개발

3. [미니어처 게임](%EB%AF%B8%EB%8B%88%EC%96%B4%EC%B2%98%20%EA%B2%8C%EC%9E%84.md)에서 

[[edit](http://rigvedawiki.net/r1/wiki.php/WYSIWYG?action=edit&section=1)]

## 1. 개요 ¶

**W**hat **Y**ou **S**ee **I**s **W**hat **Y**ou **G**et`[1]`의 약자로, 문서 및 문서 작성 방법을 [GUI](GUI.md)로 구현한 것을 이른다. 이게 나오기 전의 문서 작성, 그러니까 **[텍스트 기반](CUI.md)으로만 문서를 작성하는 것**이 얼마나 비전문가에게 불친절한지는 [더 이상 말할 필요가 없다](%EB%8D%94%20%EC%9D%B4%EC%83%81%20%EB%A7%90%ED%95%A0%20%ED%95%84%EC%9A%94%EA%B0%80%20%EC%97%86%EB%8B%A4.md). 텍스트로만 문서를 짜는 것의 예를 보면, 지금 당장 [리그베다 위키](%EB%A6%AC%EA%B7%B8%EB%B2%A0%EB%8B%A4%20%EC%9C%84%ED%82%A4.md)의 아무 항목이나 들어가서 편집을 클릭해 보라. 당연히 위키 문법을 모르면 작성에 [애로사항](%EC%95%A0%EB%A1%9C%EC%82%AC%ED%95%AD.md)을 겪게 될 것이다.`[2]`  
그래서 문서 작성의 [진입장벽](%EC%A7%84%EC%9E%85%EC%9E%A5%EB%B2%BD.md)을 줄이기 위해,
[GUI](GUI.md)를 도입한 도구라고 생각할 수 있다. 그래서 필연적으로
[마우스](%EB%A7%88%EC%9A%B0%EC%8A%A4.md) 의존도가 큰 편이다.

  

관련 지식이 없는 비전문가도 간단하게 작업을 할 수 있고 생산성 또한 오르지만,
[날코딩](%EB%82%A0%EC%BD%94%EB%94%A9.md)에 비해서 크든 작든
**[발적화](%EB%B0%9C%EC%A0%81%ED%99%94.md)**가 된다는 극명한 단점이 있다. WYSIWYG를 구현하기 위해
필연적으로 쓸모없는 요소가 들어가게 되기 때문. 이것이 거듭될수록, 날코딩으로 전환해서
[최적화](%EC%B5%9C%EC%A0%81%ED%99%94.md)를 하려고 해도 [답이없는](%EB%8B%B5%EC%9D%B4%20%EC%97%86%EB%8B%A4.md) 상황으로 변하게 된다.`[3]`  
하지만 순수 날코딩으로 작업하는 것보다는 접근성도 높고 데이터를 가지고 이것저것 응용할 수 있는 것이 매우 많아지는 것은 사실이므로, 오늘도
WYSIWYG 제작자는 어떻게든 결과물의 최적화를 위해 [갈리고 있다](%EA%B3%B5%EB%B0%80%EB%A0%88.md)...

  

웹상에서는 [그누보드](%EA%B7%B8%EB%88%84%EB%B3%B4%EB%93%9C.md),
[XpressEngine](XpressEngine.md) 등에서 빈번하게 사용하고 있는데, 기본 텍스트 폼에 비해 무거운 것은 어쩔
수가 없다(...).

  

물론 [위키위키](%EC%9C%84%ED%82%A4%EC%9C%84%ED%82%A4.md)도 위지위그 스타일로 개발된 것도 있지만
대부분은 글 편집시 위지위그 스타일로 제공하는 수준이며, 위키까지 위지위그만으로 구동하는 엔진들은 아직까지는 초기단계다. 위키 유저의 저변을
쉽게 넓힐 수 있다는 장점에도 불구하고 아직까지 개발이 난관을 겪고 있는 건 **Microsoft Word 수준의 워드프로세서와 웹뷰어**를
만들어야 기존 위키를 대체할 수 있기 때문이다. 언젠가는 현재의 사용법이 어려운 위키들도 과거의 유물이 되겠지만 아직까진 멀었다.

[[edit](http://rigvedawiki.net/r1/wiki.php/WYSIWYG?action=edit&section=2)]

## 2. 종류 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/WYSIWYG?action=edit&section=3)]

### 2.1.
[워드프로세서](%EC%9B%8C%EB%93%9C%ED%94%84%EB%A1%9C%EC%84%B8%EC%84%9C.md) ¶

[워드프로세서](%EC%9B%8C%EB%93%9C%ED%94%84%EB%A1%9C%EC%84%B8%EC%84%9C.md) 참조.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/WYSIWYG?action=edit&section=4)]

### 2.2. [그래픽 툴](%EA%B7%B8%EB%9E%98%ED%94%BD%20%ED%88%B4.md) ¶

[그래픽 툴](%EA%B7%B8%EB%9E%98%ED%94%BD%20%ED%88%B4.md) 참조.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/WYSIWYG?action=edit&section=5)]

### 2.3. [앱개발](%ED%86%B5%ED%95%A9%20%EA%B0%9C%EB%B0%9C%20%ED%99%98%EA%B2%BD.md) ¶

[통합 개발 환경](%ED%86%B5%ED%95%A9%20%EA%B0%9C%EB%B0%9C%20%ED%99%98%EA%B2%BD.md)
참조.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/WYSIWYG?action=edit&section=6)]

### 2.4. [웹](%EC%9B%B9.md) 개발`[4]` ¶

  * [나모 웹에디터](%EB%82%98%EB%AA%A8%20%EC%9B%B9%EC%97%90%EB%94%94%ED%84%B0.md)
  * [드림위버](%EB%93%9C%EB%A6%BC%EC%9C%84%EB%B2%84.md)
  * [뮤즈](%EB%AE%A4%EC%A6%88.md)
  * [셰어포인트 디자이너](Microsoft%20Office.md)
  * [씨몽키](%EC%94%A8%EB%AA%BD%ED%82%A4.md)  

[[edit](http://rigvedawiki.net/r1/wiki.php/WYSIWYG?action=edit&section=7)]

## 3. [미니어처게임](%EB%AF%B8%EB%8B%88%EC%96%B4%EC%B2%98%20%EA%B2%8C%EC%9E%84.md)에서 ¶

미니어처 게임 모델의 능력치와 장비, 그리고 특수 규칙이 눈에 보이는 그대로와 같다는 뜻으로, 의미는 1번에서 따왔다.

  

[Warhammer 40,000](Warhammer%2040%2C000.md)를 비롯한 미니어처 게임에 쓰이는 모델에는 제각기 능력치와
특수 규칙이 붙어있고, 장비도 모델별로 갈아서 끼워줄 수 있는 경우가 많다. 이 때 모델의 능력치와 장비를 규칙서에 명시된 그대로 사용하는
경우에는 WYSIWYG, 다른 모델과 장비로 치환한 경우에는
[프록시](%ED%94%84%EB%A1%9D%EC%8B%9C#s-2.md)라고 한다. 각종 토너먼트 등에서는 분쟁의 원인을 없애기 위해
모든 모델을 WYSIWYG로 만들 것, 즉 조립하고 색칠한 상태로 규칙서의 규정에 완전히 맞춰서 플레이할 것을 요구하기도 한다.

  

![http://www.spinningdicegames.com/images/detailed/0/terminator-
squad.jpg](http://www.spinningdicegames.com/images/detailed/0/terminator-
squad.jpg)

[[JPG external image]](http://www.spinningdicegames.com/images/detailed/0
/terminator-squad.jpg)

  

공식 박스에 묘사된 위 분대의 예시를 들자면, 종류는 [스페이스마린](%EC%8A%A4%ED%8E%98%EC%9D%B4%EC%8A%A4%20%EB%A7%88%EB%A6%B0.md) [터미네이터 스쿼드](%ED%84%B0%EB%AF%B8%EB%84%A4%EC%9D%B4%ED%84%B0%20%EC%8A%A4%EC%BF%BC%EB%93%9C.md)고, 투구를 벗고 깃대를 맨 분대장은 [스톰볼터](%EC%8A%A4%ED%86%B0%20%EB%B3%BC%ED%84%B0.md)와 [파워소드](%ED%8C%8C%EC%9B%8C%20%EC%9B%A8%ED%8F%B0.md)를, 맨 왼쪽 분대원은 [어썰트캐논](%EC%96%B4%EC%8D%B0%ED%8A%B8%20%EC%BA%90%EB%85%BC.md)과 [파워피스트](%ED%8C%8C%EC%9B%8C%20%ED%94%BC%EC%8A%A4%ED%8A%B8.md)를, 맨 오른쪽 분대원은 [스톰볼터](%EC%8A%A4%ED%86%B0%20%EB%B3%BC%ED%84%B0.md)와 체인 피스트를, 나머지는 [스톰볼터](%EC%8A%A4%ED%86%B0%20%EB%B3%BC%ED%84%B0.md)와 파워 피스트를 장비하고 있다.

`\----`

  * `[1]` (당신이) 행한 대로 본다
  * `[2]` 비슷한 것으로 [vi](vi.md), [LaTeX](LaTeX.md)가 있다.
  * `[3]` 특히 [HTML](HTML.md)을 다루는 WYSIWYG에서 많이 벌어지는 문제이며, 이는 해당 홈페이지에 접속하는 [스마트폰](%EC%8A%A4%EB%A7%88%ED%8A%B8%ED%8F%B0.md)이나 [태블릿 컴퓨터](%ED%83%9C%EB%B8%94%EB%A6%BF%20%EC%BB%B4%ED%93%A8%ED%84%B0.md) 등의 모바일 사용자에게 치명적이다. 데이터 무제한이 아닌 이상 **요금 폭탄**의 위험을 안고 있으니... [웹표준](%EC%9B%B9%ED%91%9C%EC%A4%80.md) 바람이 불기 전인 [2000년대](2000%EB%85%84%EB%8C%80.md) 초기 시점까지의 홈페이지가 그렇다.
  * `[4]` 일반적으로 WYSIWYG라고 하면 이쪽을 가리킨다.

