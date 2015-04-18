![http://a0.twimg.com/profile_images/600633824/VST_logo.jpg](http://a0.twimg.c
om/profile_images/600633824/VST_logo.jpg)

[[JPG external
image]](http://a0.twimg.com/profile_images/600633824/VST_logo.jpg)

VST; Virtual Studio Technology

## Contents

    

1. 개요 
2. 호환성 
3. 대표적인 VST(i) 
4. 무료 VST(i) 

[[edit](http://rigvedawiki.net/r1/wiki.php/VST?action=edit&section=1)]

## 1. 개요 ¶

  

VST. Virtual Studio Technology 의 약자. 사실상 업계 표준이다.

  

VST/i 는 [큐베이스](%ED%81%90%EB%B2%A0%EC%9D%B4%EC%8A%A4.md),
[누엔도](%EB%88%84%EC%97%94%EB%8F%84.md) 그리고 Wavelab 등의 유명한 DAW 를 개발한 독일의
Steinberg 사에서 개발한 오디오 신호처리 플러그인 [API](API.md) 규격이며, Steinberg에서 저작권을 보유하고
있지만 무료로 사용 가능하다.

  

VST는 소프트웨어 이펙터 역할을 하는 VST 와, [소프트웨어 신디사이저](%EC%86%8C%ED%94%84%ED%8A%B8%EC%9B%A8%EC%96%B4%20%EC%8B%A0%EB%94%94%EC%82%AC%EC%9D%B4%EC%A0%80.md) 역할을 하는 VSTi
로 구분된다.. 이 둘을 한번에 VST(i) 로 표기하기도 한다.

  

VST 는 페이저, 리버브, 에코, EQ, 트레몰로, 증폭 등의 많은 가상 이펙터를 제작하는 [API](API.md) 규격이다.
여담으로 일렉기타만 있고 앰프, 이펙터는 없다면 대표적으로 Native Instrument 사의 Guitar Rig 와 Guitar Rig
Kontrol 을 사용하면 앰프가 필요 없을 정도.

  

VSTi의 i는 instrument, [악기](%EC%95%85%EA%B8%B0.md)를 뜻하며,
[신시사이저](%EC%8B%A0%EC%8B%9C%EC%82%AC%EC%9D%B4%EC%A0%80.md)가 이 형식으로 제작된다. 이런
부류의 프로그램을 [가상악기](%EA%B0%80%EC%83%81%EC%95%85%EA%B8%B0.md)라고도 부른다.

  

넓은 의미에서 VST는 VSTi를 포함하는 개념이다. VST 자체가 가상 오디오 신호처리 플러그인을 위한 [API](API.md)에
대한 표준이니까.

  

그리고 [보컬로이드](%EB%B3%B4%EC%BB%AC%EB%A1%9C%EC%9D%B4%EB%93%9C.md)도 VSTi에 속하는
프로그램이다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/VST?action=edit&section=2)]

## 2. 호환성 ¶

VST 가 지원하는 플랫폼은 [Windows](Windows.md) 와 [Mac OS X](Mac%20OS%20X.md),
[Linux](Linux.md)이다.

  

[Linux](Linux.md)의 경우 공식 지원과 비공식 지원이 둘 다 존재한다. 공식 지원은 [Linux](Linux.md)용
Delphi에 포함된 VST [SDK](SDK.md) 이며, 비공식 지원은
[오픈소스](%EC%98%A4%ED%94%88%EC%86%8C%EC%8A%A4.md)
[자바](%EC%9E%90%EB%B0%94.md) VST [SDK](SDK.md) 이다.

  

[Windows](Windows.md)는 VST(i) 가 DLL 형태로 생성되어 확장자도 .dll 이 되는데 [Mac OSX](Mac%20OS%20X.md)에서는 .VST 를 확장자로 사용한다.

  

LMMS라는 오픈소스 시퀀서의 리눅스 버전에서 윈도우용 VST를 작동시킬 때 WINE을 사용한다.

  

VST3 규격이 [Cubase](Cubase.md) 5.0 과 동시에 발표되었는데, 확장자는 *.VST3 프로그래밍 규칙(?) 이
바뀌어 한번의 [프로그래밍](%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D.md)으로 쉽게 크로스
플랫폼을 만들 수 있다고는 하나 아직 VST3 규격의 악기는 많이 없다.

  

[Logic](Logic.md)의 단점 중 하나로, VST를 지원하지 않는다는 문제가 있다. 이를 해결하기 위해서는 VST를 구동하고,
OS 내 입출력은 AU처럼 동작하게 해주는 프로그램을 사용하면 된다. FXpansion의 VST-AU Adapter(유료),
[Symbiosis AU-VST](http://code.google.com/p/symbiosis-au-vst/)(무료)등의 프로그램이 이런
기능을 제공한다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/VST?action=edit&section=3)]

## 3. 대표적인 VST(i) ¶

  

\- Native Instrument  

\- Massive (신디사이저,
[스크릴렉스](%EC%8A%A4%ED%81%AC%EB%A6%B4%EB%A0%89%EC%8A%A4.md)가 사용하는 VSTi)  
\- Guitar Rig (기타 엠프및 이펙트 시뮬레이터.
[람슈타인](%EB%9E%8C%EC%8A%88%ED%83%80%EC%9D%B8.md)의 기타리스트가 사용)  
\- Kontakt (심포닉 오케스트라부터 덥스텝까지 수많은 VSTi가 있다. Kontakt은 정확히는 VSTi라기 보다는 VSTi를
실행하는 기반적인 프로그램이다. Kontakt만 설치해서 실행하는 것은 의미가 없다. 현존하는 최고의 모듈형 샘플러)  
\- Komplete 9 (Native Instrument사가 출시한/했던 대부분의 악기와 이펙트가 포함된 프로그램. Kontakt,
battery, massive guitar rig, 등등의 대부분의 악기와 이펙트가 포함되어 있다.)  
\- 8Dio (Kontakt를 기반으로 실행, 덥스텝같은 일렉트로닉에서 효과적 진행을 할때 주로 사용)  
\- Cinematic sound design (말 그대로 영화 효과음, 금속물질 부딪히는 소리 등등, Kontakt을 기반으로 사용)  
\- Ilya Efimov Acoustic Guitar Strum (통기타 시뮬레이션, Kontakt을 기반으로 사용)  
\- Virtual Guitarist (일렉기타 시뮬레이션 VST로서 이펙터로서 사용도 되고, VSTi로서 일렉기타 시뮬레이션도 가능)

\- Spectrasonics  

\- Trillian (베이스 가상악기, 실제 현악기 베이스부터 신디사이저 베이스까지 전부 있다.)  
\- Omnisphere (신디사이저 가상악기)  
\- Stylus RMX (드럼 가상악기)  
\- S.A.G.E Xpanders  
\- Tribute Series

\- East West Samples(Symphonic Orchestra 시리즈는 현존하는 최고의 오케스트라 가상악기다.)  

\- East West Quantum Leap Symphonic Orchestra Strings (오케스트라 현악기)  
\- East West Quantum Leap Symphonic Orchestra Brass (오케스트라 금관악기)  
\- East West Quantum Leap Symphonic Orchestra Woodwind (오케스트라 목관악기)  
\- East West Quantum Leap Symphonic Orchestra Percussion (오케스트라 타악기)  
\- Symphonic Orchestra (오케스트라 합창단)  

\- Wordbuilder (Symphonic Orchestra의 가사를 입힐때 사용) <del>[일본의 유명한 프로그램과 매우비슷하다.](%EB%B3%B4%EC%BB%AC%EB%A1%9C%EC%9D%B4%EB%93%9C.md)</del>

\- Stormdrum Kompakt `[1]`  
\- Colossus (사운드 모듈. 미디 채널별로 악기들을 배치할 수 있다.)  
\- Ra (전통악기를 모아놓은 가상악기)

\- Arturia (모듈이나 런치패드 등 실제 음악 프로그래밍 악기도 제작함)  

\- Spark (일렉트로니카 드럼)  
\- Spark Dubstep (덥스텝 스타일의 드럼)  
\- Spark Vintage Drum (올드스쿨 같은 스타일의 드럼)  
\- Analog Classics Series

\- IK Multimedia  

\- Amplitube (Guitar Rig과 비슷한 기타 이펙터, 파워앰프, 케비넷, 랙 시뮬레이터, 모바일과 기타를 연결시킨 애플의
iRig로 아이폰, 아이팟, 아이패드에서 사용가능 )  
\- Sample Tank (사운드 모듈. 미디 채널별로 악기를 배치 할 수 있다. 각 악기가 모두 쓸만하다)  
\- Miroslav Philharmonik  
\- Sonik Synth

\- XLN Audio  

\- Addictive Drum (드럼과, 드럼 프로듀싱을 위한 스튜디오 시뮬레이션)  
\- Addictive Keys (피아노와, 피아노 프로듀싱을 위한 스튜디오 시뮬레이션)

\- reFX  

\- Nexus (사운드 모듈)  
\- Vanguard (신디사이저 가상악기)

\- Edirol  

\- [Hyper Canvas](Virtual%20Sound%20Canvas.md) (미디 기반 사운드 모듈)  
\- Orchestral (오케스트라 가상악기. 용량 대비 상당히 쓸만한 음색을 보인다.)

\- Lennar Digital  

\- Sylenth1 (신디사이저 가상악기. 매시브와 함께 매우 보편적으로 사용된다.)

[[edit](http://rigvedawiki.net/r1/wiki.php/VST?action=edit&section=4)]

## 4. 무료 VST(i) ¶

  

-사운드 모듈계열  

Alchemy player <http://www.camelaudio.com/AlchemyPlayer.php>  
E_MU Proteus VX <http://www.creative.com/emu/proteusvx/>  
Steinburg Universal Sound Module
[ftp://ftp.steinberg.net/Download/Legacy_Plugins/PC/VSTi_Universal Sound Modul
e/](ftp://ftp.steinberg.net/Download/Legacy_Plugins/PC/VSTi_Universal%20Sound%
20Module/)  
Uviworkstation - <http://www.uvi.net/en/software/uvi-workstation.html>

-신디사이저 계열  

\- Brzoza <http://www.saltline.co.uk/brzoza.html>  
\- u-he TyrellN6 <http://www.u-he.com/cms/tyrelln6>  
\- EXD-80 Drum Synthesizer <http://www.thirdharmonic.net/exd80-free-vst-drum-
synth/>  
\- Venom VB-303 v1.00 <http://www.kvraudio.com/forum/viewtopic.php?t=380007>  
\- TONE2 FIRE BIRD [https://tone2.com/html/firebird vsti vst synthesizer plugi
n.html](https://tone2.com/html/firebird%20vsti%20vst%20synthesizer%20plugin.ht
ml)  
\- Tr-808 <http://tactilesounds.blogspot.kr/p/tactile-synthesizers.html>

-샘플러 계열  

-tx16wx <http://www.tx16wx.com>  
-<http://www.plogue.com/products/sforzando/>  
위의 두가지 vsti는 기본적으로 sfz 또는 sf2포멧의 사운드 폰트를 사용할 수 있다.  

-이펙트 및 마스터링 툴  

\- VARIETY OF SOUND <http://varietyofsound.wordpress.com/downloads/>  

(위 사이트의 모든 무료 플러그인은 상업용 플러그인에 못지 않는 퀄리티를 가졌다.)

\- Proximity(마스터링 툴) <http://www.tokyodawn.net/proximity/>  
\- Blue cat audio의 무료 플러그 인
<http://www.bluecataudio.com/Products/Category_0_Freeware/>  

-Native Instrument Komplete Players <http://www.native-instruments.com/en/products/komplete/bundles/komplete-players/>  

Kontakt Player, REAKTOR Player, Guitar rig Player 가 포함된 맛뵈기 버전, 기본적으로 공짜이며, 추가
이펙트와 콘탁트용의 악기를 구매해서 설치할 수가 있다.  

추가바람

`\----`

  * `[1]` Kontakt과 스펠링부터가 다르다.

