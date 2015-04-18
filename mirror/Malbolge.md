## Contents

    

1. 개요 
2. 상세 
3. Malbolge로 작성된 프로그램 
    

3.1. 실행기

3.2. 예제

[[edit](http://rigvedawiki.net/r1/wiki.php/Malbolge?action=edit&section=1)]

## 1. 개요 ¶

벤 올름스테드(Ben Olemstead)가 1998년에 만든 [난해한 프로그래밍 언어](%EB%82%9C%ED%95%B4%ED%95%9C%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20%EC%96%B8%EC%96%B4.md).
이름은 [단테](%EB%8B%A8%ED%85%8C.md)의 [신곡](%EC%8B%A0%EA%B3%A1.md)에 나오는
[지옥](%EC%A7%80%EC%98%A5.md) 중 제 8옥인 말레볼제(Malebolge)에서 왔다.

  

이름부터가 개념인 이 언어의 가장 큰 특징은, 현존하는 모든 언어중 가장 <del>개같은</del>최악의 [프로그래밍 언어](%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20%EC%96%B8%EC%96%B4.md)라는 것이다.
<del>이 인간은 [변태](%EB%B3%80%ED%83%9C.md)가 틀림없어.</del> 실제로 벤 올름스테드는
Malbolge외에도 Gis라는 난해한 프로그래밍 언어를 만들거나, Esoteric Awards이라는 난해한 프로그래밍 언어 대회 따위를
만들거나 했다. <del>변태.</del>

  

기본적으로 정말 더럽고 어렵고 복잡스럽기때문에, 첫 Malbolge 프로그램이 만들어지기까지 장장 2년이라는 세월이 걸렸다. 그것도 사람의
손으로 쓰여진 것이 아니라, LISP로 구현된 빔 탐색 알고리즘을 통해서 만들어진 것.
[#](http://acooke.org/malbolge.html)  
그 후에도 프로그램이 매우 간간히 제작되었는데, 예를 들자면 Malbolge를 통한 민감한 루프의 구현은 Malbolge가 나온지 7년만에
구현되었다(사실 이것도 처음에는 구현이 가능한지 논란이 있었다).

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Malbolge?action=edit&section=2)]

## 2. 상세 ¶

Malbolge는 3진법 가상 머신인 Malbolge 인터프리터의
[기계어](%EA%B8%B0%EA%B3%84%EC%96%B4.md)이다. a, c, d의 세 레지스터를 사용하는데, 그 중 c
레지스터는 현재 실행되는 명령을 가리키는 특수한 용도로 사용된다. 기본적으로 메모리는 삼진수 숫자로 저장되며, 메모리 공간은 310개인
59049개이다. 이 각각의 공간에는 0부터 59048까지의 주소가 붙어있고, 0부터 59048까지의 값을 저장할 수 있다. 이
Malbolge 프로그램이 시작되기 전에, 메모리의 앞부분이 프로그램으로 채워진다. 프로그램에 들어있는 모든 공백문자는 사라지고, 더욱더
사용자들을 엿먹이기 위해 공백 문자를 제외한 프로그램은 특정한 명령 중 하나로 시작되어야 한다. 나머지 메모리 공간은 Crazy 연산이라는,
이름부터 간지가 넘치는 연산으로 계산한 값으로 채워진다. 이 Crazy 연산의 식은 `[m]=crz[m-2], [m-1]`으로
나타내어지는데, 두 숫자의 각각의 3진법 자리마다 다음의 표를 적용해서 결과를 얻는다. 예를 들자면 crz 0001112220,
0120120120의 결과는 1001022211이 되는 식. 한번 계산해보자.

  

**crz**
**Input 2**

**0**
**1**
**2**

**input 1**
**0**
1

0

0

**1**
1

0

2

**2**
2

2

1

  
명령도 골때리는데, Malbolge에 존재하는 여덞 개의 명령은 `[c]`값에 c를 더하고, 그 값을 94로 나눈 나머지에 따라 어떤 명령을
실행할 지 결정한다. 이때 c는 레지스터 값의 메모리 주소, `[c]`는 그 주소에 저장된 값이다. 여덟 개의 명령에 속하지 않는 모든 값은
그냥 아무것도 하지 않는다.

  

명령이 실행된 후에, 해당 명령은 또 **암호화**가 되어서, 이동 명령이 실행되지 않으면 다음에 실행되었을 때 같은 역할을 하지 않는다!
이동 명령이 실행되면 이동된 위치 바로 앞에 있는 명령이 암호화된다. 암호화 과정도 황당한데, 일단 `[c]`의 값이 94보다 작을 때까지
94를 빼고, 특수한 표에서 결과값을 찾은 후 그 값을 `[c]`에 저장하는 방식. 그런 다음에는 c와 d의 값이 1씩 증가하고 다음 명령이
실행된다.

  

하여튼 개같기로는 이루 말할 수 없는 언어이므로, 변태가 아니면 관심을 가지지 않는게 상책.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Malbolge?action=edit&section=3)]

## 3. Malbolge로 작성된 프로그램 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/Malbolge?action=edit&section=4)]

### 3.1. 실행기 ¶

Malbolge 코드를 실행하기 위한 인터프리터는 다음 주소에서 구할 수 있다:  
<http://www.lscheffer.com/malbolge_interp.html>  
벤 올름스테드가 [C언어](C%28%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20%EC%96%B8%EC%96%B4%29.md)로 구현한 버전이다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Malbolge?action=edit&section=5)]

### 3.2. 예제 ¶

다음은 Malbolge의 [Hello, world!](Hello%2C%20world%21.md) 프로그램이다.

  

`Hello, world.`를 출력하는 버전. 출처: 위키피디아
[#](http://ko.wikipedia.org/wiki/%EB%A7%90%EB%A0%88%EB%B3%BC%EC%A0%9C)  

    
    
    (=<`:9876Z4321UT.-Q+*)M'&%$H"!~}|Bzy?=|{z]KwZY44Eq0/{mlk**hKs_dG5[m_BA{?-Y;;Vb'rR5431M}/.zHGwEDCBA@98\6543W10/.R,+O<

  

`HEllO WORld`를 출력하는 버전. 출처: <http://acooke.org/malbolge.html> `[1]`  

    
    
    (=<`$9]7<5YXz7wT.3,+O/o'K%$H"'~D|#z@b=`{^Lx8%$Xmrkpohm-kNi;gsedcba`_^]\[ZYXWVUTSRQPONMLKJIHGFEDCBA@?>=<;:9876543s+O<oLm

  

[브레인퍽](%EB%B8%8C%EB%A0%88%EC%9D%B8%ED%8D%BD.md) 이나 [Ook!](Ook%21.md),
[비펀지](%EB%B9%84%ED%8E%80%EC%A7%80.md), [화이트스페이스](%ED%99%94%EC%9D%B4%ED%8A%B8%EC%8A%A4%ED%8E%98%EC%9D%B4%EC%8A%A4.md)와 같은 언어들의 경우 그래도 일단 기호가 어떤 역할을 하는지
익히고, 머리좀 싸맬 자신만 있다면 Hello,World! 출력과 같은 간단한 프로그램 정도는 어떻게 동작하는지 프로그램을 분석할 수
있지만.. 이놈은... 진짜 자신이 [뇌](%EB%87%8C.md)
[새디스트](%EC%83%88%EB%94%94%EC%8A%A4%ED%8A%B8.md)가 아닌 이상은 위 코드가 어떻게
Hello,World!란 문장을 출력하는지 알아보려 하지 않는게 좋다. 정말로.

  

Malbolge로 작성된 [99병의 맥주](99%EB%B3%91%EC%9D%98%20%EB%A7%A5%EC%A3%BC.md) 소스
코드.[#](http://www.99-bottles-of-beer.net/language-malbolge-995.html)
<del>핸드폰으로 보지 마라</del> <del>[스압](%EC%8A%A4%EC%95%95.md)</del>

  

`\----`

  * `[1]` 위에서 소개한 Lisp으로 빔 탐색 알고리즘을 구현하여 만들어낸 버전.

