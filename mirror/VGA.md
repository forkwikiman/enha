## Contents

    

1. 기술 표준으로서의 VGA 
    

1.1. VGA의 컬러 표현 수

2. [그래픽 카드](%EA%B7%B8%EB%9E%98%ED%94%BD%20%EC%B9%B4%EB%93%9C.md)의 약칭 
3. spike Video Game Awards 
    

3.1. 올해의 게임캐릭터상

    

3.1.1. 2010년

3.1.2. 2011년

3.1.3. 2012년

3.1.4. 2013년

[[edit](http://rigvedawiki.net/r1/wiki.php/VGA?action=edit&section=1)]

### 1. 기술 표준으로서의 VGA ¶

Video Graphics Array의 약자. 1987년 [IBM](IBM.md)이 개발하여 아직까지도 거의 모든
[컴퓨터](%EC%BB%B4%ED%93%A8%ED%84%B0.md)에 내장되는 그래픽 카드의 표준으로 규정된 그래픽 표현 방식이다.

  

[CGA](CGA.md), [EGA](EGA.md)와 달리 A가 Adaptor가 아니라 Array인 이유는 여러 개의 이산 논리
칩의 조합으로 그래픽을 표현했던 CGA, EGA와 달리 하나의 칩으로 그래픽 기능을 구현했기 때문이라고 한다. CGA, EGA의 신호전송이
디지털 방식이었던 것과 달리 아날로그 방식을 채용한 것도 차이점이다. 당시의 디지털 방식으로는 한계가 있었기 때문에 이 한계를 극복하고자
아날로그 방식을 채택한 것이었는데 최근에는 다시 디지털 방식인 [DVI](DVI.md)가 표준인 것을 보면 세상은 돌고도는 법인 듯.

  

원래는 IBM의 PS/2(Personal System/2)의 발표와 함께 등장한 새로운 그래픽 카드였으나 PS/2는 MCA 등 폐쇄적인
아키텍처 설계로 인해 시장에서 실패하고 PS/2포트`[1]`와 VGA만 살아남았다. 사실 처음 PS/2에 VGA가 들어갔을 때는 그래픽카드가
아닌 메인보드에 일체화 되어있는 형태였다. 그것을 서드파티 회사`[2]`들이 [리버스 엔지니어링](%EB%A6%AC%EB%B2%84%EC%8A%A4%20%EC%97%94%EC%A7%80%EB%8B%88%EC%96%B4%EB%A7%81.md)(!)을 통해 일반 PC에도 설치
가능한 AT버스의 비디오카드 형태로 만들어낸 것.

  

초기형 VGA는 256kb 비디오 램을 갖고 있었으며 [EGA](EGA.md)의 14색에 독자적으로 16색, 최대 256색을 표현
가능했다. 해상도는 80x25 / 40x25의 텍스트 모드와 640x480 해상도의 16색 모드, 320x200 해상도의 16색 모드,
320x200의 256색 모드를 지원했다. 사실 엄밀한 의미에서의 VGA는 이 초기형의 표준을 가리키는 것.

  

이후로 VGA의 틀을 갖춘 채로 계속 개량되어 800x600 해상도를 지원하는 Super VGA, 1024x768 해상도를 지원하는 XGA
등이 나오고 컬러 표현도 2의 제곱으로 28(256)가지 색을 지원하던 8비트 초기형에서 65,536 컬러를 지원하는 16비트 컬러까지,
현재는 해상도에 상관없이 232가지 색을 지원하는 32비트 컬러를 가장 보편적으로 쓰고 있다. `[3]`

  

[[edit](http://rigvedawiki.net/r1/wiki.php/VGA?action=edit&section=2)]

#### 1.1. VGA의 컬러 표현 수 ¶

VGA의 컬러 표현에서 'xx비트'라는 것은 2의 제곱수에 의해 결정된다. 즉 256색은 2의 8제곱으로 '8비트'이며 32비트의 경우에는
2의 32제곱으로 4,294,967,296가지 컬러를 표현할 수 있다는 뜻이다. 256색까지는 모니터에 전송 가능한 24비트, 224가지의
신호 경우의 수 중 256가지를 그래픽 메모리`[4]`에 팔레트처럼 지정하여 사용하는 식으로 사용되었지만 16비트부터는 3원색(적, 녹,
청)의 비율을 직접 지정하는 방식을 사용할 수 있게 되었다. 예를 들어 16비트는 R,G,B가 5-5-5(1비트는 버림, 변형으로
5-6-5)비율로, 24비트는 8-8-8, 32비트는 24비트 방식의 8-8-8에 투명도(알파)를 나타내는 8비트(256단계)를 추가해서 총
32비트를 쓰는 식이다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/VGA?action=edit&section=3)]

### 2. [그래픽 카드](%EA%B7%B8%EB%9E%98%ED%94%BD%20%EC%B9%B4%EB%93%9C.md)의 약칭 ¶

너무 표준이 되어버렸기 때문에 이후에 개발되는 모든 그래픽 카드가 VGA라는 호칭을 수용한다. 이름이 'Video'라는 범용적인 명칭인 것도
한 몫 했다.

  

  * 주요 회사  

    * [nVIDIA](nVIDIA.md)
    * [AMD](AMD.md)(구 [ATI](ATI.md))
    * [매트록스](%EB%A7%A4%ED%8A%B8%EB%A1%9D%EC%8A%A4.md)  

[[edit](http://rigvedawiki.net/r1/wiki.php/VGA?action=edit&section=4)]

### 3. spike Video Game Awards ¶

spike TV가 해마다 주최하는 [패키지게임](%ED%8C%A8%ED%82%A4%EC%A7%80%20%EA%B2%8C%EC%9E%84.md)과 [비디오게임](%EB%B9%84%EB%94%94%EC%98%A4%20%EA%B2%8C%EC%9E%84.md) 수상제이다. 2003년도에
시작하여 라이브 음악 공연과 TV,영화,음악계의 유명인사들의 진행 등으로 유명해졌으며, 무엇보다 출시 예정인 게임들의 트레일러가 우수수
쏟아져 나오므로 [겜덕후](%EA%B2%9C%EB%8D%95%ED%9B%84.md)들에겐 가히 축제중의 축제라 할만하다. 수상식은
[GameTrailers](GameTrailers.md) TV의 제프 킬리(Geoff Keighley)가 진행하며, 매년
[로스앤젤레스](%EB%A1%9C%EC%8A%A4%EC%95%A4%EC%A0%A4%EB%A0%88%EC%8A%A4.md),
[샌타모니카](%EC%83%8C%ED%83%80%EB%AA%A8%EB%8B%88%EC%B9%B4.md),
[라스베이거스](%EB%9D%BC%EC%8A%A4%EB%B2%A0%EC%9D%B4%EA%B1%B0%EC%8A%A4.md),
[네바다](%EB%84%A4%EB%B0%94%EB%8B%A4.md) 등 다양한 지역에서 개최된다. 2013년부터는 차세대 Video
Game Award라는 뜻으로 수장제의 이름을 _VGX_로 변경하였다.

  

같은 이름을 가지고 있는 Video Games AWESOME!(VGA)라는 비디오 게이밍 웹 시리즈가 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/VGA?action=edit&section=5)]

#### 3.1. 올해의 게임캐릭터상 ¶

2010년부터 올해의 게임캐릭터상을 제정, 우승자를 포함해 매년 네다섯 명씩을 소개해왔는데, 게임성과 캐릭터성을 고려한 적절한 개그로 많은
이들의 웃음을 자아내고 있다. 위키러들의 쾌적한 인터넷 환경을 위해 영상은 링크로 대체한다.

  

당연한 이야기이지만, 참고로 VGA의 "올해의 게임상"과 "올해의 게임캐릭터상"은 각각 다른 부문에서의 수상이기 때문에 캐릭터성이 옅다든가
수상식 직전에 발매되어 특전영상을 만들 틈이 없다든가(...), 다른 쟁쟁한 후보들과의 경쟁에서 밀린다는 등의 이유로 후보에조차 들어가지
못하는 게임&캐릭터가 상당히 많다. 예를 들어 2011년 발매된 [엘더스크롤 5: 스카이림](%EC%97%98%EB%8D%94%EC%8A%A4%ED%81%AC%EB%A1%A4%205%3A%20%EC%8A%A4%EC%B9%B4%EC%9D%B4%EB%A6%BC.md)의
[도바킨](%EB%8F%84%EB%B0%94%ED%82%A8.md)이나 2013년에 발매된 [크라이시스3](%ED%81%AC%EB%9D%BC%EC%9D%B4%EC%8B%9C%EC%8A%A4%203.md)의 [알카트라즈(크라이시스2)](/
wiki/%EC%95%8C%EC%B9%B4%ED%8A%B8%EB%9D%BC%EC%A6%88%28%ED%81%AC%EB%9D%BC%EC%9D%
B4%EC%8B%9C%EC%8A%A42%29)만 봐도 그렇다.

[[edit](http://rigvedawiki.net/r1/wiki.php/VGA?action=edit&section=6)]

##### 3.1.1. 2010년 ¶

  * 우승   
[프랭크 우즈](%ED%94%84%EB%9E%AD%ED%81%AC%20%EC%9A%B0%EC%A6%88.md)/[콜 오브 듀티: 블랙 옵스](%EC%BD%9C%20%EC%98%A4%EB%B8%8C%20%EB%93%80%ED%8B%B0%3A%20%EB%B8%94%EB%9E%99%20%EC%98%B5%EC%8A%A4.md) [#](http://www.youtube.com/watch?v=kY5vvi0Ddpk)  

  * 후보   
[크레토스](%ED%81%AC%EB%A0%88%ED%86%A0%EC%8A%A4.md)/[갓 오브워](%EA%B0%93%20%EC%98%A4%EB%B8%8C%20%EC%9B%8C.md) 3 [여러모로
위험했다;;](http://www.youtube.com/watch?v=7sXpwMIecUM&list=PL2B9B0D3B712D1BF7)  
[존 마스턴](%EB%A0%88%EB%93%9C%20%EB%8D%B0%EB%93%9C%20%EB%A6%AC%EB%8E%80%EC%85%98/%EB%93%B1%EC%9E%A5%EC%9D%B8%EB%AC%BC.md)/[레드 데드 리뎀션](%EB%A0%88%EB%93%9C%20%EB%8D%B0%EB%93%9C%20%EB%A6%AC%EB%8E%80%EC%85%98.md) 영상 추가바람  
[에치오 아우디토레](%EC%97%90%EC%B9%98%EC%98%A4%20%EC%95%84%EC%9A%B0%EB%94%94%ED%86%A0%EB%A0%88.md)/[어쌔신 크리드 : 브라더후드](%EC%96%B4%EC%8C%94%EC%8B%A0%20%ED%81%AC%EB%A6%AC%EB%93%9C%20%3A%20%EB%B8%8C%EB%9D%BC%EB%8D%94%ED%9B%84%EB%93%9C.md)
<del>[수상식에서도 템플러의 위험성을 강조하시는 직업정신!</del>](http://www.youtube.com/watch?v=aLm6b
aXBtaY&list=PL2B9B0D3B712D1BF7&feature=player_embedded)  

[[edit](http://rigvedawiki.net/r1/wiki.php/VGA?action=edit&section=7)]

##### 3.1.2. 2011년 ¶

  * 우승  
[조커](%EC%A1%B0%EC%BB%A4%28DC%20%EC%BD%94%EB%AF%B9%EC%8A%A4%29/%EC%95%84%EC%BA%84%EB%B2%84%EC%8A%A4.md)/[배트맨: 아캄 시티](%EB%B0%B0%ED%8A%B8%EB%A7%A8%3A%20%EC%95%84%EC%BA%84%20%EC%8B%9C%ED%8B%B0.md) [#](http://www.youtube.com/watch?v
=iCrmj-r7WjE)  

  * 후보  
[네이선 드레이크](%EB%84%A4%EC%9D%B4%EC%84%A0%20%EB%93%9C%EB%A0%88%EC%9D%B4%ED%81%AC.md)/[언차티드 3](%EC%96%B8%EC%B0%A8%ED%8B%B0%EB%93%9C%203.md) <del>[이제 오줌이나
마셔야겠군</del>](http://www.youtube.com/watch?v=iCrmj-r7WjE)  
[마커스피닉스](%EB%A7%88%EC%BB%A4%EC%8A%A4%20%ED%94%BC%EB%8B%89%EC%8A%A4.md)/[기어즈 오브워 3](%EA%B8%B0%EC%96%B4%EC%A6%88%20%EC%98%A4%EB%B8%8C%20%EC%9B%8C%203.md)
[올ㅋ 좋은무기 getㅋ](http://www.youtube.com/watch?v=XZKFIeaQvaw)  
[휘틀리](%ED%9C%98%ED%8B%80%EB%A6%AC.md)/[포탈 2](%ED%8F%AC%ED%83%88%202.md)
[뀨잉뀨잉](http://www.youtube.com/watch?v=MXS-PYsxoLQ)  

[[edit](http://rigvedawiki.net/r1/wiki.php/VGA?action=edit&section=8)]

##### 3.1.3. 2012년 ¶

  * 우승  
[CL4P-TP](CL4P-TP.md)/[보더랜드2](%EB%B3%B4%EB%8D%94%EB%9E%9C%EB%93%9C%202.md)
[#](http://www.youtube.com/watch?v=3GE24TPoWg0)  

  * 후보  
[코너 켄웨이](%EC%BD%94%EB%84%88%20%EC%BC%84%EC%9B%A8%EC%9D%B4.md)/[어쌔신 크리드3](%EC%96%B4%EC%8C%94%EC%8B%A0%20%ED%81%AC%EB%A6%AC%EB%93%9C%203.md)
<del>[트로피도 무기로 써버리는 위엄</del>](http://www.youtube.com/watch?v=dcUwhFYEqro)  
[셰퍼드 소령](%EC%85%B0%ED%8D%BC%EB%93%9C%20%EC%86%8C%EB%A0%B9.md)/[매스 이펙트3](%EB%A7%A4%EC%8A%A4%20%EC%9D%B4%ED%8E%99%ED%8A%B8%203.md) <del>[이중자아</del
>](http://www.youtube.com/watch?feature=player_embedded&v=8dXj67VXjwU#!)  
[마스터 치프](%EB%A7%88%EC%8A%A4%ED%84%B0%20%EC%B9%98%ED%94%84.md)/[헤일로4](%ED%97%A4%EC%9D%BC%EB%A1%9C%204.md) [역대 최고로
과묵하다.](http://www.youtube.com/watch?v=xHDSJTKwQtE)  
[라울 메넨데즈](%EB%9D%BC%EC%9A%B8%20%EB%A9%94%EB%84%A8%EB%8D%B0%EC%A6%88.md)/[콜오브 듀티: 블랙 옵스 2](%EC%BD%9C%20%EC%98%A4%EB%B8%8C%20%EB%93%80%ED%8B%B0%3A%20%EB%B8%94%EB%9E%99%20%EC%98%B5%EC%8A%A4%202.md) [끔살당한다!/<del>우즈 하사의
수상욕심</del>](http://www.youtube.com/watch?v=jDy5bB9V82E)  

[[edit](http://rigvedawiki.net/r1/wiki.php/VGA?action=edit&section=9)]

##### 3.1.4. 2013년 ¶

[캐릭터별로 분리된 영상을 찾을 수 없어 편의상 영상모음으로
대체한다.](https://www.youtube.com/watch?v=BPeD_nuK0Uo)  

  * 우승   
[루테스 남매](%EB%A3%A8%ED%85%8C%EC%8A%A4%20%EB%82%A8%EB%A7%A4.md)/[바이오쇼크 인피니트](
/wiki/%EB%B0%94%EC%9D%B4%EC%98%A4%EC%87%BC%ED%81%AC%20%EC%9D%B8%ED%94%BC%EB%8B
%88%ED%8A%B8)  

  * 후보  
[라라 크로프트(2013)](%EB%9D%BC%EB%9D%BC%20%ED%81%AC%EB%A1%9C%ED%94%84%ED%8A%B8%282013%29.md)/[툼레이더(2013)](%ED%88%BC%20%EB%A0%88%EC%9D%B4%EB%8D%94%282013%29.md)  
[트레버필립스](%ED%8A%B8%EB%A0%88%EB%B2%84%20%ED%95%84%EB%A6%BD%EC%8A%A4.md)/[GTA5](GTA%205.md)  
Naiee와 Nyaa 형제/Brothers: A Tale of Two Sons`[5]`

`\----`

  * `[1]` 키보드와 마우스를 연결하는 그것
  * `[2]` Tseng Labs가 대표적이었으며, Tseng Labs가 1987년에 발표한 ET3000은 SVGA 사양 까지도 만족했다고 한다.
  * `[3]` 32비트 컬러는 엄밀하게는 232가 아닌 224(=16,777,216)컬러를 지원한다. RGB의 세 채널에 8비트씩, 그리고 알파채널(투명도)에 8비트가 할당되므로 24비트가 되는 것. 참고로 채널당 10비트씩을 할당하여 230, 약 10억 컬러를 표현 가능한 그래픽 카드도 있는데 의료 등 좀 특수한 용도에 쓰는 경우가 많다.
  * `[4]` 당시 1MB 시스템 내에 따로 할당된 VGA용 공간
  * `[5]` 스타브리즈 스튜디오에서 2013년 Xbox라이브와 스팀, 플레이스테이션 네트워크를 통해 발매한 퍼즐 플랫폼 어드벤처 장르의 인디 게임이다. 개별항목이 추가되면 수정바람.

