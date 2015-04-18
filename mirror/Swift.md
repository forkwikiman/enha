  * 이 글에서는 [애플](%EC%95%A0%ED%94%8C%28%EA%B8%B0%EC%97%85%29.md) 사의 [프로그래밍 언어](%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20%EC%96%B8%EC%96%B4.md)에 대해 설명하고 있습니다. 일반적인 의미는 [스위프트](%EC%8A%A4%EC%9C%84%ED%94%84%ED%8A%B8.md)를 참조하십시오.  

![http://upload.wikimedia.org/wikipedia/en/4/43/Apple_Swift_Logo.png?width=130
&align=right](http://upload.wikimedia.org/wikipedia/en/4/43/Apple_Swift_Logo.p
ng)

[[PNG external
image]](http://upload.wikimedia.org/wikipedia/en/4/43/Apple_Swift_Logo.png)

  

## Contents

    

1. 개요 
2. 기타 

[[edit](http://rigvedawiki.net/r1/wiki.php/Swift?action=edit&section=1)]

# 1. 개요 ¶

2014 [WWDC](WWDC.md)에서 공개된(...) 프로그래밍 언어.  

![https://lh6.googleusercontent.com/-gSschZO19ys/U6CEBe9sQZI/AAAAAAAAjMI/OWsFg
eoqkH4/w600-h399-no/dev_01-1.jpg?width=640](https://lh6.googleusercontent.com/
-gSschZO19ys/U6CEBe9sQZI/AAAAAAAAjMI/OWsFgeoqkH4/w600-h399-no/dev_01-1.jpg)

[[JPG external image]](https://lh6.googleusercontent.com/-gSschZO19ys/U6CEBe9s
QZI/AAAAAAAAjMI/OWsFgeoqkH4/w600-h399-no/dev_01-1.jpg)

  

기존 [Objective-C](Objective-C.md)의 단점을 보완하며, 같은 [LLVM](LLVM.md)컴파일러로 빌드되며
같은 런타임을 사용하는 애플의 신규 언어체계이다. 기존 [Objective-C](Objective-C.md)에 비해
[클로저](%ED%81%B4%EB%A1%9C%EC%A0%80.md), 다중 리턴 타입, 네임스페이스, 제네릭스, 타입 인터페이스,
타입추론에 기반한 문법, 연산자 오버로딩 및 생성 등 Objective-C에는 없었던 현대 프로그래밍 언어가 갖고 있는 기능을 많이
포함시켰으며, 이에 따라 일정한 성능향상을 보이고 있다.

  

<del>의외로 애플답지 않게</del> 어느정도 하위호환성도 보장하고 있어, 코드 내부에서 [C](C%28%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20%EC%96%B8%EC%96%B4%29.md)나 Objective-C 코드를
섞던지, 스크립트 언어처럼 프로그래밍 할 수 있게 되어있기도 하다.

  

![http://rigvedawiki.net/r1/wiki.php/%EC%8A%A4%EC%9C%84%ED%94%84%ED%8A%B8%28%E
D%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20%EC%96%B8%EC%96%B4%29?action=dow
nload&value=swift_objc_python_comparison.png?width=640](//rv.wkcdn.net/http://
rigvedawiki.net/r1/wiki.php/%EC%8A%A4%EC%9C%84%ED%94%84%ED%8A%B8%28%ED%94%84%E
B%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20%EC%96%B8%EC%96%B4%29?action=download&val
ue=swift_objc_python_comparison.png)

[[PNG external image]](http://rigvedawiki.net/r1/wiki.php/%EC%8A%A4%EC%9C%84%E
D%94%84%ED%8A%B8%28%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20%EC%96%B8%E
C%96%B4%29?action=download&value=swift_objc_python_comparison.png)

  

WWDC에서 연설로는 기존 Object-C 대비 1.5배, [파이썬](%ED%8C%8C%EC%9D%B4%EC%8D%AC.md) 대비
200배라고 주장하지만, 당연히 파이썬은 인터프리터 언어이므로 목적 자체가 틀려 1:1비교대상이 아닌데다가 일부러 다중 멀티쓰레드로 비교해서
싱글쓰레드 위주의 파이썬을 느리다고 까고 있으므로 저걸 믿으면 [골룸](%EA%B3%A8%EB%A3%B8.md).

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Swift?action=edit&section=2)]

# 2. 기타 ¶

<del>Objective-C 기초강의를 배우던 수많은 사람들이 발표회 이후로 절규하고 있다. 아아 난 그 동안 뭘 배운거야</del>  

![http://lh6.googleusercontent.com/-HvDG1sBU3ew/U6CDk-mtNSI/AAAAAAAAjL8/43O8yk
AkrSo/s0/BpJXGeiIMAAP7If.jpg?width=640](http://lh6.googleusercontent.com/-HvDG
1sBU3ew/U6CDk-mtNSI/AAAAAAAAjL8/43O8ykAkrSo/s0/BpJXGeiIMAAP7If.jpg)

[[JPG external image]](http://lh6.googleusercontent.com/-HvDG1sBU3ew/U6CDk-
mtNSI/AAAAAAAAjL8/43O8ykAkrSo/s0/BpJXGeiIMAAP7If.jpg)

