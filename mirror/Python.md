  * 다른 의미의 Python은 [파이선](%ED%8C%8C%EC%9D%B4%EC%84%A0.md) 항목으로.  

## Contents

    

1. 개요 
2. 높은 생산성 
3. 디자인 철학 
4. 언어 구현 
    

4.1. Python 3.x

4.2. Stackless Python

4.3. Pyston

4.4. [PyPy](PyPy.md)

4.5. C 언어 확장, Cython

4.6. 가상 머신에서 동작하는 구현체

    

4.6.1. Jython

4.6.2. IronPython

4.6.3. Jython이나 IronPython은 왜 쓰는 걸까?

5. 멀티쓰레딩 문제 
6. 만능 언어 
7. 여담 

[[edit](http://rigvedawiki.net/r1/wiki.php/Python?action=edit&section=1)]

## 1. 개요 ¶

[프로그래밍언어](%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20%EC%96%B8%EC%96%B4.md)의
일종.  
창시자는 귀도 반 로섬(Guido van Rossum).`[1]` 1989년 크리스마스 주에 연구실은 닫혀있고 **심심해서
만들었다.**`[2]`

  

귀도가 즐겨 보던 영국의 6인조 개그 그룹 [MontyPython](%EB%AA%AC%ED%8B%B0%20%ED%8C%8C%EC%9D%B4%EC%84%A0.md)에서 이름을 땄다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Python?action=edit&section=2)]

## 2. 높은 생산성 ¶

![http://imgs.xkcd.com/comics/python.png](http://imgs.xkcd.com/comics/python.p
ng)

[[PNG external image]](http://imgs.xkcd.com/comics/python.png)

  
[xkcd](xkcd.md) [353화 'Python'](http://xkcd.com/353/)

  

인터프리터 언어이면서 우수한 자료형과 다양한 모듈 등을 제공해 개발기간이 매우 단축되는 것이 특징.
'[C언어](C%EC%96%B8%EC%96%B4.md)로 2년동안 완성하지 못한 프로젝트를 파이썬으로 한달만에 해냈다'는 극적인
경험담이 있을 정도다. C언어와의 접착성도 좋기 때문에, 일단 Python으로 빨리 구현하고, 남은 시간에 속도에 병목이 되는 부분을 C로
전환하는 전략을 내세우고 있다.`[3]` <del>맛들이면 다른 언어로 전환하기 힘든 부작용이 생긴다 카더라.</del>

  

참고로 저 [만화](xkcd.md)는 import antigravity라고 하면 나오는 [이스터 에그](%EC%9D%B4%EC%8A%A4%ED%84%B0%20%EC%97%90%EA%B7%B8.md)이다.(...)[영상](http://www.youtube.com/watc
h?v=_V0V6Rk6Fp4)

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Python?action=edit&section=3)]

## 3. 디자인 철학 ¶

[Perl](Perl.md)의 '하나 이상의 해결법이 존재한다' 와는 정반대로 '가장 아름다운 하나의 답이 존재한다'라는 명제를 모토로
하고 있다. 이 모토 하에 다음과 같은 철학을 지니게 되었다.

  

  * 아름다운 것이 추한 것보다 낫다.(Beautiful is better than ugly)
  * 명시적인 것이 암시적인 것보다 낫다. (Explicit is better than implicit) 
  * 간결한 것이 복잡한 것보다 낫다. (Simple is better than complex)  

따라서 다른 언어들의 코딩 스타일은 각자의 취향에 맞게 발산진화 하는 반면`[4]`, 파이썬은 위의 철학들을 만족시키는 하나의 스타일로
수렴진화하는 성향이 있다. 이런 성향은 다른언어에는 없는 파이썬스러움(pythonic)이라는 독특한 개념을 낳게 되었는데, 복잡하지 않으면서
의미가 명확하고, 심플한, 파이썬의 철학을 따르는 것들을 지칭하는 개념이다.

  

이런 철학 때문에 문법이 굉장히 엄격한 편이다. 예를 들자면, 다른 언어에서는 해도 되고 안 해도 되는 들여쓰기가 이 언어에서는 의무로
들여쓰기 자체로 하나의 코드 블럭이 된다. 코드 블럭을 명시적으로 표시하지 않아도 돼서 비쥬얼 적으로는 굉장히 깔끔한 반면`[5]`,
자유도를 제약한다는 평도 있다.  

def factorial(x):  

if x == 0:  

return 1

else:  

return x * factorial(x - 1)

[[edit](http://rigvedawiki.net/r1/wiki.php/Python?action=edit&section=4)]

## 4. 언어 구현 ¶

보통 말하는 Python은 [C](C.md)언어로 구현되었으며, 다른 구현체와 구분하여 언급할 때에는 CPython이라고 표기한다.
C#으로 구현된 닷넷프레임워크 위에서 동작하는 IronPython, CPython에서 C 스택을 없앤 Stackless Python,
Java로 구현되어 JVM위에서 돌아가는 Jython`[6]` , 파이썬 자체로 구현된 [PyPy](PyPy.md) 등이 있으며 이
가운데 오리지날은 CPython이다. 또한, 현재`[7]` [Dropbox](Dropbox.md)에서
[Pyston](https://github.com/dropbox/pyston)이란 [LLVM](LLVM.md)과
[JIT](JIT.md) 기반 파이썬을 개발 중이다.[DROPBOX TECH
BLOG](https://tech.dropbox.com/2014/04/introducing-pyston-an-upcoming-jit-
based-python-implementation/)

  

한편 [중국](%EC%A4%91%EA%B5%AD.md)에서는 Chinese Python이라는, 중국어 문법으로 한자를 쳐서 돌아가는
언어를 독자 개발했다. <del>오오 [대륙의기상](%EB%8C%80%EB%A5%99%EC%9D%98%20%EA%B8%B0%EC%83%81.md) 오오</del>

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Python?action=edit&section=5)]

### 4.1. Python 3.x ¶

사용자가 늘다 보니 여러 단점들이 지적되었는데, 과감하게 하위 호환성을 포기하고 Python 3000 이라는 코드명으로 개발하기 시작하여
발표된 버젼이다. 내부적으로는 많이 변했다고 하는데 겉보기에는 별로 변한 것 같지 않다는 것이 함정. 그러나 소소한 부분에서 문법과 기본
라이브러리에 차이가 있어 호환이 되지 않는다. 2to3이라는 python2를 python3로 바꿔주는 컨버터가 있어서 전부 갈아 엎어야 하는
수고는 덜 수 있다.

  

Python을 실제로 사용하게 되면, 구현에 필요한 기능을 지원하는 여러 패키지를 받아서 설치해 사용하게 된다. Python 2.x vs
Python 3.x 에서 선택은 주로 "내가 사용하기 원하는 패키지가 동작하는 환경"에 따라서 선택하게 된다.  

파이썬 3.x부터는 유니코드 지원이 더 강화되어 변수나 함수 이름을 [한글](%ED%95%9C%EA%B8%80.md)로 정할 수도 있게
되었다. `[8]` 그러니까...  

이름 = "어쩌고"  
나이 = 17  
보여줘 = print

  

보여줘('{} {}'.format(이름, 나이))  

이런 식으로.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Python?action=edit&section=6)]

### 4.2. Stackless Python ¶

<http://stackless.com/>

  

파이썬의 표준 구현인 CPython은 이름 그대로 [C](C%28%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20%EC%96%B8%EC%96%B4%29.md)로 만들어져 있는데, 파이썬 프로그램의 함수 호출
[스택](%EC%8A%A4%ED%83%9D.md)(Call stack)을 구현할 때 그만 C의 호출 스택`[9]`에 그대로 얹어가도록
구현되고 말았다. 때문에 파이썬에서 얼마나 메모리를 많이 쓸 수 있느냐에 관계없이 C 호출 스택을 꽉 채우는 순간 그대로 스택 오버플로우
에러가 뜨게 되어버렸고`[10]`, 파이썬 프로그램의 호출 스택, 즉 프로그램의 실행 흐름을 CPython 스스로 제어할 수가 없게 되어
[코루틴](%EC%BD%94%EB%A3%A8%ED%8B%B4.md) 등의 실행 흐름을 제어하는 언어 기능을 쓸 수 없게 되고 말았다.

  

Christian Tismer라는 개발자는 이 문제를 타파하려면 "CPython 소스코드를 수정해서`[11]` C 스택을 쓰는 부분을 전부
들어내고 새로 호출 스택을 짤 수밖에 없다"고 생각했고, 그것을 실제로 실행에 옮긴 것이 Stackless Python이다. 이름의
Stackless는 그래서 사실 C 호출 스택이 없다는 의미. Stackless Python은 스택 오버플로우 에러가 덜 난다는 사소한
장점(...)`[12]` 외에도, 스스로 제어할 수 있는 자체적인 호출 스택을 갖고 있기 때문에 마이크로쓰레드`[13]`나
[코루틴](%EC%BD%94%EB%A3%A8%ED%8B%B4.md) 같은 기능들을 쓸 수 있게 됐고, 덕분에 쓰레드도
[고자](%EA%B3%A0%EC%9E%90.md)고 코루틴도 안되는 CPython에 비해 동시성 처리에서 훨씬 강력한 이득을 낼 수
있게 됐다.

  

다만, 앞서 말했듯이 CPython을 개조한 것이기 때문에, 파이썬의 버전이 올라갈 때마다 개조한 코드가 이상없이 동작하는지 항상 확인해야
하고, 이 기능이 운영체제나 하드웨어에도 영향을 받는 까닭에 심하면 각각의 운영체제나 CPU별로 개발을 따로 해야 하는 피곤한 작업을
Python이 망할 때까지 해야 하는 지겨운 길을 걷게 되는 것이었다. 그래서 실제로 한동안 Stackless Python의 개발이 잠시
중단된 일도 있었을 정도.

  

그런 와중에 Armin Rigo`[14]`가 "C 호출 스택도 어차피 메모리에 있잖아? **그러면 그걸 memcpy()로 통째로 복사하고
덮어씌우면 호출 스택을 저장하고 복구하는 거 아냐?**"라는 [실로 마개조스러운
아이디어](http://ricanet.com/new/view.php?id=blog/111007)를 내놓는데, Christian Tismer가
여기에 매우 깊은 감명을 받고 Armin Rigo와 함께 구현한 결과
[greenlet](http://pypi.python.org/pypi/greenlet)이라고 하는 **import만 하면
[코루틴](%EC%BD%94%EB%A3%A8%ED%8B%B4.md)을 쓸 수 있는 모듈**을 만들어내기에 이른다. 같은 걸 구현하려고
언어 인터프리터 자체를 뜯어고치는 수고에 비하면 놀랄 만큼의 노력 절약이 아닐 수 없다. 다만 이 짓을 제대로 구현한 Stackless
Python에 비하면 아무래도 성능이 딸리기 때문에 정말 절실하게 성능이 필요한 [EVE온라인](EVE%20%EC%98%A8%EB%9D%BC%EC%9D%B8.md)과 같은 경우엔 Stackless Python을 쓴다.

  

하지만... Armin Rigo와 Christian Tismer는 지금 둘 다 [PyPy](PyPy.md)를 만들고 있고, PyPy는
자체 스택을 쓸 수 있는 Stackless 모드의 **[JIT 컴파일러](JIT.md)**를 만들어낼 수 있다. <del>본격 자기
프로젝트 능욕</del> <del>[Stackless는 안될거야 아마](%EC%9A%B0%EB%A6%B0%20%EC%95%88%EB%90%A0%EA%B1%B0%EC%95%BC%20%EC%95%84%EB%A7%88.md)</del>

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Python?action=edit&section=7)]

### 4.3. Pyston ¶

[LLVM과 현대적인 JIT 기술을 사용해서 개발 중인 오픈 소스 파이썬
구현물](https://github.com/dropbox/pyston)  
2014년 4월 프로젝트가 시작되었으며, Python 2.7, x86 64비트 플랫폼을 목표로 개발 중에 있다. 우분투에서만 테스트되고
있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Python?action=edit&section=8)]

### 4.4. [PyPy](PyPy.md) ¶

본격 Python으로 직접 구현되는 Python. 언뜻 보면 CPython보다 느릴 것 같지만 실제로는 더 빠른 실행결과도 보여주는 흠좀무한
녀석이다. 어떠한 외계의 기술이 적용되어서 이것이 가능한지는 [해당 항목](PyPy.md)을 참조하라.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Python?action=edit&section=9)]

### 4.5. C 언어 확장, Cython ¶

Python의 속도를 높이고자 아예 C언어로 변환하여 컴파일하는 방법을 택한 패키지. 정적 타입 선언과 함께 C언어로 변환되어 컴파일된다는
점 때문에 ctypes 로 덧씌우는 것 없이 네이티브 코드(*.so, *.dll)를 직접 사용할 수 있다. 이것을 사용하면 적게는 열 배
정도에서 많게는 천 배 이상까지 속도 향상을 경험할 수 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Python?action=edit&section=10)]

### 4.6. 가상 머신에서 동작하는 구현체 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/Python?action=edit&section=11)]

#### 4.6.1. Jython ¶

Jython은 [Java](%EC%9E%90%EB%B0%94.md)로 구현되어
[JVM](%EC%9E%90%EB%B0%94%20%EA%B0%80%EC%83%81%20%EB%A8%B8%EC%8B%A0.md)위에서
실행된다. CPython이 C언어와 결합성, 접착성이 좋은 것처럼 Jython은 Java와 결합성이 대단히 좋으며, 실제로 Java 진영의
메이저 업체인 [Oracle](%EC%98%A4%EB%9D%BC%ED%81%B4.md), [IBM](IBM.md)등에서도 자사
제품에 Jython을 내장하여 스크립팅 기능을 제공하고 있을 정도다.

  

Jython은
[JVM](%EC%9E%90%EB%B0%94%20%EA%B0%80%EC%83%81%20%EB%A8%B8%EC%8B%A0.md)위에서
실행되며, Python Module이 제공하는 API는 물론이고, [JDK](JDK.md)가 제공하는 모든 API를 그대로 사용할 수
있다. 오히려 pycrpyto와 같이 C언어로 구현된 CPython 모듈은 Jython에서 사용할 수 없다. 그러나 일단 Java
Class라면, 설령 JNI로 되어있어서 C로 작성된 동적 모듈(*.dll, *.so등)을 사용한다고 해도 Jython에서 사용하는데 아무런
제약이 없다. 또한 JVM위에서 실행된다는 점 때문에 CPython의 GIL이 이식되지 않았으며, CPython이 멀티쓰레드에서 보이는
단점이 Jython에는 존재하지 않는다. <del>대신 당연하지만 JVM이 가지는 제약을 그대로 가진다. 그런데 이건 지난 십 수년간 꾸준히
개선되어서 이제 많이 괜찮아졌잖아?</del> threading, threadsafety등의 Python에서 제공하는 멀티쓰레드(락, 동기화
관련) 기능이 마음에 들지 않으면 java.util.concurrent 에서 제공하는 Java API를 사용하면 된다!!!

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Python?action=edit&section=12)]

#### 4.6.2. IronPython ¶

Microsoft .net Framework의 가상머신인 CLR 상에서 구현되고 이 위에서 동작하는 Python 이다. 따라서 당연히
.net Framework 환경에서 제작된 DLL과 결합성이 매우 좋다. Jython과 마찬가지로 병렬 프로그래밍 환경에서 GIL 때문에
고민할 필요가 없다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Python?action=edit&section=13)]

#### 4.6.3. Jython이나 IronPython은 왜 쓰는 걸까? ¶

시작부터 JVM 또는 .net CLR 위에서 동작하는 Python 구현체를 도입하는 경우는 매우 드물다. 기존에 Java나 .net
Framework에서 개발되어 운영되던 프로그램이나 시스템이 존재하고, 이 환경 하에서 Python의 간결하고 편리한 기능과 높은 생산성을
도입하고자 할 때 사용된다.

  

둘 다 CPython에 비하면 실행 속도가 매우 느리며, Jython은 경우에 따라서 심각할 정도로 많이 느리다. 따라서 주요 기능을
수행하는 데에는 문제가 있지만, 보조 기능에서 사용하면 매우 손쉽게 번거로운 작업들을 Python 스크립트로 Java, .net
Framework의 자원을 그대로 끌어다 써서 할 수 있기 때문에 개발 공수와 편리함에서 큰 장점이 있다.

  
  

[[edit](http://rigvedawiki.net/r1/wiki.php/Python?action=edit&section=14)]

## 5. 멀티쓰레딩 문제 ¶

파이썬은 멀티스레딩을 지원하기 위하여 GIL(Global Interpreter Lock), 즉 전역 인터프리터 락을 도입하여 사용하게
되었다. 따라서, python 스레드 10개를 만들어도 실제 Pthread/윈도우 쓰레드가 10개가 만들어지긴 하는데, GIL때문에 개중
동시에 하나밖에 안돌아가는 기이한 구조를 갖고 있다. `[15]` 이것은 구현이 매우 쉬워지고 빠른 개발을 할 수 있다는 장점이 있으나 다중
코어 CPU가 보편화된 2006년 이후에는 다중 코어를 제대로 활용하지 못하는 구조적인 문제 때문에 성능에서 밀린다는 평가를 받게 되었다.
만일 특정 프로그램에 순진하게 CPU 코어를 2개 이상 동원하려고 할 경우, 뮤텍스(MutEx), 즉 한 쓰레드에 여러개의 CPU가 연산을
행하여 내부 정보를 오염시키는 것을 방지하는 역할을 맡는 GIL이 병목 현상을 일으켜 코어 하나를 쓸 때보다 오히려 성능이 크게 저하된다는
것. 구글 내부에서 이미 [가루가 되도록 까인 부분](http://blip.tv/carlfk/mindblowing-python-
gil-2243379)이다.

  

이런 문제점 때문에 파이썬에서 병렬 처리가 필요할때는 다중 [쓰레드](%EC%93%B0%EB%A0%88%EB%93%9C.md)가 아닌
다중 [프로세스](%ED%94%84%EB%A1%9C%EC%84%B8%EC%8A%A4.md)로 GIL을 우회하는 방식을 사용한다.
2008년 이후에 Multiprocessing이라는 모듈을 제공하는데 이 모듈은 자식 프로세스를 만드는 방향으로 다중 코어 사용시 성능의
향상을 꾀하고 있다.

  

단, CPU 부하가 큰 작업을 돌리는 것이 아니면 GIL을 체감하기는 생각보다 쉽지 않다. 다중 쓰레딩으로 CPU의 여러 코어를 최대한
이용하고 싶은 경우에는 GIL가 굉장히 아쉬운 이슈지만, CPU를 별로 쓰지않거나 I/O가 주가 되는 작업은 유의미한 성능 차이가 없다.
게다가 어설프게 코어 몇개 깔짝깔짝 이용해서 계산하는 것보다는 그냥 C언어로 모듈을 짜서 붙이는게 더 빠르다. 즉, python에서 CPU를
많이 먹는 부분은 C 모듈을 짜서 붙이고 필요하다면 multiprocessing 모듈을 이용하여 멀티코어를 활용하는 편. <del>그 이상의
CPU-heavy한 작업은 동적 인터프리팅 언어 쓰지 말고 처음부터 [C](C.md), [C++](C++.md)로 짜는게
맞다</del>

  

자세히 알고싶다면 다음 링크들을 참조.

  

* [Understanding the Python GIL (유튜브)](http://www.youtube.com/watch?v=Obt-vMVdM8s)  
* [파이썬 GIL 깊숙히! (上)](http://openlook.org/blog/2006/11/12/cb-1136/)  
* [파이썬 GIL 깊숙히! (상) 에 대한 몇 가지 변명](http://openlook.org/blog/2007/02/27/cb-1146/)

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Python?action=edit&section=15)]

## 6. 만능 언어 ¶

인터넷상 Python으로 보급되는 패키지는 굉장히 다양하고 방대하게 제공된다`[16]`<del>그러나 요즘 만능 아닌 언어 거의
없다</del>. 당신이 하려는 것이 무엇이든, 무슨 언어를 써야 할지 모르겠으면 Python을 쓰면 된다. Python 으로 직접
만들었거나 또는 다른 프로그램의 Wrapper가 꼭 존재한다. 사실상 못하는 것이 없다. 웹 사이트 서버를 구현하려고 하면 Python
Web Framework 를 쳐보자 (Django, Flask, Bottle 등).
[기계학습](%EA%B8%B0%EA%B3%84%ED%95%99%EC%8A%B5.md) 알고리즘을 쓰고 쉽다면 python machine
learning 이라 검색하자 (scikit-learn). 얼굴인식을 코드 몇 줄로 할 수도 있다 (OpenCV). 게임도 만들 수 있다
(PyGame). <del>Python make girlfriend 도 된다
[카더라](%EC%B9%B4%EB%8D%94%EB%9D%BC.md)</del> 비주얼 노벨도 만들 수 있다. 비주얼 노벨 전문툴
[Ren'Py](Ren%27Py.md) 참조. <del>그래도 괴수들은 렌파이로 카드게임도 만든다.</del>

  

물론 그렇다고 Python만 쓰는 것이 답은 아니다. 실행 속도와 Python 자체의 한계로 당연히 C, C++ 같은 언어의 연산속도를
따라갈 수는 없으며, 사실
[자바스크립트](%EC%9E%90%EB%B0%94%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8.md)나
[LISP](LISP.md)계열 언어 등 동적 언어들을 전체를 주욱 놓고 비교 해봐도 속도가 빠른 편은 아니다. 보통 인터프리터 언어의
속도 문제를 극복하기 위해서 인터프리터에 [JIT](JIT.md) 컴파일러를 넣는 추세지만 Python의 표준인 CPython에서는
구현이 되어있지 있다. <del>Pyston 프로젝트가 잘 되면
[수정바람](%EC%88%98%EC%A0%95%EB%B0%94%EB%9E%8C.md)</del> R 과 같이 특정분야에 특화된 언어와
비교하면 꼭 라이브러리가 더 다양하다고 볼 수도 없다. 이에 대해서
[추가바람](%EC%B6%94%EA%B0%80%EB%B0%94%EB%9E%8C.md)

  

그리고 동적 타입 언어(dynamically typed language)라는 점이 큰 프로젝트에서는 단점으로 작용하여 자료구조 설계나
디버깅이 어렵다는 지적도 있다. 다만 정적 타입 vs. 동적 언어 논쟁은 서로의 장단점이 있으며 일종의 종교논쟁으로 취급받는다. 일례로
OCaml같은 강력한 타입 인터페이스(Hindley-Milner)를 가진 경우, 모든 타입 에러(!)를 컴파일 타임에 잡아낼 수 있는
반면에, 모든 버그가 타입 에러는 아니기 때문에 여전히 테스트 및 디버깅 과정은 필요하며, 타입 시스템으로 인한 부담 때문에 빠른 구현에는
부담이 될 수 있다. 반면에 동적 언어는 빠른 구현의 이점이 있지만 타입 에러가 많이 나는 특징이 있다. 그러나 커버리지가 높은 테스트
세트로 어느정도 커버할 수 있으며 최근의 추세와 부합하는 방식이기도 하다.

  

특정 언어를 어떻게든 돌아가게 짜는 것은 노가다를 배우는 것이라면, 프로그램의 설계는 건축가가 거대한 빌딩을 설계하는 작업이라고 할 수
있다. 1 ~ 2층 정도의 작은 집은 오로지 노가다로 해결한다고 해도, [부르즈할리파](%EB%B6%80%EB%A5%B4%EC%A6%88%20%ED%95%A0%EB%A6%AC%ED%8C%8C.md)는 이런식으로
지을 수 없다. 적절한 자재, 하중을 지탱할 수 있는 구조, 외력 등을 고려해서 설계해야 한다. 이렇게 하기 위해서는 알고리즘과 자료구조,
아키텍쳐 등의 공학적 지식과 경험이 있어야 하며, 제대로 훈련된 프로그래머와 단순 코더가 짠 코드는 생산성, 탄탄함, 버그 발생률, 확장
가능성에서 큰 차이가 난다. <del>그러나 오너 눈에는 몸값 싸고 빨리 만들기만 하면 장땡이겠지</del>

  

빠른 아이디어 구현이 생명인 연구소에서 각광을 받고 있고, 한국 밖에서는 당당한 주류 언어로 대우받고 있다.
[인스타그램](%EC%9D%B8%EC%8A%A4%ED%83%80%EA%B7%B8%EB%9E%A8.md),
[유튜브](%EC%9C%A0%ED%8A%9C%EB%B8%8C.md), [reddit](reddit.md) 등이 Python을 주로
쓰고 있다고 알려져 있으며, 외국의 구인 사이트에도 Python을 할 줄 아는 사람에 대한 수요가 많다. 컴퓨터 관련이 아닌 이공계 전반에서
많이 쓰이는 [MatLab](MatLab.md)은 오픈소스가 아니라는 점이 최근 추세와 맞지 않아 입지가 좁아지고 있다. 게다가 패키지
설치를 참 더럽게 이상하게 만들어놨다. MatLab과 같은 목적의 파이썬 패키지인 NumPy는 모종의 계약을 통해 문법과 함수 등의 많은
부분에서 MatLab 함수와 호환되게 수정해 버렸고, 안그래도 꽤 쓰였던 NumPy는 더욱 사용자가 늘어나고 있다. Python의 경우는
지원 라이브러리의 대부분이 오픈소스이기 때문에 저장소에서 그냥 커맨드 라인 (pip install 패키지) 한 줄로 필요한 거의 모든
패키지를 설치해서 쓸 수 있다. 물론 PyQt 같은 예외도 분명히 존재한다.  

대학교 프로그래밍 교육은, 예전에는 한국을 포함하여 대부분의 학교에서 C, C++ 나 Java 같은 실제 회사에서 많이 쓰는 언어 위주로
수업을 개설했으나, 미국대학들은 개론 수업 언어를 Python 으로 옮겨가는 추세다. ([UC버클리](UC%20%EB%B2%84%ED%81%B4%EB%A6%AC.md) 컴퓨터과학 개론수업인 CS 61A 를 인터넷 강의로
들어보자!)

  

마지막으로, Python이 배우기 쉽다고 해도 결국 도구일 뿐이고, 프로그래밍 자체를 마냥 쉬운 것으로 생각하면 큰 코 다친다. 프로그래밍을
할 수 있는 것과 좋게 하는 것에는 큰 차이가 있으며, 좋은 프로그래밍을 하는 것은 프로그래머의 역량에 좌우된다.

  

게다가 요즘은 프로그래밍 언어와 프레임웍의 춘추 전국 시대라고 할 수 있을만큼 매우 많은 새로운 언어와 프레임웍이 등장하고 있으며, 아예
폴리글랏(Polyglot`[17]`) 프로그래밍이라는 용어가 등장하는 시대다. 당장 [구글](%EA%B5%AC%EA%B8%80.md)만
해도 C/C++, Java, Python을 골고루 섞어서 쓴다고 알려져 있으며, 게임도 메인은 C++ 로 작성되었으나 스크립팅은
Python이나 Lua로 된 경우([시드 마이어의 문명](%EC%8B%9C%EB%93%9C%20%EB%A7%88%EC%9D%B4%EC%96%B4%EC%9D%98%20%EB%AC%B8%EB%AA%85.md), [WOW](WOW.md) 등)을 매우 쉽게 찾아볼 수 있다.
따라서 필요하다면 프로그래밍 언어를 가리지 않고 매우 능숙할 수 있게 사용할 수 있도록 공부해야 하며, 알고리즘, 디자인 패턴, 테스트
기법, 동시성 프로그래밍(멀티스레드, 멀티프로세스)등의 필요한 지식을 훤하게 꿰고 있어야 제대로 된 프로그래머/개발자가 될 수 있다.

  
  

[[edit](http://rigvedawiki.net/r1/wiki.php/Python?action=edit&section=16)]

## 7. 여담 ¶

여담으로 [구글](%EA%B5%AC%EA%B8%80.md)에서 python이라고 검색하면 제일 위에 뜨는 게 위의 바다 괴물이나 뱀이
아니라 이거다.

  

Python 의 창시자 귀도 반 로섬은 구글에 입사했다. 그리고 Python 은 구글의 3대 개발 언어 중 하나로 알려져 있다.(나머지
2개는 [C++](C++.md) 와 [Java](Java.md) 이다.) 하지만 최근에 Go로 넘어가려는 움직임이 보인다
[카더라](%EC%B9%B4%EB%8D%94%EB%9D%BC.md).  
2012년 12월 7일부로 [DropBox](DropBox.md)에 입사했다.

  

한 헤드헌터로부터 경력직 파이썬 개발자 취업제안을 받았다고 한다. 즉, 파이썬 창시자에게 파이썬 '경력직' 개발자를 구하는 수준의 메일을
보낸 것(...) [#](https://plus.google.com/115212051037621986145/posts/R8jEVrobbRj)
<del>면접관: 파이썬 어느정도 하시나요? 귀도: **제가 만들었는데요**.</del>

  

[문명 4](%EB%AC%B8%EB%AA%85%204.md)의 스크립트 언어로 쓰였다. [lua](lua.md)와 더불어 게임
스크립트 언어의 양대산맥.

  

[킹덤 언더 파이어](%ED%82%B9%EB%8D%A4%20%EC%96%B8%EB%8D%94%20%ED%8C%8C%EC%9D%B4%EC%96%B4.md)의 엔진에도 쓰였다. 500여 개의 자체모듈이 누더기처럼 돌아갔다고 한다(…).

  

[월드 오브탱크](%EC%9B%94%EB%93%9C%20%EC%98%A4%EB%B8%8C%20%ED%83%B1%ED%81%AC.md)는 상당부분이
파이썬으로 구현되어있다. 유저가 작성하는 모드도 로직 부분은 파이썬으로 구현된다.

  

[EVE 온라인](EVE%20%EC%98%A8%EB%9D%BC%EC%9D%B8.md)은 Python의 경량/고속 실행 버전인
Stackless Python으로 작성되었다. 개발사 CCP Games는 파이썬 재단의 정식 후원자이기도 하다. 2000년대 초에 싱글코어
CPU가 계속 쓰일 줄 알고 서버 코드를 구버전 파이썬으로 짰다가 다중 코어 사용이 힘들어지자`[18]`, 눈물겨운 마개조를 거듭하여
파이썬이라는 언어가 제공할 수 있는 처리 능력을 한계치까지 뽑아서 쓰고 있다. <del>버그 잡고 최적화하는 프로그래머가 게임 내에서
유명인사가 된 것은 이 게임이 유일하겠지... 이게 다 GIL 때문</del>

  

[여기](http://www.codecademy.com/en/tracks/python)
[번역판](http://www.codecademy.com/en/tracks/python-ko)에서 인터프리터 설치 없이 웹 상으로 배워볼 수
있다. 단, 한글 번역판에서만 있는 오류도 있으니 주의

  

[NumPy](http://www.numpy.org/)+[SciPy](http://www.scipy.org/)+[matplotlib](htt
p://matplotlib.org/) 조합이 과학 공학 계산용으로 써볼만하다는 의견도 있다. <del>조금있으면 독점할 기세이다.</del>

  

2014년 6월 WWDC에서 애플이 공개한 [Swift](Swift%28%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20%EC%96%B8%EC%96%B4%29.md)라는 언어에게 220배(...) 느리다고 까였다.`[19]`  

![http://rigvedawiki.net/r1/wiki.php/%EC%8A%A4%EC%9C%84%ED%94%84%ED%8A%B8%28%E
D%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20%EC%96%B8%EC%96%B4%29?action=dow
nload&value=swift_objc_python_comparison.png?width=640](//rv.wkcdn.net/http://
rigvedawiki.net/r1/wiki.php/%EC%8A%A4%EC%9C%84%ED%94%84%ED%8A%B8%28%ED%94%84%E
B%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20%EC%96%B8%EC%96%B4%29?action=download&val
ue=swift_objc_python_comparison.png)

[[PNG external image]](http://rigvedawiki.net/r1/wiki.php/%EC%8A%A4%EC%9C%84%E
D%94%84%ED%8A%B8%28%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20%EC%96%B8%E
C%96%B4%29?action=download&value=swift_objc_python_comparison.png)

  

유저들은 C 바인딩인 ctypes를 출동시킨다고 부들부들... 하지만 테스트환경 세팅을 자사 제품에 유리하게 만드는건 벤치마크의 유서깊은
전통이므로 맹신은 금물. 파이썬의 강점은 속도에 있지 않다. 더구나 [JIT](JIT.md) 없는 동적 인터프리터 언어와 컴파일 언어의
성능을 비교하면 어떤 언어를 비교하더라도 당연히 후자가 압도적으로 유리하다(..)

  

객체 지향을 배울때 추천할만한 언어이다. 많은 대학들이 C++ 환경에서 가르치지만, 이경우 필요한 객체를 만들어서 쓰는 실습이 많은데 대부분
이미 존재하는 객체를 가져다 쓴다는 개념을 이해하지 못하는 경우가 많다. STL을 쓰면 달라지지만 실습에서 STL을 요구하는 문제가 나오는
경우도 드믈고 주로 사용되는 문자열 변환, 배열 관련 연산 등은 파이썬에서 따로 임포트할 필요없이 자료형 자체가 이미 클래스로서 편리하게
클래스 함수를 던져주기 때문에, 클래스의 재활용이라는 측면을 훨씬 이해하기 쉽다. 무엇보다 하루면 다 배울 수 있는 언어이기도 하고.

  

14년 8월 30일 유서깊은 파이썬행사인 Pycon이 드디어 한국에서도 성공리에 개최되었다. 내년엔 규모를 더 늘려서 할 거라고 한다.
<http://pycon.kr/>

`\----`

  * `[1]` 네덜란드어 발음으로 '히도 판 로쉼'.
  * `[2]` [링크](https://www.python.org/doc/essays/foreword/)를 보면 알겠지만 사실이다.(…)
  * `[3]` 버전이 올라가면서 Python 자체도 그리 느리지 않게 되었다.
  * `[4]` 실제로 c계열의 언어에서 중괄호의 위치에 대한 논쟁은 거의 종교적 논쟁에 가깝다. 현재 한국에서 가장 많이 쓰이는 방식은 C언어의 창시자 Kernighan과 Ritchie의 K&R 스타일이다. 그러나 Eric Allman의 방식을 고수하는 사람들도 제법 많다. 이외에도 중괄호 위치를 정하는 다른 방법들이 있으며 자세한 내용은 <http://gyumee.egloos.com/1306012>에서 확인가능
  * `[5]` 특히 코드를 종이에 출력해보면 중괄호 있고 없고의 가독성 차이가 의외로 크다
  * `[6]` 이전문서에서 dalvik vm에서 동작하지 않는다고 java가 아닌 jvm 바이트코드로 만들어 졋다고 쓰여 있었으나 jython 은 java로 만들어 진 것이 맞다. 궁금하다면 직접 소스를 확인하자 <https://hg.python.org/jython> dalvik vm은 기본적으로 jvm 바이트코드를 dalvik vm 코드로 변환해서 실행하는 방식이나 jython이 dalvik vm 에서 동작하지 않는 것은 dalvik 이 jvm 스펙 전체를 다 구현한 것이 아니라 dynamic language 지원을 위한 스펙이 빠져 있기 때문이다.<del>어차피 이제 ART로 바뀌어서 상관없...나?</del>
  * `[7]` 2014년 6월
  * `[8]` 사실 [C++](C++.md), [자바](%EC%9E%90%EB%B0%94.md), [액션스크립트](%EC%95%A1%EC%85%98%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8.md) 등 대부분의 현대 프로그래밍 언어들도 한글을 지원하므로 파이썬만의 특징은 아니다. 문제는 IDE가 제대로 받쳐주지 못한 경우가 많다. 적어도 자바와 액션스크립트는 완벽히 지원.
  * `[9]` C 시간에 스택 영역 힙 영역 할 때 나오는 그 스택이다. 
  * `[10]` C 레벨에서 만들어주는 스택이라 "C로 짜여진 프로그램"인 CPython은 손을 댈 수가 없다. <del>원칙적으로는 말이지</del>
  * `[11]` CPython은 [GPL 호환의 독자 라이센스를 가진 오픈소스 프로젝트](http://docs.python.org/license.html)다. 
  * `[12]` 메모리의 용량이 유한한 이상 스택 오버플로우 에러가 안 날 수는 없다. 
  * `[13]` OS가 직접 관리하는 쓰레드가 아닌, 유저 프로세스 차원에서 직접 돌리는 쓰레드. 그린 쓰레드(green thread)라고도 하는데 [Ruby](Ruby.md) 1.8까지 지원하는 쓰레드가 바로 이것이다. 
  * `[14]` [PyPy](PyPy.md) 리드 개발자 
  * `[15]` 물론, 내부적으로 IO작업이 있을시 바로 다른 쓰레드로 문맥 교환을 해주고, 바이트 코트를 100번 실행한 다음에는 인터프리터 차원에서 다른 쓰레드로 교체 해주므로 동시 작업 비슷한 효과가 난다. 
  * `[16]` 여기에 **다른 언어는 비교가 안될 정도로 방대하다**고 적혀 있었지만, 사실 이런 식의 방대한 라이브러리 구축은 Tex의 CTAN 은 1992년 부터, Perl의 CPAN은 1993년 부터 구축되어 있었다. 본격적인 인터넷 보급과 함께 이러한 패키지 운용 시스템은 [Linux](Linux.md)는 물론 여러 오픈소스쪽에 적용된 것을 볼 수 있다. 과거에 파이썬처럼 매우 널리 쓰였던, 그리고 지금은 파이썬이 몰아내고 있는 Perl의 CPAN은 2015년 1월 기준 약 143,000 개의 패키지를 제공한다. 당장 [Java](Java.md)에서 널리 쓰이는 Maven의 중앙 저장소만 해도 2015년 1월 기준으로 약 95,000 여개의 패키지를 가지고 있고, Scala나 Clojure 같은 비교적 역사가 짧은 JVM 기반 언어는 고유의 언어로 작성된 패키지가 들어있는 자체 저장소와 함께 Maven 중앙 저장소에 있는 Java로 작성된 모든 JAR를 같이 끌어다 쓸 수 있게 되어있다. Emacs도 버젼 24부터 패키지 저장소와 함께 Emacs [LISP](LISP.md)으로 작성된 패키지를 손쉽게 운용가능한 시스템이 포함되었으며, Common [LISP](LISP.md)에도 quicklisp와 asdf라는 유사한 패키지 운용 시스템이 존재한다. 심지어는 누가 쓸까 싶은 [Haskell](Haskell.md) 같은 언어도 cabal이라는 프로그램과 함께 Hackage라는 자체 패키지 저장소 시스템을 운용한다. 그런데 파이썬의 PyPi 는 역시 2015년 1월 기준으로 약 54,000 개의 패키지를 제공한다. 단, Python에 광범위하고 실용적이면서 실제 프로덕션 레벨에서 쓸만한 패키지가 많은 것은 맞다. 그런데 자바나 Perl에도 그런거 많이 있지 않나? 라고 하면 그것도 맞다. 이러한 경향은 사용하는 사람들이 늘어나다 보니 전체 패키지 갯수가 늘고 실용적인 패키지의 비율이 올라가는 것일 뿐, 요즘같은 프로그래밍 언어, 프레임웍의 춘추전국 시대에서는 수 년 내에 완전히 뒤집히지 말라는 법 또한 없다.
  * `[17]` 원래 언어 쪽에서 Multilingual 과 같은 뜻으로 쓰였으나, 컴퓨터, IT 업계에서는 여러 프로그래밍 언어를 능숙하게 구사하여 적재 적소에 잘 조합하여 쓸 수 있는 능력을 뜻한다.
  * `[18]` 전장에서 일어나는 일을 제외한 나머지 시시콜콜한 일을 다른 코어로 돌리기는 하였으나, 게임의 최소 단위인 전장은 구조상의 한계로 하나의 코어만 동원할 수 있다.
  * `[19]` 하지만, [드롭박스](%EB%93%9C%EB%A1%AD%EB%B0%95%EC%8A%A4.md) 사에서 개발하고 있는 [파이썬](%ED%8C%8C%EC%9D%B4%EC%8D%AC.md)을 프론트엔드로 하고, LLVM을 백엔드로 사용하는 Pyston이 릴리즈되면 별차이 없어질 거란 전망도 나왔다.

