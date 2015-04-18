Heterogeneous System Architecture(이기종 시스템 아키텍처)의 줄임말

## Contents

    

1 HSA란?

2 역사

3 HSA의 개념

    

3.1 hUMA

3.2 hQ

3.3 HSA 의 목표와 한계

4 HSA재단

[[edit](http://rigvedawiki.net/r1/wiki.php/HSA?action=edit&section=1)]

# 1 HSA란? ¶

<del>[GPGPU](GPGPU.md)사의 CPU 과장이 GPU 대리를 우대하여 회사를 살린다는 드라마틱한 이야기</del>

  

![http://media.bestofmicro.com/amd-huma-
slide-5-chart,9-D-382657-3.jpg](http://z1.enha.kr/http://media.bestofmicro.com
/amd-huma-slide-5-chart,9-D-382657-3.jpg)

[[JPG external image]](http://media.bestofmicro.com/amd-huma-
slide-5-chart,9-D-382657-3.jpg)

  

HSA(Heterogeneous System Architecture)란 이기종 시스템 아키텍처의 줄임말이다.

  

말은 거창한데 개념은 간단하다 <del>그런데 정작 구조는 조금도 간단하지 않다.</del> 동일한 성격의 코어를 모은 프로세서(멀티코어
CPU나 GPU) 를 가리켜 [호모](%ED%98%B8%EB%AA%A8.md)지니어스 Homogeneous 라고 하는데, 이와는 반대로
전혀 다른 역할을 하는 코어를 하나로 통합한 프로세서를 가리켜 헤테로지니어스 Heterogeneous 라고 부른다.

  

HSA는 CPU와 GPU를 하나의 연산체로 간주하는 추상 계층을 생성해, GPU의 연산력을 이용하는 한편, CPU와 CPU 사이에 데이터가
오갈 필요를 없앤다는 것이다.

  

즉 HSA란 [CPU](CPU.md)와 [GPU](GPU.md)를 하나의 칩으로 통합시키고 둘 사이에 긴밀한 연계를 추구하는
것이다.

  

이는 GPU가 발전하면서 이를 새로운 연산 장치로 활용하려는시도가 생겼고, 이로부터 도출된 문제점과 그 해결책을 찾아가면서 만들어지게 된
개념이다. 간단하게 [GPGPU](GPGPU.md)를 지금보다 더 활용하기 쉽도록 하다는 아키텍쳐 설계법이라고 보면 된다.

  

[멀티코어 프로세서](%EB%A9%80%ED%8B%B0%EC%BD%94%EC%96%B4%20%ED%94%84%EB%A1%9C%EC%84%B8%EC%84%9C.md)랑 비슷한 개념이지만 전혀 다른 성격의 프로세서의 통합을 추진한다는점에서 다르다.

[[edit](http://rigvedawiki.net/r1/wiki.php/HSA?action=edit&section=2)]

# 2 역사 ¶

개념 자체는 예전부터 제시되었지만, HSA라는 이름을 가지게 된 역사는 짧다.  
HSA라는 이름이 나오게 된 것은 [2000년대](2000%EB%85%84%EB%8C%80.md) 중반 경이었고 HSA재단이 설립된 건
[2012년](2012%EB%85%84.md)경이다.  
그리고 HSA를 지원하는 AMD의 첫번째 하드웨어는
[카베리](AMD%20A%20%EC%8B%9C%EB%A6%AC%EC%A6%88#s-2.4.md)로서,
[2014년](2014%EB%85%84.md) [1월](1%EC%9B%94.md)에 발매되었다.  
또한 [OpenCL](OpenCL.md) 2.0에서 HSA 가 표준 명령어로 포함되었기 때문에
[OpenCL](OpenCL.md)을 지원하는 소프트웨어에서는 HSA를 활용할수 있을 예정이다.`[1]`

  

이외에도 [플레이스테이션4](%ED%94%8C%EB%A0%88%EC%9D%B4%EC%8A%A4%ED%85%8C%EC%9D%B4%EC%85%98%204.md)가
HSA에 기반하여 설계된 하드웨어 이다.

  

<del>하지만 가야할 길이 아직 멀다.</del>

[[edit](http://rigvedawiki.net/r1/wiki.php/HSA?action=edit&section=3)]

# 3 HSA의 개념 ¶

HSA는 크게 다음과 같은 개념으로 이루어져있다. hUMA , hQ

[[edit](http://rigvedawiki.net/r1/wiki.php/HSA?action=edit&section=4)]

## 3.1 hUMA ¶

![http://media.bestofmicro.com/amd-slide-9-introducing-
huma,9-E-382658-3.jpg](http://z3.enha.kr/http://media.bestofmicro.com/amd-
slide-9-introducing-huma,9-E-382658-3.jpg)

[[JPG external image]](http://media.bestofmicro.com/amd-slide-9-introducing-
huma,9-E-382658-3.jpg)

  

hUMA :heterogeneous Uniform Memory Access(헤테로지니어스 유니폼 메모리 액세스)의 줄임말

  

CPU와 GPU 메모리 영역을 통일하는하여 서로 다른 프로세서간에 [메모리 영역](RAM.md)을 공유한다는 개념이다. 한마디로 GPU
코어가 CPU 코어의 하나인 것처럼 메모리에 액세스할 수 있다는 것이다.

  

기존 방식은 CPU와 GPU가 서로 다른 메모리 영역으로 나뉘어져 있다.(NUMA) 이렇게 따로 떨어진 메모리 사이에서는 데이터 복사때마다
동기화와 주소 변환이 필요하다. 이를 CPU와 GPU가 공유하는 추상화된 메모리 계층을 생성해 해결한다는 것이다.  

이 과정에서의 CPU와 GPU의 양방향 메모리의 일관성을 하드웨어로 유지하게 된다. 양방향으로 하드웨어가 캐시를 스누프하고 일관성을 자동으로
확보한다. 어느 프로세서가 캐시의 데이터를 갱신했을 경우 다른 프로세서를 탐지할 수 있어 메모리 일관성의 에러가 생기지 않도록 하는
것이다.`[2]`

  

간단하게 설명하자면 지금까지의 데이터 연결방식은 "CPU < \- > 주 메모리 < \- > GPU 메모리 -> GPU" 였는데 주 메모리와
GPU메모리 영역을 통합시켜 "CPU < \- > 공유 메모리 < \- > GPU" 로 변환 한다는 것이다.  
직렬(연속적인) 작업 담당하는 CPU와 병렬화 작업를 담당하는 GPU를 효율적으로 묶는 게 hUMA의 역할이다. 이를 통해서 GPU에서
실행하는 범용 프로그램을 지금보다 더 간단하게 쓸 수 있도록 하는 것이다.

  

  * 장점 : 간단해진 작업 스케줄로 관리가 편해진다.
데이터 처리 단계가 줄어들어 작업 스케쥴이 단순해지며 지금까지는 CPU와 GPU 간 데이터 전달을 [OS](OS.md)가 관리하였기
때문에 데이터 추적이 힘들었는데, 복사할 필요가 없어짐으로써 데이터 추적이 간단해지고 메모리 관리가 훨씬 편해지게 된다.  

이로 인해 줄어든 작업 스케줄만큼 더 빠른 처리가 가능해지고 또한 불필요한 메모리 액세스가 줄어들어 전력 소비도 억제할 수 있다.  
또한 프로그래머 입장에서는 하드웨어간의 데이터 전달시의 데이터 간의 동기화 와 일관성 문제를 신경 쓸 필요가 없게 된다.`[3]`
<del>이 때문에 [소니](%EC%86%8C%EB%8B%88.md) 퍼스트 파티들이 거의 [플레이스테이션4](%ED%94%8C%EB%A0%88%EC%9D%B4%EC%8A%A4%ED%85%8C%EC%9D%B4%EC%85%98%204.md)를
찬양하는 분위기라고 [카더라](%EC%B9%B4%EB%8D%94%EB%9D%BC.md)</del>  

  * 단점 : 시대를 역행한 기술이다.  
현재 GPU속도는 매우 빠르게 발전하였고 이 속도에 맞추어 GPU전용 메모리는 주메모리보다 월등히 빠른 속도로 동작한다. 그런데 주메모리에
GPU 메모리 영역을 통합시킨다면 GPU의 동작 속도도 덩달아 떨어지게 된다. 이 점은 이 기술이 내장 그래픽 전용 기술이 될 수 밖에 없게
된 이유이다.`[4]``[5]`

게다가 지금까지의 만들어진 프로그램은 GPU 메모리로 데이터를 보내도록 만들어졌다.`[6]` 당연히 기존 프로그램과는 전혀 호환이 되지
않는다. 이러한 HSA의 장점을 살리기 위해서는 기존방식과는 다른 방식으로 데이터를 전송하도록 프로그램을 짜야 한다. 즉 기존 프로그램
사용자에게는 전혀 쓸모 없는 기술인 셈이다.

  

이외의 더 자세한 내용은 [추가바람](%EC%B6%94%EA%B0%80%EB%B0%94%EB%9E%8C.md)

[[edit](http://rigvedawiki.net/r1/wiki.php/HSA?action=edit&section=5)]

## 3.2 hQ ¶

![http://www.4gamer.net/games/147/G014731/20131021024/TN/004.jpg](http://z3.en
ha.kr/http://www.4gamer.net/games/147/G014731/20131021024/TN/004.jpg)

[[JPG external
image]](http://www.4gamer.net/games/147/G014731/20131021024/TN/004.jpg)

  
< 기존 방식 >  

![http://www.4gamer.net/games/147/G014731/20131021024/TN/007.jpg](http://z3.en
ha.kr/http://www.4gamer.net/games/147/G014731/20131021024/TN/007.jpg)

[[JPG external
image]](http://www.4gamer.net/games/147/G014731/20131021024/TN/007.jpg)

  
< hQ>  
hQ : Heterogeneous Queueing(헤테로지니어스 큐잉)의 줄임말

  

hQ 를 간단하게 말하면 CPU와 GPU 사이에 있던 높은 장벽을 줄이는 방식의 구조를 말한다.

  

간단하게 정리해서 현재의 GPU처리는 [OS](OS.md)에 의해서만 제어 될 수 있다. 그래서 GPU 접근은 애플리케이션 -> OS
API -> 드라이버 -> GPU 의 방식으로 접근하는데 GPU가 작업을 실행할 때마다 이 과정을 거치게 됨으로써 GPU를 효율적으로 사용할
수가 없을 뿐더러, 이 과정에서 [상당한 지연](%EB%B3%91%EB%AA%A9%20%ED%98%84%EC%83%81.md)이
발생한다.`[7]`

  

그래서 사용자가 직접 [GPU](GPU.md)에 프로세스나 작업을 할당할수 있도록 한다는것이 hQ의 개념이고, 이를 위해 사용자가
GPU 작업을 실행하기 위한 구조를 하드웨어 단계에서 제공하는 것이 hQ이다.  

  * 장점: GPU 작업을 유저가 직접 액세스할 수 있다. 이에 따라서 기존 방식의 복잡한 계층 변환에 의한 접근이 필요하지 않게 되면서 오버헤드를 크게 낮출 수 있다. <del>CPU : 일이 줄었다! [야 신난다](%EC%95%BC%20%EC%8B%A0%EB%82%9C%EB%8B%A4.md)</del>  
OS를 거치지 않기 때문에 GPU 작업을 실행하기 위한 패킷 형식을 HSA 기반 플랫폼 하에서 표준화할 수 있다. 즉 x86 기반 프로세서나
[ARM](ARM.md) 기반 프로세서도 HSA를 지원하기만 한다면 같은 포맷을 활용하여 GPU를 사용할 수 있게 된다.  

  * 단점 : 잠재적인 호환성 문제가 생길수 있다.  
OS가 모든 주변기기를 제어하는 것은 그것이 사용자에게 가장 편리하기 때문이다. 사용자 애플리케이션이 하드웨어에 마음대로 접속할 수 있는
환경에서는, 애플리케이션의 호환성을 보증하지 못하고 보안도 지킬 수 없다.`[8]`  
또한 hUMA와 비슷한 문제가 있는데 이 새로운 접근방식은 어플리케이션의 접근 방식도 완전히 바꾸어야 한다. 이 방식이 기존 방식보다 더
쉽고 빠르더라도 지금까지 쌓아올린 노하우를 전부 포기하고 새로운 하드웨어에 맞춘 새로운 방식의 프로그래밍 기법을 활용할 할만큼 모험심 강한
프로그래머도 많지 않다는 점이다.  
게다가 이 새로운 하드웨어를 만들고 있는 회사는 시장 점유율이 20%에 불과하고 전체 하드웨어에서는 10% 안되는 규모인데 이러한 새로운
하드웨어에 맞추어 프로그램을 만들 회사도 많지 않다는 점이다.
<del>[마이너](%EB%A7%88%EC%9D%B4%EB%84%88.md)의 비애</del>  

이 이상의 내용은 [추가바람](%EC%B6%94%EA%B0%80%EB%B0%94%EB%9E%8C.md)

[[edit](http://rigvedawiki.net/r1/wiki.php/HSA?action=edit&section=6)]

## 3.3 HSA 의 목표와 한계 ¶

![http://images.kbench.com:8080/kbench/article/2014_01/k128925p1n3.jpg](http:/
/z4.enha.kr/http://images.kbench.com:8080/kbench/article/2014_01/k128925p1n3.j
pg)

[[JPG external
image]](http://images.kbench.com:8080/kbench/article/2014_01/k128925p1n3.jpg)

  
< 현재의 GPU 활용 방식 OS의 간섭이 많고 단계가 복잡하여 활용하기가 힘들다. >  

![http://images.kbench.com:8080/kbench/article/2014_01/k128925p1n7.jpg](http:/
/z4.enha.kr/http://images.kbench.com:8080/kbench/article/2014_01/k128925p1n7.j
pg)

[[JPG external
image]](http://images.kbench.com:8080/kbench/article/2014_01/k128925p1n7.jpg)

  
< HSA의 GPU 활용방식 어플리케이션이 직접 GPU를 활용 할수 있도록 하여 효율을 높인다. >

  

HSA의 궁극적인 목적은 병렬 연산 프로그래밍의 확대이다. 이를 위해 GPGPU프로그래밍의 난이도를 낮추고 하드웨어의 제약에 얽매이지 않게
동작할 수 있는 병렬 컴퓨팅 환경을 만드는 것이다. `[9]` 이 목적은 AMD가 2000년 중반에 내세웠던 해테로지니어스 코어라는 목표를
전 플렛폼으로 확대한 모습이기도 하다.

  

궁극적인 단계에서는사용자 입장에서 GPU는 CPU의 보조 연산 코어정도로 인식할 정도로 [GPGPU](GPGPU.md) 프로그래밍의
난이도를 낮추는것이 목표이다.

  

그러나 목적만큼 그 한계 역시 뚜렷하다. GPGPU 분야에서 선두주자인 [nVIDIA](nVIDIA.md)의
[CUDA](CUDA.md)를 끌어들이지 못했다는 점`[10]`, 그리고 CPU쪽에서도 인텔을 끌어들이지 못해서 당장 대부분의
프로그래머들이 HSA에 대해서 [영 좋지못한](%EC%98%81%20%EC%A2%8B%EC%A7%80%20%EB%AA%BB%ED%95%9C.md) 시선이다. 아무리 GPGPU
난이도가 낮아진다고해도 이를 이용할 하드웨어가 없다면 무용지물이다. 그런데 AMD는
[카베리](AMD%20A%20%EC%8B%9C%EB%A6%AC%EC%A6%88#s-2.4.md)부터 비로소 HSA를 지원할정도로 늦은
속도로 HSA를 지원하는 하드웨어를 발표하고 있다.

  

게다가 [인텔](%EC%9D%B8%ED%85%94.md)과 [IBM](IBM.md)도 독자 플렛폼으로 GPGPU시장에 진출
중이라는 점은 장기적으로 HSA 프로젝트의 발목을 잡을 것으로 보인다.

[[edit](http://rigvedawiki.net/r1/wiki.php/HSA?action=edit&section=7)]

# 4 HSA재단 ¶

AMD가 2012년 이기종 시스템 아키텍쳐 연구를 하기 위해서 만들어진 설립한 비영리 재단이다.  
[ARM](ARM%28CPU%29.md) 진영을 비롯하여, 모바일 칩셋을 생산하는 회사들이 대거 가입해
있다([삼성전자](%EC%82%BC%EC%84%B1%EC%A0%84%EC%9E%90.md)도 여기에 속해 있다). 이처럼 HSA기술은
ARM 진영에서 환영 받고 있다.  
[인텔](%EC%9D%B8%ED%85%94.md), [nVIDIA](nVIDIA.md), [IBM](IBM.md)을 비롯하여
독자 플렛폼으로 [GPGPU](GPGPU.md) 분야에 진출중인 회사들은 가입되어 있지 않다. <del>더구나 이 세 업체가 차지하는
반도체 칩셋 비중이 전체의 3분의 1이다.</del>

  

자세한 내용은 [HSA 재단(영문)](http://hsafoundation.com/) 참고.

`\----`

  * `[1]` [어도비](%EC%96%B4%EB%8F%84%EB%B9%84.md)와 [LibreOffice](LibreOffice.md)가 HSA를 지원할것이라고 밝혔다.
  * `[2]` 아주 아주 아주 간단하게 말해서 [CUDA](CUDA.md)와 비슷한 방향으로 가고 있다고 생각하면 된다.
  * `[3]` 즉 과거 방식에서는 주 메모리와 GPU 메모리 간의 두 데이터의 일치 여부를 누군가가 확인해주어야 한다. 게다가 [최적화](%EC%B5%9C%EC%A0%81%ED%99%94.md)를 위해서는 GPU메모리가 어느 정도까지 데이터를 한 번에 처리할 수 있는지 여부를 직접 프로그래머가 확인하고 여기에 맞추어 처리 할 데이터양을 조절해야 했다. 그런데 HSA에서는 [그런 거 없다](%EA%B7%B8%EB%9F%B0%20%EA%B1%B0%20%EC%97%86%EB%8B%A4.md).
  * `[4]` 물론 주메모리로 GDDR5를 때려 박는다면 아주 간단하게 해결되겠지만 일반 PC에서 주 메모리로 GDDR5를 쓰는 건 여러모로 무리가 있다.
  * `[5]` 정확하게 말해서 HSA는 외장 GPU 메모리와의 통합도 추진하고 있다. 그래서 정확하게는 틀린 말이다. 그러나 현실적인 한계로 아직은 내장그래픽에서만 HSA가 적용되고 있다.
  * `[6]` 주 메모리의 속도가 GPU 처리속도를 못따라오다보니 미리 처리할 데이터를 GPU메모리에 보내준다. 이를 '프리로딩' 이라고 하는데 자세한 내용은 해당 항목 참고
  * `[7]` 물론 OS가 수행하는 모든 작업은 CPU가 담당한다. 즉 GPU를 활용하기 위해서 GPU에 접근할때 때마다 CPU는 엄청난 작업을 처리하는 셈이다.
  * `[8]` 간단하게 말해서 어플리케이션이 접근 해서는 안되는 위치의 메모리 주소에 접근하면 **시스템이 다운되어 버린다.** 이를 방지 하기 위해서 OS가 모든 하드웨어와 메모리 접근을 관리하고 있다. 그럼에도 접근할수 없는 위치에 어플리케이션이 접근한다면 OS는 [블루스크린](%EB%B8%94%EB%A3%A8%EC%8A%A4%ED%81%AC%EB%A6%B0.md) 등의 [커널 패닉](%EC%BB%A4%EB%84%90%20%ED%8C%A8%EB%8B%89.md)을 일으킨다. 즉 OS를 배제한 접근 방식은 잠재적으로 커널 불안정을 초래할 가능성을 내포하고 있다.
  * `[9]` 예를 들어 AMD GPU/APU에서 동작하는 병렬 컴퓨팅 프로그램을 만들었다면 이것이 'ARM + POWER VR'에서도 프로그램 수정없이 돌아갈수 있다는 것이다.
  * `[10]` CUDA는 대표적인 폐쇄 플랫폼이다. nVIDIA GPU에서만 돌아가는 녀석이니...

