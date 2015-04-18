## Contents

    

1. Private Use Area 
2. Pick Up Artist 

[[edit](http://rigvedawiki.net/r1/wiki.php/PUA?action=edit&section=1)]

## 1. Private Use Area ¶

**[유니코드](%EC%9C%A0%EB%8B%88%EC%BD%94%EB%93%9C.md) 문자 집합의 문자 평면**

Plane 0 - [BMP](BMP#s-3.md)  
0000 ~ FFFF

기본 다국어 평면

Plane 1 - [SMP](SMP#s-4.md)  
10000 ~ 1FFFF

보조 다국어 평면

Plane 2 - [SIP](%ED%95%9C%EC%9E%90/SIP.md)  
20000 ~ 2FFFF

보조 표의문자 평면

Plane 3 - [TIP](TIP.md)  
30000 ~ 3FFFF

삼차 표의문자 평면

Plane 14 - [SSP](SSP.md)  
E0000 ~ EFFFF

보조 특수목적 평면

Plane 15, 16 - [PUA](PUA#s-1.md)  
F0000 ~ 10FFFF

사용자 자유 영역

  

U+E000 ~ U+F8FF, U+F0000 ~ U+10FFFF

  

[유니코드](%EC%9C%A0%EB%8B%88%EC%BD%94%EB%93%9C.md)에서 사용자 정의 영역을 부르는 말. 이 영역에는
특정한 문자가 할당되어 있지 않기 때문에 프로그램 제작자의 의도에 따라 원하는 문자를 배당해서 쓸 수 있다. 때문에 프로그램 간의 호환성이
보장되지 않는다. 예를 들어 같은 U+F0000이어도 프로그램에 따라 다른 문자가 나오는 것이다.

  

대표적으로 [아래아 한글](%EC%95%84%EB%9E%98%EC%95%84%20%ED%95%9C%EA%B8%80.md)에서는 이
영역에 키캡 문자, 한글과컴퓨터 로고 등을 배당해놓았다.

  

아래아 한글에서는 2007 버전까지 옛한글을 처리하기 위해 '한양 PUA'라는 방식을 사용하였다. 이것은 옛한글 글자들을 유니코드의 사용자
정의 영역에 넣어놓았기 때문에 붙여진 이름이다. 하지만 이것은 표준 방식이 아니었고, 이 때문에 2010 버전에서는
[유니코드](%EC%9C%A0%EB%8B%88%EC%BD%94%EB%93%9C.md)와 호환되는 첫가끝(초성-중성-종성) 방식으로
옛한글 처리 방식을 바꾸었다.

  

[애플](%EC%95%A0%ED%94%8C%28%EA%B8%B0%EC%97%85%29.md)의 기기에서만 보이는 애플 로고 문자는,
애플이 이 영역의 끝자락인 U+F8FF에 독자적으로 할당해놓은 문자이다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/PUA?action=edit&section=2)]

## 2. Pick Up Artist ¶

[픽업 아티스트](%ED%94%BD%EC%97%85%20%EC%95%84%ED%8B%B0%EC%8A%A4%ED%8A%B8.md) 항목
참고.

