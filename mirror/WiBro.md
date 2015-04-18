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

한국 통신사 주파수 할당 내역 - WiBro

통신사

주파수`[1]`

대역폭`[2]`

기타

[SK텔레콤](SK%ED%85%94%EB%A0%88%EC%BD%A4.md)

LTE Band 40 2.3 GHz

27 MHz

[KT](KT.md)

LTE Band 40 2.3 GHz

27 MHz

[LG U+](LG%20U+.md)

**[그런 거 없다](%EA%B7%B8%EB%9F%B0%20%EA%B1%B0%20%EC%97%86%EB%8B%A4.md)**`[3]`
  

## Contents

    

1. 개요 
2. 기술 규격 
3. 현황 
    

3.1. [TD-LTE](TD-LTE.md)로 전환?

3.2. 와이브로 하이브리드

[[edit](http://rigvedawiki.net/r1/wiki.php/WiBro?action=edit&section=1)]

## 1. 개요 ¶

와이브로(WiBro) : **Wi**reless **Bro**adband

  

이동하면서도 초고속 인터넷을 이용할 수 있는 무선 휴대 인터넷(Portable Internet)의 명칭. 기존의 무선 인터넷인
[CDMA](CDMA.md)와 무선 랜의 장점만을 취하여 새로이 만들어 낸 것이다. [WiMAX](WiMAX.md)`[4]`
표준을 따르고 있으며, 해외에는 [Mobile WiMAX](Mobile%20WiMAX.md)로 알려져 있다.

  

[삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md)와 한국전자통신연구원(ETRI)에서 고안한
휴대인터넷 기술 표준 'HPi' (High-speed Portable Internet)를 정부가 국내 휴대인터넷 기술표준 초안으로 확정하면서
와이브로라는 명칭을 정했다. 그리고 이 기술표준은 2005년 12월 국제표준그룹인 미국 전자전자학회(IEEE)에서도 국제표준으로 채택되었다.
그리고 원래 ETRI와 삼성전자에서 만들 때도 Mobile WiMAX와 [LTE](LTE.md)가 시장을 2:8 정도로 가를 것으로
예상하였고, 실제로도 그럴듯하다.

  

현 WCDMA의 후계기술인 [LTE](LTE.md)(Long-Term Evolution)는 그 이름대로 천천히 고 스펙으로 나올
예정이었으나, 예상보다 빨리 [3G](3G.md)망이 포화 상태에 처했기 때문에, 조기에 나오지 않을 수 없게 되었고, 그 과정에서
Mobile WiMAX의 기술을 상당수 차용하게 되었다. 그렇기 때문에 ETRI와 SEC는 크게 걱정을 안 한다(...).

  

기존 2G/[3G](3G.md)망과는 다르게 시분할방식(TDD)을 사용하기 때문에 상향/하향 주파수 대역으로 나누지 않고 한 주파수
대역을 통째로 사용한다. 그래서 대한민국 통신사들이 수익이 잘 나지않는 와이브로 대신 [TD-LTE](TD-LTE.md)로 주파수 용도
변경을 요청했었지만 정부에서는 와이브로를 포기하면 주파수를 반납이라는 조건을 내세웠다.

  

보통 2.3/2.5/3.3/3.5 GHz 주파수 대역을 사용하며 대한민국
[SK텔레콤](SK%ED%85%94%EB%A0%88%EC%BD%A4.md)과 [KT](KT.md)에서 서비스 중인 주파수 대역은
2.3 GHz로 27 MHz 대역폭을 할당받았지만 전파 낭비가 따로 없게도 10 MHz 대역폭만을 사용중이다.`[5]` 30 MHz가 아닌
27 MHz 대역폭을 할당 받은 이유는 초창기 와이브로는 8.75MHz 대역폭을 사용했었고, 4.5 MHz를 가드 밴드로 사용하기 때문.
미국 [스프린트](%EC%8A%A4%ED%94%84%EB%A6%B0%ED%8A%B8%20%EC%BD%94%ED%8D%BC%EB%A0%88%EC%9D%B4%EC%85%98.md)와 일본 [KDDI](KDDI.md)는 2.5 GHz 주파수 대역을 사용한다.

  

원래 [하나로텔레콤](%ED%95%98%EB%82%98%EB%A1%9C%ED%85%94%EB%A0%88%EC%BD%A4.md)도
와이브로 사업을 추진중이었지만 2005년 4월 25일 사업을 포기했다. 원래는 KT가 할당 받은 주파수 대역 뒤의 2363―2390 MHz
대역을 할당 받을 예정이었다. <del>그리고 SK텔레콤에 합병되었다</del>

  

후계 기술로 [WiBro Evolution](WiBro%20Evolution.md)이 발표되었으며, 2010년 6월 16일, [LTEAdvanced](LTE%20Advanced.md)와 함께 [4G](4G.md) 국제 표준을 통과하였다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/WiBro?action=edit&section=2)]

## 2. 기술 규격 ¶

IEEE 표준

802.16e

사용 주파수대

2.3 GHz

통신 가능 이동 속도

60km/h, 최대 120km/h

최대 전송 거리

1km

최고 전송 속도

약 25Mbps (Wave 2 IP 대역폭 기준)

평균 전달 속도

5~6Mbps

변조 방식

광대역 OFDM 방식

`[6]`

  

WiMax Release 1은 10 MHz TDD 환경에서 다운로드 37 Mbps, 업로드 17 Mbps를 지원하며 개선된 WiMax
Release 1.5(IEEE 802.16e-2009)는 우리나라에서는 WAVE 2라고 불리우며 20 MHz TDD 환경에서 다운로드 83
Mbps, 업로드 46 Mbps를 지원한다. 이후 규격인 WiMAX Release 2는 [WiBroEvolution](WiBro%20Evolution.md)라고 불리운다.

  

국내에서 초창기에 선보인 WAVE 1은 8.75 MHz 대역폭을 사용하며 [WCDMA](WCDMA.md)(HSDPA·HSUPA)의 약
1.7배의 속도인 25Mbps를 지원하고, 이후 개선된 WAVE 2는 10 MHz 대역폭을 사용하며 WCDMA의 약 2.8배의 속도인
40Mbps를 지원한다. 환경에 따라 다르지만 WAVE 2의 실제 평균 전송 속도는 10Mbps 안팎. 신호 품질이 좋다면 18Mbps도
가능하다. 이론상 최대 하향 128Mbps, 상향 56Mbps 까지 가능하다고 하지만 [KT](KT.md)나
[SK텔레콤](SK%ED%85%94%EB%A0%88%EC%BD%A4.md) 와이브로 신규 투자가 거의 없어서 지원될 가능성이 적어졌다.
애초에 할당받은 27 MHz 중에서 17 MHz를 놀려먹고있는 상황이다.

  

KDDI의 경우 할당받은 30MHz를 낭비없이 활용하고 있으며 기본 다운로드 40Mbps, 업로드 15.4Mbps를 지원하며 2013년 7월
29일에 20MHz를 더 할당받아 후계 규격인 [WiBro Evolution](WiBro%20Evolution.md) 기반의`[7]`
WiMAX2+는 다운로드 110Mbps, 업로드 10Mbps를 지원한다. [관련
기사](http://www.it.co.kr/news/mediaitNewsView.php?nSeq=2416268) 심지어 2014년 3월에는
220Mbps까지 지원한다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/WiBro?action=edit&section=3)]

## 3. 현황 ¶

우리 나라가 원천기술을 가지고 있고 세계 최초로 상용화시킨 [4G](4G.md) 이동통신기술이지만, 개발 당초에는 적극적으로 참여하는
척하던 국내 이동통신 3사는 4G 투자를 최대한 미뤄보겠다는 생각으로 국내에서 개발한 와이브로가 아닌 [LTE](LTE.md)를
선택하려고 하고 있다. 그래서인지 국내에선 찬밥 대우라 광고도 잘 안했었다.

  

그러나 2011년 현재 [스마트폰](%EC%8A%A4%EB%A7%88%ED%8A%B8%ED%8F%B0.md)의 대중화와 이로 인한
데이터 사용량 급증으로 인해, 3G망은 포화 상태에 처해있기 때문에 4G망을 설치 안 할 수도 없는 노릇이 되었다. 주로 <del>사업
초기에는 안그랬는데 갈수록 3G망의 품질이 나빠지는</del> [KT](KT.md)에서 많이 광고로 써먹고 있다. 또한 지하철
열차내에서도 와이브로를 쓰는 퍼블릭 에그로 [Wi-Fi](Wi-Fi.md) 망을 구축하고 있다.`[8]` 와이브로를 지원하지 않는
[아이폰](%EC%95%84%EC%9D%B4%ED%8F%B0.md)을 위해 폰에 케이스처럼 끼워서 쓰는 와이브로 단말도 나온 상태.
[EVO 4G+](EVO%203D#s-5.md)등 와이브로 전용 단말도 나온 상태이며, 외국인 등을 위해
[인천국제공항](%EC%9D%B8%EC%B2%9C%EA%B5%AD%EC%A0%9C%EA%B3%B5%ED%95%AD.md)등에서는
[에그](olleh%20%EC%97%90%EA%B7%B8.md)를 일 단위로 렌탈해주기도 한다. 사용해본 외국분의 전언의 따르면
'자국에서 쓰던 유선 인터넷 수준을 어디서나 쓸수 있다니 놀랍다', '이 정도면 유선 인터넷 선을 찾지 않아도 되겠다(충전기만 꽂으면).'
뭐 스마트폰이야 4G를 좋아한다 치고, 귀찮은걸 싫어하는 일반 사용자들이 별로 안 좋아한다는게 문제. 배터리나 커버리지 등이 문제기도
하고... 그 외 KT 와이브로에 관해서는 [olleh와이브로](olleh%20%EC%99%80%EC%9D%B4%EB%B8%8C%EB%A1%9C.md)참조.

  

[SK텔레콤](SK%ED%85%94%EB%A0%88%EC%BD%A4.md)은 주로 [Wi-Fi](Wi-Fi.md)존 구축에
활용하고 있으며 스마트폰이나 브릿지 같은 개인용 단말기 판매는 다소 소극적이다. 2012년 7월
[방통위](%EB%B0%A9%ED%86%B5%EC%9C%84.md) 자료만 보더라도 가입자 수만 약 15배 정도 차이난다. 자세한 것은
[T 와이브로](T%20%EC%99%80%EC%9D%B4%EB%B8%8C%EB%A1%9C.md) 참조.

  

홈페이지의 커버리지 지도에서는 가능하다고 표기되어 있어도 실제로는 음영 지역인 경우가 많아서 사용자 간에 자체적으로 커버리지를 알려주는
커뮤니티를 만들었다. [홈페이지](http://www.coverage.co.kr/index.php)

  

외국에선 광대역 통신망을 깔 때 사용한다고 한다. 우리나라같이 땅덩어리가 좁아서 선 깔기가 쉬운게 아니기 때문이다. 그리고 우리나라는
신도시등을 건설하면서 주거형태를 아파트로 선택했는데 덕분에 관리사무소나 아파트 단자함까지만 광 통신망을 설치하면 장땡인것도 있다.`[9]`

  

[미국](%EB%AF%B8%EA%B5%AD.md)의 [4G](4G.md)로 유명한 통신사인 [스프린트](%EC%8A%A4%ED%94%84%EB%A6%B0%ED%8A%B8%20%EC%BD%94%ED%8D%BC%EB%A0%88%EC%9D%B4%EC%85%98.md)의
무선 통신망은 [LTE](LTE.md) 도입 전까지 Mobile WiMAX를 주력 4G망으로 사용해왔으며
[HTC](HTC.md)에서는 전용 단말기를 출시해왔다.`[10]` 2015년 11월 6일에 WiMAX를 종료할 예정이다. 기존
WiMAX 주파수는 [TD-LTE](TD-LTE.md)로 전환할 계획이며, 최근에 나온 WiMAX 단말기는 TD-LTE를 동시에
지원한다.

  

[일본](%EC%9D%BC%EB%B3%B8.md)의 [KDDI](KDDI.md)(au)의 자회사인 UQ와이어리스도 제공중으로
[3G](3G.md)가 미어터지자 2011년 가을 이후 스마트폰에 본격적으로 탑재하고 있다. 기본적으로 스프린트와 KDDI는
CDMA2000 1x EV-DO 망이기 때문에 이 서비스로 4G를 제공했다. 2012년부터는 삼성 갤럭시나 LG 옵티머스 등 한국제
WiMAX 탑재 기종이 본격적으로 투입되었다. KDDI는 스프린트나 국내 통신사들과는 다르게 [WiBroEvolution](WiBro%20Evolution.md)을 적극적으로 밀고 있으며, 최근에는 [LTE](LTE.md)와
WiBro Evolution를 동시 지원하는 단말기를 판매하고 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/WiBro?action=edit&section=4)]

### 3.1. [TD-LTE](TD-LTE.md)로 전환? ¶

2013년 [LTE](LTE.md)가 대세가 된 지금 와이브로 주파수를 [TD-LTE](TD-LTE.md)로 전환을 정부 차원에서
추진하고 있다. [#](http://m.news.naver.com/read.nhn?mode=LSD&mid=sec&sid1=105&oid=03
2&aid=0002339723) 그리고 미래창조과학부에서 TD-LTE로 전환을 허용했다.
[#](http://zdnet.co.kr/news/news_view.asp?artice_id=20130913153757) 다만 기존 2.3
GHz 모두를 전환하지는 않고 일부만 TD-LTE로 전환하기 때문에(예를 들어, 와이브로에 10 MHz / TD-LTE에 20 MHz)
결과적으로 와이브로 자체를 종료하지는 않을것으로 보인다. 사실 와이브로를 철수시키면 당장 버스나 지하철 전동차의 와이파이 존도 걷어내고
LTE 기반 라우터로 갈아야 하는데 미쳤다고 공짜로 LTE를 쓰도록 할 리가 없지 않은가.`[11]` 거기다 2013년 12월 23일
KT에선 스트롱 에그 3를 출시했다.

  

이미 스프린트나 KDDI에서도 와이브로와 LTE를 동시 지원하는 단말기를 제조하고 있다. 하지만 SK텔레콤이나 KT처럼 기존 와이브로망
지원을 크게 줄이고 LTE로 완전 전환이 아닌 서로 보충재의 역할을 하면서 기술 개선을 하고 있다는 점에서 차이가 난다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/WiBro?action=edit&section=5)]

### 3.2. 와이브로 하이브리드 ¶

어떻게든 계륵이 된 와이브로를 살려보고자 [KT](KT.md)에서 출시한 상품. 요금은 2배 가까이 오르지만. 와이브로 커버리지
구역에선 와이브로로 속도 제한없이 사용가능하며. 그외 촌구석이나 소도시여서 와이브로 망이 없는경우, [LTE](LTE.md) 망으로
연결되고 6 Mbps로 QoS가 걸린다.`[12]`

  

720p 정도는 간신히 볼수는 있으니, 속도에 크게 연연하지 않는다면 와이브로 비 커버리지에 살거나 자주 오가는경우, LTE 데이터 중에선
가장 싸다.`[13]`

`\----`

  * `[1]` WiBro용 Band 표기가 없기 때문에 LTE Band 표기를 따른다.
  * `[2]` WiBro를 서비스 할 수 있는 주파수 방식은 TDD 방식이다. 이 방식은 상하향이 분리되어 있지 않다.
  * `[3]` 이 때문에 다른 통신사는 다 설치하는 대중교통(지하철, 버스)내 와이파이존을 LG U+만 깔지 못한다. <del>지하철 안에서 와이파이 못쓰는 LG U+ 고객들 지못미</del>
  * `[4]` 이전까지 엔하위키에는 WiMAX가 WiBro 항목으로 리다이렉트되어 있었으나, 명백히 다른 것이다. 자세한 것은 항목 참조
  * `[5]` 당장 에그/브릿지 설명서 제원표만 봐도 2.3 GHz 대역을 10 MHz만 쓴다고 나와 있다.
  * `[6]` 출처 : 위키피디아 와이브로 문서
  * `[7]` 정확히는 WiMAX Release 2.1
  * `[8]` 이 때문에 실내만 들어가도 잘 안 되는 와이브로가 지하철 터널 안에서는 잘 되는 것을 볼 수 있다.
  * `[9]` 예로, 집에 컴퓨터가 10대 가까이 있는데 제각각 공유기와 허브와의 위치랑 동떨어진 곳에 있다면? 일일이 UTP 케이블로 연결하는 대공사를 치르는것 보다는 [Wi-Fi](Wi-Fi.md)로 연결하는게 더 나을 것이다.
  * `[10]` 이 것이 [HTC EVO](HTC%20EVO.md) 시리즈로 [KT](KT.md)에서는 [EVO 3D](EVO%203D.md)를 로컬라이징해서 [EVO 4G+](EVO%203D#s-5.md)로 들여왔다.
  * `[11]` [T 와이브로](T%20%EC%99%80%EC%9D%B4%EB%B8%8C%EB%A1%9C.md)는 30GB를 5천원에, [olleh 와이브로](olleh%20%EC%99%80%EC%9D%B4%EB%B8%8C%EB%A1%9C.md)는 10GB를 만원에 제공하지만 LG U+ LTE 라우터는 5GB를 3만원에 제공한다. 비교해보면 1MB 당 SK텔레콤은 약 0.16원 씩, KT는 약 1원 씩, LG U+는 약 6원 씩으로 패킷 당 단가의 차이가 제법 난다.
  * `[12]` 망 개선이 없이 생색내기로 깔린 중규모 도시는 와이브로 속도 제한 없는 속도가 이것과 비슷하거나 조금 나은 속도로 나온다.
  * `[13]` LG U+의 10GB 플랜이 거의 6만원에 달하나, 와이브로 하이브리드는 2만원이면 된다.

