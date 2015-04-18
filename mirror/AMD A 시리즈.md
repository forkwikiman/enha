![http://img842.imageshack.us/img842/8756/1ccs.png?align=right](http://img842.
imageshack.us/img842/8756/1ccs.png)

[[PNG external image]](http://img842.imageshack.us/img842/8756/1ccs.png)

[AMD](AMD.md)의 [APU](APU.md) 라인업 중 하나이다.

## Contents

    

1. 개요 
2. A 시리즈의 역사 
    

2.1. 라노

    

2.1.1. 아키텍처

2.1.2. 성능

2.1.3. 관련 정보

2.1.4. 라노의 APU 모델 번호 및 특징 비교

2.2. 트리니티

    

2.2.1. 아키텍처

2.2.2. 성능

2.2.3. 트리니티의 APU 모델 번호 및 특징 비교

2.3. 리치랜드

    

2.3.1. 아키텍처

2.3.2. 성능

2.3.3. 리치랜드의 APU 모델 번호 및 특징 비교

2.4. 카베리

    

2.4.1. 아키텍처

2.4.2. 성능

2.4.3. CPU클럭 하락 논란

2.4.4. 카베리의 APU 모델 번호 및 특징 비교

2.5. 카리조

[[edit](http://rigvedawiki.net/r1/wiki.php/AMD%20A%20%EC%8B%9C%EB%A6%AC%EC%A6%
88?action=edit&section=1)]

# 1. 개요 ¶

[AMD](AMD.md)에선 [경쟁사](%EC%9D%B8%ED%85%94.md)의 지옥을 달리는 통합 그래픽 감속기와 달리 뛰어난
성능을 가지고 있다고 광고중인 APU 이며, 또 그 목표를 가지고 있는 라인업이기도 하다. <del>근데 여전히 CPU 부분은
느리잖아....</del>

  

[소켓](CPU%20%EC%86%8C%EC%BC%93.md)은 이전까지의 AMx 소켓이 아닌 FMx 형의 소켓을 사용하며, 이 둘은
완전히 다른 구조를 취하고 있어, 서로 호환되지 않는다.

  

기술적으로는, 이기종 연산을 위한 진보를 단계적으로 이루어내려는 목표를 가지고 있기도 하다.

  

시장의 측면에서 보자면, 2011년 말의 첫 출시 후 2012년 10월 트리니티가 데스크탑용으로 출시될 때까지 인텔의 i3계열 까지의
CPU들과 경쟁하고 있지만, 현재와 미래의 경쟁상대는 인텔뿐만이 아니다. 휴대기기 시장에서 강력한 기반을 가지는 ARM이 그 특유의 저전력과
성능으로 강한 모습을 보여주고 있기 때문이다. 현재 인텔과 AMD, ARM 모두 전력당 성능의 효율을 높이기 위해서 노력하고 있으므로,
향후의 경쟁이 기대된다.

  

[소니](%EC%86%8C%EB%8B%88.md)의 차세대 콘솔 [플레이스테이션4](%ED%94%8C%EB%A0%88%EC%9D%B4%EC%8A%A4%ED%85%8C%EC%9D%B4%EC%85%98%204.md)의
핵심 연산장치로 결정되었다. 아무래도 그래픽과 CPU를 합쳤을 때 전력 효율에서 큰 이득을 볼 수 있고, 게임 외에도 다양한 연산이 필요한
PC와 달리 게임이라는 측면 하나에 집중했을 때는 CPU와 GPU의 별개 조합보다 더 높은 효율을 보여줄 수 있다고 판단한 듯하다. [마이크로소프트](%EB%A7%88%EC%9D%B4%ED%81%AC%EB%A1%9C%EC%86%8C%ED%94%84%ED%8A%B8.md)의
차세대 콘솔 [엑스박스 원](%EC%97%91%EC%8A%A4%EB%B0%95%EC%8A%A4%20%EC%9B%90.md)에도
사용된다.

  

모델 명 중 'K'가 붙은 모델은 배수락이 해제되어 있어 오버클럭에 용이하다. 'K'가 붙어있지 않은 모델들은 베이스클럭 오버클럭만 지원하며
베이스클럭에 따라 GPU/메모리 클럭이 같이 상승한다. 'K' 모델은 GPU/메모리 클럭을 개별로 설정할 수 있다.

  

APU의 IGP에서 사용하는 DDR 메모리는 기존 그래픽카드에서 사용하는 GDDR 메모리에 비하여 많이 느린 편이다. 하지만 그만큼 조금의
오버클럭으로도 매우 큰 성능 향상 효과를 볼 수 있다. 대부분의 메모리가 무리없이 2133MHz 정도는 오버클럭이 가능하며, 이 정도로
오버클럭하면 1333 혹은 1600MHz에 비하여 크게는 20% 가까이 그래픽 성능이 향상된다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/AMD%20A%20%EC%8B%9C%EB%A6%AC%EC%A6%
88?action=edit&section=2)]

# 2. A 시리즈의 역사 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/AMD%20A%20%EC%8B%9C%EB%A6%AC%EC%A6%
88?action=edit&section=3)]

## 2.1. 라노 ¶

2011년 말에 출시된 AMD의 첫 APU이다. FM1소켓을 사용한다. Hybrid CrossFireX로 내장그래픽과 특정 모델의 라데온
외장그래픽과 크로스파이어가 가능하다

  

[[edit](http://rigvedawiki.net/r1/wiki.php/AMD%20A%20%EC%8B%9C%EB%A6%AC%EC%A6%
88?action=edit&section=4)]

### 2.1.1. 아키텍처 ¶

라노의 아키텍처는 Stars(Phenom II 모바일)아키텍처를 약간 향상시킨 CPU 부분에 Radeon 6000시리즈의 VLIW5 GPU를
결합한 형태이다. 이 세대의 APU는 단지 CPU와 GPU를 하나의 칩 포장 안에 넣어두는 것이 목표이다. 라노의 CPU는 L3캐시가 없다.
라노의 GPU는 CPU가 사용하는 메인보드의 메모리의 일부를 따로 나눠받아서 사용한다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/AMD%20A%20%EC%8B%9C%EB%A6%AC%EC%A6%
88?action=edit&section=5)]

### 2.1.2. 성능 ¶

페넘에 근거한 아키텍처는, 비록 공정이 32나노미터 급으로 줄어들고, 약간의 향상이 있다고 해도, 경쟁상대인 샌디브릿지와 아이비브릿지를
상대로 CPU 성능에서 밀릴 수 밖에 없었지만, GPU는 여러가지 사정으로 인해 성능이 칼질당했다 하더라도
[라데온](AMD%20GPU%20%EC%9D%BC%EB%9E%8C.md)은 라데온, 그래서 인텔의 HD시리즈 보다는 벤치마크 상에서는
두 배 정도 좋은 GPU 성능을 보여주고 있으며 [드라이버](%EB%93%9C%EB%9D%BC%EC%9D%B4%EB%B2%84.md)
최적화 차이로 인하여 실제 게이밍 성능은 엄청난 차이를 보여주며 UVD3.0이라는 동영상 가속 및 후보정 기능을 지원하기에
[HTPC](HTPC.md)용도로도 우수하나 A6-3500이하의 제품들은 4K급 동영상 재생이 어렵다.

  

이런 이유로, 씨피유의 성능이 중요한 경우에는 인텔에게 밀리지만, GPU의 성능이 보다 중요한 경우에는, 인텔을 뛰어넘는 성능을 보여주고
있다. 단 중급형 이상의 외장형 그래픽 카드를 장착하여 사용한다면 이러한 장점은 없어지고 오히려 CPU 성능 때문에 그래픽 성능이 제대로
나오지도 못할수도 있기에 라노는 그래픽 성능이 어느정도 중요하면서도 중급형 이상의 외장 그래픽 카드를 사용하기가 힘든 환경에서 그 진가를
발휘한다 할 수 있다.  
한편, L3캐시가 없어서 페넘 기반 아키텍처로서의 성능을 발휘하는 데 있어서 약간 불리한 점도 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/AMD%20A%20%EC%8B%9C%EB%A6%AC%EC%A6%
88?action=edit&section=6)]

### 2.1.3. 관련 정보 ¶

앞서 언급한 특성상, APU는 저가형 노트북이나 초저가형 PC에 적절하고 실제로도 그 쪽에서 많이 팔렸다.

  

2012년 10월 17일 AMD에서 기존 라노 시리즈 가격을 인하했다. [#](http://www.techpowerup.com/173801
/AMD-Cuts-Prices-of-Socket-FM1-APUs.html)

  

[[edit](http://rigvedawiki.net/r1/wiki.php/AMD%20A%20%EC%8B%9C%EB%A6%AC%EC%A6%
88?action=edit&section=7)]

### 2.1.4. 라노의 APU 모델 번호 및 특징 비교 ¶

**AMD A시리즈 APU 모델 번호 및 특징 비교**

모델

Radeon™ 브랜드

CPU 동작 속도

CPU 코어 수 (on Die)

TDP

총 L2 캐쉬

Radeon™ 코어 수 (on Die)

GPU 동작 속도

DirectX® 버전

UVD

DDR3 속도

**AMD A시리즈 APU**

A8-3870K*

HD6550D

3.0GHz

4cores

100W

4MB

400

600MHz

11

UVD3

1866

A8-3850

HD6550D

2.9GHz

4cores

100W

4MB

400

600 MHz

11

UVD3

1866

A8-3800

HD6550D

2.7GHz/2.4GHz

4cores

65W

4MB

400

600 MHz

11

UVD3

1866

A6-3670K*

HD6530D

2.7GHz

4cores

100W

4MB

320

444 MHz

11

UVD3

1866

A6-3650

HD6530D

2.6GHz

4cores

100W

4MB

320

444 MHz

11

UVD3

1866

A6-3600

HD6530D

2.4GHz/2.1GHz

4cores

65W

4MB

320

444 MHz

11

UVD3

1866

A6-3500

HD6350D

2.4GHz/2.1GHz

3cores

65W

3MB

320

444 MHz

11

UVD3

1866

A4-3400

HD6410D

2.7GHz

2cores

65W

1MB

160

600 MHz

11

UVD3

1600

A4-3300

HD6410D

2.5GHz

2cores

65W

1MB

160

444 MHz

11

UVD3

1600

[[edit](http://rigvedawiki.net/r1/wiki.php/AMD%20A%20%EC%8B%9C%EB%A6%AC%EC%A6%
88?action=edit&section=8)]

## 2.2. 트리니티 ¶

2012년 5월에 휴대기기용이 출시되고, 2012년 10월에 데스크탑용이 출시되었다. FM2소켓을 사용하며, Dual Graphics(별칭
: Hybrid CrossFireX)로 내장 그래픽과 특정 모델의 라데온 외장 그래픽과 크로스파이어가 가능하다.(A75나 A85X칩셋 기반
메인보드가 필요함). 전작 라노의 FM1 소켓과 호환되지 않는다.`[1]`

  

Hrbrid CrossFireX를 지원하는 모델은 다음과 같다.

  

A10-5800K / A8-5600K: HD 6670 / HD 6570  
A6-5400K: HD 6570 / HD 6470

  

비공식적이긴 하지만 HD7000시리즈의 하이브리드 크로스파이어 또한
지원하는듯하다.[#](http://www.tomshardware.com/forum/id-1688717/review-
amd-a10-5800k-7750-msi-working-dual-
graphics.html)[#](http://www.techpowerup.com/forums/showthread.php?p=2924320)  
A10 5800K에 HD7750 기준으로 10~30% 성능향상이 있는것으로 보인다.

  

A4 모델은 이 기능이 제외되어 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/AMD%20A%20%EC%8B%9C%EB%A6%AC%EC%A6%
88?action=edit&section=9)]

### 2.2.1. 아키텍처 ¶

2세대 불도저 아키텍처인 파일드라이버 아키텍처의 CPU를 사용하며 (기본 구조는 비슷하나, L3캐시가 빠져있음), 라데온 HD 6000
계열에 쓰인 VLIW4 아키텍처의 GPU를 사용한다.  
트리니티의 GPU는 CPU가 사용하는 메인보드의 메모리의 일부를 따로 나눠받아서 사용한다. 메인 메모리를 사용하는 만큼, Llano와 같이
빠른 메모리가 중요하다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/AMD%20A%20%EC%8B%9C%EB%A6%AC%EC%A6%
88?action=edit&section=10)]

### 2.2.2. 성능 ¶

GPU의 성능은 전의 라노 대비 상당히 향상되었다. CPU의 성능은 파일드라이버 아키텍처의 특성을 그대로 따라가서, 기존 라노와 비슷한 면도
있고 라노보다 우월한 면도 있다. 다만 전체적으로 인텔의 씨피유보다 뒤쳐지는 것은 여전하다. 대략 최고급 모델인 A10이 <del>산업폐기물
이었던</del>FX 4100과 비슷(i3 계열과 비슷한 성능)한 성능을 보여준다. 물론, GPU는 인텔의 HD4000계열 GPU 보다 훨씬
낫지만 대략 NVIDIA GEFORCE 9600GT 수준에 머물고 있다.

  

트리니티 자체의 초기가는 제법 빠른 시간에 안정화가 되었으나 메인보드의 가격 안정화가 느리게 진행돼서 비슷한 성능의 외장 GPU를 장착할 수
있다면 인텔의 저렴한 펜티엄, 셀러론에 외장 그래픽카드를 더한 조합과 비교해서 그다지 가격적인 메리트가 있는 상황이 아니었으나 가격 안정화가
이루어진 지금은 이엠텍 등의 최신 A75 칩셋 보드가 6만원대라는 가격으로 엔트리급에선 무지막지한 가성비를 획득, 인텔을 학살 중에 있다.

  

특이하게도 램오버를 통해 그래픽 성능을 20~30%정도 향상시키는 것이 가능하다.`[2]` 마침 시장의 주력인 삼성램이 램오버가 잘 된다는
말이 많아서 램오버가 잘 되면 40만원 안팎으로 상당히 쓸만한 성능의 pc를 마련할 수 있다는 장점이 있다.

  

파일드라이버 기반이라 오버가 잘 되는 편인데, 오버를 할 경우 CPU는 i3-3220과 비슷한 성능을 내고 그래픽은 GeForce GT
640급에 가깝게 끌어 올릴 수 있다. `[3]`

  

2013년 5월 2일
[플레이웨어즈](%ED%94%8C%EB%A0%88%EC%9D%B4%EC%9B%A8%EC%96%B4%EC%A6%88.md)에서
A4-4000의 벤치마킹 결과가 공개되었다.[#](http://www.playwares.com/xe/29901416) CPU 윗면의 코드가
HL로 끝나므로 리치랜드가 아닐까 했지만, AMD 코리아에 문의한 결과 트리니티라고 한다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/AMD%20A%20%EC%8B%9C%EB%A6%AC%EC%A6%
88?action=edit&section=11)]

### 2.2.3. 트리니티의 APU 모델 번호 및 특징 비교 ¶

**AMD A시리즈 APU 모델 번호 및 특징 비교**

모델

Radeon™ 브랜드

CPU 동작 속도

터보 코어 속도

CPU 코어 수 (on Die)

TDP

총 L2 캐쉬

Radeon™ 코어 수 (on Die)

GPU 동작 속도

DirectX® 버전

UVD

DDR3 속도

A10-5800K*

HD7660D

3.8GHz

4.2GHz

4cores

100W

4MB

384

800MHz

11

UVD3

1866

A10-5700

HD7660D

3.4GHz

4.0GHz

4cores

65W

4MB

384

760MHz

11

UVD3

1866

A8-5600K*

HD7560D

3.6GHz

3.9GHz

4cores

100W

4MB

256

760 MHz

11

UVD3

1866

A8-5500

HD7560D

3.2GHz

3.7GHz

4cores

65W

4MB

256

760 MHz

11

UVD3

1866

A6-5400K*

HD7540D

3.6GHz

3.8GHz

2cores

65W

1MB

192

760 MHz

11

UVD3

1866

A4-5300

HD7480D

3.4GHz

3.6GHz

2cores

65W

1MB

128

723 MHz

11

UVD3

1600

A4-4000

HD7480D

3.0GHz

3.2GHz

2cores

65W

1MB

128

723 MHz

11

UVD3

1333

[[edit](http://rigvedawiki.net/r1/wiki.php/AMD%20A%20%EC%8B%9C%EB%A6%AC%EC%A6%
88?action=edit&section=12)]

## 2.3. 리치랜드 ¶

리치랜드 자체는 2012년에는 예정에 없었던 급조 제품이다.

  

28nm공정을 사용하는 '카베리'가 2013년 초에 출시하는 것에서 2014년 1월에 출시하는 것으로 늦어졌기 때문에 그 사이를 잇는
징검다리 역할을 한다. 소켓은 FM2을 그대로 사용한다. 트리니티 라인업은 그대로 유지되며 리치랜드가 투입되면서 트리니티 제품군은 가격을
인하하였다.

  

이때부터 내장 그래픽코어만으로 트리플모니터를 지원한다.

[[edit](http://rigvedawiki.net/r1/wiki.php/AMD%20A%20%EC%8B%9C%EB%A6%AC%EC%A6%
88?action=edit&section=13)]

### 2.3.1. 아키텍처 ¶

아키텍처 자체는 트리니티와 별반 다르지 않다. 글로벌파운드리의 32nm공정은 2013년이 돼서야 겨우 안정화 되었다.

  

이때문에 트리니티 중에서도 보다 저전력에서 고성능을 발휘하는 제품이 선별되었으며, 발열을 개선하여 리치랜드로 제품을 판매하기 시작한다.
일반사용자들은 제품의 가격 대비 성능에서 아직은 선호도가 크지 않으나, 추후 가격이 저점에서 머무를 경우 CPU 트리니티보다 저발열을 이용한
오버클럭으로 트리니티보다 좋은 성능 향상을 할 것으로 기대가 된다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/AMD%20A%20%EC%8B%9C%EB%A6%AC%EC%A6%
88?action=edit&section=14)]

### 2.3.2. 성능 ¶

위에 언급한 바와 같이 아키텍처는 트리니티 그대로다. 하지만, AMD에서 밝힌 자료에 따르면 3D마크11점수가 최대 20~40% 상승되었으며
더 낮은 소비전력에서 작동한다고 한다.  
변경점이 아예 없는 것은 아닌데, 트리니티에서는 DDR3-1866까지 였던 메모리 지원이 리치랜드에서는 공식적으로 DDR3-2133까지
지원된다. 하지만 트리니티에서도 간단한 오버클럭으로 2133Mhz을 달성할 수 있어서 큰 차이점이라고 할 수는 없다.

  

그리고 대망의 벤치결과가 나왔는데, 트리니티에서 GPU와 CPU 둘 다 약 10% 정도의 성능 향상을 보였으며`[4]`, AMD게 싱글쓰레드
연산능력이 많이 떨어지지만 GPU까지 셈한다면 i3과 비교해서는 충분히 경쟁력을 갖추게 됐다. CPU 성능은 여전히 인텔에 비해서 많이
빈약하지만 GPU에서 아주 강한 성능을 냄으로써, 외장형 그래픽을 구입하지 않고, 오직 CPU+내장 GPU만으로 비교를 한다면 매우 강력한
성능을 발휘 한다.  
또한 오버클럭 수율도 매우 좋아서. 4.1Ghz가 동작 클럭인데 5Ghz는 공랭으로도 찍고 풀로드로도 133W정도밖에 안 먹는다고 한다.
[하스웰](%ED%95%98%EC%8A%A4%EC%9B%B0.md)이 물론 새로운 GPU를 달고 나오지만 데스크탑의 최상위 GPU
HD4600 또한 리치랜드의 성능에 훨씬 못 미치며, 가격또한 높아 외장형 그래픽카드를 제외한 단일 APU에서는 리치랜드쪽이 상당히 메리트가
있다.

  

일단 2010년대에 나온 게임들도 비디오 벤치마크 결과 중하옵션 정도면 무난히 30fps이상 찍어주며, 몇몇 게임은 40fps 또한 무난하게
플레이 할수 있다. 참고로 말하자면 비슷한 가격대인 하스웰 i3 4430은 최하옵션으로도 못돌리는 게임이 허다하다. 다만
셀러론+HD77xx대의 조합이 비슷한 예산에서 훨씬 적은 소비전력과 압도적인 게임 성능 우위를 차지하고 있으므로 외장 그래픽카드를 사용하지
않는 컴팩트한 시스템을 구축하기 위한 것이 아니라면 여전히 메리트가 없는 상황.

  

8GHz 오버가 나왔다. 역시 모든 모듈이 동작하고 있는 상태에서의
오버이다.[#](http://news.softpedia.com/news/8-GHz-the-Record-Broken-by-AMD-A10
-6800K-quot-Richland-quot-APU-361339.shtml)

[[edit](http://rigvedawiki.net/r1/wiki.php/AMD%20A%20%EC%8B%9C%EB%A6%AC%EC%A6%
88?action=edit&section=15)]

### 2.3.3. 리치랜드의 APU 모델 번호 및 특징 비교 ¶

**AMD A시리즈 APU 모델 번호 및 특징 비교**

모델

Radeon™ 브랜드

CPU 동작 속도

터보 코어 속도

CPU 코어 수 (on Die)

TDP

총 L2 캐쉬

Radeon™ 코어 수 (on Die)

GPU 동작 속도

DirectX® 버전

UVD

DDR3 속도

A10-6800K*

HD8670D

4.1GHz

4.4GHz

4cores

100W

4MB

384

844MHz

11

UVD3

2133

A10-6790K*`[5]`

HD8670D

4.0GHz

4.3GHz

4cores

100W

4MB

384

844MHz

11

UVD3

2133

A10-6700

HD8670D

3.7GHz

4.3GHz

4cores

65W

4MB

384

844MHz

11

UVD3

1866

A8-6600K*

HD8570D

3.9GHz

4.2GHz

4cores

100W

4MB

256

844 MHz

11

UVD3

1866

A8-6500

HD8570D

3.5GHz

4.1GHz

4cores

65W

4MB

256

800 MHz

11

UVD3

1866

A6-6400K*

HD8470D

3.9GHz

4.1GHz

2cores

65W

1MB

192

800 MHz

11

UVD3

1866

A4-6300

HD8370D

3.7GHz

3.9GHz

2cores

65W

1MB

128

760 MHz

11

UVD3

1866

[[edit](http://rigvedawiki.net/r1/wiki.php/AMD%20A%20%EC%8B%9C%EB%A6%AC%EC%A6%
88?action=edit&section=16)]

## 2.4. 카베리 ¶

2014년 1월 14일 출시된 혁신의 시작이 되는 APU.

  

AMD가 APU에서 추구하는 이기종 시스템 아키텍처(Heterogeneous System Architecture)를 최초로 지원하는
APU로써, 이것은 CPU와 내장 GPU코어의 캐시 메모리 일관성과 동일한 메모리 사용 및 IOMMU v2등의 탑재를 의미하는 것 같다. 이
HSA를 탑재했다고 해서 바로 이득을 보는 것은 아니지만, 이러한 기능을 탑재한 제품이 없으면 관련 소프트웨어의 보급은 기대할 수 없으므로,
카베리가 그 첫걸음이 될 것이다.

  

소켓이 904핀의 FM2소켓에서 906핀의 [FM2+로 바뀌어서](http://www.coolenjoy.net/bbs/boardc.php?i
d=38&no=14585&page=1&num=13983&board=38&ss=0&sc=0&sn=0&keyword=&qa=0&ga=&cat=0
&vote=0) FM2소켓 메인보드에서 사용할 수 없다. 반대로 FM2+ 소켓 메인보드에서는 트리니티와 리치랜드의 사용이 가능하다. 카베리의
아치텍쳐 또한 기존의 파일드라이버 구조를 개선한 스팀롤러를 사용한다. 이로써 CPU의 IPC가 개선되어 멀티쓰레드 환경에서 동클럭에서 하스웰
i3 정도의 성능을 내며, 이는 기존의 리치랜드 CPU의 IPC를 최소 20%정도 개선한 것이다. 하지만 이에 따라서 동작클럭이 하락하면서
상쇄되어 제자리 걸음이 되고말았다.

  

내장 GPU 성능은 대략 GT 630~640 , GTS 250 = 450 정도의 성능이며, APU안에 GPU로써는 매우 경이로운 발전이며
굉장한 수준임에 틀림이 없다. 경쟁사 인텔의 HD시리즈와 비교해서는 압도적이고 최상위 제품인 Iris Pro 5200과 대등한 매우 준수한
편. 스펙상으로는 더 우위에 있을 수 있으나 거기에 걸맞는 대역폭을 제공해줄 수 있는 GDDR을 사용하지는 못하기에 병목현상을 일으켜 발목을
잡히는 상황.

  

그리고 당연하겠지만 가격 또한 매우 중요한 포인트인데, 한국 2014년 1월 14일 출시 가격은 A10-7850K는 213.000원(다나와
최저가는 19만원대), A10-7700K는 191.000원(다나와 최저가는 17만원대) 이다. 하지만 하루만에 18만원대,16만원대으로
하락하였다.  
현 2014년 1월 28일 [다나와](%EB%8B%A4%EB%82%98%EC%99%80.md) 기준으로 A 10 7850 K는
179,000 원에 가격이 책정되어 있으며 , 나름 초기 출시가 19만원에 비하면 다소 안정된 모습을 보인다. 다만 아직까지는 가격적
메리트가 약간 부족한 느낌이 든다.  
2월 달을 전후로 한국에서 최저가가 30만원대로 뛰는 현상이 발생했다. 현재는 다시 가격이 정상화 된 상황.

  

그래도 아직까지 속단하기엔 이른게.. 후에 나올 신기술인 [HSA](HSA.md),
[맨틀](%EB%A7%A8%ED%8B%80.md)과 새로운 버전의 카탈리스트의 지원이 제대로 된다면 , 지금보다 엄청난 성능향상을
기대할 수 있다는 잠재력은 가지고 있다. 하지만 그 기술들이 언제 제대로 나올련지는 아직 미지수다.`[6]` <del>암드는 나와봐야 안다는
옛말이 있다</del>

  

자세한건 아래 카베리 분석글을 참조하자.

  

[http://www.coolenjoy.net/bbs/boardc.php?id=review&no=18531&p=2](http://www.co
olenjoy.net/bbs/boardc.php?id=review&no=18531&p=2)

[[edit](http://rigvedawiki.net/r1/wiki.php/AMD%20A%20%EC%8B%9C%EB%A6%AC%EC%A6%
88?action=edit&section=17)]

### 2.4.1. 아키텍처 ¶

CPU 아키텍처는 스팀롤러, 내장 GPU는 GCN을 사용하며 글로벌 파운드리의 28nm공정으로 제조된다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/AMD%20A%20%EC%8B%9C%EB%A6%AC%EC%A6%
88?action=edit&section=18)]

### 2.4.2. 성능 ¶

CPU의 성능은 대량 생산 전 샘플에서 밝혀진 것에 따르면 [#](http://wccftech.com/amd-kaveri-
steamroller-performance-revealed-integor-point-results-show-viable-
competition-haswell) 전작 트리니티에 사용된 파일드라이버 아키텍쳐에 비해 30~40%의 향상을 이뤄낸 것으로 알려졌다. 6월
19일에 AMD가 개최한 기자 설명회에서 카베리 기반의 옵테론인 '베를린'의 내장 그래픽이 GCN기반이며 쉐이더 수가 512개라는 것을
발표했다. GCN의 성능은 기존 트리니티에 사용된 VILW4 보다 동클럭당 성능이 2~5%정도 높으므로 간단한 계산으로 5800K보다 내장
그래픽의 성능이 50%이상으로 상승할 것으로 기대해도 좋을 것 같다. 거기에 PCIe3.0의 대응도 발표 했으므로 카베리도 드디어
PCIe3.0을 지원하게 될 것이다.

  
  

  

APU2013에서 [배틀필드4](%EB%B0%B0%ED%8B%80%ED%95%84%EB%93%9C4.md)를 AMD 카베리
A10-7850K의 내장 그래픽으로 시연하는 영상이 등장했다. 1080p에 중옵으로 돌렸으며, 오른쪽이 APU, 왼쪽은 인텔
i7-4770K에 GT630 조합이다. 내장그래픽만으로 매우 부드럽게 게임을 돌려내고 있다.

  

[플레이웨어즈](%ED%94%8C%EB%A0%88%EC%9D%B4%EC%9B%A8%EC%96%B4%EC%A6%88.md)의 이대근님의
리뷰가 올라왔다.  
<http://udteam.tistory.com/m/post/611><http://iyd.kr/m/post/614>  
CPU 자체의 성능은 IPC의 향상이 클럭 하락과 상쇄되어 제자리걸음. 하지만 iGPU의 성능 향상이 매우 비약적으로 크고, 이외에도
주목할만한 점은 [HSA](HSA.md)를 키게 되면 i5를 후들겨 갈구는 벤치값을 얻을 수 있다는 점으로 가능성에 주목할 필요가
있다.

[[edit](http://rigvedawiki.net/r1/wiki.php/AMD%20A%20%EC%8B%9C%EB%A6%AC%EC%A6%
88?action=edit&section=19)]

### 2.4.3. CPU클럭 하락 논란 ¶

  
  

![http://www.extremetech.com/wp-content/uploads/2014/03/CPUFrequency-
640x298.jpg](http://www.extremetech.com/wp-content/uploads/2014/03
/CPUFrequency-640x298.jpg)

[[JPG external image]](http://www.extremetech.com/wp-content/uploads/2014/03
/CPUFrequency-640x298.jpg)

  
<A10 7850K의 기본 클럭은 3.7Ghz 이지만 동작 중인 클럭은 3.0Ghz>

  

2014년 7월 들어서 GPU 풀로드시 CPU 클럭이 떨어지는 문제가 국내에 최초로 보고되었다.

  

그런데 이문제는 2014년 3월에 이미 이슈가 된적이 있었고 결론이 나온 문제이다.

  

<http://www.extremetech.com/gaming/177668-turbo-trouble-amds-dual-graphics-is-
bugged-introduces-game-breaking-frame-stutter>

  

카베리 세대 부터는 고급 전력 관리 능력이 추가되어 CPU와 GPU의 작업량을 체크하여 양쪽의 클럭을 내려 다른 한쪽의 발열 여유를 확보할
수 있게 되었다.

  
  

클럭의 하락에 의해서 성능의 감소가 일어날것으로 보이고 이것이 이 현상이 알려졌을때의 국내의 반응이었으나 이 기사에서는 Skyrim,
Orcs Must Die 2, Torchlight 2, Civilization V, and Metro: Last Light 로 벤치마크를
돌려본 결과 터보코어의 활성화 여부는 크게 영향을 주지 않았고 Skyrim에서는 활성화 한 쪽이 근소하게 더 나았다고 한다

  

이는 자연스러운 것으로 대부분의 게임환경에서는 CPU와 GPU 양쪽 모두가 동시에 완전히 빈틈없이 부하가 가해지는 것이 아니라 약간의 여유가
있고 고급 전력관리 기능은 이를 이용해서 한정된 소비전력과 발열을 효율적으로 이용하고자 추가된 것 이므로 실제 사용환경에선 큰 문제가 없다.
하지만 예외는 있다. 듀얼 그래픽스 환경이다.

  

![http://www.extremetech.com/wp-content/uploads/2014/03/OverDrive-Off-vs-On-
640x223.png](http://www.extremetech.com/wp-content/uploads/2014/03/OverDrive-
Off-vs-On-640x223.png)

[[PNG external image]](http://www.extremetech.com/wp-content/uploads/2014/03
/OverDrive-Off-vs-On-640x223.png)

  
<메트로 라스트 라이트 벤치마크>  
<동일한 카베리에서 듀얼그래픽스 사용시 터보코어의 활성화시와 비활성화시의 비교.>

  

여기서는 듀얼 그래픽 사용시에 문제를 발견 하였다고 되어 있는데 그래프를 보면 특정 구간에서 프레임이 심하게 요동치는 문제 즉 마이크로
스터터링이 생긴것을 알수 있다. 이는 전력관리기능이 APU 만이 장착된게 아니라 외부의 GPU 까지 존재하는 듀얼 그래픽스 환경에서는 적절한
대응을 하지 못하면서 발생하는 문제.

  

그리고 이문제는 AMD 오버 드라이브를 사용할경우 간단하게 해결 가능하다.[AMD 오버드라이브 사용법](http://bbs2.ruliweb.
daum.net/gaia/do/ruliweb/default/pc/32/read?articleId=1646887&bbsId=G003&itemI
d=6&pageIndex=1)

  

다만 CPU 클럭하락은 iGPU에 풀로드가 걸릴때 발생한다는걸 잊지말자. AMD가 클럭 하락을 발생하도록 만든 이유가 CPU와 iGPU의
가용 TDP안에서 전력소모를 GPU, CPU에게 적당히 배분하도록 만든것인데 이걸 강제로 해제하여 CPU와 GPU 양쪽 모두 동작 클럭을
최대로 뽑아낸다면 이에 따라서 발열은 책정된 TDP를 초과하는 발열을 내게 됨으로써`[7]` 시스템을 후끈하게 만들어준다.

[[edit](http://rigvedawiki.net/r1/wiki.php/AMD%20A%20%EC%8B%9C%EB%A6%AC%EC%A6%
88?action=edit&section=20)]

### 2.4.4. 카베리의 APU 모델 번호 및 특징 비교 ¶

**AMD A시리즈 APU 모델 번호 및 특징 비교**

모델

Radeon™ 브랜드

CPU 동작 속도

터보 코어 속도

CPU 코어 수 (on Die)

TDP

총 L2 캐쉬

Radeon™ 코어 수 (on Die)

GPU 동작 속도

DirectX® 버전

UVD

DDR3 속도

**AMD A시리즈 APU**

A10-7850K

Radeon R7

3.7GHz

4.0GHz

4cores

95W

4MB

512

720MHz

11

UVD4.2

2133

A10-7700K

Radeon R7

3.5GHz

3.8GHz

4cores

95W

4MB

384

720MHz

11

UVD4.2

2133

A10-7800

Radeon R7

3.5GHz

3.9GHz

4cores

65W

4MB

512

720MHz

11

UVD4.2

2133

A8-7600`[8]`

Radeon R7

3.3GHZ

3.8GHz

4cores

65W

4MB

384

720MHz

11

UVD4.2

2133

3.1GHz

3.3GHz

45W

A6-7400K

Radeon R5

?

?

2cores

65W

1MB

256

?

11

UVD4.2

?

A4-7300

Radeon R5

3.4GHz

3.8GHz

2cores

65W

1MB

192

514MHz

11

UVD4.2

?

  
GCN 아키텍처이기 때문에 [맨틀](%EB%A7%A8%ED%8B%80.md)도 지원하며 2014년 1월 31일 맨틀을 지원하는
카탈리스트 베타 드라이버가 발표되었다.

  

A8-7600은 특이하게도 바이오스에서 사용자가 직접 TDP조절이 가능하다고 한다. 주목할 점은 45W 상태에서 벤치에서도 큰 성능저하가
일어나지
않았다.[#](http://www.guru3d.com/articles_pages/amd_a8_7600_apu_review,9.html)
[##](http://www.guru3d.com/articles_pages/amd_a8_7600_apu_review,10.html)
[###](http://www.guru3d.com/articles_pages/amd_a8_7600_apu_review,13.html)
요약하면 저전력모드에서도 GPU성능은 유지되기 때문에 그래픽 성능은 A10-6800K보다 더 좋음을 확인할 수 있으며, 동영상 인코딩
속도(CPU성능)도 A10-5800K랑 거의 비슷하였다. <del>진히로인</del> 2014년 2월 출시되며 가격은 120$로 앞으로
가성비의 끝판왕이 될 것으로 예상된다. `[9]` `[10]`  
[*](http://youtu.be/mtsNjys32Ug?t=45s)배틀필드 4를 720P 중옵에서 30프레임정도로 구동한다.

  

A8-7600과 같은 VGA를 탑재한 A10-7700K의 내장그래픽 스펙은 전작 리치랜드와 비슷하거나 낮지만,(SP 384개,720MHz)  
실제 성능은 리치랜드에 비해 클럭을 100MHz 이상 다운시켰음에도 불구하고 리치랜드보다 3D MARK 11에서 500여점정도 좋은 성능을
보여준다.`[11]` [#](http://blog.naver.com/am4410/150184609819)  
오버시 GT640 DDR3 정도의 성능을 보여준다 카더라.

[[edit](http://rigvedawiki.net/r1/wiki.php/AMD%20A%20%EC%8B%9C%EB%A6%AC%EC%A6%
88?action=edit&section=21)]

## 2.5. 카리조 ¶

2015년중 출시를 예정하는 익스카베이터 아키텍쳐를 사용하는 APU.  
상세 사항은 2014년 후반부에 밝혀질 것이다.  
<del>14년 지난걸 지적하면 지는거다</del>  
카리조의 데스크탑용 APU는 출시할 계획이 없다고 한다. [#](http://www.kbench.com/?q=node/145040)

`\----`

  * `[1]` 소켓을 유지하려 했지만 전력 관련 문제로 인해 소켓이 변경되었다고 한다. <del>FM1 사용자들은 지못미</del>
  * `[2]` DDR3램을 사용하는 특성상 램 대역폭에 의해 그래픽 성능이 저하되었기 때문이다.
  * `[3]` A10-5800K를 APU로 사용한 시스템에서 2133MHz 정도로 램 오버를 할 경우 3DMark 11 벤치마킹 결과가 P1600점대를 기본으로 넘기는 결과를 보여준다. 내장 그래픽이라고는 믿기 힘든 성능이다.
  * `[4]` 클럭 차이만큼 성능차가 발생한다고 보면 된다
  * `[5]` 2013년 12월 말에서야 국내 출시
  * `[6]` 2014년 4월 25일 멘틀을 지원하는 정식 카탈리스트 드라이버가 발표되었다. 현재 지원하는 게임은 배틀필드4인데 카베리에서는 약 10~20%정도의 성능 향상을 볼수 있다.
  * `[7]` TDP는 일반적인 사용환경에서 요구되는 쿨링 능력을 이야기하므로 실제 최대 소비전력과는 다소 차이가 있다. 이전세대의 리치랜드 A10-6800K의 경우에도 책정된 TDP는 100W이나 CPU와 iGPU를 최대클럭으로 작동시킨 최대소비전력은 프로세서만으로 사용환경에 따라서 150W에 근접한다. 이는 전력효율이 개선되었다는 카베리 세대에서도 마찬가지. 다만 기존세대에서는 온도와 정해진 프로필을 기준으로 조율하였기 때문에 쿨링능력에 여유가 있어 과열되지 않는 데스크탑에서는 클럭저하가 가시화되지 않았으나 현세대인 카베리세대에서는 전력량을 기준으로 통제하기 때문에 iGPU의 부하가 커지면 칼같이 CPU 클럭이 TDP 상한에 맞추어 하락하는 것. 이 제한을 풀면 리치랜드 세대와 마찬가지로 TDP를 넘어서는 발열이 발생한다. 
  * `[8]` 바이오스에서 TDP조절가능
  * `[9]` 2014년 8월 초, 다나와에서 최저가 105,000원에 그 모습을 드러냈다.
  * `[10]` 2015년 1월 기준으로 가성비가 20위이다. 하지만 20위까지 7600보다 성능이 한참 뒤떨어 지거나, AM3시리즈같이 전기먹는 하마들뿐인데다가 7600은 APU이기 때문에 사실상 1위 
  * `[11]` 이건 당연한 게 GPU의 아키텍쳐가 다른 이상 단순 외형적인 스펙만으로 비교할 수는 없기 때문이다. 일례로 HD 6950의 경우 스트림 프로세서의 갯수와 클럭에서 HD 7850을 앞서지만, 아키텍쳐가 다르므로 결과적으론 7850이 앞서는 것과 같은 이치이다.

