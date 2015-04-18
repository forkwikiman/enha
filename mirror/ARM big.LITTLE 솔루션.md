  * 상위 항목 : [ARM(CPU)](ARM%28CPU%29.md)  

![http://www.blogcdn.com/www.engadget.com/media/2012/11/arm-big-little-
layout.jpg](http://www.blogcdn.com/www.engadget.com/media/2012/11/arm-big-
little-layout.jpg)

[[JPG external image]](http://www.blogcdn.com/www.engadget.com/media/2012/11
/arm-big-little-layout.jpg)

## Contents

    

1. 개요 
2. 상세 
    

2.1. 클러스터 마이그레이션

2.2. IKS 모드

2.3. HMP 모드

3. 라이센스 취득사 
    

3.1. ARMv7명령어셋 기반 아키텍쳐 조합

    

3.1.1. [ARM Cortex-A15](ARM%20Cortex-A15.md) \+ [ARMCortex-A7](ARM%20Cortex-A7.md) 조합

3.1.2. [ARM Cortex-A17](ARM%20Cortex-A17.md) \+ [ARMCortex-A7](ARM%20Cortex-A7.md) 조합

3.2. ARMv8 명령어셋 기반 아키텍쳐 조합

    

3.2.1. [ARM Cortex-A57](ARM%20Cortex-A57.md) \+ [ARMCortex-A53](ARM%20Cortex-A53.md) 조합

3.2.2. [ARM Cortex-A72](ARM%20Cortex-A72.md) \+ [ARMCortex-A53](ARM%20Cortex-A53.md) 조합

3.3. 기타

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20big.LITTLE%20%EC%86%94%EB%A3%
A8%EC%85%98?action=edit&section=1)]

## 1. 개요 ¶

[ARM Holdings](ARM%20Holdings.md)에서 개발한 전력 소모 개선 솔루션.

  

[ARM Holdings](ARM%20Holdings.md)에서 개발하는 [CPU](CPU.md) [마이크로아키텍처](%EB%A7%88%EC%9D%B4%ED%81%AC%EB%A1%9C%EC%95%84%ED%82%A4%ED%85%8D%EC%B2%98.md)인
[ARM Cortex-A 시리즈](ARM%20Cortex-A%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md)가 시간이
지나면서 점차 고성능화되자, [ARM Cortex-A시리즈](ARM%20Cortex-A%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md)의 특성이라 부를 수 있는 전력 대
성능비가 점차 떨어지고 있었다. 이러한 단점을 개선하고자 개발되었다.

  

원래는 현 세대 명령어셋인 ARMv7의 후속 명령어셋인 ARMv8로 제작된 [ARM Cortex-A시리즈](ARM%20Cortex-A%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md)를 위해 준비 중에 있었으나, [ARMCortex-A15](ARM%20Cortex-A15.md)가 **미칠듯한 발열**과 **자비없는 전력 소모율**을 보여주자
<del>스마트폰 계의 [프레스 핫](%ED%8E%9C%ED%8B%B0%EC%97%84%204.md)</del> 부랴부랴 [ARMCortex-A15](ARM%20Cortex-A15.md)에 이식되어 상용화되었다.

  

정식 명칭이 'big.LITTLE'이다. **절대로 대소문자 구별을 무시한 것이 아니다**.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20big.LITTLE%20%EC%86%94%EB%A3%
A8%EC%85%98?action=edit&section=2)]

## 2. 상세 ¶

간단히 서술하면, 고성능 코어와 저전력 코어를 조합하여 전력 효율과 성능을 전부 잡겠다는 목적으로 만들어졌다. 전성비가 좋고, 전력 소모량이
적을 경우 필연적으로 성능이 떨어지는 단점을 개선한 부분.

  

![http://www.seeko.co.kr/zboard4/data/freeboard/cdpkorea-1358435682-1.jpg?Widt
h=500](http://www.seeko.co.kr/zboard4/data/freeboard/cdpkorea-1358435682-1.jpg
)

[[JPG external image]](http://www.seeko.co.kr/zboard4/data/freeboard/cdpkorea-
1358435682-1.jpg)

  

크게 3가지 구동 방법으로 구성되어 있다. 명칭이 공개될 때마다 변경되고 있다. **굵은 글씨**는 다양한 명칭 중, 정착된
명칭이다.`[1]`

  

  * **클러스터 마이그레이션** (Cluster Migration) → CPU 코어 마이그레이션 (CPU Core Migration)
  * CPU 마이그레이션 (CPU Migration) → **IKS** (In-Kernel Switcher)
  * big.LITTLE 멀티 프로세싱 (big.LITTLE Multi Processing / Global Task Scheduling / **H**eterogeneous **M**ulti-**P**rocessing)  

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20big.LITTLE%20%EC%86%94%EB%A3%
A8%EC%85%98?action=edit&section=3)]

#### 2.1. 클러스터 마이그레이션 ¶

일의 가중에 따라 리틀코어 부분의 멀티코어 혹은 빅코어 부분의 멀티코어 중 한 쪽의 코어 클러스터만 선택해서 활성화 시킨다. 이는 기존의
가버너와 크게 다르지 않으며, 내부적으로 클럭을 반토막 내거나 두 배로 뻥튀기해서, 두 클러스터 간을 조정한다.

  

3가지 구동 방법 중 가장 기본적이면서 가장 효율과 유연성이 **상대적**으로 떨어지는 기술이지만, 구현이 쉽고 **절대적**으로 비교하면
효율 자체는 나쁘지 않다. 당장 [갤럭시 S4](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20S4.md)
[WCDMA](WCDMA.md) 모델이 [갤럭시 S4](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20S4.md)
[LTE](LTE.md) 모델과 배터리 타임이 비슷하거나 비교 우위를 점하는 상황이 보이는 것이 증거로 들 수 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20big.LITTLE%20%EC%86%94%EB%A3%
A8%EC%85%98?action=edit&section=4)]

#### 2.2. IKS 모드 ¶

![http://www.linaro.org/linaro-blog/wp-
content/uploads/2013/07/Pic1.jpg?Width=500](http://www.linaro.org/linaro-blog
/wp-content/uploads/2013/07/Pic1.jpg)

[[JPG external image]](http://www.linaro.org/linaro-blog/wp-
content/uploads/2013/07/Pic1.jpg)

  

리눅스 커널단에서 가상 코어를 구성한 뒤, 빅코어와 리틀코어 사이를 아키텍쳐의 구분없이 이동한다. 사실, 클러스터 마이그레이션 자체도 IKS
모드의 범주에 포함되지만, IKS 모드의 진정한 목적은 **빅코어와 리틀코어의 혼용**이다. 최대 쿼드코어로 구성하되, 일의 경중에 따라
사용되는 아키텍쳐가 다르게 구성된다.

  

리눅스 커널은 첫 번째부터 네 번째 까지의 가상 코어를 구성하고, 각 가상 코어는 빅코어 싱글코어와 리틀코어 싱글코어로 이루어져있다. 리눅스
스케줄러는 4개의 코어에 일을 전담하되, 들어오는 작업량에 따라 능동적으로 빅코어와 리틀코어 구분없이 사이사이를 오고간다.`[2]` 아마
처음 구상한 big.LITTLE 모델에 가장 가까운 형태라고 추정된다.

  

이미 2013년 5월에 관련 소스가 처음으로 공개되었으며, 정식 지원은 아니지만, 엑시노스 5420기기에 기존 클러스터 마이그레이션을 대체한
커스텀 커널들이 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20big.LITTLE%20%EC%86%94%EB%A3%
A8%EC%85%98?action=edit&section=5)]

#### 2.3. HMP 모드 ¶

![http://www.linaro.org/linaro-blog/wp-
content/uploads/2013/07/Pic2.jpg?width=500](http://www.linaro.org/linaro-blog
/wp-content/uploads/2013/07/Pic2.jpg)

[[JPG external image]](http://www.linaro.org/linaro-blog/wp-
content/uploads/2013/07/Pic2.jpg)

  

간단히 말해서 빅코어로 이루어진 클러스터와 리틀코어로 이루어진 클러스터를 **동시에 사용**한다. IKS 모드와 같이 가상 코어를 사용해
일을 분담하는 것이 아니라, 스케줄러 자체에서 코어 각각을 통솔해 모든 코어 전체를 구동한다. 이 경우에도 전력 효율을 위해 리틀코어부터
작업이 할당되며, 처음 HMP 모드는 서버 같이 전력 소비보다 퍼포먼스가 중시되는 사용 환경에서의 필요성에 따라 만들어 졌기에 크게
부각되지는 않았다.

  

하지만, Linaro Connect 2012에서 [ARM Cortex-A7](ARM%20Cortex-A7.md) 트리플+[ARMCortex-A15](ARM%20Cortex-A15.md) 듀얼 구성의 테스트 칩, 'TC2'를 시연하면서 HMP 모드가 IKS 모드
대비 약 1.4배의 전력을 소모'한다면서, 이는 'HMP 모드에서 [ARM Cortex-A15](ARM%20Cortex-A15.md)가
필요없이 켜지기 때문'이라는 문제를 크게 다루기도 하었고, IKS 모드는 구조상 빅코어와 리틀코어의 코어 수가 같아야 하는 구조상의 문제가
있기에 AP 설계에 제약이 걸리지만, HMP 모드에서는 관련 문제가 없다는 이점이 있다. 이후,
[삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md)에서 기존 AP의 HMP 지원 선언을 한 이후에
유출된 [엑시노스](%EC%97%91%EC%8B%9C%EB%85%B8%EC%8A%A4.md) 5260의 [CPU-Z](http://bb
s2.ruliweb.daum.net/gaia/do/ruliweb/default/news/520/read?articleId=1290031&ob
jCate1=&bbsId=G003&searchKey=subjectNcontent&itemGroupId=31&itemId=&sortKey=de
pth&searchValue=5260&platformId=&pageIndex=1) 구동 스크린샷을 볼 때, 모바일 기기에서도 IKS 모드보다
HMP 모드를 전면으로 내세운 것으로 추측되고 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20big.LITTLE%20%EC%86%94%EB%A3%
A8%EC%85%98?action=edit&section=6)]

## 3. 라이센스 취득사 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20big.LITTLE%20%EC%86%94%EB%A3%
A8%EC%85%98?action=edit&section=7)]

### 3.1. ARMv7명령어셋 기반 아키텍쳐 조합 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20big.LITTLE%20%EC%86%94%EB%A3%
A8%EC%85%98?action=edit&section=8)]

#### 3.1.1. [ARM Cortex-A15](ARM%20Cortex-A15.md) \+ [ARMCortex-A7](ARM%20Cortex-A7.md) 조합 ¶

  * 르네사스  

    * MP6530 : 듀얼+듀얼 조합의 쿼드코어
  * [미디어텍](%EB%AF%B8%EB%94%94%EC%96%B4%ED%85%8D.md)  

    * MT8135 : 듀얼+듀얼 조합의 쿼드코어
  * [삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md)  

    * [엑시노스](%EC%97%91%EC%8B%9C%EB%85%B8%EC%8A%A4.md) 5 Octa (5410 / 5420 / 5422 & 5800 / 5430) : 쿼드+쿼드 조합의 옥타코어
    * [엑시노스](%EC%97%91%EC%8B%9C%EB%85%B8%EC%8A%A4.md) 5 Hexa (5260) : 듀얼+쿼드 조합의 헥사코어
  * [하이실리콘](%ED%95%98%EC%9D%B4%EC%8B%A4%EB%A6%AC%EC%BD%98.md)`[3]`  

    * Kirin 920 / 925 : 쿼드+쿼드 조합의 옥타코어 
  * [Allwinner](Allwinner.md)  

    * A80 : 쿼드+쿼드 조합의 옥타코어
  * [LG전자](LG%EC%A0%84%EC%9E%90.md)  

    * [Nuclun](LG%20Nuclun.md) 7111 : 쿼드+쿼드 조합의 옥타코어  

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20big.LITTLE%20%EC%86%94%EB%A3%
A8%EC%85%98?action=edit&section=9)]

#### 3.1.2. [ARM Cortex-A17](ARM%20Cortex-A17.md) \+ [ARMCortex-A7](ARM%20Cortex-A7.md) 조합 ¶

  * [미디어텍](%EB%AF%B8%EB%94%94%EC%96%B4%ED%85%8D.md)  

    * MT6595 : 쿼드+쿼드 조합의 옥타코어  

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20big.LITTLE%20%EC%86%94%EB%A3%
A8%EC%85%98?action=edit&section=10)]

### 3.2. ARMv8 명령어셋 기반 아키텍쳐 조합 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20big.LITTLE%20%EC%86%94%EB%A3%
A8%EC%85%98?action=edit&section=11)]

#### 3.2.1. [ARM Cortex-A57](ARM%20Cortex-A57.md) \+ [ARMCortex-A53](ARM%20Cortex-A53.md) 조합 ¶

  * [삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md)  

    * [엑시노스](%EC%97%91%EC%8B%9C%EB%85%B8%EC%8A%A4.md) 7 Octa (5433 / 7420) : 쿼드+쿼드 조합의 옥타코어
  * [엔비디아](%EC%97%94%EB%B9%84%EB%94%94%EC%95%84.md)  

    * [Tegra](nVIDIA%20Tegra.md) X1 : 쿼드+쿼드 조합의 옥타코어
  * 퀄컴  

    * [스냅드래곤](%ED%80%84%EC%BB%B4%20%EC%8A%A4%EB%83%85%EB%93%9C%EB%9E%98%EA%B3%A4.md) 808 MSM8992 : 듀얼+쿼드 조합의 헥사코어
    * [스냅드래곤](%ED%80%84%EC%BB%B4%20%EC%8A%A4%EB%83%85%EB%93%9C%EB%9E%98%EA%B3%A4.md) 810 MSM8994 : 쿼드+쿼드 조합의 옥타코어  

이외에도 카더라 통신으로는 [애플](%EC%95%A0%ED%94%8C%28%EA%B8%B0%EC%97%85%29.md)도 라이센스를
취득했다는 루머가 존재한다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20big.LITTLE%20%EC%86%94%EB%A3%
A8%EC%85%98?action=edit&section=12)]

#### 3.2.2. [ARM Cortex-A72](ARM%20Cortex-A72.md) \+ [ARMCortex-A53](ARM%20Cortex-A53.md) 조합 ¶

  * [미디어텍](%EB%AF%B8%EB%94%94%EC%96%B4%ED%85%8D.md)  

    * MT8173 : 듀얼+듀얼 조합의 쿼드코어
  * 퀄컴  

    * [스냅드래곤](%ED%80%84%EC%BB%B4%20%EC%8A%A4%EB%83%85%EB%93%9C%EB%9E%98%EA%B3%A4.md) 618 : 듀얼+쿼드 조합의 헥사코어
    * [스냅드래곤](%ED%80%84%EC%BB%B4%20%EC%8A%A4%EB%83%85%EB%93%9C%EB%9E%98%EA%B3%A4.md) 620 : 쿼드+쿼드 조합의 옥타코어
  * [하이실리콘](%ED%95%98%EC%9D%B4%EC%8B%A4%EB%A6%AC%EC%BD%98.md)  

    * kirin 940 / 950 : 쿼드+쿼드 조합의 옥타코어

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20big.LITTLE%20%EC%86%94%EB%A3%
A8%EC%85%98?action=edit&section=13)]

### 3.3. 기타 ¶

  * 퀄컴  

    * [스냅드래곤](%ED%80%84%EC%BB%B4%20%EC%8A%A4%EB%83%85%EB%93%9C%EB%9E%98%EA%B3%A4.md) 615 MSM8939 : [ARM Cortex-A53](ARM%20Cortex-A53.md) 옥타코어를 쿼드+쿼드로 나누어 한 쪽은 고클럭으로, 다른 한 쪽은 저클럭으로 세팅하여 big.LITTLE 솔루션을 모방.
  * [하이실리콘](%ED%95%98%EC%9D%B4%EC%8B%A4%EB%A6%AC%EC%BD%98.md)  

    * kirin 930 : [ARM Cortex-A53](ARM%20Cortex-A53.md) 옥타코어를 쿼드+쿼드로 나누어 한 쪽은 고클럭으로, 다른 한 쪽은 저클럭으로 세팅하여 big.LITTLE 솔루션을 모방.

`\----`

  * `[1]` 위 사진은 2012년 12월에 [삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md)의 [프레젠테이션](%ED%94%84%EB%A0%88%EC%A0%A0%ED%85%8C%EC%9D%B4%EC%85%98.md)에서 사용된 명칭이다.
  * `[2]` 예를 들어 작업의 부담이 덜 할 경우 리틀코어를 4개로 구동하고, 리소스가 조금 더 필요할 경우엔 리틀코어 2개의 작업을 빅코어로 옮겨 리틀코어 1개+빅코어 3개 또는 리틀코어 2개+빅코어 2개로 구성을 자유자재로 변경한다.
  * `[3]` [화웨이](%ED%99%94%EC%9B%A8%EC%9D%B4.md)의 자회사이다.

