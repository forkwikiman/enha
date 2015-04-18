[영어](%EC%98%81%EC%96%B4.md): Long Range Navigation  
주로 음역해서 로란으로 부른다.

## Contents

    

1. 개요 
2. 어떻게 돌아가나 
3. 시스템 구성 
    

3.1. 제어 시스템

3.2. 증폭 시스템

3.3. 출력 시스템

4. 한국 체인 소속 

[[edit](http://rigvedawiki.net/r1/wiki.php/LORAN?action=edit&section=1)]

## 1. 개요 ¶

바다에 다니는 사람들이 중요하게 여기는 것으로, 현재 [GPS](GPS.md)와
[글로나스](%EA%B8%80%EB%A1%9C%EB%82%98%EC%8A%A4.md)를 제외하면 유일하게 대체 가능한 범지구적 측위
시스템이다. 다른 지상파 쌍곡선 측위 시스템은 20세기 말에 전부 멸종(...)했기 때문에... 현재 사용하는 LORAN 은 LORAN -
C 로서, 100Khz 를 사용하는 시스템에 대해 언급한다. 구소련의
[차이카](%EC%B0%A8%EC%9D%B4%EC%B9%B4.md)도 100kHz를 사용했고, 후일 로란과 묶여 LORAN -
C/CHAYKA로 부르기도 한다. 뭐 나중에 기술이 진보하면 eLORAN 이 예정되어 있는데 그때가면 문서가 바뀔테니까, 지금은 이것으로도
충분할 것이다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/LORAN?action=edit&section=2)]

## 2. 어떻게 돌아가나 ¶

LORAN-C 는 예전 GNSS 시스템이 사용하는 쌍곡선 시간차 측위를 사용하여 현재 위치를 추정한다. 쌍곡선 시간차 측위란, 두 개의
동기화된 쌍곡선의 포락선과, 그것에 딸려오는 리딩 엣지(leading Edge) 를 역계산하여 2차원
[좌표](%EC%A2%8C%ED%91%9C.md)를 추정해 내는 것이다. LORAN-C 는 각 무선국이 chain 이라는 형식으로
동기화 되며, 전파의 속도는 이론상 불변이므로 이를 사용하여 2개의 LOP 를 형성하면 계산 완료.

  

LORAN-C 역시 [첨두파](%EC%B2%A8%EB%91%90%ED%8C%8C.md) 형태의 파형을 가지는데, 다른 시스템과 달리
유연한 곡선을 따라 급격하게 증가했다가 다시 낮아지는 형태의 100khz 파형을 발생한다.

  

![http://loran9930.go.kr/tech/images/a_index03_img01.gif](http://loran9930.go.
kr/tech/images/a_index03_img01.gif)

[[GIF external image]](http://loran9930.go.kr/tech/images/a_index03_img01.gif)

  

이는 후속 파형은 교란을 받기 쉽기 때문에`[1]` 초기 6사이클 이내에 99% 의 전파출력을 담기 위해서이다. 참고로, LORAN-C 의
송신기 출력은 수백 kW 에 달한다.

  

앞서 말했듯이, LORAN 송신기는 chain 이라는 형태로 묶여 운용되는데, 이 때에 주국이 마스터 시그널을 날리는 시점과 다음 마스터
까지의 시간을 Group Repetition Interval, GRI 라고 부르며, 이 시간동안 chain 내 주국과 종국이 동기화된 시간
동안 특정 펄스주기를 가지고 운용되게 된다. 한국에 있는 LORAN-C는 99,300㎲ 의 주기를 가지므로 GRI9930 이라고 불리며,
이를 엮은 체인을 GRI9930chain 으로 부른다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/LORAN?action=edit&section=3)]

## 3. 시스템 구성 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/LORAN?action=edit&section=4)]

### 3.1. 제어 시스템 ¶

  

① TOPCO(Transmitter Operational Control)  
② PATCO(Pulse Amplitude and Timing Controller)  
③ RCU(Remote Control Unit)  
④ LTU(Loran Timer Unit)  
⑤ 세슘원자시계

  

[[edit](http://rigvedawiki.net/r1/wiki.php/LORAN?action=edit&section=5)]

### 3.2. 증폭 시스템 ¶

① Pules Generator Assembly  
② Half Cycle Generator

  

[[edit](http://rigvedawiki.net/r1/wiki.php/LORAN?action=edit&section=6)]

### 3.3. 출력 시스템 ¶

① Coupling Network  
② Switching Network

  

그리고 안테나. 장파를 쓰는 고로 크고 아름답다. 150m 넘으니 꼭 보자. 두번보자.

  
  

[[edit](http://rigvedawiki.net/r1/wiki.php/LORAN?action=edit&section=7)]

## 4. 한국 체인 소속 ¶

[해양수산부 군산지방해양항만청 위성항법중앙사무소 홈페이지](http://www.ndgps.go.kr/html/kr/index.html)

  

한국 체인은 GRI9930 이며, 각 국은 다음과 같다.

  

MASTER : Pohang Master 150kw  
SLAVE : Kwangju slave 50kw (w)  

Kesashi slave 1500kw (x)  
Nijima slave 1600kw (y)  
Ussurijsk slve 700kw (z) - Unknown (NOT REGISTERED)  

우리나라 법상 위치는 역시 **나**등급 보안이지만, 실제로는 각 국의 좌표가 정확하게 나온다. 그거 입력해야 계산이 가능하거든…….

  

그리고, 한국체인은 특히 출력 작기로 유명하다. 그것도 주국인 한국이.

`\----`

  * `[1]` 이건 모든 전파 및 음향에서도 똑같다. 초음파 거리계에서도 초기에 도달한 신호는 온전하나 후반부로 갈수록 리버브 등의 공간음에 의해 교란되어 신호가 망가진다.

