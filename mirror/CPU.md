  * [컴퓨터 관련 정보](%EC%BB%B4%ED%93%A8%ED%84%B0%20%EA%B4%80%EB%A0%A8%20%EC%A0%95%EB%B3%B4.md)  

Central Processing Unit(중앙 처리 장치)의 줄임말.  

## Contents

    

1. 개요 
2. 종류 
    

2.1. 데이터 크기에 따른 분류

2.2. 용도에 따른 분류

2.3. 명령어셋 방식에 따른 분류

3. 참고사항 
4. 대표적인 [x86계열](x86%20%EC%95%84%ED%82%A4%ED%85%8D%EC%B2%98.md) 제조사와 제품 
    

4.1. [인텔](%EC%9D%B8%ED%85%94.md)

4.2. [AMD](AMD.md)

4.3. [VIA](VIA.md)

5. 비x86 및 RISC계열 CPU 
6. [마인크래프트](%EB%A7%88%EC%9D%B8%ED%81%AC%EB%9E%98%ED%94%84%ED%8A%B8.md)
7. 관련용어 

[[edit](http://rigvedawiki.net/r1/wiki.php/CPU?action=edit&section=1)]

## 1. 개요 ¶

![basic-instruction-processing-
cycle.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/CPU/basic-instruction-
processing-cycle.jpg)

[JPG image (10.68 KB)]

  
간단화 한 CPU Instruction Cycle  

![basic-instruction-processing-cycle-with-exseption-
hangling.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/CPU/basic-
instruction-processing-cycle-with-exseption-hangling.jpg)

[JPG image (10.37 KB)]

  
예외처리를 추가한 간단한 CPU Instruction Cycle

  

명령어를 해석하여 데이터를 연산/처리를 하는 부분, 혹은 그 기능을 내장한 칩을 말한다. 그 외에도 캐시 같은 부가 장치도 들어가 있는
경우가 대다수. 기본 구성으로는 레지스터`[1]`프로그램카운터`[2]`, 명령어 레지스터 `[3]`, 산술논리연산장치(ALU:
arithmetic logic unit)`[4]`, 제어부(control unit)`[5]`과 내부 버스 등이 있다.

  

CPU 중에서도 각종 전자 부품과 반도체 칩을 하나의 작은 칩에 내장한 전자 부품을 **마이크로프로세서**라고 한다. 마이크로프로세서는 전기
밥통에 쓰이는 낮은 성능의 제품부터 컴퓨터에 쓰이는 높은 성능의 제품까지 매우 다양하다. 마이크로프로세서들 가운데 가장 복잡하고 성능이 높은
제품은 컴퓨터의 연산 장치로 쓰인다.

  

거의 모든 종류의 CPU가 하는 일은 요약해보면 대부분 <del>고작</del> 아래 4기능이 전부다.  

  * Fetch(인출) : 메모리상의 프로그램 카운터가 가리키는 명령어를 CPU로 인출하여 적재.
  * Decode(해석) : 명령어의 해석. 이 단계에서 명령어의 종류와 타겟 등을 판단한다.
  * Execute(실행) : 해석된 명령어에 따라 데이터에 대한 연산을 수행한다.
  * Writeback(쓰기) : 명령어대로 처리 완료된 데이터를 메모리에 기록한다.
<del>가장 어려운 부분을 스킵해서 쉬워보이는건 기분탓</del>

  

[[edit](http://rigvedawiki.net/r1/wiki.php/CPU?action=edit&section=2)]

## 2. 종류 ¶

  

70년대 초 단일 칩이라는 형태로 CPU가 발명된 이후 CPU의 기술은 아래와 같은 궤적을 따라 여러 방면으로 방산-발전하여 오늘날
다종다양한 산업 생태계를 구성하게 되었으며 PC용 프로세서의 경우 2012년 기준 한해 2억unit, MCU의 경우 190억unit을
생산하는 규모까지 성장하였다.

  

  * 연산 능력의 향상:PC/워크스테이션/서버용 프로세서의 발전 방향  
\- 향상된 클럭.  
\- 향상된 클럭당 명령어 실행 숫자(IPC).  
\- 병렬실행(멀티코어, SIMD)  

  * 연산 기능의 특화:GPU및 DSP의 발전 방향.  
\- 고도의 병렬화(GPU)  
\- 특화된 연산기능(DSP)  

  * 입출력 기능의 다양화와 원가절감:MCU의 발전 방향.  
\- 다종다양한 I/O 기능의 통합.  
\- [SoC](SoC.md).  

다음은 각 분류 방식에 따른 CPU의 종류이다.

[[edit](http://rigvedawiki.net/r1/wiki.php/CPU?action=edit&section=3)]

### 2.1. 데이터 크기에 따른 분류 ¶

  * 4비트  

\- 최초의 단일칩`[6]` CPU로 인정받고 있는 인텔의 i4004가 바로 4비트 CPU이다.

  * 8비트  

\- PC시대의 서막을 연 [Z80](Z80.md)이나 [i8080](i8080.md), 마이크로컨트롤러용으로 많이 사용되는
[8051](8051.md), [AVR](AVR.md), [MC6800](MC6800.md),
[PIC](PIC.md)등이 여기에 포함된다. 최근까지도 CPU시장에서 숫적으로 주력의 자리를 차지했다`[7]`.

  * 16비트  

\- 오늘날의 PC산업을 있게 한 IBM-PC XT에 들어가는 [i8088](i8088.md)이 대표적이다.
[i80286](i80286.md) [i80196](i80196.md), [C166](C166.md)등이 있다.

  * 32비트  

\- 속칭 386으로 불리우는 [i80386](i80386.md)이 대표적이다. PC시장 발전기의 레전드급 아키텍처의 이름들이 대거
포진해 있다. [MIPS](MIPS.md), [ARM](ARM.md), [M68000](M68000.md), [PA-RISC](PA-RISC.md), [PowerPC](PowerPC.md) 등. 또한 8비트계에서 성공을 거둔 PIC이나 AVR등이
PIC32, AVR32등으로 확장된 경우도 있다`[8]`.

  * 64비트  

\- 보통은 32비트급의 네임드 아키텍처가 64비트로 확장되어 개발된 경우가 대부분. [x86-64](x86-64.md),
[Alpha](Alpha.md), [MIPS64](MIPS64.md), [ARMv8](ARMv8.md)
[Power](Power.md)등이 대표적이다.  

[[edit](http://rigvedawiki.net/r1/wiki.php/CPU?action=edit&section=4)]

### 2.2. 용도에 따른 분류 ¶

  * MPU  

\- 일반적인 PC/워크스테이션 등에 사용되는 일반적인 CPU를 MPU로 지칭한다. 다만 이러한 용어들의 경우 그 개념이 명확하지 않은
경우가 많은데 이는 업계에서 자사 제품을 지칭하는 용어가 관례적으로 굳어진 경우가 대부분이기 때문`[9]`.

  * MCU  

\- 마이크로컨트롤러로도 불리우며 오늘날 지구상에 존재하는 CPU 숫자의 대다수를 차지하고 있다. 2013년 한해 동안 추정되는 생산량은
190억개로 PC용 프로세서 2억개의 100배 규모. PC용 CPU가 사용자가 작성하거나 소유한 다종다양한 프로그램을 구동시키는데 비해
MCU는 주로 제조사에서 작성한 고정된 특정 프로그램을 미리 집어넣은 상태에서 완제품에 탑재하여 출시하는 경우가 대부분이다`[10]`.
일반적으로 잘 알려진 [아두이노](%EC%95%84%EB%91%90%EC%9D%B4%EB%85%B8.md)에 탑재된 ATmega칩이
바로 전형적인 MCU이다.

  * [DSP](Digital%20Signal%20Processor.md)  

\- 특정 종류의 신호 데이터 형식을 고속연산, 특히 행렬연산을 하는데 최적화된 CPU. 때문에 보통 DSP를 부를 때에는 목표로 하는
데이터 종류에 따라 오디오DSP, 16비트 정수DSP, 32비트 실수DSP 등으로 타겟 데이터 형식을 명시하는 경우가 많다.
[TI](TI.md)의 TMS시리즈가 유명하다. 특정 데이터 포맷 처리에 특화되었기 때문에 그 외의 데이터 포맷이나 메모리핸들링,
프로그램 제어쪽의 기능은 부실한 경우가 많다.

  * FPU  

\- 실수 연산에 특화된 CPU로 인텔의 i80X87계열이 대표적이다. 프로그래밍에 필요한 제어 구조가 없어서 위에서 설명한 DSP와는 달리
단독으로 프로그램을 구동시키지는 못하고 범용 CPU와 묶여 Co-Processor 형태로 사용되는 경우가 대부분이었으며 2000년대 이후로는
독립된 제품 보다는 주로 범용 CPU내의 연산유닛으로 포함되는 것이 대세.

  * GPU  

\- DSP 중에서도 비디오 출력 데이터 처리에만 극단적으로 특화된 제품`[11]`. 제어구조가 없거나 매우 부실하지만 (연산해야 하는
데이터의 특성으로 인해)병렬성이 극히 높아서 연산 쓰루풋이 대단히 높은 특징을 가지고 있다. 다만 대부분 제어구조가 부실하므로 일반적인
프로그래밍을 GPU에서 돌리는 것은 무리.`[12]`  

[[edit](http://rigvedawiki.net/r1/wiki.php/CPU?action=edit&section=5)]

### 2.3. 명령어셋 방식에 따른 분류 ¶

  * CISC 방식 CPU  

\- 초기에 CPU가 원칩 형태로 등장하기 이전부터 <del>일단 만들기 시작해서 그냥 막 만들었던</del> 발전해 왔던 명령어셋을 사용한
CPU. x86계열이나 M6800/M68k등이 대표적이다.

  * RISC 방식 CPU  

\- 80년대부터 문제로 지적된 명령어셋의 복잡화와 그로 인한 CPU설계의 복잡화를 해결하기 위해 등장한 간략화된 명령어셋을 도입한 CPU.
x86이나 8051 계열을 제외한 대부분의 현용 CPU 아키텍처가 RISC 방식 명령어를 채택하고 있다.

  * VLIW 방식 CPU  

\- 90년대부터 등장한 명령어 레벨의 병렬 실행이 가능한 명령어셋을 가지고 있는 CPU. 대표적으로
[크루소](%ED%81%AC%EB%A3%A8%EC%86%8C.md)와 [TI](TI.md)의 TMS6400시리즈, 그리고
<del>이타닉</del>[아이태니엄](%EC%95%84%EC%9D%B4%ED%83%9C%EB%8B%88%EC%97%84.md)이
있다.

  * SIMD  

\- 명령어 레벨의 병렬성이 아닌 데이터 병렬성을 구현한 CPU 이지만`[13]` 현재는 별도의 제품이 아닌 기존 CPU에 확장 명령어셋과
실행유닛을 추가한 형태로 구현되어 있다. [MMX](MMX.md), [3D-Now!](3D-Now%21.md),
[SSE](SSE.md)가 대표적.  

[[edit](http://rigvedawiki.net/r1/wiki.php/CPU?action=edit&section=6)]

## 3. 참고사항 ¶

[CPU 벤치마크 사이트](http://www.cpubenchmark.net/cpu_list.php)`[14]`

  

<http://www.cpu-world.com> 지금까지 출시 된 CPU들을 거의 모두 볼 수 있는 사이트이다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/CPU?action=edit&section=7)]

## 4. 대표적인 [x86계열](x86%20%EC%95%84%ED%82%A4%ED%85%8D%EC%B2%98.md) 제조사와 제품 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/CPU?action=edit&section=8)]

### 4.1. [인텔](%EC%9D%B8%ED%85%94.md) ¶

[인텔 CPU 목록](%EC%9D%B8%ED%85%94%20CPU%20%EB%AA%A9%EB%A1%9D.md) 항목 참조

  

[[edit](http://rigvedawiki.net/r1/wiki.php/CPU?action=edit&section=9)]

### 4.2. [AMD](AMD.md) ¶

[AMD CPU 목록](AMD%20CPU%20%EB%AA%A9%EB%A1%9D.md) 항목 참조  

[[edit](http://rigvedawiki.net/r1/wiki.php/CPU?action=edit&section=10)]

### 4.3. [VIA](VIA.md) ¶

코드네임은 대부분 [성경](%EC%84%B1%EA%B2%BD.md)에 나오는 지명이나 인명에서 따왔다.  
CPU칩 단품으로 유통되는 경우는 거의 없고, 대부분 온보드 형식으로 팔린다.  

  * [에덴](%EC%97%90%EB%8D%B4.md)
  * [C3 느헤미야](C3.md)
  * [C7 에스더](C7.md)
  * [나노](%EB%82%98%EB%85%B8.md)  

[[edit](http://rigvedawiki.net/r1/wiki.php/CPU?action=edit&section=11)]

## 5. 비x86 및 RISC계열 CPU ¶

  * [ARM](ARM%28CPU%29.md)
  * [CELL-Broadband Engine](CELL-Broadband%20Engine.md)
  * [POWER](POWER%28%EB%A7%88%EC%9D%B4%ED%81%AC%EB%A1%9C%ED%94%84%EB%A1%9C%EC%84%B8%EC%84%9C%29.md) \- [IBM](IBM.md)
  * [PowerPC](PowerPC.md) \- [IBM](IBM.md), [모토로라](%EB%AA%A8%ED%86%A0%EB%A1%9C%EB%9D%BC.md), [애플](%EC%95%A0%ED%94%8C.md)
  * [68000](68000.md) \- [모토로라](%EB%AA%A8%ED%86%A0%EB%A1%9C%EB%9D%BC.md)
  * [SPARC](SPARC.md) \- [SUN](SUN.md)
  * [Z80](Z80.md) \- [자일로그](%EC%9E%90%EC%9D%BC%EB%A1%9C%EA%B7%B8.md)
  * Alpha`[15]` \- DEC `[16]`
  * R시리즈 - MIPS
  * [크루소](%ED%81%AC%EB%A3%A8%EC%86%8C.md)
  * [군사&우주용 CPU](%EA%B5%B0%EC%82%AC%26%EC%9A%B0%EC%A3%BC%EC%9A%A9%20CPU.md)  

[[edit](http://rigvedawiki.net/r1/wiki.php/CPU?action=edit&section=12)]

## 6. [마인크래프트](%EB%A7%88%EC%9D%B8%ED%81%AC%EB%9E%98%ED%94%84%ED%8A%B8.md) ¶

  

마인크래프트의 논리회로 블럭들을 이용하면 이론상 현존하는 모든 회로를 구현할 수 있다. 물론 가장 복잡한 회로인 CPU의 구현에도 많은
용자들이 도전하였고 성공한 케이스도 [유튜브](%EC%9C%A0%ED%8A%9C%EB%B8%8C.md)에서 심심치 않게 볼 수 있다.

  

<http://blog.naver.com/torudia/150124648938>  
네이버 블로그 TORUDIA가 구현한 CPU. 아직 완전히 CPU의 완성을 본것은 아니나 상당부분 진척되어 있다. 쿼드코어를 구현했다.

  

이제 컴퓨터 성능만 받쳐준다면 컴퓨터에서 마인크래프트를 돌려서, CPU를 만들고 메모리장치와 디스플레이를 구현하고(일단 여기까지는 현재
구현되어있다) 그렇게 구현한 마인크래프트 컴퓨터 내부에 마인크래프트를 또 실행하고 또 실행하는 것이 가능은 해졌다. `[17]`

  

[[edit](http://rigvedawiki.net/r1/wiki.php/CPU?action=edit&section=13)]

## 7. 관련용어 ¶

  * [CPU 소켓 목록](CPU%20%EC%86%8C%EC%BC%93%20%EB%AA%A9%EB%A1%9D.md)
  * [멀티코어 프로세서](%EB%A9%80%ED%8B%B0%EC%BD%94%EC%96%B4%20%ED%94%84%EB%A1%9C%EC%84%B8%EC%84%9C.md)
  * [인공지능](%EC%9D%B8%EA%B3%B5%EC%A7%80%EB%8A%A5.md)
  * [4GHz의 벽](4GHz%EC%9D%98%20%EB%B2%BD.md)
  * [클럭](%ED%81%B4%EB%9F%AD.md)
  * [오버클럭](%EC%98%A4%EB%B2%84%ED%81%B4%EB%9F%AD.md)
  * [x86](x86.md)
  * [CISC](CISC.md)
  * [RISC](RISC.md)
  * [MIPS](MIPS.md)
  * <del>[너의 CPU를 믿어봐](%EC%9E%84%EC%9A%94%ED%99%98.md)</del>

`\----`

  * `[1]` Register(REG or R) : 연산유닛과 연결된 액세스속도가 가장 빠른 기억장치
  * `[2]` Program Counter(PC) : 다음에 인출할명령어의 주소를 가지고 있는 레지스터, 각 명령어가 인출된 후에는 명령어 길이만큼 주소를 증가시킴으로써 주소를 포인팅함. 분기(jump) 명령어가 실행되는 경우에는 목적지주소로 갱신한다
  * `[3]` Instruction Register(IR) : 현재 실행중인 명령의 내용을 기억하고 있는 레지스터
  * `[4]` 각종 산술연산(덧셈, 뺄셈, 곱셈, 나눗셈)과 논리연산(AND, OR, NOT, XOR 등)들을 수행하는 회로들로 이루어진 회로
  * `[5]` 명령어를 해석하고, 그것을 실행하기 위한 제어 신호들(control signals)을 순차적으로 발생하는 회로
  * `[6]` 말 그대로 CPU의 기능을 원칩화한 것을 의미한다. 즉 i4004 이전에도 멀티칩 형태의 CPU가 보드 형태로 존재했다.
  * `[7]` 2012년 기준 출하량 60억개로 PC용 프로세서의 예상출하량 2억개의 30배에 달하는 수량이다.
  * `[8]` 애초에 i80386계열도 8051과의 확장관계라고도 볼 수 있는데 이는 8051이 i8080의 분가에 해당하는 위치이기 때문.
  * `[9]` 예를 들어 CPU는 처음에는 인텔이 자사의 원칩 솔루션을 부를때 쓰던 용어이고 MPU는 그에 대응하여 모토롤라가 쓰던 용어이다. 마이크로프로세서는 말 그대로 MPU를 한글로 풀어놓은 용어. 그리고 CPU가 원보드 솔루션에서 원칩솔루션으로 전환한 현재 시점에서는 CPU와 MPU, 마이크로프로세서라는 단어는 서로 혼용해도 별 문제가 없다. 다만 MPU는 MCU에 상대적인 느낌으로 인해 MCU가 아닌 마이크로프로세서도 포괄하는 의미로 MPU라는 단어를 사용하는 경우도 있다. 즉 그냥 MCU의 개념만 잘 구분할 수 있으면 문제되지 않는 부분.
  * `[10]` 이를 펌웨어 Firmware라고 부른다.
  * `[11]` 초기 GPU는 그냥 상용 DSP를 활용하는 경우도 많았다.
  * `[12]` 물론 굳이 하려면 할 수는 있다. [GPGPU](GPGPU.md) 참조.
  * `[13]` 초기 SIMD는 두 개 이상의 CPU를 사용하여 프로그램 메모리 포인터를 공유하고 데이터메모리 포인터를 따로 두는 방식으로 SIMD를 구현했다.
  * `[14]` 분류를 보면 알겠지만 각각의 분류에는 동일한 아키텍쳐를 가진 CPU들만 열거되어 있다. 호환이 다른 CPU를 하나의 절대지표에 놓고 평가를 하는 것이 쉽지 않기 때문이다.
  * `[15]` 64Bit, GHz급 클럭을 먼저 적극적으로 사용한 CPU로, 20C가 끝나기 전까지 워크스테이션용 CPU로 상당히 많이 사용되었다.
  * `[16]` 후반기에 삼성전자에서 CPU를 생산한 적이 있다.
  * `[17]` 하지만 마인크래프트는 [자바 가상 머신](%EC%9E%90%EB%B0%94%20%EA%B0%80%EC%83%81%20%EB%A8%B8%EC%8B%A0.md)에서 돌아가는 게 함정. 만일 저런 것을 실제로 구현한다면 처음부터 바이트코드를 명령어 셋으로 쓰도록 설계하는 게 효율적일 것이다.

