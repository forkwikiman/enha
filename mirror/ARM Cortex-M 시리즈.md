## Contents

    

1. 개요 
2. 역사 
3. 특징 
4. 종류 
5. 뒷이야기 

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20Cortex-M%20%EC%8B%9C%EB%A6%AC
%EC%A6%88?action=edit&section=1)]

## 1. 개요 ¶

[ARM](ARM.md)사의 Cortex-A/R/M 제품 라인업 중 [MCU](MCU.md)전용 라인업에 해당하는 CPU IP 및
마이크로 아키텍처.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20Cortex-M%20%EC%8B%9C%EB%A6%AC
%EC%A6%88?action=edit&section=2)]

## 2. 역사 ¶

2000년대 초반까지만 해도 ARM의 제품 개발 전략은 단일 코어 개발 방식을 고수하고 있었다. 예를 들어 ARM920이라는 애플리케이션
프로세서용 제품을 하나 개발해 놓고 거기에서 메모리 계층을 RTOS에 적합하도록 변경하여 ARM940 등의 이름으로 출시하는 방식을
고수하였고 MCU용 제품 라인업은 따로 개발을 하지 않고 구형의 ARM7TDMI 코어에 의존하고 있는 상황이었다.  
이러한 개발방식이 Cortex 라인업 단계로 넘어오면서 큰 전기를 맞게 되었는데 이때부터 ARM사는
애플리케이션프로세서/리얼타임프로세서/마이크로컨트롤러 계열의 제품을 완전히 분리하여 동시에 개발하는 방식을 유지하게 된다.  
이러한 정책에 따라 2004년 이후 ARM 라인업은 폭발적으로 증가하게 되고 Cortex-M도 예외는 아니라서 2004년에서 2014년
현재까지 5개의 라인업이 출시되었다.

  

2014년 기준으로 Cortex-M 생산 라이센스 계약을 체결한 업체는 220개가 넘으며 관련 제품은 3000개, 생산량은 누적 160억개에
도달한
상황[#](http://pc.watch.impress.co.jp/img/pcw/docs/651/424/html/034.jpg.html).

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20Cortex-M%20%EC%8B%9C%EB%A6%AC
%EC%A6%88?action=edit&section=3)]

## 3. 특징 ¶

\- ARM7TDMI과 비교하여 ARM 명령어가 폐지되고 Thumb/Thumb-2 명령어만 사용 가능하도록 변경되었다. 이것으로 명령어
디코딩 회로가 간략화 되면서 회로 코스트와 전력소모가 동시에 감소하였다. 또한 Thumb명령어는 16비트 길이를 가지고 있으므로 코드밀도
면에서 8비트급 MCU와 비교해도 크게 떨어지지 않는다`[1]`.  
\- 파이프라인 단수가 3단`[2]`으로 조정되었으며 이는 ARM7TDMI와 비교했을 동일한 수준이다.  
\- Thumb-2를 도입하면서 ARM7TDMI 대비 예외처리 특성이 향상되었다. ARM7TDMI 시절에는 예외 상황이 Thumb모드에서
직접 처리되지 않고 ARM모드로 전환해야만 했지만 Thumb-2에서는 Thumb모드에서 예외 처리가 가능하게 되었다. 사실 이 특징으로 인해
Cortex-M계열이 Thumb 명령어만 사용 가능한 제품군으로 분리하는 게 가능해진 것.  
\- NVIC 인터럽트 구조 채택과 위의 Thumb-2의 예외처리 성능 개선을 통해 인터럽트 레이턴시를 Cortex-M3 기준으로
ARM7TDMI의 24~42사이클에서 12사이클로 크게 줄였다. 인터럽트 특성은 [MCU](MCU.md) 시장에서는 매우 중요한
스펙으로 기능 구현과 시스템 안정성 관련 처리 등에 직접 연관되는 내용이다.  
\- 메모리 공간을 8단계까지 분할 관리할 수 있는 MPU(Memory Protection Unit)를 옵션으로 추가할 수 있게
되었다`[3]`.  

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20Cortex-M%20%EC%8B%9C%EB%A6%AC
%EC%A6%88?action=edit&section=4)]

## 4. 종류 ¶

![http://www.arm.com/ja/images/roadmap/Cortex-
M_Roadmap.gif](http://www.arm.com/ja/images/roadmap/Cortex-M_Roadmap.gif)

[[GIF external image]](http://www.arm.com/ja/images/roadmap/Cortex-
M_Roadmap.gif)

  

Cortex-M1은 FPGA전용, M4는 DSC를 위한 특수목적용의 성격이 강하다는 점을 고려하면 실질적인 시장 주력은 M0/0+와
M3이다.

  

  * Cortex-M0  
2009년에 도입 되었으며 3단 파이프라인이 적용 되었고 사용된 게이트(트랜지스터) 수가 가장 적을 경우 12000개 이하, 평균으로 잡아도
25,000개 정도이다`[4]`. 이 정도의 게이트 숫자는 초 i80386의 275,000개의 1/10에 불과한 정도로 웬만한 8비트급
MCU와도 경쟁이 될 정도이며 실제로도 8비트 MCU시장을 잡아먹는 데 1등공신 역할을 하고 있는 중 `[5]`. Thumb/Thumb-2
명령어셋을 지원하지만 Thumb중 나눗셈 관련 명령이 제외되었고 Thumb-2 명령어는 일부만을 지원한다. 클럭당 실행 속도는
0.84DMIPS/MHz`[6]`.  

  * Cortex-M0+  
2012년에 처음 소개된 Cortex-M0의 개선판 제품. 파이프라인 단수가 2단으로 줄었으며 클럭당 실행속도는 0.93DMIPS/MHz로
증가. M0과는 다르게 MPU(Memory Protection Unit)을 옵션으로 추가할 수 있다.  

  * Cortex-M1  
FPGA 전용 라인업으로 대체적인 스펙은 M0과 유사하다.  

  * Cortex-M3  
2004년 Cortex-M 라인업의 첫번째 타자로 출시되었으며 Cortex 제품군의 첫번째 타자이기도 하다`[7]`. 게이트 수는
60,000개
정도로[#](http://pc.watch.impress.co.jp/img/pcw/docs/651/424/html/f11.png.html)
Cortex-M0 대비 2.5~5배 수준. 출시 시기나 성능상으로 ARM7TDMI의 후속 제품이며 3단 파이프라인과 투기적 분기예측,
풀-스펙의 Thumb/Thumb-2를 지원한다. 하드웨어 곱셈기와 나눗셈기가 포함되어 있으며`[8]`. 연산 성능은 ARM7TDMI의
0.95DMIPS/MHz 대비 1.25DMIPS/MHz로 30% 증가하였고 옵션으로 MPU를 포함시킬 수 있다.  

  * Cortex-M4  
M3에서 MDSP확장 명령어와 유닛, 단정도 실수연산용 FPU를 추가하여 DSC(Digital Signal
Controller)`[9]`용으로 특화한 제품. 2010년 출시되었다.  

[[edit](http://rigvedawiki.net/r1/wiki.php/ARM%20Cortex-M%20%EC%8B%9C%EB%A6%AC
%EC%A6%88?action=edit&section=5)]

## 5. 뒷이야기 ¶

Cortex-M3의 등장에 의해 ARM사는 기존의 ARM7TDMI를 투입했던 고급형 32비트 MCU시장에서의 우위를 수성할 수 있었을 뿐
아니라 이후 Cortex-M0을 출시하여 기존 8비트 MCU에 의존하는 고객들도 32비트 MCU 시장으로 끌어오는 데 성공하게 되었다. 업계
상황을 보면 기존 ARM7TDMI가 들어간 컨트롤러 제품군들은 대체로 M3으로의 이전이 활발하게 진행되고 있고
[8051](8051.md)같은 8비트급 코어가 포함된 제품들은 M0/M0+로 이전중. 대표적으로
[아두이노](%EC%95%84%EB%91%90%EC%9D%B4%EB%85%B8.md)의 2014년 6월 최신작 아두이노 제로가
Atmel사의 8비트 AVR 컨트롤러에서 Cortex-M0+가 내장된 동사의 SAMD21계열 컨트롤러로 갈아탔다.  
다만 16비트급 MCU시장의 경우 ARM과 같은 타사 아키텍처 IP를 구매하는 경우 보다는 자사 내부 아키텍처를 기반으로 제품화 하는 경우가
많아 상대적으로 큰 변동은 없는 편이다.  

`\----`

  * `[1]` 8비트급 MCU도 명령어 길이는 대체로 16비트 수준이다. 8051계열이 1~3바이트 가변길이 명령어로 평균 16bit정도, AVR이나 PIC도 비슷한 수준
  * `[2]` Cortex-M0+는 2단
  * `[3]` 통상적으로 MPU를 이용하면 특정 태스크에서 오버플로우나 메모리 오버런이 발생할 경우 그 영향으로 다른 태스크가 망가지는 것을 막을 수 있어서 런타임 안정성을 높일 수 있게 된다.
  * `[4]` 게이트 갯수가 차이나는 이유는 옵션 선택에 따라 곱셈기 등이 추가될 수 있기 때문이다.
  * `[5]` M0이 출시된 시점을 전후하여 32비트MCU 중에서도 1달러 이하 제품이 등장하기 시작했고 세계 MCU시장 매출 1위가 8비트 MCU에서 32비트 MCU로 역전되었다.
  * `[6]` 이 수치 역시 옵션에 따라 달라진다.
  * `[7]` Cortex-A8은 2005년도에 출시되었다
  * `[8]` MCU 분야에서 하드웨어 나눗셈기가 들어간 칩은 상당히 고급으로 취급된다. 이는 하드웨어 나눗셈기의 설계가 매우 복잡하기 때문.
  * `[9]` DSC의 경우 필터 다이나믹스를 모사하기 위해서 32비트 정수 혹은 단정도 실수를 사용하여 대량의 행렬 연산이 필요한 경우가 많다. 이러한 연산 부하에 대응하기 위해 연산유닛을 특화하거나 아니면 전용 DSP를 추가하기도 한다.

