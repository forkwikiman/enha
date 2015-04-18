Perl  

## Contents

    

1. 개요 및 소개 
2. 특장점 
3. 단점 
4. Perl 6 
5. 기타 
6. 정규표현식 
7. 관련 사이트 

[[edit](http://rigvedawiki.net/r1/wiki.php/Perl?action=edit&section=1)]

## 1. 개요 및 소개 ¶

[프로그래밍언어](%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20%EC%96%B8%EC%96%B4.md)의
일종.

  

1987년 발표되어 2015년 현재 28년 된 언어이다.

  

만든 이는 래리 월(Larry Wall).`[1]`

  

이름 자체는 Practical Extraction and Reporting Language(실용적인 데이터 취득 및 리포트 작성 언어)의
약자라고 한다. 본래는 붙일만한 이름을 찾을 수 없었던 제작자가 성서에서 아무 단어나 따와서 붙인 이름.
Pearl([진주](%EC%A7%84%EC%A3%BC.md))라는 이름을 붙이고 싶어했지만, 이미 그런 이름을 가진 프로그래밍 언어가
있었기에 철자만 살짝 바꿔서 Perl이라는 이름을 붙였다. 약자는 나중에 가져다 붙인 것. 그냥 진주랑 철자가 비슷한게 아니다!

  

철학은 TIMTOWTDI(There is more than one way to do it, 무언가를 하는 방법은 (언제나)하나보다
많다).`[2]`

  

유닉스쪽에서는 디폴트 컴파일 언어인 C 와 함께 디폴트 스크립팅 언어로 베이스 시스템에 들어가있는 경우가 많다<del>CPerl 발음이 좀
뭐같다.`[3]`</del>.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Perl?action=edit&section=2)]

## 2. 특장점 ¶

[C](C%28%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20%EC%96%B8%EC%96%B4%29.md)와 비슷한 구문에 sed, AWK, 셸 스크립트 등과 같은 여러 유명한 유닉스 기능을 포함하고 있으며 언어 자체의 자유도가 높고
표현력도 뛰어나며 코딩도 쉽다.

  

특히 텍스트를 처리하는 기능이 최강점으로 꼽힌다. 프로그래밍을 좀 해본 사람이라면 텍스트를 다루는 코딩이 얼마나 번거로운지 알고 있을
것이다. Perl은 텍스트를 처리하는 기능이나 문자열의 일치 여부 검색 및 치환등을 매우 짧은 코드로 처리 가능하고 성능도 매우 뛰어나다.
보간 처리에 있어서는 스크립트 언어 뿐만 아니라 전체 언어 중에서 성능, 기능상 탁월하다.
[#](http://raid6.com.au/~onlyjob/posts/arena/)

  

GUI, 웹프로그래밍, 시스템 관리, 그 밖에 간단한 작업을 하는 스크립트 작성하는 데에 넓게 이용되며 생물정보학 쪽에서도 광범위하게
이용되는 편. 특히 다른 언어에 비해 정규표현식과 함께 문자열을 다루는 방법이 다양하고 강력하게 제공되고 있으므로, 언어학쪽에서 많이 다루는
언어이기도 하다. 특히 웹프로그래밍에서는 거의 필수적으로 쓰인다고 보면 된다.

  

인터프리터 언어다 보니 코드를 수정할 때마다 컴파일을 반복할 필요가 없어 프로그램 구현이나 디버깅이 쉬운 편이기도 하다. 자유 및 무료
소프트웨어여서 비용 면에서도 굉장한 장점을 지니고 있는 편. 각종 유닉스 시스템이나 맥 OS X에 기본으로 탑재되어 있다.

  

한편으로는 미칠 듯한 축약이 가능하다는 점에서 "Perl은 Pathologically Eclectic Rubbish Lister(병적
절충주의 잡동사니 출력장치)의 약자."라는 농담도 가끔 들을 수 있다.`[4]`

  

또한 [CPAN](http://www.cpan.org/)이라고 펄로 제작된 소프트웨어들을 모아놓은 자료실이 있다. 이 CPAN의 방대함은 펄
관련 문제 해결의 보고이자 펄의 자랑거리이다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Perl?action=edit&section=3)]

## 3. 단점 ¶

하지만 단점도 없는 건 아니다. 인터프리터 언어라는 태생적 한계에 의해 처리 속도가 C처리 속도보다 조금 느리다. 요즘 컴퓨터들은 성능이
뛰어나 웬만한 프로그램들이야 그 차이를 체감할 일은 별로 없겠지만, 그래도 단순 계산 반복 면에서는 오래 하다 보면 꽤 큰 차이가 되는
경우가 있다. 그러나, 사실 인터프리터 언어와 컴파일 언어를 성능으로 단순비교하는것은 의미없는 일이다. 이 둘은 보통 용도가 확연히 달라,
경쟁하는 언어라 보기 힘들기때문이다. 퍼포먼스가 중요치 않은, 스크립팅 언어로 간단히 끝낼 작업에 C 와 같은 언어를 끌어쓰는것도
웃긴일이며, 반대로 퍼포먼스가 최우선순위인 부분에 스크립팅 언어를 사용하는 경우도 당연히 찾아보기 힘들다. 즉, 오늘날 언어 1개로 모든것을
처리하는 경우는 거의 없다 볼 수 있다. 게다가 특정 환경/목적에서 펄에 더 빠른 수행 시간을 내는 경우도 있으며, 언어 자체와 하드웨어의
발전으로 인해 수행시간의 차이도 점점 줄어들고 있다. [Perl, Python, Ruby, PHP, C, C++, Lua, tcl,
javascript, Java 성능비교](http://aero2blog.blogspot.com/2011/12/perl-python-ruby-
php-c-c-lua-tcl.html) 참조

  

일부 부분에서 기교적인 사용을 요구하는 것도 문제. 함수와 객체의 선언이 가장 기교적인 부분인데 Moose를 사용하지 않는 경우는 직관적으로
이해하기 어려운 문제가 있다. 지연연산과 제너레이터, 레퍼런스를 사용하는 부분에 있어서는 경쟁 언어들에 비해 조금 어려운 감이 있다.

  

특히 가독성이 낮은 것은 가장 큰 단점으로 꼽힌다. Write Once, Read Never 언어 중의 하나라고도 한다. 펄로 짜놓으면
일자리가 보장된다는 농담반 진담반도 있다.`[5]` 자유도가 높기때문에 아무래도 돌아가는것만 중시한다거나 초심자들의 경우 더러운 코드를
만들기 쉬운것이 단점. 그러나, 숙련된 프로그래머들만으로 팀을 이룬 경우, 프로젝트가 꽤 커져도 그다지 큰 문제는 없다는 이야기도 있긴
하다. 어쨌든 낮은 가독성과 기교적 사용에 대한 반성(?)으로 modern Perl programming 을 제시하고 있다. <del>서예로
치면 [초서](%EC%B4%88%EC%84%9C.md)</del>

  

심지어 이런 연구도 있다. 초보자에게 프로그래밍 문법을 가르쳐주고 얼마나 정확하게 짜는지 측정해보았는데, **문법을 랜덤으로 생성한 언어가
더 나았다**고 한다.(…) [#](http://developers.slashdot.org/story/11/10/27/213231/is-
perl-better-than-a-randomly-generated-programming-language)

  

웹프로그래밍에 많이 쓰이고, 소스코드가 더러워보이는 특성 때문에, "인터넷을 땜빵 연결하고 있는 청테이프(정확히 말하면 'duct
tape')"라고 불리기도 한다(...). 다시 말하지만 이런건 초심자의 얘기고 코딩을 깨끗하게 하는 경력자가 짜면 가독성이 나쁘지 않다.

  

perlcc라는 툴을 이용하면 단독으로 사용되는 코드를 만들 수 있었으나 지금은 제대로 작동되지 않는다. 대체재로는 [PAR::Packer가](PAR%3APacker%EA%B0%80%20.md)있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Perl?action=edit&section=4)]

## 4. Perl 6 ¶

Perl 6은 언어 명세 그 자체를 뜻한다. Perl 6의 테스트 케이스를 모두 통과한 프로그램은 Perl 6를 구현한 컴파일러라 부를 수
있다.

  

프로그래밍 언어계 희대의 떡밥으로 유명하다. Perl 6 개발은 2000 년도부터 시작됐었고 나온다 나온다 소리가 계속 있었으나 지금까지
무려 13년간 개발중이다. (...) 어느 정도 Specification 은 나온 상태고 그 것에 기반한 컴파일러도 몇 개 있긴 하지만
Production-level 사용은 불가능한 수준이다. 이렇게 늦어지는 이유중 하나는 OOP 도 보강하고, Lisp 이나
[Haskell](Haskell.md) 등에서 사용되는 기능들도 넣고 여러모로 Perl 5 에서 이어진다기보다 재창조에 가까운 수준의
기획인 점도 있으나 무엇보다 어떤 기업의 지원도 받지 못하고 있어 완전한 Community-Driven 개발이 이루어지고 있기 때문이다.
그리고 이렇게 늦어지다보니 이미 상당수의 스크립트 유저들은 파이썬으로 넘어간 상태. Python 3 vs Perl 6 의 떡밥도 웹에서 자주
보이나, 상당수는 Python 4 vs Perl 6 이 현실적이지 않냐는 반응.

  

2015년 1월, Larry Wall이 Production Level의 Perl 6를 공개 발표할 예정이다.`[6]` MoarVM을 백엔드로
쓰는 Rakudo는 이미 대부분의 언어 스펙을 구현했고 퍼포먼스도 크게 향상되었는데 `[7]` 여전히 느리긴 하다. 하지만 20년 가까이 된
세월만에 첫 발을 내딛은 Perl 6이다. 기대를 가져봄직하다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Perl?action=edit&section=5)]

## 5. 기타 ¶

한국에서는 과거 개인용 웹 프로그램용 언어로 각광을 받았으나, 현재는 [PHP](PHP.md)에 완전히 자리를 내준 상태. 하지만
미국, 일본등 여타 국가에서는 아직도 펄을 많이 사용하고 있다`[8]`. 웹 게임(배틀로얄)이나 건담 배틀 류가 일본에서 온 perl
CGI.

  

1997년 ~ 2000년대 초까지 웹 CGI로 널리 쓰였고, 당시 게스트 북 purelife dream, pury bbs이나 현재 블로그와
유사한 IRiS 시리즈도 펄로 작성 되었다. 이 때문인지 perl == CGI 로 인식되는 경향이 있는데, 웹 관련 프레임 웍,
비동기/네트웍/동시성 프레임웍, GUI 및 그래픽, 과학 및 수치계산, 시스템관리 및 자동화 등에 쓸 수 있는 등 사용 방법은 무궁무진하다.

  

어쩐지 [파이썬](%ED%8C%8C%EC%9D%B4%EC%8D%AC.md)과 라이벌 관계를 형성하고 있다. 둘 다 스크립트 언어에서
시작해서 세를 넓혔지만, 파이썬은 TIMTOWTDI를 배제하고 문제를 해결하는 명확한 하나의 방법을 추구하기 때문. 문법적으로도 매우
자유분방한 펄과는 달리, 들여쓰기까지도 문법의 일부로 제한하는 등 덜 자유롭지만 정갈한 코드를 지향한다. 이 점에 매료되어 펄과 파이썬
사이의 선택지에서 파이썬을 선택하는 사람이 많고, 특히 펄 커뮤니티가 사멸하다시피(...) 한 한국에서는 파이썬 쪽이 대중적이다.

  

소스만 1.9메가인 c++ 소스를 java로 포팅 하는데, 펄의
[정규표현식](%EC%A0%95%EA%B7%9C%ED%91%9C%ED%98%84%EC%8B%9D.md)과 직접 제작한 논리엔진으로
사흘만에 포팅, 실행에 성공했다는 사례도 있다카더라.

[[edit](http://rigvedawiki.net/r1/wiki.php/Perl?action=edit&section=6)]

## 6. 정규표현식 ¶

[정규표현식](%EC%A0%95%EA%B7%9C%ED%91%9C%ED%98%84%EC%8B%9D.md) 항목 참조.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Perl?action=edit&section=7)]

## 7. 관련 사이트 ¶

펄 코리아 <http://perl.kr/> <http://www.perl.or.kr>  
펄마니아<http://www.perlmania.or.kr>  
한글 펄문서 프로젝트<http://doc.perl.kr>  
IRC #perl-kr<http://webchat.freenode.net/?channels=perl-kr>

  

Perlog<http://blog.perl.kr/>  
Naver Perl Cafe<http://cafe.naver.com/perlstudy>  
Perl Books in Korean<http://books.perl.kr/>

  

Perl Advent Calendar 2010<http://advent.perl.kr/2010/> `[9]`  
Perl Advent Calendar 2011<http://advent.perl.kr/2011/>  
Perl Advent Calendar 2012<http://advent.perl.kr/2012/>  
Perl Advent Calendar 2013 <http://advent.perl.kr/2013/>  
Perl 석가탄신일 기념 달력<http://lotus.perl.kr/>

  

[2008 Korean Perl Workshop](http://event.perl.kr/kpw2008/)  
[2012 Korean Perl Workshop](http://event.perl.kr/kpw2012/)  
[Perl 소스](http://perl5.git.perl.org/perl.git/tags)

`\----`

  * `[1]` 본인말로는 가장 많은 명성과 **가장 적은 돈**을 가져다 줬다나(프로그래밍언어론 8판 수록 인터뷰 참고)
  * `[2]` [파이썬](%ED%8C%8C%EC%9D%B4%EC%8D%AC.md)은 '가장 아름다운 하나의 답이 존재한다'
  * `[3]` 발전된 드립으로 **C PERL [GNOME](GNOME.md) [JAVA](Java.md)** 가 있다 <del>당연하지만 해석은 **씨펄 그 놈 잡아**</del>
  * `[4]` 본인이 인터뷰에서 직접 언급했다
  * `[5]` 다른 프로그래머가 해독하지 못해 인원 대체가 불가능하다는 뜻
  * `[6]` <https://fosdem.org/2015/schedule/event/get_ready_to_party/>
  * `[7]` <http://jnthn.net/papers/2014-yapceu-performance.pdf>
  * `[8]` 유행<del>갑의 요구</del>에 따라 급변하는 한국의 특성상 특정 언어가 대세로 자리 잡히면 여타 언어는 씨가 말라버리곤 한다 
  * `[9]` 2010, 2011년 달력의 각 날짜를 클릭하면 온갖 기괴한 사용 사례를 볼 수 있다. 하루에 하나씩 배우는 펄 사용 방법.

