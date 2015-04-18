MAX/MSP

## Contents

    

1. 개요 
    

1.1. 역사

2. 주요 Object 
    

2.1. MAX

    

2.1.1. Bang

2.1.2. Toggle

2.1.3. Print

2.1.4. Gate

2.1.5. Metro

2.1.6. Delay, Pipe

2.1.7. zl. (nth, mth...ETC)

2.1.8. 그 외

2.2. MSP

    

2.2.1. DAC~, ADC~

2.2.2. Cycle~

2.2.3. Scope~

2.3. 교육기관

2.4. 참조항목

[[edit](http://rigvedawiki.net/r1/wiki.php/MAX/MSP?action=edit&section=1)]

# 1. 개요 ¶

  

현재 Cycling' 74 에 의해서 판매, 배급되어지고 있는 미디어 아트 프로그램이다. Max 프로그램의 정확한 이름은
Max/MSP/Jitter이다. 하지만 지금까지 용도에 따라 주로 음악적인 용도로 사용되었던 Max/MSP와 영상 처리를 위한 Jitter를
따로 구분해서 불러왔다.

  

국내에서는 많이 생소한 분야인 [전자음악](%EC%A0%84%EC%9E%90%EC%9D%8C%EC%95%85.md) 등의 순수예술
분야에서 널리 활용되고 있는 오픈 소스 프로그래밍 툴이며, 다양한 활용 범위로 인해 미술쪽의 인터랙티브 아티스트들도 사용하고 있다. [이런
거라든가.](http://kikibossa.tistory.com/218) 주로 영화음악이나 영상음악에서 활용도가 높으며, 광고음악에도 종종
응용되어진다. <del>가끔 이 프로그램의 그래픽적인 부분을 이용해
[게임](http://blog.naver.com/scolonleader/50143955291) 같은 것을 만드는 괴물들도 있다.</del>
MSP부분만 잘 공부하면 신디사이저도 손쉽게 만들 수 있을 정도로, 쓰다 보면 정말 활용도가 높은 프로그램.

  

Max라는 명칭은 컴퓨터 음악과 디지털 신호 처리에 있어서 중요한 공헌을 한 Max V. Mathews에게서 유래하였고, 오늘날 우리가 보는
것과 같은 Max는 1989년부터 개발에 참가한 David Zicarelli에 의해 실현되었다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/MAX/MSP?action=edit&section=2)]

## 1.1. 역사 ¶

  

출처 : <http://makeprocessing.com/maxmsp_01/3020>

  

1986년에 프랑스의 IRCAM(Institte de Recherche et Coordination Acoustique/Musicue의
약칭으로 파리의 퐁피두 센터에 인접해 있는 국립 음향 음악 연구소)에서 Miller Puckette를 중심으로 Max의 개발이 시작되었다.
당시 Max는 거대한 4X 신디사이저를 제어하기 위하여 만든 일종의 음악용 프로그래밍 환경으로 개발되었다. Max는 미디(MIDI) 기능을
중심으로 오브젝트와 패치 코드라는 그래픽적인 프로그래밍 스타일을 갖춘 매킨토시용 애플리케이션으로써 완성되었고, 1990년에
Intelligent Music사로부터 시판 패키지로 배포되어 다음해인 1991년에 Opcode사에서 발매되었다.

  

Max는 1995년에 멀티미디어 기능을 대폭 확장하여 Max 3.0으로 버전 업 되었고, 1996년 12월에는 파워PC에 대응한 Max
3.5가 발표되어 고속처리를 실현하였다. 1997년 12월, MSP가 Max에 추가되면서 디지털 신호처리(DSP) 기능이 가능해졌고 미디와
외부 음원에 의존하지 않고 컴퓨터 자체가 음향을 직접 생성할 수 있는 환경을 제공하였다. 그 후 Opcode사로부터 Max의 판매권을 얻어서
Cyclyng’74에서 Max를 발매하였다.

  

1999년에 영상 처리 기반의 nato와 2000년에는 영상 처리를 가능하게 해주는 Jitter와 OpenGL 기반의 3D CG 구현
소프트웨어인 GEM for Macintosh가 출시되었다. 2001년 6월에는 Max4.0과 MSP2.0이 발표되었다. Max4.0에서는
많은 윈도우가 Max 자체에 기술되어, 독자의 스크립트 기능을 갖는 등 기본 구조에 있어서 대폭적인 개선이 있었다. 또 레이어 구조와
인스펙터 등의 편집 기능이 향상되었고, 오리지널 유저 인터페이스를 작성하는 기능도 추가되었다. MSP2.0도 기본적인 DSP 기능을
향상시키고, 견고하고 유연한 오디오 입·출력 기능을 갖추게 되었고, Jitter가 플러그인으로 추가되면서 다양한 영상 처리가 가능하게
되었다. 지금은 Max 6이 출시되면서 Max/MSP/Jitter가 Max 6으로 통일되었다.

  

맥 OS와 윈도우 OS를 지원하며, 유투브 등에서 MAX/MSP 등의 검색어를 쓰면 여러 사람들(대부분이 외국 유저)이 프로그래밍 한 패치를
볼 수 있다. 참고하도록 하자.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/MAX/MSP?action=edit&section=3)]

# 2. 주요 Object ¶

  

MAX에서의 Object 는 명령어라고 생각하면 편하다.  
Object 안에 어떠한 명령어를 입력하면, Object 는 그 명령어에 해당하는 기능을 실행한다.  
(가령 Object 안에 Metro 1000 을 입력하면, 1000ms(1초) 에 한 번 씩 Bang 이 나가게 된다.)  
이름이 심히 비범하다…….

  

[[edit](http://rigvedawiki.net/r1/wiki.php/MAX/MSP?action=edit&section=4)]

## 2.1. MAX ¶

  

[[edit](http://rigvedawiki.net/r1/wiki.php/MAX/MSP?action=edit&section=5)]

### 2.1.1. Bang ¶

  

Bang 이란 MAX/MSP 에서 가장 기본 중의 기본이다. 이 걸 모르면 MAX를 건드릴 수도 없다.  
총의 방아쇠라고 생각하면 편하다. 한번 누르면 Bang 과 연결된 오브젝트들이 딱 한 번 작동한다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/MAX/MSP?action=edit&section=6)]

### 2.1.2. Toggle ¶

  

Toggle 의 개념은 스위치라고 생각하면 편하다.  
토글이 작동되면, 토글의 out과 연결된 오브젝트들이 지속적으로 작동하게 된다.  
토글은 숫자 1을 in 에서 받으면 작동하게 되고, 0을 받으면 꺼진다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/MAX/MSP?action=edit&section=7)]

### 2.1.3. Print ¶

  

말 그대로 Print.  
Print Object의 in 으로 받은 메세지 박스의 내용을 MAX창에서 출력해준다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/MAX/MSP?action=edit&section=8)]

### 2.1.4. Gate ¶

  

[[edit](http://rigvedawiki.net/r1/wiki.php/MAX/MSP?action=edit&section=9)]

### 2.1.5. Metro ¶

  

[[edit](http://rigvedawiki.net/r1/wiki.php/MAX/MSP?action=edit&section=10)]

### 2.1.6. Delay, Pipe ¶

  

[[edit](http://rigvedawiki.net/r1/wiki.php/MAX/MSP?action=edit&section=11)]

### 2.1.7. zl. (nth, mth...ETC) ¶

  

[[edit](http://rigvedawiki.net/r1/wiki.php/MAX/MSP?action=edit&section=12)]

### 2.1.8. 그 외 ¶

  

Uzi = uzi 뒤에 쓰여진 숫자만큼 Bang 을 순식간에 내보내준다. 예를 들어 uzi 65535 라고 쓰여있으면, 순식간에
65535개의 Bang 을 내보낸다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/MAX/MSP?action=edit&section=13)]

## 2.2. MSP ¶

  

[[edit](http://rigvedawiki.net/r1/wiki.php/MAX/MSP?action=edit&section=14)]

### 2.2.1. DAC~, ADC~ ¶

  

[[edit](http://rigvedawiki.net/r1/wiki.php/MAX/MSP?action=edit&section=15)]

### 2.2.2. Cycle~ ¶

  

[[edit](http://rigvedawiki.net/r1/wiki.php/MAX/MSP?action=edit&section=16)]

### 2.2.3. Scope~ ¶

  
  

[[edit](http://rigvedawiki.net/r1/wiki.php/MAX/MSP?action=edit&section=17)]

## 2.3. 교육기관 ¶

  

국내에서는 [한예종](%ED%95%9C%EC%98%88%EC%A2%85.md),
[서울대학교](%EC%84%9C%EC%9A%B8%EB%8C%80%ED%95%99%EA%B5%90.md), [추계예술대학교](%EC%B6%94%EA%B3%84%EC%98%88%EC%88%A0%EB%8C%80%ED%95%99%EA%B5%90.md) 등의 현대 음악을 주로
가르치는 작곡과에서 전문적으로 가르치고 있다. 특히나
[서울대학교](%EC%84%9C%EC%9A%B8%EB%8C%80%ED%95%99%EA%B5%90.md)에서 새로
[전자음악](%EC%A0%84%EC%9E%90%EC%9D%8C%EC%95%85.md) 학과를 신설함에 따라, 이 프로그램의 활용 범위나
보급률은 높아질 것이라 생각된다.

  

국내에서는 MAX/MSP 커뮤니티가 있지만 활동이 없다고 보아도 무방한 상태, 매뉴얼 마저도 영어로 되어 있는지라 자신의 독해 실력이
부족하거나 패치에서 알 수 없는 버그가 일어난다면 어떻게 해서든 인터넷을 통해 도움을 얻도록 하자. 사설 교육기관으로는 메이크프로세싱이라는
곳이 있긴 하다.

  
  

[[edit](http://rigvedawiki.net/r1/wiki.php/MAX/MSP?action=edit&section=18)]

## 2.4. 참조항목 ¶

  * [컴퓨터 관련 정보](%EC%BB%B4%ED%93%A8%ED%84%B0%20%EA%B4%80%EB%A0%A8%20%EC%A0%95%EB%B3%B4.md)  

    * [프로그래밍 언어](%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20%EC%96%B8%EC%96%B4.md)  

  * [전자음악](%EC%A0%84%EC%9E%90%EC%9D%8C%EC%95%85.md)
  * [컴퓨터 음악](%EC%BB%B4%ED%93%A8%ED%84%B0%20%EC%9D%8C%EC%95%85.md)  

    * [음악 작곡 프로그램](https://mirror.enha.kr/wiki/%EC%86%8C%ED%94%84%ED%8A%B8%EC%9B%A8%EC%96%B4/%EB%AA%A9%EB%A1%9D#s-14)
    * [신디사이저](%EC%8B%A0%EB%94%94%EC%82%AC%EC%9D%B4%EC%A0%80.md)  

  * [예술 관련 정보](%EC%98%88%EC%88%A0%20%EA%B4%80%EB%A0%A8%20%EC%A0%95%EB%B3%B4.md)
  * [미디어아트](%EB%AF%B8%EB%94%94%EC%96%B4%EC%95%84%ED%8A%B8.md)  

    * [Arduino](Arduino.md)
    * [Processing](Processing.md)
    * [vvvv](vvvv.md)

