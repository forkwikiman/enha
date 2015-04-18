  * 상위 항목 : [3G](3G.md)  

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

> **Time-Division Synchronus Code Division Multiple Access **  
시분할 연동코드 분할 다중 접속

## Contents

    

1. 개요 
2. 상세 
3. 전용 단말기 수급 
4. 발전 기술 
    

4.1. TD-HSDPA

4.2. TD-HSUPA

5. 후속 기술 

[[edit](http://rigvedawiki.net/r1/wiki.php/TD-SCDMA?action=edit&section=1)]

## 1. 개요 ¶

[중국](%EC%A4%91%EA%B5%AD.md)의 CATT가 중심이 되어 [중국](%EC%A4%91%EA%B5%AD.md)의
통신 장비업체인 다탕 모바일과 [독일](%EB%8F%85%EC%9D%BC.md)의 지멘스가 공동으로 개발한 제 3세대 이동통신
기술이다. 한국이 주도한 [Mobile WiMAX](Mobile%20WiMAX.md)와 마찬가지로 퀄컴 등 타국의 기술인
[CDMA](CDMA.md)와 [WCDMA](WCDMA.md)를 사용하는 대가로 로열티 지급을 하지않고 로열티를 받아 먹기위해서
개발했다고 한다.

  

다만, [Mobile WiMAX](Mobile%20WiMAX.md)는 나름대로 보급이 되었지만, 이건 사실상 중국의
[차이나모바일](%EC%B0%A8%EC%9D%B4%EB%82%98%EB%AA%A8%EB%B0%94%EC%9D%BC.md) 단독 사용
규격이 되어버렸다. 거창한 다른 문제 때문이 아니라 보급이 전혀 되지를 않아서 **보급 실패**(...)라는 아주 간단한 이유 되시겠다.
이후 시간이 흘러 4세대 이동통신 기술이 활성화 될 시기가 오자 TD-SCDMA 대신에 [TD-LTE](TD-LTE.md)를 보급하는데
주력하고 있다. 재밌는 사실이 있다면 [TD-LTE](TD-LTE.md)는 TD-SCDMA와는 다르게 중국 기술도 아니다. 자세한
내용은 후술.

  

1998년부터 연구되고 상용화까지 되었으며 국제통신연맹(ITU)으로 부터 [CDMA2000](CDMA2000.md),
[WCDMA](WCDMA.md)와 함께 3세대 이동통신 기술 표준으로 인증받았다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/TD-SCDMA?action=edit&section=2)]

## 2. 상세 ¶

사실 이 기술은 **UMTS-TDD**라는 이름으로도 불리고있다. 이는 흔히 우리가 알고있는 [WCDMA](WCDMA.md)의 첫번째
기술인 UMTS와 유사하지만 전혀 다른 모습을 하고있기 때문이다.

  

기본적으로 많은 사람들이 알고있는 [CDMA](CDMA.md)나 [WCDMA](WCDMA.md) 등의 통신 기술들은 FDD 방식을
이용한다. 이는 사용하는 주파수에 송수신 주파수가 따로 있어서 따로따로 처리 할 수 있다는 장점이 있다. 또한 대부분의 통신 기술이 FDD
방식으로 개발되기 때문에 주파수를 재활용 할 수 있다.`[1]`

  

TD-SCDMA의 경우 TDD 방식(시분할 방식)을 이용한다. TDD 방식이란 송수신 주파수가 따로 있지 않은 하나의 스펙트럼으로만 구성되어
있으며 송수신 신호를 **짧은 시간적 간격을 두고 전환**하면서 사용하게 된다. 이 경우 상대적으로 널널한 송신 주파수 대역을 과감하게
줄이고 트래픽이 넘쳐나는 수신 주파수에 많은 대역폭을 할당해서 보다 효율적으로 통신 서비스를 할수가 있다는 것이 특징이다. 중국 국영기관의
연구 결과에 따르면 이러한 방식으로 인구 밀도가 높은 대도시에 적용할 경우 기존 [WCDMA](WCDMA.md)보다 30% 이상의
주파수 효율을 높일수 있다고 한다.

  

다만, 이러한 방식은 단점도 존재한다. FDD 방식의 경우 송수신 주파수가 따로 되어있기 때문에 송신이든 수신이든 끊김이 없다. 하지만
TDD 방식은 아무리 빠르게 전환한다고 하지만 결과적으로는 그 짧은 시간에 송신이나 수신이 먹통이 된다. 따라서 전반적으로 커버리지가
좁아질수 밖에 없다. 거기에 TDD 방식의 주파수들은 2 GHz 이상의 고주파수 들이다. 높은 주파수일수록 멀리가지 못하고 건물을 통과하기가
힘들기 때문에 좁은 커버리지라는 단점을 더욱 심화시켜 버린다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/TD-SCDMA?action=edit&section=3)]

## 3. 전용 단말기 수급 ¶

[Mobile WiMAX](Mobile%20WiMAX.md)처럼 소수, 이쪽은, 전 세계에서 유일하게
[차이나모바일](%EC%B0%A8%EC%9D%B4%EB%82%98%EB%AA%A8%EB%B0%94%EC%9D%BC.md)만 유일하게
사용하는 통신 기술이기 때문에 단말기 수급 자체는 [CDMA](CDMA.md)는 물론 [MobileWiMAX](Mobile%20WiMAX.md)보다 더 어렵다. 때문에 통신 모뎀 개발 자체가 통신 서비스가 상용화 된 2000년도
초기에도 활발하지 않아서 TD-SCDMA의 지원은 FPGA 보드를 이용해서 간접적으로 구현하는 정도였다. 하지만, 2004년에
[삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md)에서 TD-SCDMA와
[GSM](GSM.md) 원칩 통신 모뎀을 상용화 하는 것을 시작으로 미약하지만 TD-SCDMA를 지원하는 통신 모뎀의 개발이
시작되었다. 또한 2012년 들어서 퀄컴의 AP 브랜드인 [퀄컴 스냅드래곤](%ED%80%84%EC%BB%B4%20%EC%8A%A4%EB%83%85%EB%93%9C%EB%9E%98%EA%B3%A4.md)이 S4 라인업 부터 TD-SCDMA 통신을 지원하기 때문에 따로 통신
모뎀을 넣는 번거로움은 이제 없어진 상황이다.`[2]`

  

물론, 이 내용은 기술과 상용화 정도만 생각한 부분이지만, 이 모든 것을 상쇄하고도 남을 무기가
[차이나모바일](%EC%B0%A8%EC%9D%B4%EB%82%98%EB%AA%A8%EB%B0%94%EC%9D%BC.md)에게는
존재한다. 바로 **가입자 수**다. 가입자 수가 7억 6천만명이라는 방대한 규모를 자랑하는 전세계 1위 사업자이기 때문에 기술적인
번거로움이 있더라도 제조사들이 알아서 만들어준다. 이런 상황이기 때문에
[차이나모바일](%EC%B0%A8%EC%9D%B4%EB%82%98%EB%AA%A8%EB%B0%94%EC%9D%BC.md)로의 공급은
상당한 수준을 넘어 [WCDMA](WCDMA.md) 급으로 원활한 편이다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/TD-SCDMA?action=edit&section=4)]

## 4. 발전 기술 ¶

[WCDMA](WCDMA.md)의 초기 기술인 UMTS가 HSDPA와 HSUPA 등으로 개선된 것처럼 TD-SCDMA도 TD-
HSDPA, TD-HSUPA 등으로 발전되었다. 이 두 기술 모두 [WCDMA](WCDMA.md)와 마찬가지로 이쪽도 3.5G~
3.9G로 분류되기도 하나, 대외적으로는 [그냥 TD-SCDMA](%EA%B7%B8%EB%83%A5%20%EC%8B%9C%EC%B2%B4.md)로 통일된다. 자세한 내용은 하단에 후술한다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/TD-SCDMA?action=edit&section=5)]

### 4.1. TD-HSDPA ¶

**TD-HSDPA**  
**시분할 연동 고속 하향 패킷 접속**

  

UMTS와 HSDPA의 차이점과 동일하다. 다운로드 속도가 기존보다 7배 빠른 2.8 Mbps로, 동영상, 사진 등의 멀티미디어 콘텐츠와
대용량 파일 다운로드가 수월해졌다. 이는 중국 정부가 추진한 3.5G 이동통신 규격으로
[차이나모바일](%EC%B0%A8%EC%9D%B4%EB%82%98%EB%AA%A8%EB%B0%94%EC%9D%BC.md)이 단독으로
서비스하고 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/TD-SCDMA?action=edit&section=6)]

### 4.2. TD-HSUPA ¶

**TD-HSUPA**  
**시분할 연동 고속 상향 패킷 접속**

  

UMTS와 HSUPA의 차이점과 동일하다. TD-HSDPA가 다운로드 속도를 개선했다면, 이쪽은 업로드 속도를 중점적으로 개선하여 기존
384 Kbps에서 2.2 Mbps로 빨라졌다. 역시
[차이나모바일](%EC%B0%A8%EC%9D%B4%EB%82%98%EB%AA%A8%EB%B0%94%EC%9D%BC.md)이 단독으로
서비스하고 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/TD-SCDMA?action=edit&section=7)]

## 5. 후속 기술 ¶

WCDMA의 후속 기술이 [LTE](LTE.md)-FDD인 것처럼 이쪽도 TD-SCDMA의 후속 기술은 [TD-LTE](/wiki
/TD-LTE)라고 **언플을 글로벌 급으로 하고 있다**. 다만, [TD-LTE](TD-LTE.md) 항목에도 나와있듯이 [TD-LTE](TD-LTE.md)는 TD-SCDMA와는 **근본부터가 다른 기술**이다.

  

TD-SCDMA는 누가 뭐래도 중국측 기술이 다량으로 들어간 진성 **중국 독자 기술**이라면 [TD-LTE](TD-LTE.md)는
그저 [LTE](LTE.md)-FDD를 TDD식의 주파수에서도 사용할 수 있게 개량한 것`[3]`으로 중국 기업 외에도 많은 기업들이
[TD-LTE](TD-LTE.md)의 상용화를 위해 별도적으로 통신 연합체를 구성해서 교류를 하고 있다. 여기서 중국의 역할을 뽑자면
**많은 기업이 밥상에 앉아있고 중국이 숟가락을 나눠준 것**이라 표현 할 수 있다. 그리고 그 숟가락을 나눠준 대가로 본래의
[LTE](LTE.md)-TDD라는 명칭이 TD-SCDMA를 계승한다는 의미로 [TD-LTE](TD-LTE.md)라
변경되었다.`[4]`

`\----`

  * `[1]` [KT](KT.md)가 [CDMA](CDMA.md)를 서비스 하던 1.8 GHz 주파수를 그대로 [LTE](LTE.md)로 사용할 수 있었던 것도 이것 때문이다.
  * `[2]` AP가 지원한다는 것은 통신 모뎀까지 AP안에 들어있는 원칩인 상태에서 TD-SCDMA까지 지원을 한다는 이야기다. 물론, 2013년 현재 퀄컴에서 제조하는 원칩 통신 모뎀(즉, AP에 포함이 되어 있지 않은 상태)에도 TD-SCDMA는 지원하고 있다.
  * `[3]` 예를 한가지 들자면 TD-SCDMA의 경우 [WCDMA](WCDMA.md)와는 무관하게 ITU의 인증을 받아야 했었다. 하지만 [TD-LTE](TD-LTE.md)의 경우 ITU의 인증을 받지 않았다. 그 이유는 **이미 [LTE](LTE.md)가 인증 받았는데 같은 것을 또 인증받는 바보는 없거든**(...). <del>이름이 다르다고 TD-SCDMA와 [WCDMA](WCDMA.md)가 따로따로 인증 받은게 아니다</del>
  * `[4]` 다만, 일본 [소프트뱅크](%EC%86%8C%ED%94%84%ED%8A%B8%EB%B1%85%ED%81%AC.md)는 그냥 무시하고 **AXGP**라는 명칭으로 서비스 하고 있다. 초창기에는 독자 규격이라고 우려있는 목소리가 많았으나 [TD-LTE](TD-LTE.md)와 호환된다는 소식이 나오자 잠잠해졌다.

