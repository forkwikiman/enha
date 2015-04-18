## Contents

    

1. 개요 
    

1.1. 브랜드 - [라데온](%EB%9D%BC%EB%8D%B0%EC%98%A8.md)

1.2. 생산방식

1.3. 네이밍 방식

2. ATI의 기술 
    

2.1. [크로스파이어](%ED%81%AC%EB%A1%9C%EC%8A%A4%ED%8C%8C%EC%9D%B4%EC%96%B4.md)

2.2. 친 ATI 게임

2.3. 드라이버

2.4. AVIVO

2.5. [GPGPU](GPGPU.md)

2.6. [Eyefinity](%EC%95%84%EC%9D%B4%ED%94%BC%EB%8B%88%ED%8B%B0.md)

2.7. TrueAudio

3. 칩셋 일람 
4. 그 외 
5. ATI 브랜드의 끝 

[[edit](http://rigvedawiki.net/r1/wiki.php/ATI?action=edit&section=1)]

## 1. 개요 ¶

![HQ.jpg](//z.enha.kr/http://rigvedawiki.net/r1/pds/HQ.jpg)

[JPG image (15.28 KB)]

  

현재는 [AMD](AMD.md)의 그래픽사업부로 합병된 회사. AMD의 그래픽사업부 항목은 이 항목에서 설명한다.

  

ATI란 명칭은 **A**rray **T**echnology **I**ndustry의 약어로, 1985년에 중국의 투자자 3명이
[캐나다](%EC%BA%90%EB%82%98%EB%8B%A4.md)에 설립한 회사가 기원이다. 창업자금 30만 달러를 가지고 만들만한
제품을 찾다가 그래픽카드 시장을 주목하게 되었고, 이후 OEM 시장에 물건을 공급하는 방식으로 성장 전략을 찾았다.

  

2006년 6월, AMD에게 인수되어 동일연도 연말에 합병하였으나, 운영은 독립적으로 하고 있다. 저명한 사이트 뻥콰...아니,
인콰이어러(the inquirer)는 합병한 이 회사 이름을 **DAAMIT**(AMD+ATI)이라고 부르고 있다. <del>절대
**DAMN IT**이 아니다.</del> 현재는 [nVIDIA](nVIDIA.md)와 라이벌 관계의 회사.

  

게임에 대해 엔비디아와, 동영상에 대해 ATI의 기술이 서로 비슷한 수준에 이르러서 새로운 차이점을 만들어내야했고, 엔비디아가 GPGPU의
기술에 대한 연구와 3D 비전에 대한 기술 지원을 하는 한편, ATI는 딱히 다른 걸 하지 않는 듯 했지만, 5XXX 시리즈에서 기존의 듀얼
모니터만을 사용할 수 있던 걸 트리플 이상의 다중 모니터가 사용하게 만들면서 그쪽으로 방향을 잡았다는 걸 알 수 있게 됐다. ...엔비디아가
큰일났다기보다는 [매트록스](%EB%A7%A4%ED%8A%B8%EB%A1%9D%EC%8A%A4.md)가 잘못하면 망할지도.(...)

  

하지만, 파헬리아 시리즈 이후 매트록스는 일반유저용 시장에서 손을 놔버렸고, 이후 파헬리아의 마이너 버전인 P600 시리즈를 출시하기도
했지만, 성능은 말 그대로 안습...`[1]`

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ATI?action=edit&section=2)]

### 1.1. 브랜드 - [라데온](%EB%9D%BC%EB%8D%B0%EC%98%A8.md) ¶

2014년 시점에서는 더 이상 [그래픽카드](%EA%B7%B8%EB%9E%98%ED%94%BD%20%EC%B9%B4%EB%93%9C.md)에만 사용하지 않는 브랜드이다.
자세한 사항은 [라데온](%EB%9D%BC%EB%8D%B0%EC%98%A8.md) 참조.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ATI?action=edit&section=3)]

### 1.2. 생산방식 ¶

[nVIDIA](nVIDIA.md)와 마찬가지로, 주로 설계만 담당하고 생산은 다른 곳에서 맡기는
[팹리스](%ED%8C%B9%EB%A6%AC%EC%8A%A4.md) 회사이다. AMD에 인수된 이후는 AMD fabs에서도 일부 제품을
생산하고 있다.

  

그러나 최신 기술인 40nm공정을 맡았던 [TSMC](TSMC.md)의 불만족스러운 생산 수율로 인해 2010년 이후에 등장할 공정인
32nm나 28nm 칩셋은 ATI에서 분사해서 만들어진 파운드리 회사인 [글로벌 파운드리](%EA%B8%80%EB%A1%9C%EB%B2%8C%20%ED%8C%8C%EC%9A%B4%EB%93%9C%EB%A6%AC.md)에서 새로 제작중이라는 그래픽 칩셋용 생산라인으로 옮겨갈
가능성이 높다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ATI?action=edit&section=4)]

### 1.3. 네이밍 방식 ¶

라데온 제품군은 하이엔드는 R~숫자, 메인스트림이나 보급형 제품은 RV~숫자 형식의 코어 네이밍 방식을 사용했다. 그러나 현재는
RVxxx만을 개발한다. Rxxx 등급의 제품은 RVxxx 코어를 2개 꽂아서 성능을 높이는 방법을 사용중.

  

RV870부터는 번호가 아니라 이름을 붙이고 있다. 예를 들어 RV870은 사이프레스(cypress)로 부르고 RV860은
주니퍼(Juniper)로 부르는 것이다. 뭐하러 이런 귀찮은 짓을 하냐면 번호로 부르면 대충 봐도 경쟁사에서 그 제품의 성능을 짐작할 우려가
있기 때문이다. 정보공개를 극도로 꺼리는 <del>연막덕후</del>ATI답다. 심지어는 개발팀 내에서도 정보를 숨겨서(Eyefinity
항목 참조) 정작 드라이버를 만드는 소프트웨어팀을 패닉상태에 빠트리기도 했다.

  

**자네 이런 걸 전에 본 적이 있나?**  

![http://pds11.egloos.com/pds/200809/07/81/d0053681_48c3c8d42586e.gif](//z.enh
a.kr/http://pds11.egloos.com/pds/200809/07/81/d0053681_48c3c8d42586e.gif)

[[GIF external
image]](http://pds11.egloos.com/pds/200809/07/81/d0053681_48c3c8d42586e.gif)

  

[nVIDIA](nVIDIA.md)가 그래픽 코어를 GPU라고 부르는데 반해, ATI는 VPU라고 부른다. 특별한 의미의 차이는 없다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ATI?action=edit&section=5)]

## 2. ATI의 기술 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/ATI?action=edit&section=6)]

### 2.1.
[크로스파이어](%ED%81%AC%EB%A1%9C%EC%8A%A4%ED%8C%8C%EC%9D%B4%EC%96%B4.md) ¶

[크로스파이어](%ED%81%AC%EB%A1%9C%EC%8A%A4%ED%8C%8C%EC%9D%B4%EC%96%B4.md) 항목 참고.

  

![P091104002.jpg](//z.enha.kr/http://rigvedawiki.net/r1/pds/P091104002.jpg)

[JPG image (33.32 KB)]

  
`[2]`  
참고로 ATI는 2D게임인 **[미연시](%EB%AF%B8%EC%97%B0%EC%8B%9C.md)**에서도 CF를 지원하는 굉장한
모습을 보여주고 있다. <del>근데 CF 지원해봤자 3D가 되는 것도 아니잖아</del>

  

뭐 ATI가 나서서 지원한 게 아니니 ATI는 관계 없는 일이긴 하다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ATI?action=edit&section=7)]

### 2.2. 친 ATI 게임 ¶

![ati_logo_game.jpg](//z.enha.kr/http://rigvedawiki.net/r1/pds/ati_logo_game.j
pg)

[JPG image (8.44 KB)]

최근에서야 ATI와의 기술교류를 통한 친 ATI 게임들이 등장하기 시작하였다.  
대표적인 예로는 [C9](C9.md)이 있으며, 앞으로 나올
[블리자드](%EB%B8%94%EB%A6%AC%EC%9E%90%EB%93%9C.md)의 [스타크래프트2](%EC%8A%A4%ED%83%80%ED%81%AC%EB%9E%98%ED%94%84%ED%8A%B8%202.md)와 [디아블로3](%EB%94%94%EC%95%84%EB%B8%94%EB%A1%9C%203.md) 또한 친 ATI 노선을 선언했다.  
대체적으로 [하복 엔진](%ED%95%98%EB%B3%B5%20%EC%97%94%EC%A7%84.md)이 적용된 게임이 친 ATI
노선이라고 보면 된다.

  

2010년 9월 현재 블리자드의 친 ATI 노선은 그냥 흐지부지된 모양이다. 라데온 최적화로 나올 거라 예상되었던 스타크래프트 2가 특별히
그런 모습을 보이지 않고 있다. 오히려 '스타크래프트 2: 자유의 날개'는 엔비디아와 블리자드가 공동 프로모션을 열었을 정도. 하복 물리
엔진은 인텔 소유이기 때문에 AMD 라데온과 이쪽을 연결시켜 생각하는 것도 좀 머쓱한 상황. PhysX와 주로 엮이는 언리얼 엔진이 경우,
그 PhysX는 아예 Nvidia아니면 구동조차 되지않는 경우와는 달리 하복 엔진은 라데온에서도 멀쩡히 돌아가므로 상대적으로 하복 엔진은
라데온과 친하다는 구도로 보이는 것도 있다.

  

다만 현재 2013년 시점에서에선 의외로 최소 프레임 유지능력에선 엔비디아에 비해 꽤 우월한 모습을 보여 주고는 있다.  
이 외에도 툼 레이더, 더트, 히트맨, 크라이시스3, 배틀필드 4 등에서도 선전하는 모습을 보이고 있는데,  
이는 쉐이더 쪽에 치중하는 게임 특성상 케플러 대비 GCN쪽이 힘을 쓰기가 쉬워서이기도 하다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ATI?action=edit&section=8)]

### 2.3. 드라이버 ¶

본 항목의 본문은 [카탈리스트(소프트웨어)](%EC%B9%B4%ED%83%88%EB%A6%AC%EC%8A%A4%ED%8A%B8%28%EC%86%8C%ED%94%84%ED%8A%B8%EC%9B%A8%EC%96%B4%29.md)입니다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ATI?action=edit&section=9)]

### 2.4. AVIVO ¶

nVDIA의 퓨어비디오와 비슷한 역할을 맡는 기술로 블루레이나 TP등 초고화질영상의 재생을 도와주기도 하며 잔상을 줄이고 색감을 개선하는
등의 역할도 맡는다. NVDIA와 달리 ATI에서 제공하는 프로그램만 설치해줘도 작동한다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ATI?action=edit&section=10)]

### 2.5. [GPGPU](GPGPU.md) ¶

그래픽 카드 라인업에 GPGPU에 특화된 FireStream을 보유하고 있다. 세계 최초 배정밀도 소수연산을 지원하는 라인업이라는 타이틀을
가지고 있으며, **RVxxx 칩을 GPGPU에 특화시켜서 개조한 것**이므로 해당 칩을 사용하는 카드와 성능과 특성이 동일하다. (사실
**FireGL도 똑같이 RVxxx 칩을 [OpenGL](OpenGL.md)에 특화시켜서 개조한 것**이다. 칩셋 하나로 대체 어디까지
가는 거냐 ATI...)사실 알고보면 그냥 드라이버 차이뿐이고 FireGL은 기판에 전용 출력포트가 있다는 점을 제외하고 동일하며
FireStream에 가서는 기존 제품군과 VRAM용량과 클럭 수준말고는 더 차이가 없어서 오히려 기업체에 대한 공식기술지원을 보장한
카드라고 보면 된다. 전용 드라이버를 일반제품군에 깔리게하는 개조로 FireGL이나 FireStream을 써볼 수 있다는것도 특징.`[3]`

  

지원 솔루션으로 자체 GPGPU 개발 SDK인 CAL과 Brook+을 보유하고 있으며`[4]`, nVIDIA가 자체 GPGPU 솔루션인
CUDA를 미는 것과는 달리 개방형 표준인 [OpenCL](OpenCL.md)과 [DirectX](DirectX.md) 11을
적극적으로 밀어줄 것을 선언했다.

  

최근 5XXX 시리즈의 실적으로 숨통이 좀 트였는지, 엔비디아처럼 적극적으로 개발자들을 포섭하기로 발표했다. 가령 <del>돈을
쥐어주고</del>. 그러나 엔비디아에 비하면 아직 갈길이 먼 게 사실.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ATI?action=edit&section=11)]

### 2.6. [Eyefinity](%EC%95%84%EC%9D%B4%ED%94%BC%EB%8B%88%ED%8B%B0.md) ¶

[항목 참고](%EC%95%84%EC%9D%B4%ED%94%BC%EB%8B%88%ED%8B%B0.md)

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ATI?action=edit&section=12)]

### 2.7. TrueAudio ¶

어지간한 [사운드 카드](%EC%82%AC%EC%9A%B4%EB%93%9C%20%EC%B9%B4%EB%93%9C.md)도 못하는
**음원 가속 기능**을 지원한다. <del>어?</del> 다만 2014년 시점에서는 R 200 시리즈의 일부 제품`[5]`만 지원한다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ATI?action=edit&section=13)]

## 3. 칩셋 일람 ¶

  * [AMD 칩셋 일람](AMD%20%EC%B9%A9%EC%85%8B%20%EC%9D%BC%EB%9E%8C.md) \- 메인보드용 ATI 칩셋 항목 포함
  * [AMD GPU 일람](AMD%20GPU%20%EC%9D%BC%EB%9E%8C.md).  

[[edit](http://rigvedawiki.net/r1/wiki.php/ATI?action=edit&section=14)]

## 4. 그 외 ¶

블리자드에서 ATI 지원 중. 이에 맞춰 [월드 오브 워크래프트](%EC%9B%94%EB%93%9C%20%EC%98%A4%EB%B8%8C%20%EC%9B%8C%ED%81%AC%EB%9E%98%ED%94%84%ED%8A%B8.md)의 확장팩인 [리치왕의분노](%EB%A6%AC%EC%B9%98%EC%99%95%EC%9D%98%20%EB%B6%84%EB%85%B8.md) 발매와 맞춰
라데온 HD 4670을 발매한 뒤 WOW에 최적화되어 있다고 광고, 판매하며 경품 이벤트를 실시하기도 했었다.

  

사실 WOW는 CPU빨을 더 먹는 게임이라 엔비디아든 ATI든 아무래도 상관없고(...) 이후에 나올 스타2나 디아3가 영향을 크게 받지
않을까 예측되고 있다. 스타2의 경우 하복 물리 엔진을 사용한다고 한다. 하지만 출시하고보니 별반 차이도 없다.

  

다만 ATI는 장기적인 관점에서 볼 때, 독자 엔진인 피직스로 가고 있는 엔비디아보다 하복 엔진에 대해 유리하다. 현재 공식적으로 하복
엔진을 지원하는 게 아니고, 앞으로 [인텔](%EC%9D%B8%ED%85%94.md), [AMD](AMD.md)가 하복 엔진에
대한 지원을 늘림과 동시에 하복 엔진을 정식적으로 지원한다는 개념이기 때문이다. (단, [엔비디아](nVIDIA.md)가 하복 엔진도
지원하겠다고 선언하고 그렇게 실행한다면 어떻게 될지 모를 일이다. 하복 엔진은 ATI가 만든 게 아니고 엔비디아 카드로 지원 불가능한 건
아니니까. 단지 그럴 가능성은 사실상 없을 거다.)

  

한편 요즘 ATI는 [우분투](%EC%9A%B0%EB%B6%84%ED%88%AC.md)에 리눅스용 최신 카탈리스트 드라이버를 선행
배포하고 있기도 하다.

  

덤으로 엔비디아 그래픽카드는 급사할 때까지 군말없이 일하기 때문에 중고를 구입할 때 좀 조심하라는 얘기가 있지만, ATI 그래픽카드는 죽을
때가 다가오면 VPU 리커버리 에러가 자꾸 떠서 유저를 짜증나게 만들기 때문에 금방 확인이 된다는 믿거나 말거나성 얘기도 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ATI?action=edit&section=15)]

## 5. ATI 브랜드의 끝 ¶

AMD에서 6천번대 시리즈부터는 더이상 ATI 브랜드를 사용하지 않기로 발표하였다. 앞으로의 신제품에는 AMD RADEON 시리즈로
출시된다.

  

![http://img43.imageshack.us/img43/2528/m5x1.png](http://img43.imageshack.us/i
mg43/2528/m5x1.png)

[[PNG external image]](http://img43.imageshack.us/img43/2528/m5x1.png)

  
변경된 뱃지로고.

  

`\----`

  * `[1]` 원래 매트록스 VGA는 비디오 편집이나 산업용, 의료용으로 특화된 분야에서 주로 사용했었고, 현재도 그쪽 분야에선 확실한 점유율을 자랑하고 있기 때문에 일반 유저용 시장에 대해서는 그리 신경쓰지 않고있다. 문제는 다중 모니터 지원에 ATI가 젓가락을 놓기 시작했다는 것. 사실 산업용이나 의료용은 그렇다쳐도 주식용이나 그쪽으로 ATI가 비집고 들어갈 틈이 있다. 거기다가 **[내장**으로 3모니터를 돌리는 물건](AMD%20A%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md)까지 나와 버렸다...
  * `[2]` 위의 게임은 ALICEぱれーど～ふたりのアリスと不思議の乙女たち～다.
  * `[3]` 엔비디아도 칩 한 종류로 지포스 테슬라(GPGPU) 쿼드로(OpenGL)를 쓰지만, 일반 지포스 제품군의 드라이버 개조를 방지하기 위해 일반 제품군에 모종의 조치가 취해져 나온다.
  * `[4]` 둘을 합쳐 ATI Stream이라고 칭하며 CAL은 저수준 언어, Brook+는 고수준 언어 지향이다.
  * `[5]` [카베리](%EC%B9%B4%EB%B2%A0%EB%A6%AC.md) 내장, R9 260X, R9 280, R9 280X, R9 290, R9 290X, R9 295X2

