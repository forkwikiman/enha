## Contents

    

1 개요

2 어떻게 구현하나

3 JIT, 그리고 마개조

4 아직 해야 할 과제

5 예제

[[edit](http://rigvedawiki.net/r1/wiki.php/PyPy?action=edit&section=1)]

## 1 개요 ¶

  

![http://pypy.org/image/pypy-logo.png](http://z1.enha.kr/http://pypy.org/image
/pypy-logo.png)

[[PNG external image]](http://pypy.org/image/pypy-logo.png)

  
<del>[우로보로스](%EC%9A%B0%EB%A1%9C%EB%B3%B4%EB%A1%9C%EC%8A%A4.md)</del>

  

[PyPy 프로젝트 사이트](http://pypy.org/)  
[표준 구현인 CPython과의 속도비교. PyPy를 개발하면서 지속적으로 업데이트하고 있다.](http://speed.pypy.org/)

  

[Python](%ED%8C%8C%EC%9D%B4%EC%8D%AC#s-2.md)의 언어 구현 중 하나로, [C](C%28%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20%EC%96%B8%EC%96%B4%29.md)로 짜여진 기존의
CPython과 달리 **Python으로 Python을 만드는 프로젝트**이다. 여기까지 얘기하면 뭔가 이상한 짓 하는 프로젝트 내지
실험적인 프로젝트처럼 느껴지겠지만, 이 프로젝트의 진짜 놀라운 점은 기존 CPython에 비해 전혀 느리지 않을 뿐더러, **오히려
성능면에서 CPython을 능가하고 있다는 거다.** 심지어 [이 링크](http://speed.pypy.org/)에서 보이는 대로,
**계속해서 빨라지고 있다!**

  

애초에 이 구현은 그저 장난질이나 하려고 시작한 프로젝트가 아니다. [Psyco](http://psyco.sourceforge.net/)라고
하는, 기존 파이썬 위에다가 [Just-In-Time 컴파일](JIT.md)을 구현해서 실행성능을 높히는 프로젝트가 있었는데, 이걸
개발하던 [Armin Rigo](http://codespeak.net/~arigo/)라는 사람이 아예 JIT 컴파일을 하는 파이썬을 처음부터
다시 구현하기로 생각했다. 그래서 2003년부터 PyPy 개발을 시작하여
[유럽연합](%EC%9C%A0%EB%9F%BD%EC%97%B0%ED%95%A9.md)의 연구자금 지원을 받아가며 지금까지 개발하고
있다.

[[edit](http://rigvedawiki.net/r1/wiki.php/PyPy?action=edit&section=2)]

## 2 어떻게 구현하나 ¶

  

[기계어](%EA%B8%B0%EA%B3%84%EC%96%B4.md)로
[컴파일](%EC%BB%B4%ED%8C%8C%EC%9D%BC.md)하지 않고 기껏해야 인터프리팅 성능을 빠르게 하기 위해
[바이트코드](%EB%B0%94%EC%9D%B4%ED%8A%B8%EC%BD%94%EB%93%9C.md)만을 쓰는
[Python](%ED%8C%8C%EC%9D%B4%EC%8D%AC#s-2.md)을 가지고 파이썬으로 돌리는 파이썬을 어떻게 만들었을까.
PyPy의 접근법은 이렇다.

  

  1. 먼저 RPython이라고 하는, 파이썬 문법을 엄격하게 만들어 컴파일이 가능하게 만든 해석기(translate.py)를 Python 코드로 작성한다.`[1]`
  2. RPython의 효과적인 컴파일을 위해 다른 언어로 툴체인을 만든다.`[2]`
  3. Python 구현(런타임)을 RPython 문법으로 작성한다.
  4. 3에서 만든 구현을 1 또는 2에서 만든 RPython 해석기로 컴파일한다.
  5. 4으로 만든 후보를 이전 또는 다른 구현과 비교(성능 측정), 만족스럽지 않으면 수정한다.(nightly builds)
  6. 5에서 만족스러운 결과를 냈다면 출시하고 1 또는 2부터 다시 시작한다.(release)  

<del>뭔가 속는 느낌이지만</del> 처음 한번만 기존 파이썬의 도움을 받으면 그 다음부터는 스스로 만든 구현으로 저 과정을 자체적으로
계속 반복할 수 있다. 이게 얼핏 보면 '닭이 먼저냐 달걀이 먼저냐' 같은 것으로 착각할 수도 있지만, 이런 식의 접근법은 실제로 프로그래밍
언어를 제작할 때 해당되는 사항이며, 더 좋은 장비의 개발을 위해 기존의 장비를 사용하는 것과 다름이 없다. 이러한 이유로 로고가
[우로보로스](%EC%9A%B0%EB%A1%9C%EB%B3%B4%EB%A1%9C%EC%8A%A4.md)인 셈. 다만 PyPy는 문자
그대로 **[진화](%EC%A7%84%ED%99%94.md)**하고 있다.

  

사실 이런 식으로 어떤 언어로 자기 자신을 구현하는 것을 **부트스트래핑**(Bootstrapping) 또는
**부팅**(Booting)`[3]`이라고 하는데, 사실 이렇게 하는 이유는 처음부터 작업하는 것보다 생산성에서 낫기 때문이다. 처음부터
어셈블리어로 작업하면 [이론상 최강](%EC%9D%B4%EB%A1%A0%EC%83%81%20%EC%B5%9C%EA%B0%95.md)의
성능을 발휘할 수는 있으나 그 가능성은 매우 낮고 생산성도
최악이다.([최적화](%EC%B5%9C%EC%A0%81%ED%99%94.md)가 그래서 힘들다.) 이 때문에 대부분의 프로그래밍 언어도
초창기에는 어셈블리어나 다른 고급언어의 도움을 받지만, 일정 단계를 넘어서면서 그 한계가 오면 스스로의 컴파일러/인터프리터를 제작하게 된다.
Haskell 컴파일러인 GHC와 C/C++ 컴파일러인 GCC가 대표적인 예. 물론 생산성에 중점을 두기 때문에 성능이 눈에 띄게 빨라지는
일은 잘 드러나지 않으며, 단지 우연한 발견 등 여러 이유로 성능이 향상되는 것 뿐이다. PyPy의 경우 Python의 한계를 극복하기 위해
정적인 컴파일이 가능한 RPython을 따로 만들었고 뒤에도 언급할 듯 성능 향상을 위해 **7년이라는 긴 세월**을 소모했는데, 이것도
어셈블리어로 처음부터 하는 것보다는 짧은 것이다.`[4]`

[[edit](http://rigvedawiki.net/r1/wiki.php/PyPy?action=edit&section=3)]

## 3 JIT, 그리고 마개조 ¶

  

PyPy는 RPython으로 이루어진 Python 인터프리터와 (역시 RPython으로 이루어진) C, .Net, JVM등을 타게팅한 해석
툴체인으로 이루어져 있는데, 해석 툴체인은 해당 플랫폼을 위한 효율적인 코드를 생성하는 데 초점이 맞춰져 있으며, Tracing JIT을
통해 인터프리터 단위의 JIT 컴파일이 가능하므로, CPython보다 빠른 결과물이 나오게 된다.

  

여기까지만이어도 그냥 기존 구현에 비해 그다지 느리지 않은 파이썬 구현을 다른 언어의 도움 없이 파이썬 스스로 만든 셈이지만, 여기서 하나가
더 들어간다. Armin Rigo가 뭐 만들던 사람이라고 아까 얘기했던가? 그렇다. PyPy는 [JIT](JIT.md)
compiler다. 그것도 그냥 JIT가 아니라 meta tracing JIT라는 괴랄한 물건을 구현했는데, JIT이 필요한 부분에 약간의
힌트 코드를 넣으면 **RPython 해석기가 알아서 JIT compile이 되는 언어 구현을 만들어준다.** 다른 언어 구현들이 JIT 좀
해보자고 무지막지한 삽질을 하는 것에 비해`[5]` 거의 공짜나 다름없다.`[6]`

  

하지만, 사실 만들고 나서 보니 그렇게 보이는 거고 PyPy는 그냥 JIT를 구현한 게 아니라 **JIT 구현을 만들어주는 컴파일러를
구현**한 셈이 되므로 실제 작업은 훨씬 더 어려웠을 것이다. 당장 PyPy가 CPython보다 빨라지게 된 게 PyPy 1.3 이후부터인데
[그게 2010년
중순이다.](http://morepypy.blogspot.com/2010/06/pypy-13-released.html)`[7]` 다시 말해
7년동안 아무도 알아주지 않았던 '진화'가 드디어 빛을 본 셈. 심지어 본인들도 ["우리는 영웅이 아니며, 단지 인내심이 많았을
뿐이다."](http://morepypy.blogspot.com/2010/12/we-are-not-heroes-just-very-
patient.html)라고 말하고 있다. 잠시 PyPy 개발팀의 [근성](%EA%B7%BC%EC%84%B1.md)에 경의를 표하자
(…) 여담으로, 이 녀석의 해석은 사람만 힘든 게 아니라 컴퓨터도 힘든 모양이다. 써볼 사람들은 <del>시간이 남아돌고</del>
사용하는 컴퓨터가 어지간히 고사양이 아니라면 미리 컴파일된 것을 받아 사용하자. CPython을 통한 Bootstrapping에 엄청난
시간과 메모리를 요구한다.`[8]`

  

이런 구조로 만든 덕분에 보너스로, RPython 컴파일을 할때 목적 타겟을 다르게 주면 다른 플랫폼에서 돌아가는 파이썬 구현이 나온다.
그래서 똑같은 PyPy 소스코드로 [CPython](%ED%8C%8C%EC%9D%B4%EC%8D%AC#s-2.md)같은 놈도 나오고
[Jython](%EC%9E%90%EB%B0%94.md)같은 놈도 나오고
[IronPython](.NET%20Framework.md)같은 놈도 나오고 한다. 추가로
[코루틴](%EC%BD%94%EB%A3%A8%ED%8B%B4.md)을 쓰는 [StacklessPython](Stackless%20Python.md)같은 것도 비슷한 방법으로 만들 수 있어서 Stackless Python 개발하던
Christian Tismer가 아예 PyPy 개발팀에 와서 같이 일하고 있다. `[9]` <del>[이쯤되면 뭔가 무섭다](%EB%AA%B0%EB%9D%BC%20%EB%AD%90%EC%95%BC%20%EC%9D%B4%EA%B1%B0%20%EB%AC%B4%EC%84%9C%EC%9B%8C.md)</del>

[[edit](http://rigvedawiki.net/r1/wiki.php/PyPy?action=edit&section=4)]

## 4 아직 해야 할 과제 ¶

  

2014년 3월 현재 최신 버전은 [PyPy
2.2.1](http://morepypy.blogspot.com/2013/11/pypy-221-incrementalism1.html)이며,
CPython 2.7.3과 호환된다. Python 3.x 를 위한 PyPy는 [PyPy3 2.1
beta1](http://morepypy.blogspot.kr/2013/07/pypy3-21-beta-1.html)이 최근 릴리즈되었다.
PyPy 개발팀의 호환성 기준은 매우 심플해서, **이유 여하를 막론하고 CPython에서 되던 게 PyPy에서 안 되면 그냥 PyPy
버그**다. (...) 거의 C 확장모듈 쓴 코드 빼고는 모두 돌아간다고 보면 된다. 현재 PyPy 사이트에서 Python 3.x와의
호환성과 [NumPy](NumPy.md) 지원`[10]`을 위한 기부를 받고 있다. NumPy 쪽은 이미 대부분의 경우 사용에 지장이
없는 수준까지 구현했다고. [#](http://morepypy.blogspot.com/2014/03/numpy-status-update-
february.html)

[[edit](http://rigvedawiki.net/r1/wiki.php/PyPy?action=edit&section=5)]

## 5 예제 ¶

  

심심하면 다음 코드로 테스트 해 보자.  

    
    
    import randomdef populate_doors(): # put a car behind one doordoor=['goat', 'goat', 'goat']door[random.randint(0,2)]='car'return doorwins = 0losses = 0# playing the game 100,000 times:for x in range(100000):doors=populate_doors()first_choice=random.randint(0,2) # choose a random doorfor y in range(3): # reveal first losing, unchosen doorif doors[y] != 'car' and y != first_choice:doors[y] = 'out'breakif doors[first_choice] == 'car':losses = losses + 1 # contestant switched to losing doorelse:wins = wins + 1 # contestant switched to winning doorprint "All choices were switched."print "Wins:", winsprint "Losses:", losses

코드 출처: <http://www.danielveazey.com/tag/monty-hall-problem/>

  

PyPy가 대략 **5**배 빠른 것을 알 수 있다. 물론 어떤 코드냐에 따라 배율에 차이가 있고 가끔씩 더 느린 코드도 있지만 2014년
3월 현재 어지간한 경우엔 PyPy쪽이 빠르다고 봐도 된다.

`\----`

  * `[1]` RPython는 Python의 일부만 구현한 언어(부분 언어)이기 때문에 모든 RPython 코드는 Python 코드이기도 하다. (역은 성립하지 않는다.)
  * `[2]` [시뮬레이터](%EC%8B%9C%EB%AE%AC%EB%A0%88%EC%9D%B4%ED%84%B0.md)나 [에뮬레이터](%EC%97%90%EB%AE%AC%EB%A0%88%EC%9D%B4%ED%84%B0.md)를 제작할 때에도 이 과정은 반드시 거친다.
  * `[3]` 운영체제의 부팅과 같은 어원이다.
  * `[4]` 컴퓨터 하드웨어의 발전도 마찬가지다. 처음 IC나 LSI를 설계할 때는 레이아웃을 손으로 그렸지만, 지금 나오는 칩들은 손으로 하기에는 회로의 규모가 지나치게 크기 때문에 전부 CAD로 개발하고 있다. 사실 이러한 일은 망치를 만들기 위해 망치를 쓰거나 간석기를 만들기 위해 뗀석기를 썼던 것 처럼 **인류의 역사를 대표하는 방법론** 중 하나이므로 전혀 속는 느낌 가질 거 없다.
  * `[5]` 인터프리트나 바이트코드 컴파일 방식을 취하는 언어 구현 중에 [JIT](JIT.md)를 실용적으로 하는 구현은 [JVM](%EC%9E%90%EB%B0%94%20%EA%B0%80%EC%83%81%20%EB%A8%B8%EC%8B%A0.md)이나 [.NET CLR](.NET%20Framework.md) 정도밖에 없다. [둘](%EC%8D%AC%EB%A7%88%EC%9D%B4%ED%81%AC%EB%A1%9C%EC%8B%9C%EC%8A%A4%ED%85%9C%EC%A6%88.md) [다](%EB%A7%88%EC%9D%B4%ED%81%AC%EB%A1%9C%EC%86%8C%ED%94%84%ED%8A%B8.md) 돈 좀 쓰고 다닐 것 같은 느낌이 들지 않는가?
  * `[6]` PyPy가 대체 무슨 마개조를 벌이는지 더 자세히 알고 싶으면 [이 글을 참고하자](http://blog.dahlia.kr/post/5124874464). <del>뭔가 여기하고 많이 비슷해 보이는 건 착각......이 아닐 거다.</del> 이 위키 항목의 작성에 상당부분을 참조했다 (...) 
  * `[7]` 위에서도 얘기했지만 **2003년에 개발을 시작했다.**
  * `[8]` 준비물이 모두 갖춰진 상태에서 PyPy 2.2.1 달랑 하나를 빌드하는 데에 [모질라 파이어폭스](%EB%AA%A8%EC%A7%88%EB%9D%BC%20%ED%8C%8C%EC%9D%B4%EC%96%B4%ED%8F%AD%EC%8A%A4.md)와 그것이 의존하는 모든 다른 패키지들을 빌드하는 것보다 시간이 더 걸린다! **Core i7 3.33GHz, 다른 작업 방해 없이 코어 1개 풀사용, 8GB 램** 기준으로 **최소 3시간**은 각오해야 한다. 64비트 CPython으로 컴파일하다 보면 Python 프로세스 하나가 램을 5GB 가까이 [처묵처묵](%EC%B2%98%EB%AC%B5%EC%B2%98%EB%AC%B5.md)하는 것도 볼 수 있다. <del>[Garbage collection 따위는 장식입니다](%EB%8B%A4%EB%A6%AC%20%EB%94%B0%EC%9C%84%EB%8A%94%20%EC%9E%A5%EC%8B%9D%EC%9E%85%EB%8B%88%EB%8B%A4.md)</del> PyPy로 PyPy를 빌드해보신 분이 있으면 [추가바람](%EC%B6%94%EA%B0%80%EB%B0%94%EB%9E%8C.md).
  * `[9]` 여담이지만 [이 두 사람이 모여서 만든](https://bitbucket.org/ambroff/greenlet/src/77363116e78d/AUTHORS) 또 하나의 작품이 [greenlet](http://pypi.python.org/pypi/greenlet)인데, Psyco처럼 기존의 CPython에다가 [마개조](%EB%A7%88%EA%B0%9C%EC%A1%B0.md)를 해서 원래 지원 안 되는 코루틴을 만들어 올리는 라이브러리다... [참고](http://ricanet.com/new/view.php?id=blog/111007)
  * `[10]` [NumPy](http://www.numpy.org/)는 속도 문제 때문에 C 확장을 쓴 대표적인 파이썬 라이브러리이자, 과학계산 분야에서 쓰이는 파이썬 코드에서 절대적인 영향을 가진 라이브러리이다. 하지만 PyPy는 때때로 C로 짠 코드보다도 빨라지기 때문에(…) PyPy 측에서는 아예 NumPy를 순수 파이썬 코드로 재작성할 계획을 가지고 있다.

