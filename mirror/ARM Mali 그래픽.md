![http://gadgetmix.com/wp-content/uploads/2012/06/ARM-
Mali-T658-graphics.jpg](http://gadgetmix.com/wp-content/uploads/2012/06/ARM-
Mali-T658-graphics.jpg)

[[JPG external image]](http://gadgetmix.com/wp-content/uploads/2012/06/ARM-
Mali-T658-graphics.jpg)

## Contents

    

1. 개요 
2. 상세 
3. GPU 제품 라인업 
    

3.1. Utgard 기반

    

3.1.1. Mali-200 / Mali-300

3.1.2. Mali-400

3.1.3. Mali-450

3.2. 1세대 Midgard

    

3.2.1. Mali-T604

3.2.2. Mali-T658

3.3. 2세대 Midgard

    

3.3.1. Mali-T62X

3.3.2. Mali-T678

3.3.3. Mali-T720

3.3.4. Mali-T760

4. GPU외 제품 라인업 
    

4.1. Mali Video

    

4.1.1. Mali-V500

4.2. Mali Display

    

4.2.1. Mali-DP500

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20Mali%20%EA%B7%B8%EB%9E%98%ED%
94%BD?action=edit&section=1)]

## 1. 개요 ¶

[ARM Holdings](ARM%20Holdings.md)에서 설계하는 GPU 브랜드다. 잉글랜드 본사가 아닌 [ARMHoldings](ARM%20Holdings.md) 노르웨이 지사에서 주로 개발을 담당한다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20Mali%20%EA%B7%B8%EB%9E%98%ED%
94%BD?action=edit&section=2)]

## 2. 상세 ¶

2006년, [ARM Holdings](ARM%20Holdings.md)가 Falanx Microsystems를 인수한 후에 본격적으로
개발에 들어간 GPU 솔루션이다.`[1]`

  

ARM이 GPU 개발에 뛰어든 이유는 크게 두 가지로,  

  * 모바일 AP, 특히 ARM 아키텍쳐 기반의 AP에서 사용할 GPU 솔루션의 부재.
  * 일종의 대세가 되어가는 [GPGPU](GPGPU.md) 기술개발의 목적.  

등이 있다.

  

ARM의 경우, 과거 [피쳐폰](%ED%94%BC%EC%B3%90%ED%8F%B0.md) 시절부터 모바일 AP 부분에서는 강자에
속했었다. [인텔](%EC%9D%B8%ED%85%94.md)역시 모바일 AP 시장에 진출하기 위해서 과거
[XScale](XScale.md)를 ARM 아키텍쳐 기반으로 만들기도 했다. 다만, 모바일 임베디드 시장이 점진적으로 확대되고, 이
시장이 [기존의 PC의 영역까지 침범](%EC%8A%A4%EB%A7%88%ED%8A%B8%ED%8F%B0.md)하게 될 가능성이
높아지자 CPU가 처리하지 못하는 더욱 높은 수준의 그래픽 작업 능력을 지원하기 위해 AP 안에 GPU를 탑재하기 위해 개발에 들어갔다는
것이다. 비단 ARM 뿐만이 아니라 대표적인 CPU 아키텍처 라이센스 구입사인 퀄컴에서도 舊 [ATI](ATI.md)에서 인수한
Imageon 모바일 사업부의 자체 GPU를 자사의 AP에 통합하기 시작했고, TI같은 타 라이센스 구입사의 경우 PC 그래픽 시장에서
도태되어 모바일 GPU 시장으로 시선을 돌린 Imagination Technology사의 PowerVR SGX 시리즈를 GPU 솔루션으로
사용하고 있었다. 때문에 ARM에서는 기존의 ARM의 CPU 아키텍쳐를 라이센스를 받는 것과 비슷한 형식으로 GPU 솔루션을 개발,
라이센스를 판매하여 기반 기술이 부족한 구매사라도 수월하게 시장에 진출하게 하기위해 GPU 솔루션을 개발하기로 한 것이다. <del>회사
항목에도 나왔지만, ARM은 지들끼리 싸워야 돈을 번다.</del>

  

또한 연산유닛이 CPU에 비해 압도적으로 많은 GPU를 [일반적인 연산에 응용](GPGPU.md)하기 위해서 당시에 여러 회사에서 많은
시도가 있었기 때문에 시장에서 도태되지 않기 위해 개발을 한 것이라고 한다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20Mali%20%EA%B7%B8%EB%9E%98%ED%
94%BD?action=edit&section=3)]

## 3. GPU 제품 라인업 ¶

**관련 성능은 모두 ARM의 발표치로 실 성능은 1/3토막 정도 난다고 보면 편하다.** 였는데... 지금까지 실 성능을 측정하던 GFXbench 앱이 3.0으로 업데이트 되고난 후 이론 성능에 90%에 가까운 성능은 보여주고 있다. <del>측정 어플의 최적화 문제라니...</del>

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20Mali%20%EA%B7%B8%EB%9E%98%ED%
94%BD?action=edit&section=4)]

### 3.1. Utgard 기반 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20Mali%20%EA%B7%B8%EB%9E%98%ED%
94%BD?action=edit&section=5)]

#### 3.1.1. Mali-200 / Mali-300 ¶

![http://www.arm.com/images/OCT12-Mali-300_-
_Small_200x200.jpg](http://www.arm.com/images/OCT12-Mali-300_-
_Small_200x200.jpg)

[[JPG external image]](http://www.arm.com/images/OCT12-Mali-300_-
_Small_200x200.jpg)

  

클럭

성능

타겟공정

210 MHz

23 Mtri/s, 210 Mpix/s

40nm LP

500 MHz

55 Mtri/s, 500 Mpix/s

28nm HPM

  
극 초창기의 Mali 제품군이다. 사용한 예를 거의 찾아 볼 수 없다. 굳이 찾자면 국내 업체인 텔레칩스의 TCC89XX시리즈 정도가
Mali-200을 탑재한 사례다. 당시 기준으로는 그렇게 좋지않은 성능은 아니었으나, 시기 자체가 GPU의 중요도가 없었던 시기였기 때문에
묻힌 감이 없지않아 있다.

  

현재 Mali-200은 ARM 공식 사이트에서도 언급되지 않는 상태이며 성능이 비슷한 Mali-300만 남아있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20Mali%20%EA%B7%B8%EB%9E%98%ED%
94%BD?action=edit&section=6)]

#### 3.1.2. Mali-400 ¶

![http://www.arm.com/images/OCT12-Mali-400_-
_Small_200x200.jpg](http://www.arm.com/images/OCT12-Mali-400_-
_Small_200x200.jpg)

[[JPG external image]](http://www.arm.com/images/OCT12-Mali-400_-
_Small_200x200.jpg)

  

싱글코어 기준

클럭

성능

타겟공정

210 MHz

23 Mtri/s, 210 Mpix/s

40nm LP

500 MHz

55 Mtri/s, 500 Mpix/s

28nm HPM

  

쿼드코어 기준`[2]`

클럭

성능

타겟공정

210 MHz

23 Mtri/s, 840 Mpix/s

40nm LP

500 MHz

55 Mtri/s, 2 Gpix/s

28nm HPM

<del>표만보면 Mali-300의 멀티코어 지원 버전으로 보인다.</del>

  

멀티코어 구성이 가능한 최초의 Mali GPU이다. 최대 지원 개수는 4개이다. 이전의 Mali-300과 같이 독립 쉐이더 구조로, 버택스를
담당하는 코어와 픽셀을 담당하는 코어가 각각 나누어져 있다.

  

버택스 코어는 항상 하나로 코어 수에 포함되지 않고 독립적으로 픽셀을 처리하는 Fragment Processor 하나가 추가되는 수준이다..
<del>그래서 별명이 버택스 고자</del> 그렇기에 싱글코어든 쿼드코어든 버택스 성능은 같아 Mali-400을 탑재한 기기들이 벤치마크
점수에서 힘을 못 쓰는 발단이 되었다.

  

[삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md)의 자체 AP인
[엑시노스](%EC%97%91%EC%8B%9C%EB%85%B8%EC%8A%A4.md) 4210에 쿼드코어 266 MHz 구성으로 최초로
탑재되었다. 당시 ARM에서는 400 MHz로 들어갈 것을 권고했으나, 발열 문제를 우려해 클럭을 낮췄다고 한다. 그리고 이 AP를 최초로
사용한 [갤럭시 S II](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20S%20II.md)에서 역시 Mali-400을 최초로
사용했다. <del>물론 루팅하면 기존 클럭치인 400 MHz로 가능하나, 역시나 발열 ..</del>초반에는 호환성이 있는 애플리케이션이
전혀 없는 관계로 많은 사람들이 우려를 표했으나, [갤럭시 SII](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20S%20II.md) 자체가
[삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md)의 플래그쉽 스마트폰이었고, 또 당시 안드로이드
진영에서는 유일하게 [아이폰](%EC%95%84%EC%9D%B4%ED%8F%B0.md)에 맞설 수 있는 기업이었기 때문에 글로벌
판매량이 상당히 높았다. 그로인해 실질적으로 사용하는 사람들이 많아졌고, 더 나아가
[삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md) 자체에서도
[쇼미더머니](%EC%87%BC%EB%AF%B8%EB%8D%94%EB%A8%B8%EB%8B%88.md)를 시전하여 호환성을 끌어올렸기
때문에 문제가 쉽게 해결 될 수 있었다고 한다. <del>그렇게 우리가 생각하는 삼성 최대 전성기인 갤럭시s2가 되었다</del>

  

이후 [엑시노스](%EC%97%91%EC%8B%9C%EB%85%B8%EC%8A%A4.md) 4210의 공정 개선판인
[엑시노스](%EC%97%91%EC%8B%9C%EB%85%B8%EC%8A%A4.md) 4212에는 정상적으로 440 MHz의 클럭으로
탑재되었고, 같은 공정을 사용하는 [엑시노스](%EC%97%91%EC%8B%9C%EB%85%B8%EC%8A%A4.md) 4412에도
그대로 적용되어 이 AP를 사용한 [갤럭시 S III](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20S%20III.md)와
[갤럭시 노트 II](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20%EB%85%B8%ED%8A%B8%20II.md)에는 최대
533 MHz의 클럭까지 적용되었다고 한다.

  

[삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md)의
[엑시노스](%EC%97%91%EC%8B%9C%EB%85%B8%EC%8A%A4.md) 4210이 호환성 문제를 해결하자, 후발 주자로
ST에릭슨과 [락칩](%EB%9D%BD%EC%B9%A9.md)에서도 다양한 구성으로 사용되었다.

  

구세대인 독립 쉐이더 구조 떄문에 떨어지는 버택스 성능으로 인한 병목 현상이 많이 일어나며 절대적인 성능도 2013년 현재 퀄컴 Adreno
320 같은 경쟁 GPU와 비교했을 때 떨어지는 편이지만, 아직까지 모바일에서는 버택스 성능이 중요한 폴리곤보다 픽셀 성능이 중요한 텍스처를
주로 많이 쓰기 때문에 무난한 성능을 보여주고 있다. 특히 [갤럭시 SII](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20S%20II.md), [갤럭시 SIII](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20S%20III.md)를 비롯한
[엑시노스](%EC%97%91%EC%8B%9C%EB%85%B8%EC%8A%A4.md) 4210, 4412 탑재 기기들이 안드로이드
점유율에 지대한 영향력을 끼치기 때문에 각종 애플리케이션 개발자들로부터 지원 역시 활발히 받고 있다. <del>특히 카톡 게임들이
있다.</del> <del>역시 물량의 삼성</del>

  

다만, Open GL 3.0을 지원하지 않기에 Android 4.3 젤리빈에서는 큰 영향력을 행사하기 어려울 전망이다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20Mali%20%EA%B7%B8%EB%9E%98%ED%
94%BD?action=edit&section=7)]

#### 3.1.3. Mali-450 ¶

![http://www.arm.com/images/OCT12-Mali-450_-
_Small_200x200.jpg](http://www.arm.com/images/OCT12-Mali-450_-
_Small_200x200.jpg)

[[JPG external image]](http://www.arm.com/images/OCT12-Mali-450_-
_Small_200x200.jpg)

  

쿼드코어 기준

클럭

성능

타겟공정

270 MHz

59 Mtri/s, 1.1 Gpix/s

40nm LP

650 MHz

142 Mtri/s, 2.6 Gpix/s

28nm HPM

  

옥타코어 기준`[3]`

클럭

성능

타겟공정

270 MHz

59 Mtri/s, 2.2 Gpix/s

40nm LP

650 MHz

142 Mtri/s, 5.2 Gpix/s

28nm HPM

<del>레알 옥타코어 GPU</del>

  

Utgard 기반의 끝판왕으로 불리지만 구조 자체는 Mali-400을 2개 붙인 것과 크게 다르지 않다. 다만, Mali-400에서
문제점으로 지적된 버택스 성능이 두 배로 증가시켜 어느정도 문제를 해결하였다. 또한 Mali-400이 쿼드코어까지 지원했기 때문에 단순히
2개를 붙인 Mali-450은 총 8개까지 지원할 수 있다.

  

여기에 약간의 기술 개선이 이루어져 권고 클럭까지 상승하여 Mali-400의 버택스 성능보다 약 3배 가능 높은 성능을 보여준다. 또한 원래
괴물이었던 픽셀 성능은 2013년 현재 고성능 GPU 중 하나인 퀄컴 Adreno 320보다 **2.5배** 더 높은 성능을 보여준다.

  

다만, Mali-400이 모체인 만큼 구세대 독립 쉐이더 구조의 GPU라는 것은 변하지 않기 때문에 전력 소모 문제를 생각하면 이 것보다는
차기작인 Midgard 기반의 GPU를 탑재하는 것이 정신건강에 이롭다. 때문에 실제로 탑재할 AP가 있을지는 의문인 상황. 거기에 Open
GL 지원 역시 Mali-400을 따라 2.0까지만 지원한다.

  

2013년 4분기 드디어 실 탑제 제품이 등장했다. 미디어텍의 MTK6592와 Amlogic의 AML-M802. [벤치](http://gfx
bench.com/compare.jsp?D1=Amlogic+AML-M802+K200&D2=Google+Nexus+10&cols=2)를 보면
코어수는 <del>포커처서</del>단순 마켓팅만이 아닌 성능을 보여준다. 버텍스 코어가 2개 로 늘어서 병목현상이 대폭 줄었는지
MAli400을 단순 2배 한 것보다도 성능이 잘 나온다. 이는 넥서스10의 Mali T604보다 높으며, 예상대로 Adreno320급의
성능. 특히 Mali400에서 최적화가 끝난 드라이버와 앱의 호환성 그리고 전력대비 성능이 매우 우수하다. <del>의외로 쓸만했다...
그것도 많이</del>

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20Mali%20%EA%B7%B8%EB%9E%98%ED%
94%BD?action=edit&section=8)]

### 3.2. 1세대 Midgard ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20Mali%20%EA%B7%B8%EB%9E%98%ED%
94%BD?action=edit&section=9)]

#### 3.2.1. Mali-T604 ¶

![http://www.arm.com/images/MaliT604__200.png](http://www.arm.com/images/MaliT
604__200.png)

[[PNG external image]](http://www.arm.com/images/MaliT604__200.png)

  

쿼드코어 기준`[4]`

클럭

성능

타겟공정

533 MHz

533 Mtri/s, 2 Gpix/s

28nm HPM

[출처](http://gamma0burst.tistory.com/487)

  

[삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md)의 [엑시노스5250](%EC%97%91%EC%8B%9C%EB%85%B8%EC%8A%A4#s-2.5.md)에 최초로 탑재되었으며 출시된 제품으로는
[넥서스 10](%EB%84%A5%EC%84%9C%EC%8A%A4%2010.md)이 있다.

  

1세대 Midgard기반의 첫 GPU이며, 이전 Utgard기반의 GPU와 비교 시 가장 큰 차이점은 통합 쉐이더 구조라는 점에 있다.
때문에 각각의 코어에 코어 당 2개씩 연산 유닛이 있고, 텍스처 유닛이 별도로 들어간다. 이로 인해 기존의 Utgard기반에서 하나의 코어만
버택스 작업을 담당했다면 이번에는 픽셀 코어와 동등한 버택스 코어를 가지게 되었다. 때문에 기존보다 4배 이상 버택스 성능이 상향되었다.

  

픽셀 성능은 기존에 비해 크게 오르지 않았지만, 기존의 픽셀 성능이 매우 <del>기형적으로</del> 훌륭했다는 것을 볼 때 별 문제가
아닌 것으로 보인다. 그래도 전체적인 성능은 퀄컴 Adreno 320 400 MHz와 비슷하다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20Mali%20%EA%B7%B8%EB%9E%98%ED%
94%BD?action=edit&section=10)]

#### 3.2.2. Mali-T658 ¶

?

![http://cdn0.mos.techradar.futurecdn.net//art/mobile_phones/ARM/Mali-T658_Chi
p_Diagram_web_medium_750w-580-90.jpg](http://cdn0.mos.techradar.futurecdn.net/
/art/mobile_phones/ARM/Mali-T658_Chip_Diagram_web_medium_750w-580-90.jpg)

[[JPG external
image]](http://cdn0.mos.techradar.futurecdn.net//art/mobile_phones/ARM/Mali-
T658_Chip_Diagram_web_medium_750w-580-90.jpg)

  

1세대 Midgard 기반으로 T604와 같이 발표되었다.

  

기본적으로 Mali-400과 Mali-450처럼 Mali T604를 2개를 붙여 놓은 모습을 가지고 있지만, 각 쉐이더 코어 당 연산 유닛의
수가 4개로 늘어 총 32개의 연산 유닛을 가지고 있게되었다. 한 마디로 말해서 **괴물**.

  

정확한 수치가 공개되지 않아 언급하기 어려운 점이 있지만, ARM의 발표대로라면 Mali-400의 10배, Mali T604의 4배의 성능을
보인다고 한다.

  

하지만, ARM에서 라인업 개편을 시행하면서 ARM의 라인업에서 사라졌다. 여담으로 비슷한 시기에
[삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md)에서
[엑시노스](%EC%97%91%EC%8B%9C%EB%85%B8%EC%8A%A4.md) 5410의 GPU를 선정하려 움직였으나 1순위였던
이 녀석이 드랍되는 바람에 결국 PowerVR SGX544 트리플코어를 채용하는 방향으로 틀어졌다고 한다. <del>그리고 이 것은 **신의
악(惡)수**가 되었다.</del>

  

그래도 존재 자체는 아직도 있는 것으로 보인다. [화웨이](%ED%99%94%EC%9B%A8%EC%9D%B4.md)의 자체 AP인
K3V2의 후속으로 계획 중인 big.LITTLE 기술 적용 AP인 K3V3에 들어간다는
[뉴스](http://www.gizmochina.com/2013/03/25/huawei-is-working-on-hass-core-k3v3
-with-mali-t658-gpu/)가 뜬금없이 떴다. <del>다만 전작을 볼 때 성능은 보장을 못한다.</del>

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20Mali%20%EA%B7%B8%EB%9E%98%ED%
94%BD?action=edit&section=11)]

### 3.3. 2세대 Midgard ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20Mali%20%EA%B7%B8%EB%9E%98%ED%
94%BD?action=edit&section=12)]

#### 3.3.1. Mali-T62X ¶

![http://www.arm.com/images/Mali-
T622_block_diagram_small.jpg](http://www.arm.com/images/Mali-
T622_block_diagram_small.jpg)

[[JPG external image]](http://www.arm.com/images/Mali-
T622_block_diagram_small.jpg)

  

![http://www.arm.com/images/OCT12-Mali-T624_-
_Small_200x200.jpg](http://www.arm.com/images/OCT12-Mali-T624_-
_Small_200x200.jpg)

[[JPG external image]](http://www.arm.com/images/OCT12-Mali-T624_-
_Small_200x200.jpg)

  

![http://www.arm.com/images/OCT12-Mali-T628_-
_Small_200x200.jpg](http://www.arm.com/images/OCT12-Mali-T628_-
_Small_200x200.jpg)

[[JPG external image]](http://www.arm.com/images/OCT12-Mali-T628_-
_Small_200x200.jpg)

  

헥사코어 기준

클럭

성능

700 MHz

600 Mtri/s, 4.2 Gpix/s

533 MHz

457 Mtri/s, 3.2 Gpix/s

[출처](http://gamma0burst.tistory.com/661)

  
  

2012년 8월 2세대 Midgard기반의 T624와 T628이 T678과 같이 공개되었다. T622는 2013년 6월 2일에 CPU
아키텍쳐인 Cortex-A12와 함께 따로 공개되었다. 2013년 9월 기준으로 사용하는 AP는
[삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md)의 [엑시노스5420](%EC%97%91%EC%8B%9C%EB%85%B8%EC%8A%A4#s-2.6.2.md)이 유일하며 탑재된 기기로 [갤럭시노트 3](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20%EB%85%B8%ED%8A%B8%203.md)와 [갤럭시 노트10.1 2014 에디션](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20%EB%85%B8%ED%8A%B8%2010.1%202014%20%EC%97%90%EB%94%94%EC%85%98.md)이 있다.  
ASTS 압축 포맷을 지원하고 Open Gl 4.3과 Open Gl ES 3.0에 대응한다.

  

이전 T60X 시리즈에 비해서 약 50%의 성능 향상이 있다고 한다.

  

벤치마크상 헥사코어버전의 성능은 퀄컴의 Adreno330과 거의 비슷한 성능, 다만 MAli계열은 이전까지 6개월 정도 드라이버 최적화 과정
후 성능이 눈에띄게 올라가는것이 다반사였기 때문에 조금 더 지켜볼 필요가 있다.

  
  

여담으로, GPU 명에 마지막으로 들어가는 숫자는 최대 코어 개수를 의미한다. 때문에 [엑시노스5420](%EC%97%91%EC%8B%9C%EB%85%B8%EC%8A%A4#s-2.6.2.md)이 T628을 옥타 코어가 아닌 쉐이더
코어 2개를 덜어내어 헥사 코어로 사용하고 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20Mali%20%EA%B7%B8%EB%9E%98%ED%
94%BD?action=edit&section=13)]

#### 3.3.2. Mali-T678 ¶

![http://www.arm.com/images/OCT12-Mali-T678__-
_Small_200x200.jpg](http://www.arm.com/images/OCT12-Mali-T678__-
_Small_200x200.jpg)

[[JPG external image]](http://www.arm.com/images/OCT12-Mali-T678__-
_Small_200x200.jpg)

  

2012년 8월 2세대 Midgard기반의 T624와 T628과 같이 공개되었으며 T658의 후속작으로 보인다. 아직 탑재된 AP가 없어
자세한 내용은 아직 불명

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20Mali%20%EA%B7%B8%EB%9E%98%ED%
94%BD?action=edit&section=14)]

#### 3.3.3. Mali-T720 ¶

![http://www.arm.com/images/Mali-T720MP-SM.jpg](http://www.arm.com/images
/Mali-T720MP-SM.jpg)

[[JPG external image]](http://www.arm.com/images/Mali-T720MP-SM.jpg)

  

헥사코어 기준

클럭

성능

공정

695 MHz

695 Mtri/s, 5.6 Gpix/s

28nm HPM

  

2013년 10월 발표된 ARM의 새로운 중급 라인업의 GPU이다. 2세대 Midgard 기반의 GPU지만`[5]`, 일단 라인업상
Mali-450을 잇는 중급 라인업. 그러나 공개된 스펙을 보면 중급의 그것이 아닌데, 현세대인 Mali-T62X 시리즈와 비슷하거나 그
이상의 성능을 보여준다. `[6]`

  

현재 시장에서 T62X시리즈를 탑제하고 시장에 출시된 제품은 엑시노스 5420이 유일하며, 이것은 Utgard 기반의 GPU가 라이센스와
양산이 쉬워서 많은 제조사들이 채택했다는 것에 비해서 너무 접근성이 떨어진다는 상황을 잘 보여주고 있다. 양산이나 설계 능력이 떨어지는
제작사들은 Midgard 보다는 기존의 Utgard 기반의 Mali-450을 탑제하고 있는 상황에서 양산의 용이성을 높이고 성능 효율을
끌어올린 기존 T600 시리즈를 최적화한 버전이라고 할 수 있겠다.`[7]`

  
  

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20Mali%20%EA%B7%B8%EB%9E%98%ED%
94%BD?action=edit&section=15)]

#### 3.3.4. Mali-T760 ¶

![http://www.arm.com/images/Mali-T760MP-SM.jpg](http://www.arm.com/images
/Mali-T760MP-SM.jpg)

[[JPG external image]](http://www.arm.com/images/Mali-T760MP-SM.jpg)

  

16코어 기준

클럭

성능

공정

695 MHz

1390 Mtri/s, 11.2 Gpix/s

28nm HPM

  
Mali-T720과 같이 공개된 하이엔드 라인업. 공개된 성능만으로 보면 Mali-T720과 같은 코어로 추정되며, 최대 16개의 코어를
추가할 수 있다. 전력효율은 기존 1세대 Midgard인 T604의 4배라고.

  

압축 기술인 AFBC(ARM Frame Buffer Compression)과 Smart Composition 기술을 적용해, 이미지와
텍스쳐를 읽어들일 때 기존보다 메모리 대역폭과 전력 소비가 50% 줄었다고 한다.

  

이론 성능이 [엑스박스 원](%EC%97%91%EC%8A%A4%EB%B0%95%EC%8A%A4%20%EC%9B%90.md)의
것`[8]`과 가까워졌다. 차세대 테그라인 프로젝트 로건을 뛰어넘는 수준.

  

CES 2014에서 첫 탑제 AP가 공개되었다. 제조사는 중국의 락칩. 4개라는 비교적 적은수의 쉐이더 코어가 탑제된 T764 구성으로도
[현재 시장에 정식 출시된 모든 AP를 상회하는
성능](http://images.imp3.net/article/2014/01/09/290015.jpg)을 보여준다고. <del>다만 어차피
GPU에 몰빵한 테그라K1이 있어서 안될꺼야</del>

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20Mali%20%EA%B7%B8%EB%9E%98%ED%
94%BD?action=edit&section=16)]

## 4. GPU외 제품 라인업 ¶

  

원래는 GPU가 담당할 비디오의 인/디코딩이나 디스플레이 출력을 위한 Mali 라입업들이 있다. 이는 기존의 GPU가 고사양을 필요로 하는
3D연산을 하는것은 물론, 4K해상도 비디오의 인/디코딩 및 디스플레이 출력 등에 많은 리소스가 필요해짐에 따라서 본래 GPU의 목적인
GPU의 3D연산을 발목 잡거나 리소스의 처리에 GPU를 활용하는것이 전력 효용성이 떨어지는 부분을 보충하기 위한 보조 코어로써 단독이 아닌
Mali62x/7xx 번때 GPU와 같이 사용되는 것을 전제로 설계되었다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20Mali%20%EA%B7%B8%EB%9E%98%ED%
94%BD?action=edit&section=17)]

### 4.1. Mali Video ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20Mali%20%EA%B7%B8%EB%9E%98%ED%
94%BD?action=edit&section=18)]

#### 4.1.1. Mali-V500 ¶

![http://www.arm.com/images/Mali-V500-small.png](http://www.arm.com/images/Mal
i-V500-small.png)

[[PNG external image]](http://www.arm.com/images/Mali-V500-small.png)

  

Mali-V500은 최대 8코어 구성의 비디오 인/디코딩 전용 칩이다. 최대 600mhz로 동작하며, 1개의 코어로 1080p 60f의
인/디코딩을, 8개의 모든 코어를 사용하다면, 2160p 120f을 처리 가능하다.

  

H265를 제외한 대부분의 API를 지원하며, ARM의 대역폭 압축 기술인 ARM Frame Buffer Compression
(AFBC)기술로 기존의 50%의 대역폭만 사용하여 영상을 처리할 수 있다.

  
  

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20Mali%20%EA%B7%B8%EB%9E%98%ED%
94%BD?action=edit&section=19)]

### 4.2. Mali Display ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20Mali%20%EA%B7%B8%EB%9E%98%ED%
94%BD?action=edit&section=20)]

#### 4.2.1. Mali-DP500 ¶

![http://www.arm.com/images/Mali-DP500\(2\)_203.png](http://www.arm.com/images
/Mali-DP500\(2\)_203.png)

[[PNG external image]](http://www.arm.com/images/Mali-DP500\(2\)_203.png)

  

2014년 2월 Cortex A17과 같이 공개된 Mali-DP500은 디스플레이 출력전용 칩이다.

  

비디오의 합성,색채,회전 및 3D효과를 처리하며, 4K 12bit를 VESA, CEA, HDMI and MIPI DPI등의 규격으로 출력이
가능하다.  
Mali-V500과 같이 ARM의 대역폭 압축 기술인 ARM Frame Buffer Compression (AFBC)기술로 기존대비 대역폭의
사용이 50%감소.

  
  
  
  

[추가바람](%EC%B6%94%EA%B0%80%EB%B0%94%EB%9E%8C.md)

`\----`

  * `[1]` 이후 이 회사는 ARM 노르웨이 지사로 개편되었다.
  * `[2]` Mali-400의 최대 구성 가능 개수
  * `[3]` 최대 지원 개수
  * `[4]` 최대 지원 개수
  * `[5]` T700 시리즈로 넘버링이 올라가면서 3세대 미드가르드로 바뀌었을 가능성을 배제할 수 없으니, 세대가 밝혀지면 추후에 수정 바람.
  * `[6]` 전력효율은 150%, 성능은 50% 상승이라고 하는데, 기준이 Utgard 라고 하면 너무 높고 Midgard 라고 한다면 낮다.
  * `[7]` 특히 중요한 점은, 동일 공정에서 다이 사이즈도 30% 줄었다는 것.
  * `[8]` 28nm HPM 기준, 853MHz에서 1600MTri/s, 13Gpix/s

