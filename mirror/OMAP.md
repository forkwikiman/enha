![http://info.arteris.com/Portals/48858/images/ti-omap-4-system-diagram-
omap44x-resized-600.gif](http://info.arteris.com/Portals/48858/images/ti-
omap-4-system-diagram-omap44x-resized-600.gif)

[[GIF external image]](http://info.arteris.com/Portals/48858/images/ti-omap-4
-system-diagram-omap44x-resized-600.gif)

## Contents

    

1. 개요 
2. 상세 
3. 주요 모델 
    

3.1. OMAP 3

3.2. OMAP 4

3.3. OMAP 5

4. 개발 포기? 
5. 그 외 

[[edit](http://rigvedawiki.net/r1/wiki.php/OMAP?action=edit&section=1)]

## 1. 개요 ¶

[텍사스 인스트루먼트](%ED%85%8D%EC%82%AC%EC%8A%A4%20%EC%9D%B8%EC%8A%A4%ED%8A%B8%EB%A3%A8%EB%A8%BC%ED%8A%B8.md)에서 [캠코더](%EC%BA%A0%EC%BD%94%EB%8D%94.md),
[PMP](PMP.md), [PDA](PDA.md), 및
[스마트폰](%EC%8A%A4%EB%A7%88%ED%8A%B8%ED%8F%B0.md)등
[멀티미디어](%EB%A9%80%ED%8B%B0%EB%AF%B8%EB%94%94%EC%96%B4.md)시장을 겨냥해 내놓은
[SoC](SoC.md).

  

OMAP라는 이름은 Open Multimedia Application Platform의 줄임말이다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/OMAP?action=edit&section=2)]

## 2. 상세 ¶

TI사에서 이전에 밀었던 멀티미디어용 SoC인 DaVinci 칩셋을 계승하는 개념으로 출발하였다.
[ARM](ARM%28CPU%29.md) 아키텍쳐가 적용된 CPU와, 모바일 GPU로 이름이 높은 PowerVR의 GPU코어가 융합된
구조를 가지고 있으며, 다빈치칩에서 약점으로 손꼽혔던 <del>저질</del>CPU의 성능을 보완하여, OMAP3 기준 동세대의 ARM기반
SoC중 가장 높은 클럭 효율을 가지고 있었지만`[1]`... 삼성의 [엑시노스3 싱글](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90%20%ED%97%88%EB%B0%8D%EB%B2%84%EB%93%9C.md)에 자리를 내주게 되었다.

  

다른 SoC와 차별되는 점으로서, 하드웨어 동영상 코덱 탑재로 유명한 DaVinci로부터 이어져 내려오는
[DSP](Digital%20Signal%20Processor.md)가 탑재되어 많은 수의 동영상 코덱을 별도의 인코딩을 거치지
않고서도 하드웨어적으로 인코딩 및 디코딩할 수 있다. 이러한 고성능 GPU와, DSP의 탑재 때문에 멀티미디어 성능이 뛰어난 것으로 평가받고
있다. 그래서 멀티미디어 인코딩 및 디코딩 기능을 내세우는 [캠코더](%EC%BA%A0%EC%BD%94%EB%8D%94.md)나
비디오카메라 기능이 뛰어난 디지털카메라 및 스마트폰에 많이 채택되며, 일부 오픈 플랫폼 방식
[게임기](%EA%B2%8C%EC%9E%84%EA%B8%B0.md)에도 탑재되고 있다.

  

OMAP4 기준 ARM Cortex-A9 듀얼코어 CPU와 클럭을 높인 PowerVR SGX540 GPU, 듀얼채널 메모리 컨트롤러를
탑재하여 [nVIDIA Tegra](nVIDIA%20Tegra.md) 2 및 2세대 [퀄컴 스냅드래곤](%ED%80%84%EC%BB%B4%20%EC%8A%A4%EB%83%85%EB%93%9C%EB%9E%98%EA%B3%A4.md) SoC를 능가하는 성능을 과시했다.

  

[스마트폰](%EC%8A%A4%EB%A7%88%ED%8A%B8%ED%8F%B0.md) 중에서는
[모토로라](%EB%AA%A8%ED%86%A0%EB%A1%9C%EB%9D%BC.md)의
[모토로이](%EB%AA%A8%ED%86%A0%EB%A1%9C%EC%9D%B4.md),
[모토쿼티](%EB%AA%A8%ED%86%A0%EC%BF%BC%ED%8B%B0.md),
[모토글램](%EB%AA%A8%ED%86%A0%EA%B8%80%EB%9E%A8.md),
[디파이](%EB%94%94%ED%8C%8C%EC%9D%B4.md), [노키아N8](%EB%85%B8%ED%82%A4%EC%95%84%20N8.md), 그리고 [옵티머스마하](%EC%98%B5%ED%8B%B0%EB%A8%B8%EC%8A%A4%20%EB%A7%88%ED%95%98.md) 등에 사용된 바
있고 [비글 보드](http://beagleboard.org/)나 [오픈판도라](http://www.openpandora.org/)에도
사용되었다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/OMAP?action=edit&section=3)]

## 3. 주요 모델 ¶

  

OMAP 3  

[프로](SoC.md)  
[세서](SoC.md)

[CPU](CPU.md) 아키텍쳐

클럭

[GPU](GPU.md) 아키텍쳐

클럭

3430

[ARM](ARM.md) Cortex-A8 MP1

600 MHz

PowerVR SGX530 MP-

\-- MHz

[모토로이](%EB%AA%A8%ED%86%A0%EB%A1%9C%EC%9D%B4.md),
[모토쿼티](%EB%AA%A8%ED%86%A0%EC%BF%BC%ED%8B%B0.md)

3440

[ARM](ARM.md) Cortex-A8 MP1

720 MHz ~ 800 MHz

PowerVR SGX530 MP1

\-- MHz

[모토글램](%EB%AA%A8%ED%86%A0%EA%B8%80%EB%9E%A8.md), [갤럭시A](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20A.md)

3530

[ARM](ARM.md) Cortex-A8 MP1

720 MHz

PowerVR SGX530 MP1

\-- MHz

[노키아 N8](%EB%85%B8%ED%82%A4%EC%95%84%20N8.md)

3630

[ARM](ARM.md) Cortex-A8 MP1

600 MHz ~ 1.2 GHz

PowerVR SGX530 MP1

\-- MHz

[디파이](%EB%94%94%ED%8C%8C%EC%9D%B4.md), [노키아N9](%EB%85%B8%ED%82%A4%EC%95%84%20N9.md), [옵티머스마하](%EC%98%B5%ED%8B%B0%EB%A8%B8%EC%8A%A4%20%EB%A7%88%ED%95%98.md), [옵티머스빅](%EC%98%B5%ED%8B%B0%EB%A8%B8%EC%8A%A4%20%EB%B9%85.md), [옵티머스블랙](%EC%98%B5%ED%8B%B0%EB%A8%B8%EC%8A%A4%20%EB%B8%94%EB%9E%99.md), [갤럭시S](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20S.md) scLCD  
[갤럭시 플레이어 3.6](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20%ED%94%8C%EB%A0%88%EC%9D%B4%EC%96%B4%203.6.md), [갤럭시 플레이어 4.2](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20%ED%94%8C%EB%A0%88%EC%9D%B4%EC%96%B4%204.2.md), [모토 360](%EB%AA%A8%ED%86%A0%20360.md)

  

OMAP 4  

[프로](SoC.md)  
[세서](SoC.md)

[CPU](CPU.md) 아키텍쳐

클럭

[GPU](GPU.md) 아키텍쳐

클럭

4430

[ARM](ARM.md) Cortex-A9 MP2

1 GHz ~ 1.2 GHz

PowerVR SGX540 MP1

304 MHz

[RAZR](RAZR/%EC%8A%A4%EB%A7%88%ED%8A%B8%ED%8F%B0#s-2.1.md), [RAZRMAXX](RAZR/%EC%8A%A4%EB%A7%88%ED%8A%B8%ED%8F%B0#s-2.2.md), [RAZRV](RAZR/%EC%8A%A4%EB%A7%88%ED%8A%B8%ED%8F%B0#s-2.3.md), [아트릭스 2](%EB%AA%A8%ED%86%A0%EB%A1%9C%EB%9D%BC%20%EC%95%84%ED%8A%B8%EB%A6%AD%EC%8A%A4#s-2.2.md)  
[옵티머스 3D](%EC%98%B5%ED%8B%B0%EB%A8%B8%EC%8A%A4%203D.md), [옵티머스 3D큐브](%EC%98%B5%ED%8B%B0%EB%A8%B8%EC%8A%A4%203D%20%ED%81%90%EB%B8%8C.md),
[프라다폰 3.0](%ED%94%84%EB%9D%BC%EB%8B%A4%ED%8F%B0%203.0.md), [갤럭시 SII](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20S%20II.md)`[2]`  
[갤럭시 플레이어 70 플러스](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20%ED%94%8C%EB%A0%88%EC%9D%B4%EC%96%B4%2070%20%ED%94%8C%EB%9F%AC%EC%8A%A4.md), [갤럭시 플레이어 5.8](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20%ED%94%8C%EB%A0%88%EC%9D%B4%EC%96%B4%205.8.md)  
[킨들 파이어](%ED%82%A8%EB%93%A4%20%ED%8C%8C%EC%9D%B4%EC%96%B4.md) 1세대 / 1.5 세대,
[갤럭시 탭 2](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20%ED%83%AD%202.md) 7.0 / 10.1, [블랙베리플레이북](%EB%B8%94%EB%9E%99%EB%B2%A0%EB%A6%AC%20%ED%94%8C%EB%A0%88%EC%9D%B4%EB%B6%81.md)

4460

[ARM](ARM.md) Cortex-A9 MP2

1.2 GHz ~ 1.5 GHz

PowerVR SGX540 MP1

384 MHz

[갤럭시넥서스](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20%EB%84%A5%EC%84%9C%EC%8A%A4.md)`[3]`,
[킨들 파이어 HD](%ED%82%A8%EB%93%A4%20%ED%8C%8C%EC%9D%B4%EC%96%B4%20HD.md)

4470

[ARM](ARM.md) Cortex-A9 MP2  
[ARM](ARM.md) Cortex-M3 MP2

1.3 GHz ~ 1.8 GHz(A9)  
266 MHz(M3)

PowerVR SGX544 MP1, Vivante CGPU

384 MHz

[갤럭시 프리미어](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20%ED%94%84%EB%A6%AC%EB%AF%B8%EC%96%B4.md), [킨들 파이어 HD8.9](%ED%82%A8%EB%93%A4%20%ED%8C%8C%EC%9D%B4%EC%96%B4%20HD%208.9.md)

  
자세한 정보는 아래 참조.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/OMAP?action=edit&section=4)]

### 3.1. OMAP 3 ¶

65nm와 45nm 공정으로 제작. ARM Cortex-A8 기반이다. GPU는 PowerVR SGX530을 탑재하였다.

  

  * OMAP 3430 - 65nm 공정 및 600MHz의 클럭. [모토로라](%EB%AA%A8%ED%86%A0%EB%A1%9C%EB%9D%BC.md)의 [모토로이](%EB%AA%A8%ED%86%A0%EB%A1%9C%EC%9D%B4.md), [모토쿼티](%EB%AA%A8%ED%86%A0%EC%BF%BC%ED%8B%B0.md)에 사용되었다.  

  * OMAP 3440 - 65nm 공정 및 800MHz의 클럭. [모토글램](%EB%AA%A8%ED%86%A0%EA%B8%80%EB%9E%A8.md), [갤럭시 A](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20A.md) `[4]`에 사용되었다.  

  * OMAP 3530 - 65nm 공정 및 720MHz의 클럭. [노키아 N8](%EB%85%B8%ED%82%A4%EC%95%84%20N8.md)에 사용.  

  * OMAP 3630 - 45nm 공정이며 600MHz에서 1.2GHz 까지의 클럭을 갖는다. 800MHz 클럭의 경우 [디파이](%EB%94%94%ED%8C%8C%EC%9D%B4.md)`[5]`, 1GHz 클럭의 경우 [노키아 N9](%EB%85%B8%ED%82%A4%EC%95%84%20N9.md), [옵티머스 마하](%EC%98%B5%ED%8B%B0%EB%A8%B8%EC%8A%A4%20%EB%A7%88%ED%95%98.md), [옵티머스 빅](%EC%98%B5%ED%8B%B0%EB%A8%B8%EC%8A%A4%20%EB%B9%85.md), [옵티머스 블랙](%EC%98%B5%ED%8B%B0%EB%A8%B8%EC%8A%A4%20%EB%B8%94%EB%9E%99.md), [모토 360](%EB%AA%A8%ED%86%A0%20360.md)에 사용되었다.  
  

여담으로 Omap 34xx버전의 cpu코어는 어떠한 수정도 가해지지않은 순수한 Cortex A8기반의 코어이다. Ti가 ARM과 매우 밀접한
관계가 있었던 이 시기에, Cortex A8은 처음으로 출시하는 ARM v7기반의 코어였기에 준 레퍼런스 SoC를 만들기 위해서 ARM의
Cortex A8 설계를 그대로 사용했다. `[6]`  
삼성이 [엑시노스3 싱글](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90%20%ED%97%88%EB%B0%8D%EB%B2%84%EB%93%9C.md)을 설계할 당시에 ARM은 OMAP 34xx 보다 효율을 올리기 어렵다고 개발을 만류하였으나 이미 Ti도
34xx 시리즈의 설계를 개선한 36xx시리즈를 기획했다는 일화가 있다.

  
  

[[edit](http://rigvedawiki.net/r1/wiki.php/OMAP?action=edit&section=5)]

### 3.2. OMAP 4 ¶

듀얼 코어 CPU. 45nm 공정으로 제작되며 ARM Cortex-A9 기반이다. 듀얼 채널 LPDDR2 메모리 컨트롤러가 탑재되었다.

  

  * OMAP 4430 - 1GHz에서 1.2GHz의 클럭을 갖는다. GPU는 PowerVR SGX540이며 304MHz의 클럭으로 동작한다. 1GHz 클럭은 [옵티머스 3D](%EC%98%B5%ED%8B%B0%EB%A8%B8%EC%8A%A4%203D.md), [프라다폰 3.0](%ED%94%84%EB%9D%BC%EB%8B%A4%ED%8F%B0%203.0.md)에 사용되었다. 1.2GHz 클럭의 모델은 모토로라 [RAZR](RAZR.md)에 사용되었다.  

  * OMAP 4460 - 1.2GHz와 1.5GHz의 클럭. [구글](%EA%B5%AC%EA%B8%80.md)의 레퍼런스 폰인 [갤럭시 넥서스](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20%EB%84%A5%EC%84%9C%EC%8A%A4.md)에 탑재되었다. GPU는 OMAP 4430의 것과 같으나 동작하는 클럭은 384MHz...여야 하지만 배터리 문제 때문인지 갤럭시 넥서스에는 307MHz로 탑재되었다.<del>어째서</del> 순정 커널 대신 다른 커널들은 384MHz로 클럭을 높인 커널과 512MHz로 클럭을 높인 커널이 있다. 전자가 전력 대비 효율이 높다고 하니 원래 SGX540의 성능을 뽑고싶은 사람은 384MHz로 가자.  

  * OMAP 4470 - 1.5GHz<del>와 1.8GHz</del>`[7]` 의 클럭. 전원 관리 능력 향상을 위해 266MHz로 동작하는 ARM Cortex-M3을 기반으로 하는 코어가 추가로 들어가며, 전용 2D 가속기가 탑재된다고 한다. GPU는 PowerVR SGX544이며 클럭은 384MHz. [아마존](%EC%95%84%EB%A7%88%EC%A1%B4.md)의 [킨들 파이어 HD 8.9](%ED%82%A8%EB%93%A4%20%ED%8C%8C%EC%9D%B4%EC%96%B4%20HD%208.9.md)와 [시너직 Uno](%EC%8B%9C%EB%84%88%EC%A7%81%20Uno.md)에 탑재되었다.  

[[edit](http://rigvedawiki.net/r1/wiki.php/OMAP?action=edit&section=6)]

### 3.3. OMAP 5 ¶

TSMC의 28nm SiON 공정으로 제작되며 ARM Cortex-A15 듀얼코어 CPU 탑재 및 전원 관리 능력 향상을 위해 별도의 ARM
Cortex-M4 듀얼코어 프로세서가 탑재된다. M4의 클럭은 불명. 저전력 모드시 전력소모가 큰 A15에서 M4 프로세서로 전환하여
전력소모를 최대한 억제한다. GPU는 PowerVR SGX 544MP2로 확정. 또한 Ti의 2D전용 그래픽 칩셋이 들어간다고 한다.
2012년 3분기 상용화 예정이었는데... 아래의 이유로 2013년 2분기 상용화 예정. 현재 이 AP보다 훨씬 좋은 AP들이 나온 상태에서
경쟁력이 있을지는 불명이다.

  

  * OMAP 5430 - 1.5GHz와 1.7GHz 두 개의 클럭 모델이 있다. GPU로는 SGX544MP2를 탑재한다. 5432와는 다르게 LPDDR2 메모리 컨트롤러를 탑재한다. 그 외엔 5432와 동일.  

  * OMAP 5432 - 5430과 스펙은 거의 똑같지만 듀얼 채널 DDR3 메모리 컨트롤러를 탑재했다.  

[[edit](http://rigvedawiki.net/r1/wiki.php/OMAP?action=edit&section=7)]

## 4. 개발 포기? ¶

개발 포기를 선언했다. 이유는 OMAP을 사용하는 제품이 적어 경쟁에서 밀린다고 판단되기 때문이라고. 그러나 완전히 포기하는 것은 아니라고.
그리고 OMAP 5도 만들고 있다고 한다. [http://bbs2.ruliweb.daum.net/gaia/do/ruliweb/detail/r
ead?articleId=895187&bbsId=G003](http://bbs2.ruliweb.daum.net/gaia/do/ruliweb/
detail/read?articleId=895187&bbsId=G003) <del>그런데 얼버무리는 것 같단 건 뭐지?</del>

  

그리고 결국 [워싱턴 포스트지 11월 15일자 기사에서](http://www.washingtonpost.com/business/texas-
instruments-eliminating-1700-jobs-in-drive-to-trim-
costs/2012/11/15/3dacaa64-2ee5-11e2-b631-2aad9d9c73ac_story.htm)  
TI가 1700명을 해고하고 모바일 전자기기 부분에서 철수하고 차량, 산업용 프로세서 분야에 집중한다고 발표하였다

  

그래서 OMAP 프로세서를 사용한 제품은 안드로이드 4.2 커널(3.4.0)을 지원하지 않아 4.1 커널(3.0.31)`[8]`을 쓰는
형편이다. 자세한 내용은 [갤럭시넥서스](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20%EB%84%A5%EC%84%9C%EC%8A%A4.md) 참조.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/OMAP?action=edit&section=8)]

## 5. 그 외 ¶

아마존이 OMAP 사업부를 매의 눈으로 노리고 있다는 소문이 있다.

`\----`

  * `[1]` 어느 정도냐면, OMAP3630늘 탑재한 모토로라 디파이는 4Ghz까지 오버클럭하는 데 성공했다. 물론 성능은 똥망.
  * `[2]` GT-I9100G 버전. 항목 참조
  * `[3]` 모종의 이유로 GPU 클럭이 307 MHz로 하향되어 있다.
  * `[4]` 모토글램과 갤럭시 A의 경우 720MHz로 다운클럭되어 출시되었다.
  * `[5]` 이는 모토로라에서 전력 소비 절약을 위해 의도적으로 다운클럭한 것이다. 그리고 PowerPC 만들던 노하우를 살렸는지 전력 절약한답시고 제조 공정을 약간 뜯어고쳤단다...
  * `[6]` 같은 Cortex A~ 시리즈라도 AP형태로 만드는 과정에서 코어부분을 필요에 따라 커스텀 한다. 이는 각 회사의 재량이지만 현재는 거의 모든 회사가 커스텀을 거치고 순수 ARM코어는 거의 없다고 보면 된다.
  * `[7]` 제조사의 AP 성능발표할 때에는 작동클럭을 1.8GHz까지로 소개했지만 실제로 **기본클럭이 1.8GHz인 기기**가 없다!
  * `[8]` 커널 버전이 높을수록 IO등에 최적화가 더 된다거나 최신 코드들이 적용되기 때문에 성능면에서는 이득이다. 고로 갤넥 [지못미](%EC%A7%80%EB%AA%BB%EB%AF%B8.md).. [망했어요](%EB%A7%9D%ED%96%88%EC%96%B4%EC%9A%94.md)

