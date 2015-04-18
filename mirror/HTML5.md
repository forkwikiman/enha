  * 상위 항목: [HTML](HTML.md)  

## Contents

    

1. 개요 
2. 설명 
3. 변경사항 
    

3.1. [선언문](DTD.md)

3.2. 시맨틱 태그

    

3.2.1. 레이아웃 태그

    

3.2.1.1. 예시

3.2.2. 멀티미디어 태그

3.2.3. 폼 관련

3.2.4. 기타 태그

3.2.5. 용도가 바뀐 태그

3.2.6. 사용 불가 태그

4. 기타 

[[edit](http://rigvedawiki.net/r1/wiki.php/HTML5?action=edit&section=1)]

## 1. 개요 ¶

[2008년](2008%EB%85%84.md) [1월](1%EC%9B%94.md)부터 논의가 시작된 버전으로 2014년 10월
28일 확정된 최신 표준이다. XHTML에서 다시 HTML로 회귀하게 되었다. 따라서 HTML5는 XHTML의 상위 버전이 아니라,
HTML4.01의 상위 버전이다. [플래시](%ED%94%8C%EB%9E%98%EC%8B%9C.md)나
[실버라이트](%EC%8B%A4%EB%B2%84%EB%9D%BC%EC%9D%B4%ED%8A%B8.md) 등의
[플러그인](%ED%94%8C%EB%9F%AC%EA%B7%B8%EC%9D%B8.md)을 기반으로 하는
[인터넷](%EC%9D%B8%ED%84%B0%EB%84%B7.md) [앱](%EC%95%B1.md)에 대한 필요성을 줄이는 것에
초점을 맞추고 있다.

  

2014년 10월 28일, HTML5의 최종 권고안이 확정되어 최신 표준으로 지정되었다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/HTML5?action=edit&section=2)]

## 2. 설명 ¶

지지리도 안 지켜지던 [웹표준](%EC%9B%B9%ED%91%9C%EC%A4%80.md)에 새로운 바람을 불게 했으며, 단순히
'코더'라고 불리던 HTML 개발자들의 이미지를 바꾸어 줄 만큼 좋은 녀석이다.

  

이전에는 [자바스크립트](%EC%9E%90%EB%B0%94%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8.md)를
사용해서 엄청나게 긴 코드를 써야만 했던걸 간단한 단어 몇개로 구현해낼 수 있고, 불필요하게 길게 적어야했던 이전 버전에서 꼭 필요한 부분만
남기도록 개선되었다.

  

반면, 세간에 성능이 과장되게 알려진 감이 있는데, 일반적인 인식과는 달리
[액티브X](%EC%95%A1%ED%8B%B0%EB%B8%8CX.md),
[플래시](%EC%96%B4%EB%8F%84%EB%B9%84%20%ED%94%8C%EB%9E%98%EC%8B%9C.md),
[실버라이트](%EC%8B%A4%EB%B2%84%EB%9D%BC%EC%9D%B4%ED%8A%B8.md),
[자바](%EC%9E%90%EB%B0%94.md),
[자바스크립트](%EC%9E%90%EB%B0%94%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8.md)의 **극히
일부분**밖에 대체하지 못한다. 저 "일부분"이라고 하는 게 <video>태그 같은 건데, 그나마도 영상을 표시만 하지 저기다가 뭔가 컨트롤
같은 걸 좀 붙이려고 하면 다시 자바스크립트가 동원되어야 한다.`[1]` 애초에 HTML5의 기능이라고 알려진 것 중 상당수가 자바스크립트를
끌어와서 쓰는 것이다. HTML5의 목적은 저것들을 완전히 대체하는 것이 아니라, 기술의 발전에 표준이 못 따라가다보니 발생한 각종 비표준
코드에서 사용하던 기능들을 수용할 수 있도록 그 판을 넓혀 놓은 것이다. 단순한 경쟁자라기보단, 상호 보완적인 관계라고 보는 것이 맞다.

  

[인터넷 익스플로러](%EC%9D%B8%ED%84%B0%EB%84%B7%20%EC%9D%B5%EC%8A%A4%ED%94%8C%EB%A1%9C%EB%9F%AC.md)는 9부터 지원한다. 8 이하를 지원하려면 html5shiv.js 라는 자바스크립트를 이용하면 된다. 단 이
경우 자바스크립트를 사용하기에 페이지 렌더링 속도가 느려진다는 단점이 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/HTML5?action=edit&section=3)]

## 3. 변경사항 ¶

HTML5로 접어들어 HTML이 다양한 기능을 포함하면서 새롭게 추가된 태그들과 의미가 변경된 태그들이 여럿 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/HTML5?action=edit&section=4)]

### 3.1. [선언문](DTD.md) ¶

이전 버전의 HTML과 XHTML이 유효성 검사를 위한 선언문이 쓸데없이 길었던 반면, HTML5에서는 간단하게 몇 자만 적으면 된다.

  

    
    
    <!DOCTYPE html>

  

[[edit](http://rigvedawiki.net/r1/wiki.php/HTML5?action=edit&section=5)]

### 3.2. 시맨틱 태그 ¶

기존 웹 표준에서는 <div> 태그를 잔뜩 사용하여 화면을 분할, 여러가지 레이아웃을 만들어냈지만, HTML5에서는 [시맨틱웹](%EC%8B%9C%EB%A7%A8%ED%8B%B1%20%EC%9B%B9.md)을 중요시하여 여러가지 태그를 새롭게 만들었다.
이러한 태그들을 **시맨틱 태그**라고 한다.

  

사용방법은 기존의 <div> 태그와 차이가 없으나, 시맨틱 태그를 사용한 레이아웃은 컴퓨터가 읽어낼 수 있다. 이게 무슨 말이냐면, 검색
사이트에서 어디가 내용인지를 알 수 있어서 검색 노출을 용이하게하고, **궁극적으로 [눈으로 페이지를 볼 수 없는사람들](%EC%8B%9C%EA%B0%81%EC%9E%A5%EC%95%A0%EC%9D%B8.md)에게 사이트의 어디가 본문인지 아닌지
알려줄 수 있다는 장점이 있다.**

  

기존 태그는 일부분을 제외하고는 HTML 4.01에서 사용되던 태그가 거의 그대로 사용된다. 원래 HTML을 표준에 맞게 사용했다면 큰
어려움 없이 HTML5에도 적응할 수 있다.

[[edit](http://rigvedawiki.net/r1/wiki.php/HTML5?action=edit&section=6)]

#### 3.2.1. 레이아웃 태그 ¶

  * <header>  
일반적으로 페이지나 해당 섹션의 가장 윗부분에 위치한다. 페이지 맨 위에 쓸 때는 사이트의 제목이 보통 들어가며, 선택적으로 상단바나 검색창
등이 안에 들어갈 수 있다. <head> 태그랑 헷갈리면 매우 곤란하다. section이나 article, aside 등으로 묶어놓은 섹션
안의 헤더 용도로 사용해도 된다. 이건 아래 footer 태그도 마찬가지다.

  * <nav>  
내비게이션(**nav**igation)의 약자로, 일반적으로 상단바 등 사이트를 안내하는 요소에 사용된다. 보통은 안에 <ul>을 넣어 목록
형태로 사용한다.

  * <article>  
웹 페이지의 내용에 사용하는 태그이다. 문서나 페이지, 사이트에서 독립적으로 배포 혹은 재사용(예를 들어 투고 같은)할 수 있는 섹션에
사용한다.

  * <section>  
웹 페이지의 섹션에 사용하는 태그이다. 웹 페이지를 의미적으로 각각의 파트로 구분하기 위해 쓰는 태그이다. 이 태그를 사용하면 검색엔진이
긁어가지 않는다는 이야기가 있는데 루머다. [HTML5 표준
문서](http://html5.clearboth.org/sections.html)에 보면 "요소의 내용을 배포(syndicate)해도 이치에
맞다면 section 요소 대신 article 요소를 사용하기를 권합니다."라는 부분이 있는데, 이 부분의 해석이 잘못 퍼진 것으로
추정된다.

  * <aside>  
본문의 주요 부분을 표시하고 남은 부분을 설명하는 태그이다. 특별한 일이 아니면 사이드바나 광고창 등 중요하지 않은 부분에 사용된다.

  * <footer>  
일반적으로 페이지나 해당 파트의 가장 아랫부분에 위치한다. 페이지 맨 아래에 쓸 때는 사이트의
[라이선스](%EB%9D%BC%EC%9D%B4%EC%84%A0%EC%8A%A4.md), 주소, 연락처 등을 넣는다.  

[[edit](http://rigvedawiki.net/r1/wiki.php/HTML5?action=edit&section=7)]

##### 3.2.1.1. 예시 ¶

레이아웃 태그를 사용한 HTML5 마크업의 기초 뼈대는 다음과 같다.

  

    
    
    <!DOCTYPE html><html lang="ko"><head><meta charset="utf-8"><title>[페이지 제목]</title></head><body><header><h1>[사이트 제목]</h1><h2>[사이트 부제목]</h2><nav><ul><li>[메뉴1]</li><li>[메뉴2]</li><li>[메뉴3]</li></ul></nav></header><section><article><p>[본문 내용]</p></article></section><aside>[사이드바 내용]</aside><footer><address>[주소 내용]</address></footer></body></html>

[[edit](http://rigvedawiki.net/r1/wiki.php/HTML5?action=edit&section=8)]

#### 3.2.2. 멀티미디어 태그 ¶

  * <audio>  
음성, 음악 파일 등을 재생할 수 있는 태그. [웹브라우저](%EC%9B%B9%20%EB%B8%8C%EB%9D%BC%EC%9A%B0%EC%A0%80.md)마다 지원하는 확장자가
달라`[2]` 멀티브라우저 지원을 위해서는 <source> 태그를 안에 넣어 두가지 이상의 확장자를 가진 음악 파일을 넣어야 한다. 가장
많이 사용하는 조합은 [mp3](MP3.md)+[ogg](OGG.md)

  * <video>  
영상 파일을 재생할 수 있는 태그. 사실상 HTML5에서 가장 주목받는 태그이다. 별다른
[플러그인](%ED%94%8C%EB%9F%AC%EA%B7%B8%EC%9D%B8.md) 없이도 자체 재생이 가능하다는 점이 가장 큰
장점이다. <audio> 태그와 마찬가지로 <source> 태그를 넣어 [mp4](MP4.md)+[ogv](OGG.md)의
조합으로 짜주면 거의 대부분의 브라우저를 지원한다.

  * <canvas>  
스크립트를 이용하여 그래픽을 표현하는 태그이다. 일반적으로는
[자바스크립트](%EC%9E%90%EB%B0%94%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8.md)를 많이
사용하며, 응용하면 웹에서 [게임](%EA%B2%8C%EC%9E%84.md) [앱](%EC%95%B1.md), 3D 엔진 등을
돌리는 다양한 응용이 가능하다.  

[[edit](http://rigvedawiki.net/r1/wiki.php/HTML5?action=edit&section=9)]

#### 3.2.3. 폼 관련 ¶

  * <output>  
계산의 결과값을 전송하는 데에 쓰인다.

  * <input> 내 요소 - date, datetime, time, color, range 등  
자바스크립트를 통해서만 구현됐던 기능이 내장되었다. 하지만 현 시점에서는 [오페라](%EC%98%A4%ED%8E%98%EB%9D%BC%28%EC%9B%B9%20%EB%B8%8C%EB%9D%BC%EC%9A%B0%EC%A0%80%29.md)만 완전 지원한다.

  * <datalist>  
<input>에 들어갈 값을 미리 정의하는 태그이다.

  * <keygen>  
암호화용 키쌍을 생성하는 태그이다. 서버에는 공개 키가 전송되고, 개인 키는 클라이언트에 저장된다.  

[[edit](http://rigvedawiki.net/r1/wiki.php/HTML5?action=edit&section=10)]

#### 3.2.4. 기타 태그 ¶

  * <menu>  
툴바, 팝업 메뉴를 넣을 때 쓴다.

  * <menuitem>  
툴바, 팝업 메뉴의 각 항목을 정의한다.

  * <details>
  * <embed>  
외부 애플리케이션이나 플러그인을 삽입할 때 쓰는 태그이다. 대표적으로 [어도비플래시](%EC%96%B4%EB%8F%84%EB%B9%84%20%ED%94%8C%EB%9E%98%EC%8B%9C.md)를 웹페이지에
삽입할 때 이걸 쓴다. 원래 HTML에 없던 비표준 태그였는데 거의 모든 브라우저가 이 태그를 지원한데다, 기존에 표준으로 존재하던
object 태그보다 사용방법이 간편해서 사실상 표준처럼 쓰이던 태그였고 결국 HTML5 표준에 포함되었다.

  * <object>  
외부 문서, 매체, 플러그인 등을 웹페이지에 삽입할 때 쓰는 태그이다.

  * <figure>  
그림, 도표, 다이어그램 등의 글의 이해를 돕기 위한 내용들을 나타내는 태그이다.

  * <figcaption>  
<figure> 태그 안에 사용되는 태그로, <figure> 태그 안에 있는 내용의 설명을 적는 태그이다.

  * <em>  
강조를 나타내는 엠퍼시스(**em**phasis)의 줄임말이다. HTML5에서는 <b>와 <strong> 사이의 강조를 나타낼때 사용한다.

  * <hr>  
원래 단순한 가로줄을 나타내는 태그였으나, 페이지의 주제가 바뀔 때 내용을 분리시키는 의미가 HTML5에서 추가되었다.  

[[edit](http://rigvedawiki.net/r1/wiki.php/HTML5?action=edit&section=11)]

#### 3.2.5. 용도가 바뀐 태그 ¶

  * <s>  
더이상 옳지 않은 내용을 나타내는 데에 쓴다.

  * <u>  
양식상 일반적인 텍스트보다 돋보여야 할때 쓴다. 예를 들어 철자가 틀린 단어나, 중국어의 고유 명사 등이 있다.

  * <i>  
어떠한 이유로 일반적인 텍스트보다 돋보여야 할때 쓴다. 예를 들어 전문 용어, 외국어의 구절 등이 있다.  
더 적절한 시맨틱 태그가 있을 경우 그쪽을 쓴다.  

[[edit](http://rigvedawiki.net/r1/wiki.php/HTML5?action=edit&section=12)]

#### 3.2.6. 사용 불가 태그 ¶

대개 [시맨틱 웹](%EC%8B%9C%EB%A7%A8%ED%8B%B1%20%EC%9B%B9.md)에서 사용을 지양하는 태그라든가, 특정
브라우저<del>[IE](IE.md)라든가 IE라든가 IE라든가</del>에서만 작동하는 태그가 속한다.

  

  * <font> → [CSS](CSS.md)가 있기 때문에 폐기되었다.
  * <applet> → 자바 애플릿을 넣을 때 쓰는 태그였다. <object>, <embed>로 대체한다.
  * <strike> → <del>, <s>로 대체되었다.
  * <frame> → <iframe>로 대체되었다. <frame>과 함께 쓰이던 <frameset>, <noframes> 태그 역시 함께 사용 불가 태그가 되었다.
  * <acronym> → <abbr>로 대체되었다.  

[[edit](http://rigvedawiki.net/r1/wiki.php/HTML5?action=edit&section=13)]

## 4. 기타 ¶

[2012년](2012%EB%85%84.md) [12월 17일](12%EC%9B%94%2017%EC%9D%BC.md)자로 권고
후보안(Candidate Recommendation)으로 등록되어 표준 지정을 기다리고있다. 표준화 일정에 따르면
[2014년](2014%EB%85%84.md) 4분기까지는 표준을 제정하고, 처리하기 힘든 문제들은 HTML5.1 이상의 버전에서 다룰
예정이었고,[#](http://dev.w3.org/html5/decision-policy/html5-2014-plan.html)  
결국 2014년 10월 28일 최종 권고안이 확정, HTML의 최신 표준으로 지정되었다.

`\----`

  * `[1]` 그냥 태그만 쓰면 브라우저에서 <del>뭔가 안쓰러운지</del> 기본적인 컨트롤을 제공해주기는 한다.
  * `[2]` 이는 이런저런 [어른의 사정](%EC%96%B4%EB%A5%B8%EC%9D%98%20%EC%82%AC%EC%A0%95.md) 때문에 빚어진 현상. video 태그는 더 심하다.

