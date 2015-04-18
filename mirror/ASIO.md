## Contents

    

1. 소개 
2. Low Latency 
3. ASIO 2.0 
4. ASIO 2.1 
5. [Windows](Windows.md) 이외의 다른 [운영체제](%EC%9A%B4%EC%98%81%EC%B2%B4%EC%A0%9C.md)와 비교 
6. [Windows](Windows.md) 기반 [PC-FI](PC-FI.md)와 ASIO의 관계 
7. 관련 링크 

[[edit](http://rigvedawiki.net/r1/wiki.php/ASIO?action=edit&section=1)]

## 1. 소개 ¶

  

<del>[ASIO를 ASIO?](%EC%96%B8%EC%96%B4%EC%9C%A0%ED%9D%AC.md)</del>

  

ASIO는 [Cubase](Cubase.md)를 만든 Steinberg에서 제정한 디지털 오디오 입출력에 대한
[API](API.md) 표준이다. 응용 프로그램과 컴퓨터 [사운드카드](%EC%82%AC%EC%9A%B4%EB%93%9C%20%EC%B9%B4%EB%93%9C.md) 사이에 적용되어 낮은
지연`[1]`과 고품질 디지털 오디오 신호 인터페이스를 제공하는 것을 목적으로 하며, [Windows](Windows.md)에서
사용된다.

  

[DirectSound](DirectX.md)는 보통 게임을 즐기는 일반적인 사용자를 위해 사용된다면, ASIO는 주로 전문 음악인과
사운드/레코딩 엔지니어를 위해 사용된다. 다채널로, 다입력, 다출력, 여러 프로그램에서 동시에 접근 등을 염두에 두고 설계되었기 때문이다.

  

현재 출시되는 오디오 인터페이스와 고급 [사운드카드](%EC%82%AC%EC%9A%B4%EB%93%9C%20%EC%B9%B4%EB%93%9C.md)가 이를 지원하고 있다.

  

**오디오 인터페이스**는 전문적인 오디오 녹음과 재생에 특화된 장치이며, 일반 [사운드 카드](%EC%82%AC%EC%9A%B4%EB%93%9C%20%EC%B9%B4%EB%93%9C.md)보다 훨씬 고급 부품과 회로가 사용되고, 실제 스튜디오에서 사용하는 마이크, 여러 전기 신호 크기가 다른 악기, [믹서](%EB%AF%B9%EC%84%9C.md)와 ADAT 등으로 프로용 광단자 입출력 디지털 오디오 장비를 연결할 수 있게 된 것들이 대다수이다. 즉, 비싸다. 

  

하지만 이 역시 입문자를 위해서 간단하게 최소한의 ASIO 입출력만 가능하도록 제작된 오디오 인터페이스도 많이 있다. 기타나 베이스를
연결하거나 콘덴서 마이크를 연결하여 사용하여 녹음을 할 것이 아닌, [소프트웨어 신디사이저](%EC%86%8C%ED%94%84%ED%8A%B8%EC%9B%A8%EC%96%B4%20%EC%8B%A0%EB%94%94%EC%82%AC%EC%9D%B4%EC%A0%80.md)와
일반적인 오디오 신호 녹음, 재생 전용으로 10 ~ 20만원 사이에서 싼 제품을 구입할 수 있다.

  

이것도 구입하기가 어렵다면, [ASIO4ALL](http://www.asio4all.com/), 또는
[ASIO2KS](http://www.asio2ks.de/) 같은 가상 ASIO 지원 드라이버를 설치하면 된다. 단, 500ms 보다
지연시간이 줄기는 하지만, 연주를 해보면 느껴질 정도의 지연은 여전히 존재한다.

  
  

[[edit](http://rigvedawiki.net/r1/wiki.php/ASIO?action=edit&section=2)]

## 2. Low Latency ¶

Latency 라는 단어 자체는 무언가 숨겨져 있거나 잠복되어 있어서 보이지 않는 것을 뜻한다. 그러나 디지털 오디오에서는 "드러나지 않은,
숨어있는 요소 때문에 발생하는 지연 또는 지연되는 시간"을 뜻한다.

  

[DAW](DAW.md)와 [소프트웨어 신디사이저](%EC%86%8C%ED%94%84%ED%8A%B8%EC%9B%A8%EC%96%B4%20%EC%8B%A0%EB%94%94%EC%82%AC%EC%9D%B4%EC%A0%80.md) 등장 초기인 1990년대 중후반부터
[Windows](Windows.md) 환경에서 실시간 오디오 입출력을 하는 것이 이전 대비 대단히 중요해졌다. 그러나 아무리 해도
해결을 할 수 없는 근본적인 문제가 [Windows](Windows.md)에 숨어있었다.

  

일반적인 Windows 2000 이후 버젼의 Windows에서 프로그램이 오디오 데이터를 출력하면 대략 아래 그림의 오른쪽과 같은 과정을
거치게 된다.

  
  

![windows_xp_audio.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/ASIO/wind
ows_xp_audio.jpg)

[JPG image (30.29 KB)]

  

위 그림의 오른쪽을 보면, 잘 모르겠어도 뭔가 엄청나게 복잡하지 않은가? 하드웨어를 추상화하고, 볼륨을 조절하는 믹서를 이렇게 위치시키면
운영체제를 만드는 입장에서는 좋을 것 같기도 하다. 그러나 거쳐야 하는 계층이 많다는 것은 그만큼 시간을 많이 잡아먹는다는 것을 뜻한다.
특히 이 중에 KMixer가 자동으로 Sampling Rate를 변환하면서 시간을 잡아먹는 것으로 악명이 높았다. KMixer를 거치면
Latency가 200 ~ 500 ms, DirectSound를 통해 거치지 않아도 50 ~ 100 ms 수준의 Latency가 발생했다.
<del>아니, 느리기까지 한데 원래 프로그램이 출력한 오디오 데이터가 지 마음대로 변환까지 되면서 출력된다고?!?!?</del>

  

그래서 위 그림의 왼쪽처럼 KMixer를 확실하게 우회하고, 중간에 있는 다른 계층을 없애버려서 응용 프로그램이 하드웨어인 [사운드카드](%EC%82%AC%EC%9A%B4%EB%93%9C%20%EC%B9%B4%EB%93%9C.md)에 디지털 오디오 신호를 이전대비
훨씬 적은 계층을 통해서 전달할 수 있는 방법에 대한 고민이 시작되었고, 회사별로 여러 가지 방식이 우후죽순처럼 쏟아져 나왔다. 이들 중
최종적으로 남은 것이 바로 Steinberg의 ASIO(Audio Streaming Input/Output) 이며, 위 그림의 왼쪽과 같이
경로가 단축되면서 문제의 핵심이던 KMixer를 우회하게 되었다.

  

ASIO가 있는 쪽에 OpenAL 이라는 다른 것을 볼 수 있는데, 이것은 ASIO가 사실상 업계 표준이지만 Steinberg에 귀속되어
있는 기술이기 때문에 [오픈소스](%EC%98%A4%ED%94%88%EC%86%8C%EC%8A%A4.md) 진영에서 제정한 Open
Audio Library라는 같은 역할을 하는 또 다른 표준이다. 관심있는
[위키러](%EC%9C%84%ED%82%A4%EB%9F%AC.md)는 이
[링크](http://connect.creativelabs.com/openal/default.aspx)를 참조하라.

  

당연히 ASIO는 빠르게 시장에 퍼져나가서 사실상의 표준이 되었다. 이후에 [DirectX](DirectX.md)에도 KMixer를
우회하여 오디오 데이터를 출력할 수 있는 API가 추가되었다. (위 그림에서 DirectSound가 KMixer를 거치지 않고 우회하는 것이
바로 이것이다.) <del>그러나 세상은 이미 ASIO 가 접수했지.</del>

  

ASIO를 사용하면 보통 3 ~ 5 ms 정도의 Latency를 만들 수 있으며, 극단적으로 좋은 상황에서는 1 ms 이하의 Latency도
드물게 실현 가능하다.

  
  

![audio_vista_whitepaper_im2.JPG](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds
/ASIO/audio_vista_whitepaper_im2.JPG)

[JPG image (23.66 KB)]

  

[Windows Vista](Windows%20Vista.md) 부터 [Microsoft](Microsoft.md)는
WASAPI와, 이것과 같은 목적에 보다 추상화된 WaveRT [API](API.md)를 만들고, 디지털 오디오 출력 부분을 위와 같이
개선하였다.

  

CPT는 Cross Process Transport로, 디지털 오디오 데이터를 Windows Audio Service 로 전달하는 역할을
한다.  
APO는 Audio Processing Object로, 디지털 오디오 데이터를 처리하기 위한 일종의 [DSP](DSP.md) 기능을
한다.  
KST는 Kernel Streaming Transport로, 디지털 오디오 데이터를 현재 실행중인 컴퓨터에 장착된 오디오 장치에게 전달하기
위해 렌더링을 한다. <del>어? 어?!</del>

  

실제 테스트를 해본 사람들에 의하면, 24 bit로 출력을 하면 Sampling Rate 변환이 일어나지 않지만, 그렇지 않은 경우는 변환이
일어난다고 한다. 그런데 전문 오디오 편집 또는 [DAW](DAW.md) 프로그램이면 모를까, 어떤 프로그램이 24 bit 출력을
지원할까?`[2]`

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ASIO?action=edit&section=3)]

## 3. ASIO 2.0 ¶

  

이전대비 몇 가지 차이점이 있지만, 사용자한테 가장 크게 부각되는 차이점은 오디오 입력을 컴퓨터를 거치지 않고 그대로 출력하는 모니터링
기능이 추가되었다는 점이다. 현재 판매되고 있는 ASIO를 지원하는 [사운드카드](%EC%82%AC%EC%9A%B4%EB%93%9C%20%EC%B9%B4%EB%93%9C.md)와 오디오 인터페이스는 대부분
이것을 지원한다.

  
  

[[edit](http://rigvedawiki.net/r1/wiki.php/ASIO?action=edit&section=4)]

## 4. ASIO 2.1 ¶

  

[소니](%EC%86%8C%EB%8B%88.md)에서 만든 새로운 디지털 오디오 방식인 DSD(Direct Stream
Digital)을 지원한다. 이것을 제외하면 ASIO 2.0 과 차이가 없다.

  
  

[[edit](http://rigvedawiki.net/r1/wiki.php/ASIO?action=edit&section=5)]

## 5. [Windows](Windows.md) 이외의 다른
[운영체제](%EC%9A%B4%EC%98%81%EC%B2%B4%EC%A0%9C.md)와 비교 ¶

  

과거 [Mac OS](Mac%20OS.md)에는 Sound Manager라는 것이 있었는데 이것 덕에 50 ms 정도의 Latency가
발생했다. 그러나 [Mac OS X](Mac%20OS%20X.md)의 Core Audio`[3]`에는 [그런 거없다](%EA%B7%B8%EB%9F%B0%20%EA%B1%B0%20%EC%97%86%EB%8B%A4.md). 애초부터 노리고
Latency를 최소화하도록 설계되었기 때문이다.<del>근데 [Mac OS](Mac%20OS.md)라 해도 윈도우보다 적어도 2배는
나았네?</del>

  

[Linux](Linux.md)는 노리지는 않았지만 커널 모듈 상에서 별다른 문제가 발생하지 않고 있다. 다만 일부 Studio 에디션
등은 커널 단 스케쥴러를 사용하지 않고 스트림으로 처리하는 Linux RT`[4]`를 사용해 일반적으로 10ms~20ms대의 레이턴시를
가졌지만 RT 커널에선 1ms 이하의 레이턴시를 보이고있다. 다만 어플리케이션과 커널 드라이버 (Jack, OSS, ALSA,
Pulseaudio 등)와 버퍼 샘플을 얼마나 줄지에 따라 최종 레이턴시는 달라진다.

  
  

[[edit](http://rigvedawiki.net/r1/wiki.php/ASIO?action=edit&section=6)]

## 6. [Windows](Windows.md) 기반 [PC-FI](PC-FI.md)와 ASIO의 관계 ¶

  

원 소스의 디지털 신호가 변환되지 않고, 즉 프로그램이 출력한 오디오 데이터를 그대로, 오디오 출력 하드웨어까지 전달되는 것을 Bit
Perfect 라고 한다. 그런데 위에서 살펴본 것처럼 Windows에서는 아직까지 특정 조건을 만족하지 못하면 디지털 오디오 신호의 왜곡을
피할 수 없다. 즉 사실상 Bit Perfect 가 아니다. (물론 특정 조건을 만족시키면 Bit Perfect가 되기는 하지만, 사실상
Windows가 기본으로 제공하는 환경에서는 이 조건을 충족하기가 어려운 것이 현실이다.)

  

그러므로 제 아무리 CD에서 직접 추출한 WAV 파일 또는 FLAC 파일이라도, 최종 출력 기기인 [사운드카드](%EC%82%AC%EC%9A%B4%EB%93%9C%20%EC%B9%B4%EB%93%9C.md) 또는 오디오 인터페이스에 전달되는
데이터는 운영체제에 의해 바뀌게 된다!!

  

이 문제를 해결하기 위해서는 [Foobar2000](Foobar2000.md)등의 ASIO 출력을 지원하며 사용자가 세세한 설정을 바꿀
수 있는 재생 소프트웨어를 사용하거나, 아니면 [매킨토시](%EB%A7%A4%ED%82%A8%ED%86%A0%EC%8B%9C.md)나
[Linux](Linux.md)로 갈아타야 한다.

  

보통은 체감하기 상당히 어려운 부분`[5]`이기 때문에 다 무시하고 그냥 사용해도 별 문제는 없다. 컴퓨터를 살 때 덤으로 받은 중저가형
컴퓨터용 스피커 정도로는 티도 안난다. 게다가 손실압축 방식인 [MP3](MP3.md)가 디지털 음원 유통의 주류로 자리매김한 현실을
생각해보라.

  

물론 [HI-FI](HI-FI.md)와 [PC-FI](PC-FI.md)등에 관심이 많고 보유중인 각종 음향기기의 성능이 괜찮다면
시도해 보는 것 자체는 나쁘지는 않으나, 어차피 이렇게 해 봐야 수 백, 수 천 만원을 넘어가는 앰프와 스피커조차 전기적, 물리적 한계를
최종적으로 극복하지 못하는 경우가 대부분이기 때문에 얼마나 의의와 체감효과가 있을지는 잘 모르겠다. 그러나 방송 음향계, 영화 음향계
종사자, 음반 제작자, 음원 제작자 등 음향과 음악을 생산하는 사람들한테는 중요한 문제일 수 있다.<del>그러나 차이를 느꼈다는 사람도 꽤
있다니까 뭐</del>`[6]`

  
  

[[edit](http://rigvedawiki.net/r1/wiki.php/ASIO?action=edit&section=7)]

## 7. 관련 링크 ¶

  

  * [소프트웨어 신디사이저](%EC%86%8C%ED%94%84%ED%8A%B8%EC%9B%A8%EC%96%B4%20%EC%8B%A0%EB%94%94%EC%82%AC%EC%9D%B4%EC%A0%80.md)
  * [DAW](DAW.md)
  * [VST](VST.md)

`\----`

  * `[1]` Low Latency
  * `[2]` 최근에는 기본값이 16비트여서 그렇지 내장 사운드 칩셋도 24비트 출력을 지원한다.
  * `[3]` [OpenAL](OpenAL.md) 기반이다.
  * `[4]` 윈도 RT 같은 ARM 용 말고 Real Time 의 약자
  * `[5]` 인터넷상에 음색과 음질의 우열을 논하는 글이 많은데, 오디오 신호가 믹서 등을 거치면서 왜곡이 생긴다 하더라도 그냥 들어서는 구분이 어려운 수준이다. 애초에 [ASIO](ASIO.md)와 이와 동종인 기술이 등장한 목적은 [DAW](DAW.md)와 실시간 음 합성에 장애가 되는, 재생을 지연시키는 숨어있는 지연 요소, 즉 레이턴시를 제거하기 위한 것이었다. 구현을 하다 보니 Windows 내부의 KMixer를 우회하여 Bit Perfect가 되었을 뿐, KMixer를 거치지 않는다고 해도 결국 하드웨어 수준에서 사운드 카드와 오디오 인터페이스가 재생 가능한 주파수로 변환되어야 출력이 가능하기 때문에, 음질 향상에 미치는 영향은 그리 크지 않다. 다만, 이런 식으로 윈도우 믹서를 우회하여 스피커를 독차지하는 방식을 사용하면 음악 재생시 다른 프로그램의 소리 및 윈도우 효과음이 들리지 않는 효과가 있는데, 이는 단점이 될 수도 있지만 사람에 따라서는 선호할 수도 있다.
  * `[6]` 번들 스피커를 벗어나면 중요해질수 있다.KMixer를 지나면서 잡음이 섞인다는 주장도 있고,실제로WASAPI(Exclusive)나 ASIO를 적용해보면 음이 좀 더 또렷해지는 결과를 얻을수 있다는 주장도 있다.앰프와 스피커들이 한계가 있어서 그런걸 못느낀다고 해도,KMixer에서의 음질열화를 막는 것으로도 충분한 가치가 있다는 주장이다.물론 스피커가 흔한 저가형/번들이라면 <del>어차피 잡음부터 표현을 못할테니</del> 그런거 없겠지만 스피커가 어느정도 좋다면 적용해보는것도 나쁘지 않다.시스템에 문제를 일으킬 위험이 있거나 하지는 않으니까.

