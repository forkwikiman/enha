## Contents

    

1. 개요 
2. 생산 기업 
3. AP 목록 
    

3.1. A4

3.2. A5

3.3. A5X

3.4. A6

3.5. A6X

3.6. A7

3.7. A8

3.8. A8X

[[edit](http://rigvedawiki.net/r1/wiki.php/%EC%95%A0%ED%94%8C%20A%20%EC%8B%9C%
EB%A6%AC%EC%A6%88?action=edit&section=1)]

## 1. 개요 ¶

[애플](%EC%95%A0%ED%94%8C%28%EA%B8%B0%EC%97%85%29.md)의 소형 디바이스에 탑재되는
[SoC](SoC.md). [CPU](CPU.md)는 [ARM Holdings](ARM%20Holdings.md)의 [ARMCortex-A 시리즈](ARM%20Cortex-A%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md)를 라이센스 취득하거나
명령어 셋을 라이센스 받아서 자체 CPU 아키텍쳐를 제작해서 사용하며 [GPU](GPU.md)는 이매지네이션 테크놀러지의 PowerVR
시리즈를 라이센스 취득해서 사용한다.

  

다른 AP와는 다르게, 애플 A 시리즈의 경우에는 아이폰 또는 아이패드를 발표하는 키노트에서 공개되는 정보 이외에는 어떤 정보도 주어지지
않는데, 이는 [애플](%EC%95%A0%ED%94%8C%28%EA%B8%B0%EC%97%85%29.md)이 AP 시장에 진출한 목적
자체가 특수하기 때문이다. [애플](%EC%95%A0%ED%94%8C%28%EA%B8%B0%EC%97%85%29.md)은 오로지 자사의
제품에만 사용할 목적으로 독자 아키택쳐까지 개발하는 <del>변태</del>특수한 기업이다. 사실상 소수 기종을 천문학적인 단위로 팔아치우는
애플만이 가능한 재주로, [삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md)와 같은 제품 다변화를
통해 수요 창출에 나서는 다른 기업과의 차이에서 생기는 특수성 때문이다. 타 AP 제조사의 경우에는, 일단 모바일 시장을 주력으로 하는 것은
애플과 같지만 [ARM](ARM.md) 아키텍쳐의 장점인 저전력을 무기로 차량용 AP,
[몇몇](nVIDIA%20SHIELD%20Portable.md) [게임기](PS%20VITA.md)용 AP,
[전자시계](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20%EA%B8%B0%EC%96%B4.md)용 AP, 심지어는 서버용
AP까지 수요를 확대하려는 노력을 하고 있다.`[1]`

  

또한 괴물같은 최적화 능력으로 동 시기에 출시된 안드로이드 기기들을 상회하는 퍼포먼스를 자랑한다.`[2]``[3]` 이렇게 함으로써 AP에
[CPU](CPU.md)가 차지하는 부분을 최소화`[4]`하고 최적화만으로 해결하기 어려운 [GPU](GPU.md)에게 면적을
할당하는 경향이 있다.`[5]` 덕분에 애플 A 시리즈는 AP 다이샷을 보면 숫자가 커질수록 [GPU](GPU.md)가 [크고아름다운](%ED%81%AC%EA%B3%A0%20%EC%95%84%EB%A6%84%EB%8B%A4%EC%9A%B4.md) 사이즈를
자랑하며, 성능 역시 동 시기에 출시되는 경쟁사의 AP의 [GPU](GPU.md)를 압도한다.`[6]` 위에서 언급한대로
[삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md)를 포함한 타 AP 제조사들은 서버용 시장까지
고려하고 있기 때문에 [CPU](CPU.md)의 비중을 줄이기 어렵다. 때문에 [GPU](GPU.md)의 비중이 큰 애플 A
시리즈와 차이를 보인다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/%EC%95%A0%ED%94%8C%20A%20%EC%8B%9C%
EB%A6%AC%EC%A6%88?action=edit&section=2)]

## 2. 생산 기업 ¶

전통적으로 [삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md) 시스템 LSI 사업부의 팹에서 생산하고
있다. 이는 애플 A 시리즈가 정식 공개되기 이전의 모델인
[아이폰](%EC%95%84%EC%9D%B4%ED%8F%B0/1%EC%84%B8%EB%8C%80.md)과 [아이폰3G](%EC%95%84%EC%9D%B4%ED%8F%B0%203G.md), [아이폰3GS](%EC%95%84%EC%9D%B4%ED%8F%B0%203GS.md)가
[삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md)의 AP를 그대로 사용했고, 애플 A 시리즈역시
Apple A5X 이전까지는 [삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md) 시스템 LSI
사업부가 설계 분야에 관여한 부분이 있기 때문이다.

  

다만, [삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md) 무선 사업부가 애플을 제외하면 가장
영향력이 큰 [스마트폰](%EC%8A%A4%EB%A7%88%ED%8A%B8%ED%8F%B0.md) 제조사`[7]`가 되었기 때문에 보안
등의 이유로 이른바 '탈 삼성'이 이루어지고 있다. AP부분에서는 대체할 기업이 마땅치 않아서 완벽한 자체 설계로 전환된 Apple A6
이후에도 [삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md) 시스템 LSI 사업부에서 생산하고 있다.

  

하지만, AP 부분에서도 비중은 적어지고 있는 상황이다. 이미 [TSMC](TSMC.md)에 대규모의 20nm급 공장에 투자하고 있으며
매해마다 끊이지 않고 [TSMC](TSMC.md) 전환 설이 흘러나오고 있다.

  

2013년 11월 12일, 2차 공급사로 '글로벌 파운더리'(이하 'GF')가 될 것이라는 [주장](http://www.zdnet.co.kr
/news/news_view.asp?artice_id=20131112063742&type=xml)이 나왔다. 현재
[디스플레이](%EB%94%94%EC%8A%A4%ED%94%8C%EB%A0%88%EC%9D%B4.md) 패널을
[LG디스플레이](LG%EB%94%94%EC%8A%A4%ED%94%8C%EB%A0%88%EC%9D%B4.md)와 샤프 디스플레이가 주로
공급하는 것처럼 AP도 [TSMC](TSMC.md)와 GF가 주 공급사가 될 가능성이 높다.`[8]`

  

[[edit](http://rigvedawiki.net/r1/wiki.php/%EC%95%A0%ED%94%8C%20A%20%EC%8B%9C%
EB%A6%AC%EC%A6%88?action=edit&section=3)]

## 3. AP 목록 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/%EC%95%A0%ED%94%8C%20A%20%EC%8B%9C%
EB%A6%AC%EC%A6%88?action=edit&section=4)]

### 3.1. A4 ¶

![http://i1-news.softpedia-static.com/images/news2/iPhone-Prototype-Teardown-
Vietnam-Reveals-Apple-A4-Chip-2.jpg?width=400](http://i1-news.softpedia-
static.com/images/news2/iPhone-Prototype-Teardown-Vietnam-Reveals-
Apple-A4-Chip-2.jpg)

[[JPG external image]](http://i1-news.softpedia-static.com/images/news2
/iPhone-Prototype-Teardown-Vietnam-Reveals-Apple-A4-Chip-2.jpg)

  

프로세서

S5L8930

[CPU](CPU.md)

[ARM Cortex-A8](ARM%20Cortex-A8.md) MP1 800 MHz ~ 1 GHz

[GPU](GPU.md)

IT PowerVR SGX535 -- MHz

[메모리](%EB%A9%94%EB%AA%A8%EB%A6%AC.md)

32-bit 듀얼채널 LPDDR -- MHz

생산 공정

삼성 S.LSI 45nm

주요  
사용 기기

[아이폰 4](%EC%95%84%EC%9D%B4%ED%8F%B0%204.md),
[아이패드/1세대](%EC%95%84%EC%9D%B4%ED%8C%A8%EB%93%9C/1%EC%84%B8%EB%8C%80.md),
[아이팟 터치 4세대](%EC%95%84%EC%9D%B4%ED%8C%9F%20%ED%84%B0%EC%B9%98%204%EC%84%B8%EB%8C%80.md), 애플 TV 2세대

  
[애플](%EC%95%A0%ED%94%8C%28%EA%B8%B0%EC%97%85%29.md) 브랜드의 AP인 A 시리즈의 첫번째
AP이다. [애플](%EC%95%A0%ED%94%8C%28%EA%B8%B0%EC%97%85%29.md)은 이전까지
[삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md)의 AP를 그대로 납품 받았다.

  

[엑시노스](%EC%97%91%EC%8B%9C%EB%85%B8%EC%8A%A4.md) 브랜드의 전신인 [삼성전자 허밍버드](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90%20%ED%97%88%EB%B0%8D%EB%B2%84%EB%93%9C.md)와
코어 구성이 거의 같다.`[9]` 당시 [삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md)는
[ARM](ARM.md) Cortex-A8의 클럭을 1 GHz를 넘기기 위해서 별의 별 행동을 다 하고 있었는데, 애플이 데려온
인트린시티 사와 함께 코어 커스텀을 하고 [삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md)의 도미노
로직을 사용해 최초로 1 GHz의 클럭을 달성했다.

  

다만, 전력 문제로 [아이폰 4](%EC%95%84%EC%9D%B4%ED%8F%B0%204.md)에는 800 MHz, 배터리의 여유가
있는
[아이패드/1세대](%EC%95%84%EC%9D%B4%ED%8C%A8%EB%93%9C/1%EC%84%B8%EB%8C%80.md)에는 1
GHz로 클럭이 조정되어 들어간다.

  

[엑시노스](%EC%97%91%EC%8B%9C%EB%85%B8%EC%8A%A4.md) 3110과 차이가 있다면 GPU가 SGX540에서
SGX535로 다운그레이드 되어 있다는 점 정도가 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/%EC%95%A0%ED%94%8C%20A%20%EC%8B%9C%
EB%A6%AC%EC%A6%88?action=edit&section=5)]

### 3.2. A5 ¶

![http://www.engineering.com/Portals/0/BlogFiles/Electronics%20Design/A5%20Sin
gle%20Core%20Digital%20Blocks%20Annotated.png?width=400](http://www.engineerin
g.com/Portals/0/BlogFiles/Electronics%20Design/A5%20Single%20Core%20Digital%20
Blocks%20Annotated.png)

[[PNG external image]](http://www.engineering.com/Portals/0/BlogFiles/Electron
ics%20Design/A5%20Single%20Core%20Digital%20Blocks%20Annotated.png)

  

프로세서

S5L8940

S5L8942

S5L8947

[CPU](CPU.md)

[ARM Cortex-A9](ARM%20Cortex-A9.md) MP2 800 MHz ~ 1 GHz

[ARM Cortex-A9](ARM%20Cortex-A9.md) MP1 -- MHz

[GPU](GPU.md)

IT PowerVR SGX543 MP2 -- MHz

[메모리](%EB%A9%94%EB%AA%A8%EB%A6%AC.md)

\---bit --채널 LPDDR2 -- MHz

생산 공정

삼성 S.LSI 45nm

삼성 S.LSI 32nm HKMG

주요  
사용 기기

[아이폰 4s](%EC%95%84%EC%9D%B4%ED%8F%B0%204s.md), [아이패드2](%EC%95%84%EC%9D%B4%ED%8C%A8%EB%93%9C%202.md)`[A]`, [아이팟 터치 5세대](%EC%95%84%EC%9D%B4%ED%8C%9F%20%ED%84%B0%EC%B9%98%205%EC%84%B8%EB%8C%80.md)

[아이패드 2](%EC%95%84%EC%9D%B4%ED%8C%A8%EB%93%9C%202.md)`[A]`, [아이패드미니](%EC%95%84%EC%9D%B4%ED%8C%A8%EB%93%9C%20%EB%AF%B8%EB%8B%88.md)

애플 TV 3세대

  
A4 AP를 [삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md)와 같이 협력한 인트린시티를
[애플](%EC%95%A0%ED%94%8C%28%EA%B8%B0%EC%97%85%29.md)이 인수한 후, 본격적으로 애플의 비중이
커진 AP다. 이전 A4가 [삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md)의 비중이 컸다면, A5
부터는 [애플](%EC%95%A0%ED%94%8C%28%EA%B8%B0%EC%97%85%29.md)의 비중이 커지고,
[삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md)는 생산의 역할이 강해졌다. 다만,
[삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md) 역시 [ARM](ARM.md)에게 라이센스를
사와서 [엑시노스](%EC%97%91%EC%8B%9C%EB%85%B8%EC%8A%A4.md)를 만드는 만큼, 관련 기술자가 상주하고
있어 큰 차질없이 협력을 할 수 있었다고 한다.`[11]`

  

[ARM](ARM.md) Cortex-A9 듀얼 코어 구성으로 최대 클럭은 1 GHz이다. [아이폰4s](%EC%95%84%EC%9D%B4%ED%8F%B0%204s.md)와 아이팟터치 5세대는 800 MHz, 아이패드 미니,
[아이패드 2](%EC%95%84%EC%9D%B4%ED%8C%A8%EB%93%9C%202.md)와 애플 TV에는 1 GHz로 들어간다.
그런데, 퍼포먼스는 800 MHz로 돌리는 소형 기기나 1 GHz로 돌리는 대형 기기나 별 차이 없다. 애플의 괴물같은
[최적화](%EC%B5%9C%EC%A0%81%ED%99%94.md) 능력을 과시한 사례 중 하나로 꼽히고 있다.

  

GPU는 PoweVR SGX543 듀얼 코어를 사용하여 당시 모든 AP들을 성능으로 압도했다.

  

현재는 [엑시노스](%EC%97%91%EC%8B%9C%EB%85%B8%EC%8A%A4.md) 4210의 Mali-400 쿼드 코어가 수
많은 최적화가 지속적으로 개선되어 비슷한 성능을 보여주지만, A5는 애플의 AP를 논할 때 많은 사람들이 CPU가 아닌 GPU를 기대하게
되는 시발점이 되었다.

  

[엑시노스](%EC%97%91%EC%8B%9C%EB%85%B8%EC%8A%A4.md) 4210이 공정 미세화를 위해 32nm 공정을
사용하는 [엑시노스](%EC%97%91%EC%8B%9C%EB%85%B8%EC%8A%A4.md) 4212로 리버전 된 것 처럼 A5역시
32nm로 재생산되어 [아이패드 2](%EC%95%84%EC%9D%B4%ED%8C%A8%EB%93%9C%202.md)에 들어갔다. 성능
차이는 미미하지만, 공정 개선에 힘입어 30%정도 전력 효율이 올라갔다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/%EC%95%A0%ED%94%8C%20A%20%EC%8B%9C%
EB%A6%AC%EC%A6%88?action=edit&section=6)]

### 3.3. A5X ¶

![http://cdn.arstechnica.net/wp-content/uploads/2012/09/Apple-A5X-
640x634.jpeg?width=400](http://cdn.arstechnica.net/wp-content/uploads/2012/09
/Apple-A5X-640x634.jpeg)

[[JPEG external image]](http://cdn.arstechnica.net/wp-content/uploads/2012/09
/Apple-A5X-640x634.jpeg)

  

프로세서

S5L8945

[CPU](CPU.md)

[ARM Cortex-A9](ARM%20Cortex-A9.md) MP2 1 GHz

[GPU](GPU.md)

IT PowerVR SGX543 MP4 250 MHz

[메모리](%EB%A9%94%EB%AA%A8%EB%A6%AC.md)

2x64-bit 듀얼채널 LPDDR2 800 MHz

생산 공정

삼성 S.LSI 45nm`[12]`

주요  
사용 기기

[아이패드/3세대](%EC%95%84%EC%9D%B4%ED%8C%A8%EB%93%9C/3%EC%84%B8%EB%8C%80.md)

  
[아이패드/3세대](%EC%95%84%EC%9D%B4%ED%8C%A8%EB%93%9C/3%EC%84%B8%EB%8C%80.md) 공개
당시 기습적으로 공개된 A5의 파생 모델이다. **2048 x 1536**이나 되는, 당시 PC시장에서도 보기 힘든 해상도를 처리하기 위해서
A5의 GPU를 강화시킨 AP다.

  

A5에 들어갔던 PowerVR SGX543 듀얼 코어 구성을 **쿼드 코어**로 재구성하여 결과적으로 동시대 모든 AP를 압도하는 엄청난
그래픽 성능을 얻었다.

  

GPU를 강화하였지만 그 무식한 해상도를 버티기에는 완전히 만족스럽지 못했다. 특히 45nm LP공정으로 생산되어 발열이 문제가 되어서
모바일 AP로써는 이례적으로 히트 스프레더를 요했다.`[13]` 또한 GPU의 다이 사이즈가 커지다 보니 양산 수율도 빡빡해졌다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/%EC%95%A0%ED%94%8C%20A%20%EC%8B%9C%
EB%A6%AC%EC%A6%88?action=edit&section=7)]

### 3.4. A6 ¶

![http://regmedia.co.uk/2012/09/25/a6.jpg?width=400](http://regmedia.co.uk/201
2/09/25/a6.jpg)

[[JPG external image]](http://regmedia.co.uk/2012/09/25/a6.jpg)

  

프로세서

S5L8950

[CPU](CPU.md)

[Apple Swift](Apple%20Swift.md) MP2 1.3 GHz

[GPU](GPU.md)

IT PowerVR SGX543 MP3 350 MHz

[메모리](%EB%A9%94%EB%AA%A8%EB%A6%AC.md)

64-bit 듀얼채널 LPDDR2 1066 MHz

생산 공정

삼성 S.LSI 32nm HKMG

주요  
사용 기기

[아이폰 5](%EC%95%84%EC%9D%B4%ED%8F%B0%205.md), [아이폰5c](%EC%95%84%EC%9D%B4%ED%8F%B0%205c.md)

  
[아이폰 5](%EC%95%84%EC%9D%B4%ED%8F%B0%205.md)의 공개 키노트 행사에서 공개된 AP로, 기존에
[ARM](ARM.md)의 CPU 아키텍쳐를 라이센스를 취득하여 AP를 제작했다면, 이번에는 애플이 **명령어 셋 자체를 라이센스
취득**하여 아키텍쳐 자체를 직접 설계해 사용했다.

  

기존 [ARM](ARM.md) Cortex-A15까지 사용된 ARMv7 명령어 셋을 커스텀한 **ARMv7s**을 이용하여 [퀄컴 스냅드래곤](%ED%80%84%EC%BB%B4%20%EC%8A%A4%EB%83%85%EB%93%9C%EB%9E%98%EA%B3%A4.md)
에 들어가는 Scorpion, Krait 아키텍쳐처럼 **Swift**라는 자체 CPU 아키텍쳐를 사용한다.`[14]` 성능은 Krait와
비슷한 수준이며 [아이폰 5](%EC%95%84%EC%9D%B4%ED%8F%B0%205.md)에는 1.3 GHz의 클럭으로 들어간다.
성능은 기존 A5보다 두 배 정도의 성능을 보인다고 한다.

  

GPU는 PowerVR SGX543을 3개를 묶어 **트리플 코어**로 사용한다. 보편적으로 보기 힘든 홀수개 코어 구성으로, 동일한
GPU로 쿼드 코어를 구성한 A5X보다 동일한 클럭일 경우에는 성능은 떨어지지만, 둘 다 클럭 조절을 했기 때문에 결과적으로는 A5X와
동급의 성능을 보여준다.

  

이 때부터 [삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md)는
[엑시노스](%EC%97%91%EC%8B%9C%EB%85%B8%EC%8A%A4.md) 라인업에 [ARM](ARM.md)
Cortex-A 라인업을 지속적으로 사용하고 있었기 때문에 "애플 AP 삼성 설계설"은 근거가 빈약하다. 오히려 삼성이
[애플](%EC%95%A0%ED%94%8C%28%EA%B8%B0%EC%97%85%29.md)의 AP에 관여하는 정도가 크게 줄어든
것으로 보인다.

  
  

[[edit](http://rigvedawiki.net/r1/wiki.php/%EC%95%A0%ED%94%8C%20A%20%EC%8B%9C%
EB%A6%AC%EC%A6%88?action=edit&section=8)]

### 3.5. A6X ¶

![http://i1-news.softpedia-static.com/images/news2/Chipworks-Apple-s-A6X-Chip-
Is-a-Beast-2.jpg?width=400](http://i1-news.softpedia-static.com/images/news2
/Chipworks-Apple-s-A6X-Chip-Is-a-Beast-2.jpg)

[[JPG external image]](http://i1-news.softpedia-static.com/images/news2
/Chipworks-Apple-s-A6X-Chip-Is-a-Beast-2.jpg)

  

프로세서

S5L8955

[CPU](CPU.md)

[Apple Swift](Apple%20Swift.md) MP2 1.4 GHz

[GPU](GPU.md)

IT PowerVR SGX554 MP4 300 MHz

[메모리](%EB%A9%94%EB%AA%A8%EB%A6%AC.md)

64-bit 듀얼채널 LPDDR2 1066 MHz

생산 공정

삼성 S.LSI 32nm HKMG

주요  
사용 기기

[아이패드/4세대](%EC%95%84%EC%9D%B4%ED%8C%A8%EB%93%9C/4%EC%84%B8%EB%8C%80.md)

  
A5X 처럼 [아이패드](%EC%95%84%EC%9D%B4%ED%8C%A8%EB%93%9C.md) 레티나 모델의 크고 아름다운 그래픽을
처리하기 위해 나온 A6칩의 파생 모델로,
[아이패드/4세대](%EC%95%84%EC%9D%B4%ED%8C%A8%EB%93%9C/4%EC%84%B8%EB%8C%80.md) 공개때
같이 공개되었다. 다들 처음에는 A6이 A5, A5X와 동일한 GPU를 사용하기 때문에 A5X와 같은 GPU 구성에 클럭으로 조정한 것으로
예상했었는데, 나중에 밝혀진 바로는 PowerVR **SGX554 쿼드 코어**를 사용한다고 밝혀지면서 전 세계 관련 커뮤니티와 수많은
전문가들에게 충격을 안겨주었다.

  

[애플](%EC%95%A0%ED%94%8C%28%EA%B8%B0%EC%97%85%29.md) 내부적으로 크고 아름다운 고 해상도를
처리하기에는 기존의 GPU로는 역부족하다는 것을 인지하고 더 나은 성능을 보이기 위해 이 같은 선택을 한 것으로 보인다.

  

때문에 AP 자체가 32nm HKMG 공정 구성임에도 불구하고 x86 기반의 CPU와 다이 사이드가 버금갈 정도로 크며 설계 역시 CPU보다
GPU에 더 중점을 둔 것 처럼 보인다.

  

이 때문에 GPU 성능이 매우 막강해서 경쟁사들은 **1년이 지난** 2013년 3분기의 상급 모델인 [퀄컴 스냅드래곤](%ED%80%84%EC%BB%B4%20%EC%8A%A4%EB%83%85%EB%93%9C%EB%9E%98%EA%B3%A4.md) 800의 Adreno
330, [nVIDIA Tegra](nVIDIA%20Tegra.md) 4의 ULP Geforce,
[엑시노스](%EC%97%91%EC%8B%9C%EB%85%B8%EC%8A%A4.md) 5420의 [ARM](ARM.md) Mali
T-628 헥사 코어로 겨우 A6X를 넘을 수 있었다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/%EC%95%A0%ED%94%8C%20A%20%EC%8B%9C%
EB%A6%AC%EC%A6%88?action=edit&section=9)]

### 3.6. A7 ¶

![http://www.chipworks.com/components/com_wordpress/wp/wp-content/uploads/2013
/09/New-A7-Floorplan.pngwidth=400](http://www.chipworks.com/components/com_wor
dpress/wp/wp-content/uploads/2013/09/New-A7-Floorplan.png)

[[PNG external image]](http://www.chipworks.com/components/com_wordpress/wp
/wp-content/uploads/2013/09/New-A7-Floorplan.png)

  

프로세서

S5L8960

[CPU](CPU.md)

[Apple Cyclone](Apple%20Cyclone.md) MP2 1.3 GHz

[GPU](GPU.md)

IT PowerVR G6430 450 MHz

[메모리](%EB%A9%94%EB%AA%A8%EB%A6%AC.md)

2x32-bit 듀얼채널 LPDDR3 -- MHz

생산 공정

삼성 S.LSI 28nm HKMG

주요  
사용 기기

[아이폰 5s](%EC%95%84%EC%9D%B4%ED%8F%B0%205s.md), [아이패드에어](%EC%95%84%EC%9D%B4%ED%8C%A8%EB%93%9C%20%EC%97%90%EC%96%B4.md), [아이패드 미니2](%EC%95%84%EC%9D%B4%ED%8C%A8%EB%93%9C%20%EB%AF%B8%EB%8B%88%202.md)

  
[아이폰 5s](%EC%95%84%EC%9D%B4%ED%8F%B0%205s.md)의 공개 키노트 행사에서 공개된 AP이며 모바일
AP로는 **세계 최초**로 64 bit를 지원하는 CPU 아키텍쳐를 내장했다.`[15]` 때문에 CPU 아키텍쳐도 기존 Swift를
사용하지 않고 새로 설계한 **Cyclone** 아키텍쳐를 사용한다.`[16]`

  

ARMv8을 적용한 64-bit 아키텍쳐이고 CPU가 차지하는 면적의 비율이 증가해서인지`[17]` **퍼포먼스가 아닌 벤치마킹**에서도
타사의 AP와 맞먹는 상황이다.`[18]` 원래부터 가상머신 위에서 춤추는
[안드로이드](%EC%95%88%EB%93%9C%EB%A1%9C%EC%9D%B4%EB%93%9C%28OS%29.md)
[스마트폰](%EC%8A%A4%EB%A7%88%ED%8A%B8%ED%8F%B0.md)에 비해 적은 코어 수와 낮은 클럭으로도 퍼포먼스는
꿀리지 않았던 아이폰인 만큼 당분간 ARMv8을 사용한 AP를 탑재한 스마트폰이 나오기 전의 A7칩을 장착한 애플 모바일 기기들의 퍼포먼스는
압도적일 것이다.`[19]`

  

GPU의 경우, 오프스크린에서 엄청난 성능을 자랑하나 [퀄컴 스냅드래곤](%ED%80%84%EC%BB%B4%20%EC%8A%A4%EB%83%85%EB%93%9C%EB%9E%98%EA%B3%A4.md) 800의 Adreno 330에 비하면 약간 뒤쳐지는 성능이다. 그러나
아이폰 5s의 해상도와 4인치 화면이라는 사이즈 때문에 별 문제가 되지 않는다고 한다. 온스크린 벤치마킹에서는 쿨링팬을 단 [nVIDIASHIELD Portable](nVIDIA%20SHIELD%20Portable.md) 말고는 대적할 상대가 없는 상황이다.
<del>1년만에 뭔짓을 한거지</del> <del>뭐긴 뭐야 공밀레지</del>

  

여담으로, GPU의 경우 아난드텍의 리뷰에서 이메지네이션 그래픽스 사의 PowerVR G**6**430을 사용한 것이라는 주장이 제기되었으나
[OpenGL ES3.0](OpenGL.md)을 지원한다던 애플의 말과 달리 밴치마크에서 OpelGL ES2.0이라는 충공깽한 결과를
내놔서 의심받았다. 게다가 G6430은 타겟공정이 16nm인데 A7은 28nm이다. 그런데, 칩웍스에서 리버스 엔지니어링으로 직접 뜯어봐
PowerVR G6430 쿼드 클러스터가 들어간 것을 확인했다고 한다. [#](http://www.gsmarena.com
/iphone_5s_specs_revealed_arm_v8_cpu_powervr_series_6_gpu-news-6849.php) 다만
어째서 OpenGL ES2.0인지는 미스터리이며, 쿨럭도 밝혀지지 않은 상태. 시간이 더 지나야 자세한 정보가 확인될 것 같다.

  

다이 내부 사진에 기존에는 존재하지 않던 SRAM 부분이 생겼다. Anandtech의 LMBench를 통한 성능 분석을 통해 4MB의 L3
cache인 것으로 밝혀졌다. 지문인식 정보를 저장하는 부분으로 잘못 알려져 있으나 Area도 넓고 Leakage도 심한 거대한
SRAM덩어리를 지문정보 저장에 쓴다는건 엄청난 낭비다.

  

Apple A4 이후로 나온 AP 중 유일하게 X 버전으로 리뉴얼 되지 않았다.
[아이패드](%EC%95%84%EC%9D%B4%ED%8C%A8%EB%93%9C.md) 시리즈의 5세대 모델인 [아이패드에어](%EC%95%84%EC%9D%B4%ED%8C%A8%EB%93%9C%20%EC%97%90%EC%96%B4.md)에 A7이 그대로
들어간다. 다만 1.4GHz으로 오버클럭된 버전이 들어간다. 또한 [아이패드 미니2](%EC%95%84%EC%9D%B4%ED%8C%A8%EB%93%9C%20%EB%AF%B8%EB%8B%88%202.md)에도
탑재되었는데 이쪽은 아이폰 5s와 똑같이 1.3GHz 버전이 탑재된다.

  

2014년 3월 31일에 아난드텍에서 Swift와 Cyclone의 [비교
설명](http://www.anandtech.com/show/7910/apples-cyclone-microarchitecture-
detailed)을 올리면서 어느정도 A7에 대해 윤곽이 잡혔다. 그전까지 공개된 자료가 별로 없어서 [아이패드에어](%EC%95%84%EC%9D%B4%ED%8C%A8%EB%93%9C%20%EC%97%90%EC%96%B4.md)와 [아이폰5s](%EC%95%84%EC%9D%B4%ED%8F%B0%205s.md) 리뷰 당시 애로사항이 있었다고. 결론만 말하면, 이 A7란
물건이 상당히 "무시무시한" 물건이라는 것. 아이폰 5s가 공개되었을 때만 해도 대부분의 기술 전문가들은 A7가 단순히 Swift의 진보한
프로세서라고 생각했었는데 그 예상이 모조리 틀렸음이 드러난 것이다. 단적인 예로, Cyclone의 리오더(재정렬) 버퍼는 엔트리가 192개로
확 늘었는데, 이는 [인텔](%EC%9D%B8%ED%85%94.md)의
[하스웰](%ED%95%98%EC%8A%A4%EC%9B%B0.md)과 같은 수준이다. 아난트덱은 A7 SoC가 데스크톱급 아키텍쳐라는
애플의 발표가 과장이 아니었음을 인정하였다.

  

다만, 현재로썬 앱 중에서 A7의 괴물급 성능을 제대로 활용하는 앱은 거의 없는 듯 하다고 한다. 이는 앱 개발자들이 구형 기기들에 대한
하위 호환을 생각하기 때문인 것으로 추측된다. 또한 A7칩이 탑재된 [아이폰5s](%EC%95%84%EC%9D%B4%ED%8F%B0%205s.md)와 [아이패드에어](%EC%95%84%EC%9D%B4%ED%8C%A8%EB%93%9C%20%EC%97%90%EC%96%B4.md), [아이패드 미니2](%EC%95%84%EC%9D%B4%ED%8C%A8%EB%93%9C%20%EB%AF%B8%EB%8B%88%202.md)의 경우 램이
1기가이기 때문에 A7의 고성능을 못 따라가는 상황이다. 오랜 세월동안 기기들을 사용하다보면 CPU 성능의 한계를 느끼기도 전에, 메모리의
한계가 먼저 와닿을 것이라고. 이는 바꿔 말하면 세월이 흘러도 A7의 싱글 스레드 처리는 여전히 상당히 우수할 것이라는 말이다. 물론 수년이
지나서도 그 성능을 체험하려면 메모리 관리는 꾸준히 해야 할 것으로 보인다. <del>근데 이미 사파리쓰다가 튕기는걸 보면... 또
ios버전이 올라가면서 점점 무거워진 경향도 있기 때문에...</del>

  

[[edit](http://rigvedawiki.net/r1/wiki.php/%EC%95%A0%ED%94%8C%20A%20%EC%8B%9C%
EB%A6%AC%EC%A6%88?action=edit&section=10)]

### 3.7. A8 ¶

![Apple_A8.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/_ec_95_a0_ed_94_8
c_20A_20_ec_8b_9c_eb_a6_ac_ec_a6_88/Apple_A8.jpg)

[JPG image (251.25 KB)]

  

프로세서

APL1011

[CPU](CPU.md)

[Apple Cyclone](Apple%20Cyclone.md) MP2 1.4 GHz

[GPU](GPU.md)

IT PowerVR GX6450 450 MHz

[메모리](%EB%A9%94%EB%AA%A8%EB%A6%AC.md)

[추가바람](%EC%B6%94%EA%B0%80%EB%B0%94%EB%9E%8C.md)

생산 공정

TSMC 20nm SoC

주요  
사용 기기

[아이폰 6](%EC%95%84%EC%9D%B4%ED%8F%B0%206.md), [아이폰 6Plus](%EC%95%84%EC%9D%B4%ED%8F%B0%206%20Plus.md)

  
[아이폰 6](%EC%95%84%EC%9D%B4%ED%8F%B0%206.md)와 [아이폰 6Plus](%EC%95%84%EC%9D%B4%ED%8F%B0%206%20Plus.md)의 공개 키노트 행사에서 공개된 AP이며 [애플A 시리즈](%EC%95%A0%ED%94%8C%20A%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md) 중에서는 20nm로
생산된 최초의 모바일 AP다.`[20]` 또한, 메인 생산사가 [TSMC](TSMC.md)로 교체되었다.

  

전작이 사용한 [Apple Cyclone](Apple%20Cyclone.md) [CPU](CPU.md)의 리비전 버전과
이매지네이션 테크놀러지의 PowerVR GX6450 [GPU](GPU.md)가 탑재되었다. Apple A7의 약 두 배 가량인
**20억 개**의 트랜지스터가 박혀있으며 다이사이즈는 89 mm^2로 Apple A7와 비교해서 확 작아졌다. <del>그런데 배터리
체감은 a7이나 a8이나 비슷하다고 한다.</del>

  

[[edit](http://rigvedawiki.net/r1/wiki.php/%EC%95%A0%ED%94%8C%20A%20%EC%8B%9C%
EB%A6%AC%EC%A6%88?action=edit&section=11)]

### 3.8. A8X ¶

![http://cdn.macrumors.com/article-
new/2014/11/a8x_die_photo.jpgwidth=400](http://cdn.macrumors.com/article-
new/2014/11/a8x_die_photo.jpg)

[[JPG external image]](http://cdn.macrumors.com/article-
new/2014/11/a8x_die_photo.jpg)

  

프로세서

APL1012

[CPU](CPU.md)

[Apple Cyclone](Apple%20Cyclone.md) MP3 1.5 GHz

[GPU](GPU.md)

IT PowerVR **GXA6850**`[21]` 550 MHz

[메모리](%EB%A9%94%EB%AA%A8%EB%A6%AC.md)

2x64-bit 듀얼채널 LPDDR3 -- MHz

생산 공정

TSMC 20nm SoC

주요  
사용 기기

[아이패드 에어2](%EC%95%84%EC%9D%B4%ED%8C%A8%EB%93%9C%20%EC%97%90%EC%96%B4%202.md)

  
[아이패드 에어2](%EC%95%84%EC%9D%B4%ED%8C%A8%EB%93%9C%20%EC%97%90%EC%96%B4%202.md)에 들어간
CPU로, A8의 개량버전이다. 예전에 그래픽 코어 수만 늘렸던 X시리즈 칩과 달리 이번에는 CPU도 1.5GHz의 트리플 코어로
업그레이드했다. 벤치마크 결과에 따르면 A8보다 싱글 코어에서는 13%, 멀티코어는 55% 빠르다고 한다. L2 Cache가 2MB로
증가했으며, 일부 연산 명령어의 소요 시간을 줄였다. 메모리의 경우 2GB로 늘었으며 A5X처럼 메모리 컨트롤러를 추가하여 128bit
width를 갖는다. 30억 개의 트랜지스터가 박혀 있다. GPU는 PowerVR GXA6850이며 A8의 GPU인 GX6450에 비해 2배
많은 코어가 들어있다..... <del>이놈덕에 에어2 배터리타임은 에어1 보다 줄었다고 한다</del>

`\----`

  * `[1]` [삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md)의 자체 AP 브랜드인 [엑시노스](%EC%97%91%EC%8B%9C%EB%85%B8%EC%8A%A4.md)도 비슷한 목적을 가지고 있기 때문에 [엑시노스](%EC%97%91%EC%8B%9C%EB%85%B8%EC%8A%A4.md) 자체 정보와 [스마트폰](%EC%8A%A4%EB%A7%88%ED%8A%B8%ED%8F%B0.md) 관련 정보는 분리해서 다루고 있다.
  * `[2]` 다만 [퀄컴 스냅드래곤](%ED%80%84%EC%BB%B4%20%EC%8A%A4%EB%83%85%EB%93%9C%EB%9E%98%EA%B3%A4.md)이 Krait 아키텍쳐를 사용한 이후로는 이런 경향이 덜해졌다.
  * `[3]` 안드로이드 운영체제가 갖는 자체적인 문제도 있다.
  * `[4]` 사실, AP의 성능을 높이는 최적의 방법은 아키텍쳐 개선이나 공정미세화가 아닌 트랜지스터를 더욱 많이 집어넣는 것이다. 이러면 면적은 넓어지고 전력 소비량역시 늘어나지만, 성능역시 정비례해서 늘어나기 때문이다. 반대의 경우도 동일하다. [애플](%EC%95%A0%ED%94%8C%28%EA%B8%B0%EC%97%85%29.md)은 트랜지스터를 많이 집어 넣으면서 얻어지는 디메리트를 최적화로 해결해서 [CPU](CPU.md)가 차지하는 부분을 줄일 수 있는 것이다.
  * `[5]` 이는 [애플](%EC%95%A0%ED%94%8C%28%EA%B8%B0%EC%97%85%29.md)이 비용 문제로 공정 미세화에 미온적으로 대응하는 것과 착탈식 배터리를 지원할 생각이 없기 때문에 이렇게 한다는 주장도 있다. 공정 미세화가 지지부진하면 다이 사이즈가 줄어들지 않고, 또한 배터리 용량역시 한계가 있으며 착탈도 되지 않으니 [CPU](CPU.md) 사이즈를 줄여야할 필요가 있기 때문이다.
  * `[6]` 역시, [퀄컴 스냅드래곤](%ED%80%84%EC%BB%B4%20%EC%8A%A4%EB%83%85%EB%93%9C%EB%9E%98%EA%B3%A4.md)이 Adreno 320과 330을 사용하면서부터 격차가 줄었다.
  * `[7]` 일반적인 [스마트폰](%EC%8A%A4%EB%A7%88%ED%8A%B8%ED%8F%B0.md) 판매량은 [삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md) 무선 사업부가 더 많다. 다만, 단일 브랜드 및 제품군([삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md)에서는 [갤럭시 S 시리즈](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20S%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md).)으로는 애플이 더 우세하다.
  * `[8]` 다만, [디스플레이](%EB%94%94%EC%8A%A4%ED%94%8C%EB%A0%88%EC%9D%B4.md) 패널의 경우 [삼성 디스플레이](%EC%82%BC%EC%84%B1%20%EB%94%94%EC%8A%A4%ED%94%8C%EB%A0%88%EC%9D%B4.md)가 주 공급사 <del>특히 샤프 디스플레이의</del> 사정으로 모든 물량을 공급받지 못하는 경우 백업을 뛰고 있다. [삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md) 시스템 LSI 사업부 역시 백업을 뛸 가능성이 높다.
  * `[9]` 삼성 내부적으로 S5PC110A01 이라는 코드명도 있을 정도다. 여담으로, [엑시노스](%EC%97%91%EC%8B%9C%EB%85%B8%EC%8A%A4.md) 브랜드가 공개됨에 따라 기존 [삼성전자 허밍버드](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90%20%ED%97%88%EB%B0%8D%EB%B2%84%EB%93%9C.md) S5PC110은 [엑시노스](%EC%97%91%EC%8B%9C%EB%85%B8%EC%8A%A4.md) 3110으로 개편되었다.
  * `[A]` [아이패드 미니](%EC%95%84%EC%9D%B4%ED%8C%A8%EB%93%9C%20%EB%AF%B8%EB%8B%88.md) 출시 이전에는 S5L8940을, [아이패드 미니](%EC%95%84%EC%9D%B4%ED%8C%A8%EB%93%9C%20%EB%AF%B8%EB%8B%88.md) 출시 이후에는 S5L8942를 사용했다.
  * `[11]` 현재 [TSMC](TSMC.md)로 넘어갈 경우의 큰 불안요소 중 하나. [TSMC](TSMC.md)는 말 그대로 생산만 하는 업체라 설계도 상의 문제가 있을 때 대처 능력이 떨어진다는 평을 받고 있다. [삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md)의 경우에는 사소한 문제 정도는 **애플에 통보만 하고 알아서 고쳐버린다**고 한다.
  * `[12]` [AnandTech](http://www.anandtech.com/show/5685/apple-a5x-die-size-measured-16294mm2-likely-still-45nm)에서는 32nm 공정으로 추측하였으나, Chipworks에서 45nm 공정이며 다이사이즈는 162.94 mm^2이라고 밝혔다.
  * `[13]` 그나마 태블릿은 소형기기는 아니고 보통 들거나 세워놓고 사용하기 때문에 실제로 느끼는 체감온도는 적다.
  * `[14]` 물론, Scorpion과 Krait는 ARMv7으로 만들어진다.
  * `[15]` [ARM](ARM.md)의 64 bit 지원 CPU 아키텍쳐인 [ARM](ARM.md) Cortex-A53/57은 2012년 10월에 이미 공개되었다. 하지만 권장공정이 20nm대 초반 이하로 낮은 편이기 때문에 라이센스 취득사들은 2014년을 목표로 로드맵을 잡고 있다. 운영체제가 준비되지 않아 사용하지 않는다는 주장이 있으나, 64-bit 지원은 ARMv8 명령어 셋의 특징 중 하나일 뿐이고 ARMv8이 ARMv7에 단순히 64-bit 지원만 추가시킨 것이 아니기 때문에 성능이 개선된 아키텍쳐가 필요하다면 32-bit라도 사용할 것이다.
  * `[16]` 기존에는 **Oscar**로 알려졌으나, 이는 M7 프로세서의 코드 네임이라고 한다.
  * `[17]` 원래 애플 A 시리즈는 전통적으로 GPU의 크기가 [크고 아름다워](%ED%81%AC%EA%B3%A0%20%EC%95%84%EB%A6%84%EB%8B%B5%EB%8B%A4.md) CPU는 GPU의 손톱만한게 일반적.
  * `[18]` [퀄컴 스냅드래곤](%ED%80%84%EC%BB%B4%20%EC%8A%A4%EB%83%85%EB%93%9C%EB%9E%98%EA%B3%A4.md) 800 MSM8X74에 비해 멀티코어 성능에서 뒤지지만, A7은 **듀얼 코어 1.3 GHz** [CPU](CPU.md)를 사용한다.
  * `[19]` [아이폰 5s](%EC%95%84%EC%9D%B4%ED%8F%B0%205s.md), [아이패드 에어](%EC%95%84%EC%9D%B4%ED%8C%A8%EB%93%9C%20%EC%97%90%EC%96%B4.md), [아이패드 미니 2](%EC%95%84%EC%9D%B4%ED%8C%A8%EB%93%9C%20%EB%AF%B8%EB%8B%88%202.md)
  * `[20]` 모바일 AP 전체로 확대해보면, 동급인 22nm로 [인텔 아톰 시리즈](%EC%9D%B8%ED%85%94%20%EC%95%84%ED%86%B0%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md)의 BayTrail 시리즈가 있고, 20nm로는 [삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md) [엑시노스](%EC%97%91%EC%8B%9C%EB%85%B8%EC%8A%A4.md) 5430과 5433이 있다.
  * `[21]` 해당 [GPU](GPU.md)는 이매지네이션 테크놀러지의 공식 로드맵에서 확인되지 않다. 이 때문에 여러 IT 웹진 등 관련 커뮤니티에서는 임의적으로 A를 붙여서 구별하고 있다.

