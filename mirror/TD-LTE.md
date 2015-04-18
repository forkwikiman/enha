**국제전기통신연합(ITU) 인증 이동통신 기술**

구분

3GPP 계열

3GPP2 계열

IEEE 계열

기타

1세대(1G)

\-

AMPS

2세대([2G](2G.md))

[GSM](GSM.md)

[cdmaOne](CDMA.md)

2.5세대(2.5G)

GRPS  
EDGE  
(E-GPRS)

[CDMA2000 1x](CDMA2000.md)

3세대([3G](3G.md))

[WCDMA](WCDMA.md) \- UMTS  
[TD-SCDMA](TD-SCDMA.md)

[EV-DO](CDMA2000.md)  
[EV-DO rev. A·B](CDMA2000.md)

3.5세대(3.5G)

[HSDPA, HSUPA](WCDMA.md)  
[TD-HSDPA](TD-SCDMA#s-4.1.md)  
[TD-HSUPA](TD-SCDMA#s-4.2.md)

[EV-DO rev. C](CDMA2000.md)  
(UMB)

4세대([4G](4G.md))

HSPA+, [LTE](LTE.md)·[TD-LTE](TD-LTE.md)  
[LTE Advanced](LTE%20Advanced.md)  
([Carrier Aggregation](Carrier%20Aggregation.md))

[WiBro](WiBro.md)/[Mobile WiMAX](Mobile%20WiMAX.md)  
[WiBro Evolution](WiBro%20Evolution.md)

**Time-Division [Long-Term Evolution](LTE.md)**

이 항목은 [소프트뱅크](%EC%86%8C%ED%94%84%ED%8A%B8%EB%B1%85%ED%81%AC.md)가 서비스 하는 TD-
LTE의 공식 명칭인 [AXGP](AXGP.md)로도 들어오실수 있습니다.

이 문서는 블로거 초코버리의 ["LTE FDD, TDD 개요 / TD-LTE에 대한 오해와
진실"](http://chocoberry.pe.kr/166405782?Redirect=Log&from=postView) 포스트에 기반하여
작성되었다.

  

## Contents

    

1. 개요 
2. 상세 
3. 장단점 
4. [Mobile WiMAX](Mobile%20WiMAX.md)와 TD-LTE와의 관계 
5. 상용 통신사 
    

5.1. 한국에서의 TD-LTE 서비스 예정

[[edit](http://rigvedawiki.net/r1/wiki.php/TD-LTE?action=edit&section=1)]

## 1. 개요 ¶

세계 최대의 이통사이자 중국의 이통사인
[차이나모바일](%EC%B0%A8%EC%9D%B4%EB%82%98%EB%AA%A8%EB%B0%94%EC%9D%BC.md)을 중심으로
통신장비 제조업체인 중국의 다탕 텔레콤, [화웨이](%ED%99%94%EC%9B%A8%EC%9D%B4.md),
[ZTE](ZTE.md), 핀란드의 [노키아](%EB%85%B8%ED%82%A4%EC%95%84.md), 프랑스의 알카텔, 미국의
퀄컴, 영국의 ST-에릭슨 등이 협력해서 세운 **Global TD-LTE Initiative**이 주축이 되어 개발한 4세대 이동통신
서비스.

  

후속기술로는 **TD-LTE Advanced**가 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/TD-LTE?action=edit&section=2)]

## 2. 상세 ¶

통신 단말기와 기지국 사이에서 교신을 할 때 다른 신호와 섞이지 않게 구분하기 위한 방법이 필요하다. 방법은 다양하지만 현재 LTE에 적용된
방법은 두 가지인데 하나는 FDD(Frequency Division Duplexing), 다른 하나는 **TDD**(Time Division
Duplexing)이다.

  

FDD는 상향링크(**UL**)와 하향링크(**DL**)가 서로 다른 주파수 채널을 이용한다. 또한 UL과 DL은 서로 짝지어져야 한다.
가령 2.1 GHz 주파수를 이용할 때 UL의 대역폭이 60 MHz이라면 DL 역시 똑같이 60 MHz의 대역폭을 가지고 있어야
한다.`[1]` 또한 UL과 DL은 서로 간의 간섭을 최소화 하기 위해서 어느 정도 간격이 있어야 한다.`[2]` 이로 인해 UL과 DL을
동시에 이용하는 이른바 **풀 듀플렉스**가 가능해진다는 장점이 있다.

  

TDD는 UL과 DL 주파수가 따로 주어지지 않고는 **하나의 스펙트럼**을 같이 이용한다. 이로 인해 풀 듀플렉스를 이용하는게 불가능
해지지만, **UL과 DL을 짧은 시간적인 간격을 두고 전환**을 함으로써 **풀 듀플렉스를 모방**하게 만든다.

  

현재 사람들이 [LTE](LTE.md)라 부르는 것은 FDD 방식인 LTE-FDD(이하 [LTE](LTE.md)로 통칭.)를
의미하고 있다. 이는 현재까지 주로 서비스 되었던 GSM, WCDMA, CDMA의 주파수 대역을 재활용이 가능하기 때문이다.

  

![ROK_Cellular_Frequency_2014_11_04-1.png](//rv.wkcdn.net/http://rigvedawiki.n
et/r1/pds/ROK_Cellular_Frequency_2014_11_04-1.png)

[PNG image (96.8 KB)]

  

상세한 내역은 [대한민국의 이동통신 주파수](%EB%8C%80%ED%95%9C%EB%AF%BC%EA%B5%AD%EC%9D%98%20%EC%9D%B4%EB%8F%99%ED%86%B5%EC%8B%A0%20%EC%A3%BC%ED%8C%8C%EC%88%98.md) 항목을
참고바랍니다.

  
한국에서 상용화된 통신 서비스는 현재 WiBro를 서비스 하는 대역을 제외한 모든 통신 서비스가 FDD 방식으로 이루어 진다는 것을 알 수
있다.

  

그러나, 중국의
[차이나모바일](%EC%B0%A8%EC%9D%B4%EB%82%98%EB%AA%A8%EB%B0%94%EC%9D%BC.md)을 중심으로
위의 기업들을 포함해서 일본의 [소프트뱅크](%EC%86%8C%ED%94%84%ED%8A%B8%EB%B1%85%ED%81%AC.md)를
비롯한 인도, 중동, 유럽의 이동통신사들이 'Global TD-LTE Initiative' 창설해 **TD-LTE**라는 이름으로 LTE-
TDD를 보급하고 상용화 하기 시작했다. 서비스명칭이 TD-LTE로 선정된 이유는 주도 기업
[차이나모바일](%EC%B0%A8%EC%9D%B4%EB%82%98%EB%AA%A8%EB%B0%94%EC%9D%BC.md)의 3세대
이동통신 서비스인 [TD-SCDMA](TD-SCDMA.md)에서 **진화한 것처럼 보이기 위해** 변경했다고 한다. 즉, TD-LTE는
[TD-SCDMA](TD-SCDMA.md)와는 그다지 큰 관련은 없으며 **오로지 마케팅을 위해서** 명명된 것이다. 다만, [TD-SCDMA](TD-SCDMA.md)의 보급 및 기술 개발을 위한 포럼인'[TD-SCDMA](TD-SCDMA.md) 포럼'이 'TD
포럼'으로 개칭하고 TD-LTE 역시 다루고 있어 TD-LTE는 LTE의 범주 내에서도 다뤄지고 [TD-SCDMA](TD-SCDMA.md)와의 연계로도 다뤄지고 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/TD-LTE?action=edit&section=3)]

## 3. 장단점 ¶

장점으로는 UL과 DL의 비율을 능동적으로 변경할 수 있다는 점이다. 특정 구간에 다운로드 트래픽이 증가하게 된다면 1:1 비율로 유지되던
UL과 DL이 DL에 더욱 치중해서 1:2, 1:3 등으로 변경할 수 있다는 것이다. 대부분의 이용자들은 업로드보다 다운로드를 더 많이
이용하게 되므로 오로지 1:1 대응이라 UL은 널널한 채로 있어야 하는 [LTE](LTE.md)와는 다르게 UL의 할당구간을 줄이고
나머지를 전부 DL로 넘길 수 있다. 거기에 [LTE](LTE.md)에 간섭을 주지 않기 때문에 높은 트래픽이 몰리는 곳에서는 좋은
트래픽 완화 수단으로 사용될 수 있다.`[3]` 또한 현재 TDD 방식을 이용할 수 있는 주파수 대역은 대부분 2 GHz 이상의 높은
주파수이기 때문에 FDD 방식의 주파수 대역보다 주파수가 **저렴하다**. <del>싼게 장땡이다.</del>

  

단점으로는 UL과 DL이 짧은 시간 간격으로 전환한다 해도 UL이 기지국과 신호가 끊어지는 경우가 있기 때문에 커버리지가 좁아지게 된다.
또한 주파수 대역이 너무 높은 대역이라는 것이다. 높은 주파수일수록 멀리 가지 못하고 건물을 통과하기가 힘들기 때문에 좁은 커버리지라는
단점을 더욱 심화시켜 버린다는 것이다. <del>주파수는 싸지만 기지국 설치할 땐
[망했어요](%EB%A7%9D%ED%96%88%EC%96%B4%EC%9A%94.md)</del> <del>[얘빼고](%EC%B0%A8%EC%9D%B4%EB%82%98%EB%AA%A8%EB%B0%94%EC%9D%BC.md)</del>

  

LTE의 단일 최고 대역폭은 20Mhz다. 한정적인 주파수 자원 상황을 고려하지 않고 속도 경쟁을 할 경우.  
한 라인에서 UL과 DL을 같이 하는 TDD방식은 풀 듀풀렉스의 FDD방식에 비해 속도가 뒤쳐질 수밖에 없다.  
TDD는 한 대역에서 UL/DL 20Mhz를 사용하고 FDD는 40Mhz(UL 20Mhz, DL 20Mhz)를 사용하기 때문이다.

  

이것은 듀얼 밴드를 활용하는 CA([캐리어 어그리게이션](%EC%BA%90%EB%A6%AC%EC%96%B4%20%EC%96%B4%EA%B7%B8%EB%A6%AC%EA%B2%8C%EC%9D%B4%EC%85%98.md))을 사용한다고 해도 40Mhz(UL/DL 20*2Mhz),
FDD 80Mhz(UL+DL 40*2)이기 때문에 여전히 FDD방식이 더 빠르다.

  

그러나 이미 충분하다고 느껴지는 통신속도와 한정된 주파수 자원으로 인해 TDD방식의 효율성이 주목받고 있다.  
위에서 말한 것처럼 데이터의 유동은 업로드보다 다운로드가 더 많고 그것을 조절할 수 있으며 같은 대역폭 내에서 TDD방식이 FDD방식보다
UL, DL 모두 더 빠르다. 단점은 커버리지 정도.

  

FDD방식은 20MHz(UL 10MHz, DL 10MHz)일 때 DL속도가 최대 75Mbps, UL속도는 최고 25Mbps가 나온다.  

![tdd.PNG](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/TD_2dLTE/tdd.PNG)

[PNG image (26.32 KB)]

  

[[edit](http://rigvedawiki.net/r1/wiki.php/TD-LTE?action=edit&section=4)]

## 4. [Mobile WiMAX](Mobile%20WiMAX.md)와 TD-LTE와의 관계 ¶

상단에 있는 한국의 주파수 할당표를 보면, 현재 [Mobile WiMAX](Mobile%20WiMAX.md) 서비스는 TDD 방식을
사용하는 2.3 GHz 대역을 이용하고 있다. 이로인해 [WiBro](WiBro.md) 서비스를 하는 많은 통신사들이 TD-LTE로
전환하려는 움직임을 보이고 있다.

  

이는 국내에서 [Mobile WiMAX](Mobile%20WiMAX.md)를 [WiBro](WiBro.md)라는 명칭으로 서비스를
하고 있는 [SK텔레콤](SK%ED%85%94%EB%A0%88%EC%BD%A4.md)과 [KT](KT.md)역시 마찬가지로,
2012년 7월에는 [KT](KT.md)에서 직접 [WiBro](WiBro.md)에서 TD-LTE로의 전환에 대한 기자간담회까지
하기도 했었다. 다만, '한국 기술인 [WiBro](WiBro.md)를 버리고 중국 기술인 TD-LTE로 넘어간다.'라는 점`[4]`
때문에 결국 당시 관계 부처였던 [방송통신위원회](%EB%B0%A9%EC%86%A1%ED%86%B5%EC%8B%A0%EC%9C%84%EC%9B%90%ED%9A%8C.md)에서 **"[WiBro](WiBro.md) 포기할거면 주파수 반납해라"**라는 엄포를 듣게되어
한발짝 물러난 상황이다.

  

다만, KT의 주장도 간과할 수 없는 것이 현재 [Mobile WiMAX](Mobile%20WiMAX.md) 장비를 대주는 회사는
[삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md)와
[화웨이](%ED%99%94%EC%9B%A8%EC%9D%B4.md) 정도로,
[삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md)는 이미 TD-LTE 장비로 웬만큼 전환했다는
것이다. 또한 [WiBro](WiBro.md)를 지원하는 단말기 역시
[스마트폰](%EC%8A%A4%EB%A7%88%ED%8A%B8%ED%8F%B0.md)과 [태블릿컴퓨터](%ED%83%9C%EB%B8%94%EB%A6%BF%20%EC%BB%B4%ED%93%A8%ED%84%B0.md)는 이미 예전에
단종되었고 현재는 **[에그](olleh%20%EC%97%90%EA%B7%B8.md)**와
**[브릿지](T%20%EC%99%80%EC%9D%B4%EB%B8%8C%EB%A1%9C.md)**로 명명된 휴대용 라우터만 유통되는
상황이다.

  

설상가상으로 [Mobile WiMAX](Mobile%20WiMAX.md)의 후속 기술이라 불리는 [WiBroEvolution](WiBro%20Evolution.md)역시 상용화가 불투명한 상황이기 때문에 현실적으로
[WiBro](WiBro.md)를 계속 끌고가는 것은 어렵다는 것이다.

  

거기에 [삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md)가 **LTE/WiMAX 듀얼모드
솔루션**을 발표해버렸다. 이 솔루션이라는게 TD-LTE와 [Mobile WiMAX](Mobile%20WiMAX.md)는 기술 상
비슷한 면이 많기 때문에 기기 소프트웨어 업그레이드와 채널 카드 추가 등으로 [MobileWiMAX](Mobile%20WiMAX.md)에서 TD-LTE로 점진적으로 전환이 가능하게 한다는 것이 주요 내용이다.

  

다만, SKT보다는 KT가 [WiBro](WiBro.md)로 해먹은 것이 상당한 만큼 실질적으로 진통없이 TD-LTE로의 전환은 쉽지
않아 보인다.`[5]`

  

[[edit](http://rigvedawiki.net/r1/wiki.php/TD-LTE?action=edit&section=5)]

## 5. 상용 통신사 ¶

중국의
[차이나모바일](%EC%B0%A8%EC%9D%B4%EB%82%98%EB%AA%A8%EB%B0%94%EC%9D%BC.md)이`[6]`
2013년 12월에 중국 정부의 지지로 상용 서비스를 시작했으며,
[차이나유니콤](%EC%B0%A8%EC%9D%B4%EB%82%98%EC%9C%A0%EB%8B%88%EC%BD%A4.md)도 서비스를
시작하였다. 본래 차이나모바일의 경우에는 2013년 8월을 목표로 준비를 했으나, [어른의사정](%EC%96%B4%EB%A5%B8%EC%9D%98%20%EC%82%AC%EC%A0%95.md)에 의해 2013년 11월로
연기되었다. 하지만, 아직 중국 정부에서 승인을 받지 못해서 2013년 12월로 상용화 시기가 또 지연되었다. 다만, 단말기는 2013년
11월부터 [삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md) [갤럭시 노트II](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20%EB%85%B8%ED%8A%B8%20II.md)와 [소니모바일](%EC%86%8C%EB%8B%88%20%EB%AA%A8%EB%B0%94%EC%9D%BC.md) [엑스페리아SP](%EC%97%91%EC%8A%A4%ED%8E%98%EB%A6%AC%EC%95%84%20SP.md)의 TD-LTE 지원 모델을
판매 개시했다. 또한 2014년 하반기를 목표로 [VoLTE](VoLTE.md)도 상용화 한다고 밝혔다.
<del>[아이폰](%EC%95%84%EC%9D%B4%ED%8F%B0.md)의 [VoLTE](VoLTE.md) 도입은 2014년
모델이나 늦으면 2015년 모델이라는 소리다.</del>`[7]`

  

[차이나텔레콤](%EC%B0%A8%EC%9D%B4%EB%82%98%ED%85%94%EB%A0%88%EC%BD%A4.md)의 경우에도,
서비스를 시작했으며, [FDD-LTE](LTE.md)와 TD-LTE를 동시에 상용화 할 것이라고 한다. FDD 방식은 광범위한 지역에
적용할 것이고, 인구 밀도가 많고 데이터 사용량이 많은 지역에 TD-LTE를 서비스 할 것이라고 한다.

  

일본의 [소프트뱅크](%EC%86%8C%ED%94%84%ED%8A%B8%EB%B1%85%ED%81%AC.md)는 **AXGP**라는
이름으로 상용화 했다. 또한 [소프트뱅크](%EC%86%8C%ED%94%84%ED%8A%B8%EB%B1%85%ED%81%AC.md)는
[아이폰 5](%EC%95%84%EC%9D%B4%ED%8F%B0%205.md)의 출시에 맞춰서 [LTE](LTE.md)도 상용화를
해버려서 TD-LTE와 [LTE](LTE.md)를 전부 상용화한 몇 안되는 통신사가 돼버렸다. 거기에
[이모바일](%EC%9D%B4%EB%AA%A8%EB%B0%94%EC%9D%BC.md)과 협력해 한국에서 멀티캐리어라 불리는 **더블
LTE**도 상용화 해버렸다. 다만, 주력은 AXGP라고 한다.`[8]`

  

인도와 사우디아라비아 역시 TD-LTE를 채택하고 있으며 특히 사우디아라비아의 모바일리의 경우
[삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md)의 LTE/WiMAX 듀얼모드 솔루션을 이용하여
[Mobile WiMAX](Mobile%20WiMAX.md)에서 TD-LTE로 전환한 첫번째 사례라고 한다. 또한 미국의
Clearwire역시 이 솔루션을 이용해 전환할 계획이라고 한다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/TD-LTE?action=edit&section=6)]

### 5.1. 한국에서의 TD-LTE 서비스 예정 ¶

현재 한국에 [SK텔레콤](SK%ED%85%94%EB%A0%88%EC%BD%A4.md), [KT](KT.md), [LGU+](LG%20U+.md)를 잇는 네번째 이동통신사가 탄생한다면, TD-LTE를 서비스할 가능성이 있다. 이는 현재 네번째
이동통신사를 위해 준비한 대역이 2.5 GHz TDD 주파수 대역이라 정부에서는 [WiBro](WiBro.md)로 사용할 것을
요구했으나, [WiBro](WiBro.md) 자체가 기술적 발전이 더딘 뿐만이 아니라 진행 자체가 되지 않기 때문에 [WiBro를
강제하는 방침을 철회](http://media.daum.net/digital/clusterview?newsId=2013091316420577
5&clusterId=958967)했기 때문이다. 때문에 단말기 수급이나 호환성을 위해서라도 TD-LTE를 서비스 할 것이 기정사실화
되었다.`[9]``[10]` 그리고 2014년 6월 제4이동통신 컨소시엄인 한국모바일인터넷(KMI)이 LTE-TDD로 사업권을 따내고
7월말에 2.5GHz 대역 주파수 경매를 할 예정**이었**다. 그러나 7월에 진행되던 사업계획서 심사에서 재정건전성 평가에서 낙제를 받아
6번째 퇴짜를 맞았다. KMI는 7수를 준비하는 중이다. 또한 9월에 접어들며 [한국자유총연맹](%ED%95%9C%EA%B5%AD%EC%9E%90%EC%9C%A0%EC%B4%9D%EC%97%B0%EB%A7%B9.md)에서 한국자유통신(KFT)라는 4이통 컨소시엄을 출범하여
준비중이었으나 10월 13일 포기한다고 밝혔다.

`\----`

  * `[1]` 다만 아래의 주파수 분배표를 보면 BAND 3의 SK LTE가 DL 20MHz, UL 15MHz로 짝이 맞지 않는다. 강제 사항은 아닌 듯.
  * `[2]` 이를 Guard Band라 한다.
  * `[3]` 현재 우리나라에서는 그 역할을 [WiBro](WiBro.md)가 하고 있다.
  * `[4]` 상단에서 언급했다시피 TD-LTE와 중국의 기술은 별 관계 없다. 그저 TD-LTE를 주도하는 회사가 중국의 [차이나모바일](%EC%B0%A8%EC%9D%B4%EB%82%98%EB%AA%A8%EB%B0%94%EC%9D%BC.md)이라는 점 뿐이다.
  * `[5]` KT는 SKT와 LG U+가 LTE를 준비할때 2G CDMA 서비스 종료를 위해 움직이느라 [WiBro](WiBro.md)를 메인으로 마케팅을 했다.
  * `[6]` 이쪽은, [TD-SCDMA](TD-SCDMA.md) 기지국에서 업그레이드 하면은 별도의 장비를 구매하지 않고도 저렴하게 망 구축이 가능하다고 한다.
  * `[7]` [아이폰](%EC%95%84%EC%9D%B4%ED%8F%B0.md) 출시의 원년 멤버인 [소프트뱅크](%EC%86%8C%ED%94%84%ED%8A%B8%EB%B1%85%ED%81%AC.md)가 AXGP로 TD-LTE를 서비스를 시작했으나, [아이폰](%EC%95%84%EC%9D%B4%ED%8F%B0.md)은 지원조차 하지 않았다. 하지만 [차이나모바일](%EC%B0%A8%EC%9D%B4%EB%82%98%EB%AA%A8%EB%B0%94%EC%9D%BC.md)과 [아이폰 5s](%EC%95%84%EC%9D%B4%ED%8F%B0%205s.md)의 출시 협상이 이루어지자, **글로벌 모델에도 TD-LTE를 박아버렸다**. 참고로, [차이나모바일](%EC%B0%A8%EC%9D%B4%EB%82%98%EB%AA%A8%EB%B0%94%EC%9D%BC.md) 용 [아이폰 5s](%EC%95%84%EC%9D%B4%ED%8F%B0%205s.md)와 [아이폰 5c](%EC%95%84%EC%9D%B4%ED%8F%B0%205c.md)는 글로벌 모델과 기기명이 다른 **전용 내수용이 들어간다**고 한다. <del>이 당시, [LG U+](LG%20U+.md)는 이런 대접을 받지 못했다</del>
  * `[8]` 현재 [소프트뱅크](%EC%86%8C%ED%94%84%ED%8A%B8%EB%B1%85%ED%81%AC.md)는 [LTE](LTE.md)보다는 HSPA+ 전국망부터 설치한다는 계획이라고 한다.
  * `[9]` 현재 할당하려는 [LTE](LTE.md) Band 38 2.5 GHz 대역은 TDD 주파수 중에서도 범용성이 높은 주파수이다. 또한 2013년 상반기부터 시판되는 퀄컴의 통신 모뎀은 [LTE](LTE.md)와 TD-LTE를 동시에 지원한다. 그리고 음성 통화로 사용되는 [VoLTE](VoLTE.md) 역시 TD-LTE로도 사용할 수 있다. 때문에 단말기 수급이나 [SIM](SIM.md) 카드 호환도 자유로울 것이다. 즉, 기술적 문제는 없고 대신 이동통신사 간 협의나 정부의 입장 등 행정적 문제만 있는 상황이다.
  * `[10]` 단, 이는 네번째 이동통신사가 출범할 시점에 [VoLTE](VoLTE.md)가 활성화 되어야 가능한 일이다. 국내에서는 이미 활성화 되어있지만, 아직 준비조차 하지 않고 있는 국가가 많기 때문에 외산 기업들에서는 가능한 하드웨어를 가지고도 [VoLTE](VoLTE.md)를 지원하지 않고 있다. [LG U+](LG%20U+.md)가 [아이폰 6](%EC%95%84%EC%9D%B4%ED%8F%B0%206.md)를 출시하면서 어느 정도 해결이 되기는는 했으나, 아직 안드로이드 쪽에서는 근본적인 방법이 나왔다고 보기는 어려운 상황이다.

