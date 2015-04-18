![http://upload.wikimedia.org/wikipedia/commons/thumb/9/92/LaTeX_logo.svg
/100px-LaTeX_logo.svg.png](http://upload.wikimedia.org/wikipedia/commons/thumb
/9/92/LaTeX_logo.svg/100px-LaTeX_logo.svg.png)

[[PNG external image]](http://upload.wikimedia.org/wikipedia/commons/thumb/9/9
2/LaTeX_logo.svg/100px-LaTeX_logo.svg.png)

개발자

Lesile Lamport

플랫폼

Cross-platform (다중 플랫폼)

타입

Typesetting

라이센스

LaTeX Project Public License (LPPL)

홈페이지

<http://www.latex-project.org>

한국 LaTeX 사용자 그룹

<http://www.ktug.org/>

  
본격 공돌이 [워드](MS%20%EC%9B%8C%EB%93%9C.md). <del>라텍스</del>**"레이텍"**이라고 읽는다.
이렇게 읽는 이유는 LaTeX의 모체인 ![Wikipedia:](//rv.wkcdn.net/http://rigvedawiki.net/r1/i
mgs//interwiki/wikipedia-16.png)[TeX](http://ko.wikipedia.org/wiki/TeX)****의
X가 라틴 문자 X(엑스)가 아니라 그리스 문자 Χ(키, 카이)를 뜻하기 때문이다. 따라서 'LaTeX는', 'LaTeX를'이 아닌
'LaTeX은', 'LaTeX을'이 맞다.

## Contents

    

1. 개요 
2. 타입세팅(Typesetting) 시스템 
3. 예시 
4. BibTeX 
5. 설치법 
    

5.1. 윈도우즈

5.2. Mac OS X

5.3. 리눅스

6. 웹에서 사용하기 
7. 팁 

[[edit](http://rigvedawiki.net/r1/wiki.php/LaTeX?action=edit&section=1)]

## 1. 개요 ¶

LaTeX은 문서 작성 도구의 일종으로, 논문이나 출판물 등의 특수 형식 문서를 작성하는 데 쓰이는 시스템이다. LaTeX은
[TeX](TeX.md)의 확장성을 염두에 둔 개선판이다. [TeX](TeX.md)의 최초 개발자는 도널드 크누스로, 자신이
프로그래밍에 대한 책을 쓰려다 보니 적당한 조판 시스템이 없어 개발했다고 한다. 보통 이를 Typesetting(타입세팅) 시스템이라
부르는데 [MS 워드](MS%20%EC%9B%8C%EB%93%9C.md)처럼 [WYSIWYG](WYSIWYG.md)(What
You See Is What You Get)방식으로 문서를 작성하는 것과 반대로 마치 프로그래밍을 하듯 (혹은 마크업 랭귀지로 문서를
작성하듯이) 문서 작성을 하는 과정을 의미한다(WYSIWYM: What You See Is What You Mean). 쉽게 말하자면
[아래아 한글](%EC%95%84%EB%9E%98%EC%95%84%20%ED%95%9C%EA%B8%80.md)의 수식 입력 시스템으로
모든 문서를 작성한다고 생각하면 편하다(LaTeX에서 따왔으니 당연한 일). [리그베다위키](%EB%A6%AC%EA%B7%B8%EB%B2%A0%EB%8B%A4%20%EC%9C%84%ED%82%A4.md) 문서를 작성할 때
목차나 각주를 넣는 작업도 비슷하다 볼 수 있다.

  

본디 출발은 텍스트 위주의 문서를 작성하는 TeX이었으나, 여러 가지 기능들이 덧대어져 LaTeX으로 진화했으며, 결국에는 출판물을 작성할
수 있는 강력한 도구로 탄생하였다. 본디 1980년에 Lesile Lamport에 의해 작성되어 지금까지 내려오는 중이다. TeX의 접근법은
본래 아무리 간략화와 매크로화를 시킨다 하더라도 시각적 조판의 측면에는 근본적으로 불리함이 있었으나 작성되는 문서의 사용분야라는 특성에 잘
부합되고, 무엇보다 다른 방식으로는 영 번거로워지는 수식 편집 측면에서 강점이 있기 때문에 높게 평가되고 있다.

  

WYSIWYG 워드프로세서가 글을 보면서 입력하고 원하면 모양을 꾸미는 과정으로 작성을 진행하는 반면, LaTeX은 전체 글의 구조가 미리
정해진 특정 규격들에 맞추어 작성한 텍스트 문서에 글의 내용과 해당 서식을 나타내는 기호들을 쫙 짜맞춰서 프로그램에게 제출하면 그걸
프로그램이 뚝딱뚝딱 돌려서(...) 결과물을 뱉어 준다는 개념으로 진행된다. 마치 소스를 작성 후 컴파일러를 돌려서 실행 파일을 만드는
것처럼, 문서 소스를 만들고 컴파일러를 돌려서 문서(예전에는 DVI라는 자체 포맷 전자 문서였으나 요즘은 PDF가 대세다)를 만든다고
생각하면 된다.

  

따라서 근본에 두고 있는 개념부터가 대단히 학계 지향적이고 사용자의 지적 구성력에 상당 부분이 전가되는 부분이 많아 이러한 철학에 생소한
사람에게 설명할 경우 그럼 이게 금형기계지 워드냐(...) 하는 반응이 돌아오기도 한다. 실제로 흔히 생각하는 워드 프로세서는 아닌 것이,
워드프로세서에게서 WYSIWYG 기능을 완전히 박탈하고 프로그래머적 마인드로 자동화를 극한까지 밀어붙여 '조판'만 남겼기 때문. 워드나
한글에만 익숙하던 컴공과 학생이 처음 접하는 경우, 숙제하면서 디버깅했는데 보고서 쓰면서 디버깅하는
[멘붕](%EB%A9%98%EB%B6%95.md) 상황을 경험하게 된다. 반면, 잘 만들어진 템플릿을 이용하여 작성자는 내용과 구조에만
신경을 쓰고, 이를 편집자(즉 LaTeX)가 예쁘게 고친다는 협업 체제로도 볼 수 있다. 사용자가 입맛대로 세세한 부분을 변경시키며
사용하려고 하지 않는다면, 명령어 30개 수준으로 단시간에 아래아 한글이나 MS워드보다도 미려한 문서를 얻을 수 있다.  
또한, LaTeX 안에 beamer class를 이용하여 프리젠테이션 파일도 만들 수 있다. LaTeX에 익숙해진 공돌이들은 막상 PPT나
word를 쓰려고 하면 불편해 한다. (인간의 적응력은 놀랍도다.) 심지어 어떤 공돌이는 LaTeX 안에서 본인이 원하는 그림을 그리기도
한다.  
그림의 예시는 <http://en.wikibooks.org/wiki/LaTeX/Picture> 에 들어가보면 일부 예시를 볼 수 있다.
(이건 애교로...)

  

주로 학계, 특히 수식이 많이 필요한 [자연과학](%EC%9E%90%EC%97%B0%EA%B3%BC%ED%95%99.md),
[공학](%EA%B3%B5%ED%95%99.md),
[사회과학](%EC%82%AC%ED%9A%8C%EA%B3%BC%ED%95%99.md) 계열에서 많이 사용되며`[1]` 기능이 막강하기
때문에 출판물 퀄리티의 문서를 작성하는 데 사용할 수 있기에 개인적인 퍼블리셔들이나 데스크 탑 퍼블리싱(개인 컴퓨터로 출판물을 만드는
행위)등에도 많이 사용 된다. 이렇게 각광받는 이유는 페이지 넘버는 물론, [각주](%EA%B0%81%EC%A3%BC.md), 미주,
[목차](%EB%AA%A9%EC%B0%A8.md), 레퍼런스, 페이지 레이아웃, 테이블, 그림 삽입 등 출판물 등급에 필요한
필수요소들을 손쉽게(라고 하지만 WYSIWYG 워드 프로세서들만 사용하던 사람들이 익히기에는 복잡하다.) 구현할 수 있기 때문이다. 특히
순서, 서식, 내용이 극도로 정형적인 학계 문서는 규격에 꼭 맞춰 틀에 찍듯이 만들어야 하기 때문에, 학계의 사랑을 받을 수밖에 없었으며,
한때는 사실상 표준이었다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/LaTeX?action=edit&section=2)]

## 2. 타입세팅(Typesetting) 시스템 ¶

LaTeX은 기본적으로 작가들이 외형적인 요소(예를 들어 페이지 수 폰트, 위치 등등 지정하기)를 배제하고 내용물(텍스트)에 집중할 수
있도록 하기 위해 작성되었다. LaTeX 문서를 작성할 때, <del>리그베다 위키와 마찬가지로</del> 챕터, 섹션, 테이블, 이미지
등의 항목들을 의미하는 명령어들을 일단 배치하고 그 밑에 내용을 채우는 방식으로 작성하는데, 일단 이렇게 작성해 두면 LaTeX 문서는
텍스트 파일에 지나지 않는다`[2]`. 이를 LaTeX 타입세팅 시스템으로 읽어들이면 내가 원하는 형식의 문서 파일로 만들어준다. 현재는
학회에서 [PDF](PDF.md)형식을 많이 사용하며, PS(PostScript)방식의 문서도 사용된다. 그 외에도 그림 파일로
만들거나 CSS를 이용한 HTML문서 또한 작성할 수 있다.

  

또한, 여러 가지 매크로 기능이 있어서, 복잡한 표, 그림 배치 등의 작업을 조금 더 수월하게 할 수 있도록 도와준다. 이 매크로 기능 중에
가장 꽃이 되는 것은 수식 편집 기능으로, 숙련되면 타 WSYWIG 방식의 프로그램들 보다 훨씬 빠르게 작업할 수 있다.
[한글과컴퓨터](%ED%95%9C%EA%B8%80%EA%B3%BC%EC%BB%B4%ED%93%A8%ED%84%B0.md)사의 [한글시리즈](%EC%95%84%EB%9E%98%EC%95%84%20%ED%95%9C%EA%B8%80.md)에 있는 수식을 다뤄 본
사람이라면 LaTeX의 수식 명령 체계가 매우 유사함을 알 수 있다. 이는 한컴사의 수식 명령체계가 LaTeX의 수식 명령 체계에서 유래했기
때문이다. `[3]`

  

[[edit](http://rigvedawiki.net/r1/wiki.php/LaTeX?action=edit&section=3)]

## 3. 예시 ¶

다음과 같은 <del>외계어</del>텍스트를 타입세팅 과정을 통하면...  

    
    
    \documentclass{{{[12pt]}}}{article}\usepackage{amsmath}\title{\LaTeX}\date{}\begin{document}  \maketitle  \LaTeX{} is a document preparation system for the \TeX{}  typesetting program. It offers programmable desktop publishing  features and extensive facilities for automating most aspects of  typesetting and desktop publishing, including numbering and  cross-referencing, tables and figures, page layout, bibliographies,  and much more. \LaTeX{} was originally written in 1984 by Leslie  Lamport and has become the dominant method for using \TeX; few  people write in plain \TeX{} anymore. The current version  is  \LaTeXe.   % This is a comment; it will not be shown in the final output.  % The following shows a little of the typesetting power of LaTeX:  \begin{align}    E &= mc^2                              \\    m &= \frac{m_0}{\sqrt{1-\frac{v^2}{c^2}‭}}  \end{align}\end{document}

  

다음과 같은 미려한 문서가 나온다.  

![LaTeX_Output.png](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/LaTeX_Output.
png)

[PNG image (43.52 KB)]

  

[[edit](http://rigvedawiki.net/r1/wiki.php/LaTeX?action=edit&section=4)]

## 4. BibTeX ¶

LaTeX의 자매품 격인 소프트웨어로, 주로 레퍼런스를 학회나 출판물 형식에 알맞게 출력해주는 역할을 담당한다. Microsoft Word
같은 WYSIWYG 프로그램을 사용하다 보면 레퍼런스를 언급할 때 일일히 해당 학회 형식에 맞도록 다 작성해야 하는 경우가 존재하는데,
BibTeX을 사용하면 한 번에 내가 원하는 스타일로 만들어 주는 기능이 있으며, 본문 내용에서 언급되었다면 자동으로 언급된 위치와 해당
참고 문헌 항목을 링크시켜 준다. 사실 MS Word 도 EndNote 등의 상용 프로그램과 함께 사용하면 비슷하게 사용할 수 있으나,
BibTeX만큼 서식을 많이 가지고 있지는 않고, 각종 학회도 자신들만의 서식을 주로 BibTeX 형식으로 배포한다.

  

LaTeX과 뗄래야 뗄 수 없는 관계라, 일단 작동하려면 LaTeX 타입세팅 프로그램이 만들어낸 .aux 파일이 필요하다. 서식 파일인
.bst 파일은 학회나 출판사마다 특유의 포맷으로 제공된다. 마지막으로 참고 문헌 목록은 .bib 파일에 저장되며, 앞의 두 파일들을
확보하고 BibTeX을 돌려 주면 .bbl 파일이 생성되며 LaTeX과 비로소 연결되어 문서에 참고 문헌 목록이 들어가게 된다. 참고 문헌은
일반적인 논문, 책은 물론, 컨퍼런스, 매뉴얼 타입의 문서, 학위 논문, 웹 페이지 등 다양한 종류를 지정해줄 수 있다. 예를 들어 책
형식의 참고 문헌을 지정하려면 다음과 같은 <del>외계어</del>명령어를 .bib 파일에 추가하면 된다.

  

@Book{abramowitz+stegun,

> author = "Milton {Abramowitz} and Irene A. {Stegun}",  
title = "Handbook of Mathematical Functions with  

>

>> Formulas, Graphs, and Mathematical Tables",

>

> publisher = "Dover",  
year = 1964,  
address = "New York",  
edition = "ninth Dover printing, tenth GPO printing"

}

  
현존하는 거의 모든 학회 사이트가 .bib 파일 형식으로 참고 문헌을 제공하고 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/LaTeX?action=edit&section=5)]

## 5. 설치법 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/LaTeX?action=edit&section=6)]

### 5.1. 윈도우즈 ¶

한국 사용자라면 위에 명기된 [KTUG](http://www.ktug.org) 사이트에서 설치 파일을 받으면 LaTeX 타입세팅 프로그램은
물론, .tex 편집 프로그램`[4]`까지 설치해 준다. 본디 TeX은 2바이트 문자를 타입세팅할 수 없는지라 한글 관련 애드온을 따로
설치해야 하는데, 이 패키지에는 모든 게 들어 있다. 최근에는 유니코드 기반으로 컴퓨터에서 설치된 트루타입 혹은 오픈타입 폰트를 자유롭게 쓸
수 있는 XeTeX 엔진이 대세가 되면서 한글 쓰기도 한층 편해졌다. XeTeX 또는 XeLaTeX을 쓴다면 한글 사용에 거의 불편을 느끼지
않고 쓸 수 있다. <del>LaTeX 자체가 쓰기가 지랄맞게 불편해서 그렇지</del>

  

인스톨러를 다운 받고 싶다면 [여기](http://www.ktug.org/xe/index.php?mid=install)로 가 보자.

  

윈도우즈에서는 TeXnicCenter라는 편집 프로그램이 가장 인기가 많다. 유니코드가 안된다는 커다란 단점이 있었는데, 버전 2부터는
지원한다고 한다. (이는, 작성자의 개인 의견인 듯 하다. 실제로 KTUG에 올라오는 글을 보면 많은 질문이 WinEDT 의 구형버젼을
가지고, 한글이 안된다는 하소연이다. 그러나, 아무도 유료 사용자가 아닌 듯 한 것이 함정이다.) <del>참고로 이 항목 원작성자는
[Emacs](Emacs.md)윈도우 버젼 씁니다!!</del>

  

[[edit](http://rigvedawiki.net/r1/wiki.php/LaTeX?action=edit&section=7)]

### 5.2. Mac OS X ¶

[MacTeX](https://www.tug.org/mactex)이라는 패키지가 나와 있어서 설치가 간단하다. 용량은 크지만 타입세팅 패키지
및 TeXShop, TeXWorks 등의 LaTeX 편집기 <del>vim 말고 편집기가 존재하긴 하나요</del> 등이 올인원으로 들어
있어 그냥 이거만 깔면 된다. 예전에는 한글 입력을 위해 ko.TeX을 받아 설치하는 등 번거로운 작업이 있었으나 지금은 모두 포함되어
있으므로 고민할 필요가 없다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/LaTeX?action=edit&section=8)]

### 5.3. 리눅스 ¶

배포판마다 설치법이 다양한데, 가장 많이 사용되는 [우분투](%EC%9A%B0%EB%B6%84%ED%88%AC.md)리눅스의 경우 매우
간단하다. 역시 타입세팅 패키지를 받기 위해서는 콘솔을 열고

  

sudo apt-get install texlive-full

  
수동으로 설치하고 싶다면 [여기](http://www.tug.org/texlive)에서 Unix용 TeXLive 인스톨러를 다운받은 후
압축을 풀고, 인스톨러 스크립트를 실행해 주면 정신 없이 (대략 1기가가 넘는다) 패키지를 다운받으며 설치를 끝낸다.

  

타입세팅 환경으로는 <del>익숙했던</del> [Emacs](Emacs.md)나 [vim](vim.md)을 사용해도 되고,
[TeXWorks](http://www.tug.org/texworks/)나 Kile 등이 제법 유용하다. 전문적으로는 사실 Emacs의
Auctex 모드가 가장 유명하다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/LaTeX?action=edit&section=9)]

## 6. 웹에서 사용하기 ¶

굳이 컴퓨터에 설치하지 않고도 LaTeX 사용에는 지장이 없다. 웹에서 LaTeX 편집 및 컴파일을 지원하는 사이트가 있으므로 설치하기
번거롭다면 [ShareLaTeX](https://www.sharelatex.com)이나
[Overleaf](https://www.overleaf.com) 등을 사용하면 된다. 심지어 ShareLaTeX은 한글 문서도 만들 수
있다. 표준적인 패키지는 모두 갖추고 있고, 다른 사람과 공유하거나 협업하는 기능도 들어 있으므로, 아주 높은 보안성을 요구하는 문서가
아니라면 오히려 사용하기 편할 수 있다. 물론 사용 인구가 적은 패키지가 필요하다든가, 혹은 자신의 컴퓨터에서 쓰는 에디터의 세팅 등은
유지가 되지 않으므로 사람에 따라 다를 수 있지만, 반면 LaTeX이 설치되어 있지 않은 기기, 특히 타블렛이나 휴대폰 등에서 작업하기는
오히려 편하다.  

[[edit](http://rigvedawiki.net/r1/wiki.php/LaTeX?action=edit&section=10)]

## 7. 팁 ¶

[여기](http://detexify.kirelabs.org/symbols.html/)에 가면 수학기호나 여러가지 기호를 그리면 그것에 대한
코드를 나타내어 준다. 처음 LaTeX을 접하는 사람들에게는 좋은 사이트가 될 것이다.

  

`\----`

  * `[1]` 이공계뿐 아니라 사회과학 계열에서도 LaTeX을 많이 사용한다. 특히 [정치학](%EC%A0%95%EC%B9%98%ED%95%99.md), [경제학](%EA%B2%BD%EC%A0%9C%ED%95%99.md), [사회학](%EC%82%AC%ED%9A%8C%ED%95%99.md), [경영학](%EA%B2%BD%EC%98%81%ED%95%99.md) 등의 분야에서 합리적 선택이론(rational choice theory)이 기본이 되는 formal/game theory를 방법론으로 삼을 경우 수식 때문에 <del>그리고 거지같은 [MS 워드](MS%20%EC%9B%8C%EB%93%9C.md)의 수식편집 기능 때문에</del> LaTeX을 많이 쓰게 된다.
  * `[2]` 보통 .tex 확장자를 많이 이용한다.
  * `[3]` 한컴에서 수식입력기를 만든 사람도 TeX을 참조하였다고 인터뷰를 한 기사도 있었던 듯하다. 그러나, TeX의 전문가들에게 물어보면 한컴의 수식입력기의 입력체계는 TeX을 참조하였지만, 좀더 많은 부분을 영향받은 다른 것이 있다고도 한다.
  * `[4]` 사실 노트패드에서 해도 되지만 귀찮다?

