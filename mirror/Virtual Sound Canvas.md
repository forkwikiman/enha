## Contents

    

1. 개요 
2. 활용 

[[edit](http://rigvedawiki.net/r1/wiki.php/Virtual%20Sound%20Canvas?action=edi
t&section=1)]

## 1. 개요 ¶

Virtual [SoundCanvas](%EC%82%AC%EC%9A%B4%EB%93%9C%20%EC%BA%94%EB%B2%84%EC%8A%A4.md).

  

[롤랜드](%EB%A1%A4%EB%9E%9C%EB%93%9C.md)에서 제작한 가상악기: 소프트웨어
[신디사이저](%EC%8B%A0%EB%94%94%EC%82%AC%EC%9D%B4%EC%A0%80.md).  
초기에는 Roland 에서 출시되는 Virtual Sound Canvas 였으나, 나중에 EDiROL`[1]` Hyper Canvas 로
브랜드와 이름이 바뀌었다. 최신 버전인 1.6은 윈도우 8도 정상적으로 지원한다.

  

[MIDI](MIDI.md)에 대해 조금 아는 이들의 대부분은 이것 혹은 [YAMAHA](YAMAHA.md)의 S-YXG50을
애용한다. [윈도우 XP](%EC%9C%88%EB%8F%84%EC%9A%B0%20XP.md) 내장 소프트웨어 신디사이저`[2]`로
[MIDI](MIDI.md) 음악을 듣던 이들이 감격의 눈물을 흘리게 되는 소프트웨어 신디사이저/가상악기.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Virtual%20Sound%20Canvas?action=edi
t&section=2)]

## 2. 활용 ¶

기본적으로 고급 오디오 인터페이스를 갖추고 있는 사용자라면, 이미 훌륭한 가상악기가 넘치게 설치되어 있기 마련이고, 가상악기가 없어도
대중적인 OS [윈도우 XP](%EC%9C%88%EB%8F%84%EC%9A%B0%20XP.md) 유저라면 그 안에 소프트웨어
신디사이저가 들어있는데도 불구하고 이것을 사용하는 이유가 있다.

  

**그 [윈도우 XP](%EC%9C%88%EB%8F%84%EC%9A%B0%20XP.md) 내장 소프트웨어 [신디사이저](%EC%8B%A0%EB%94%94%EC%82%AC%EC%9D%B4%EC%A0%80.md)가 심히 [골룸](%EA%B3%A8%EB%A3%B8.md)하기 때문이다.** 윈도우 XP를 쓰면서 에뮬레이터로 [N64](N64.md)용 [젤다의 전설](%EC%A0%A4%EB%8B%A4%EC%9D%98%20%EC%A0%84%EC%84%A4.md)을 돌려봤다면 들어보았을 그 소리다. 추억의 소리일지는 모르겠지만, Virtual Sound Canvas 등과 비교해보면 음질은 단연 최악이고, [VST](VST.md)나 DXi가 아닌 WDM`[3]`으로 되어있어서 가상악기로 쓰기에도 지연(latency)이 너무 심해(무려 0.5초다. 실시간 연주 및 협연이 절대 불가능.) 실용성도 떨어져 [MIDI](MIDI.md), [DAW](DAW.md) 음악가라면 봉인해야 할 물건이다.`[4]`

  

윈도우 XP 내장 소프트웨어 신디사이저가 Roland로부터 음원 데이터를 라이센스 받아서 만들어졌다고 해도 구동부까지 완벽하게 같지는 않다.
Virtual Sound Canvas 쪽이 윈도우 소리가 리얼하고 훨씬 매력적이다. 물론 고품질 가상악기나 하드웨어
[신디사이저](%EC%8B%A0%EB%94%94%EC%82%AC%EC%9D%B4%EC%A0%80.md)보다는 못하지만, XP 내장
소프트웨어 신디사이저를 어설프게 조정하거나 연주하느니 이것이 더 나을 수 있다.

  

사용하는 이들은 주로 에뮬레이터로 옛 게임이나 [RPG만들기](RPG%20%EB%A7%8C%EB%93%A4%EA%B8%B0%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md) 등의
[MIDI](MIDI.md) 음원을 사용하는 게임을 플레이할 때, *.mid 파일을 감상할 때, [NoteWorthyComposer](NoteWorthy%20Composer.md)만으로 곡을 만들거나, 혹은 부분적으로 소프트웨서 신디사이저를 사용하려는
이들이다.

  

비슷한 종류로 [
VirtualMIDISynth](http://coolsoft.altervista.org/en/virtualmidisynth)라는 것이 있다.
이쪽은 사운드 폰트를 자유롭게 다운받아서 적용할 수 있다는 특징이 있다.

`\----`

  * `[1]` Roland의 하위 브랜드이다.
  * `[2]` [Microsoft](Microsoft.md)가 1996년에 Roland에서 음원데이터를 라이센스 받아서 제작되었다.
  * `[3]` Windows Driver Model. 즉 일반 장치 드라이버이다. 당연히 ASIO 수준의 Low Latency는 기대할 수 없다.
  * `[4]` 웃기는 것은, [Apple](%EC%95%A0%ED%94%8C%28%EA%B8%B0%EC%97%85%29.md)도 Roland로부터 1997년에 라이센스를 받아서 [QuickTime](%ED%80%B5%ED%83%80%EC%9E%84%20%ED%94%8C%EB%A0%88%EC%9D%B4%EC%96%B4.md) 3.0 버젼부터 이를 적용하기 시작했으며, [Mac OS X](Mac%20OS%20X.md)에는 기본 내장 소프트웨어 [신디사이저](%EC%8B%A0%EB%94%94%EC%82%AC%EC%9D%B4%EC%A0%80.md) 형태로 탑재되어 있다. 그런데 이것은 Audio Unit(Mac OS X용 오디오 플러그인 시스템)으로 되어있어서 [윈도우 XP](%EC%9C%88%EB%8F%84%EC%9A%B0%20XP.md) 내장 소프트웨어 신디사이저와 달리 지연이 없다. 그래서 멀쩡하게 GarageBand, [Logic](Logic.md), [Cubase](Cubase.md) 등에서 이것을 실제로 쓰는 사람도 많다.

