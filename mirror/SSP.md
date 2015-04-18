**[유니코드](%EC%9C%A0%EB%8B%88%EC%BD%94%EB%93%9C.md) 문자 집합의 문자 평면**

Plane 0 - [BMP](BMP.md)  
0000~FFFF

Plane 1 - [SMP](SMP.md)  
10000~1FFFF

Plane 2 - [SIP](SIP.md)  
20000~2FFFF

Plane 3 - [TIP](TIP.md)  
30000~3FFFF

Plane 14 - [SSP](SSP.md)  
E0000~EFFFF

Plane 15,16 - [PUA](PUA.md)  
F0000~10FFFF

기본 다국어 평면

보조 다국어 평면

보조 표의문자 평면

삼차 표의문자 평면

보조 특수목적 평면

사용자 자유 영역

[유니코드](%EC%9C%A0%EB%8B%88%EC%BD%94%EB%93%9C.md) 문자 집합의 열 다섯 번째`[1]``[2]` 문자
평면. 7.0 버전 현재로는 아래의 두 개의 문자 집합만 정의되어 있으며, UTF-8 기준으로 모두 4바이트를 사용하여 표현된다.`[3]`

  * [태그](%ED%83%9C%EA%B7%B8.md)(U+E0000 ~ U+E007F)
  * 모양 구별 문자 보충(U+E0100 ~ U+E01EF)  

여기서 태그는 [HTML](HTML.md) 태그 같은 것이 아니고(...) 일종의 제어 문자다.

`\----`

  * `[1]` [유니코드 홈페이지](http://www.unicode.org/roadmaps/ssp/)에 Plane 14라고 명시되어 있다. 즉, [TIP](TIP.md)(Plane 3)와 SSP 사이에 새로운 평면이 추가될 것을 예고하고 있는 셈. <del>[한자](%ED%95%9C%EC%9E%90.md)라든가 한자라든가 한자라든가</del>
  * `[2]` 사실 한자를 제외하더라도 유니코드에 추가되어 있지 않은 문자 체계가 많다. [서하 문자](%EC%84%9C%ED%95%98%20%EB%AC%B8%EC%9E%90.md)가 대표적.
  * `[3]` [BMP](BMP.md) 밖의 문자는 모두 4바이트로 표현되는 문자다.

