  * [컴퓨터 관련 정보](%EC%BB%B4%ED%93%A8%ED%84%B0%20%EA%B4%80%EB%A0%A8%20%EC%A0%95%EB%B3%B4.md) \- [소프트웨어/목록](%EC%86%8C%ED%94%84%ED%8A%B8%EC%9B%A8%EC%96%B4/%EB%AA%A9%EB%A1%9D.md)  

![http://www.ffmpeg.org/ffmpeg-logo.png](http://www.ffmpeg.org/ffmpeg-
logo.png)

[[PNG external image]](http://www.ffmpeg.org/ffmpeg-logo.png)

  

## Contents

    

1. 개요 
2. FFmpeg에서 제공하는 것들 
3. 디코더 
    

3.1. FFmpeg을 기반으로 하는 동영상 플레이어

3.2. FFmpeg을 기반으로 하는 코덱

4. [동영상 인코더](%EB%8F%99%EC%98%81%EC%83%81%20%EC%9D%B8%EC%BD%94%EB%8D%94.md)
    

4.1. 특징

4.2. FFmpeg을 기반으로 하는 인코더

4.3. FFmpeg를 기반으로 하는 서비스

4.4. 일반적인 옵션

4.5. 예시

5. 그외 ffmpeg을 이용하는 프로그램들 
6. 국산 플레이어의 GPL 위반 의혹 
7. ffmpeg? libav? 

[[edit](http://rigvedawiki.net/r1/wiki.php/FFmpeg?action=edit&section=1)]

## 1. 개요 ¶

[공식 홈페이지](http://www.ffmpeg.org/)

  

Michael Niedermayer의 주도하에 개발되고 있는 모든 동영상, 음악, 사진 포맷들의 디코딩과 인코딩을 목표로 만들어지고 있는
[LGPL](LGPL.md) 또는 [GPL](GPL.md)라이센스를 따르는
[오픈소스](%EC%98%A4%ED%94%88%EC%86%8C%EC%8A%A4.md) 프로젝트.

  

관련업계에서는 [마이크로소프트](%EB%A7%88%EC%9D%B4%ED%81%AC%EB%A1%9C%EC%86%8C%ED%94%84%ED%8A%B8.md)+[애플](%EC%95%A0%ED%94%8C.md)급의 영향력을 가지고 있는 멀티미디어계의
[최종보스](%EC%B5%9C%EC%A2%85%EB%B3%B4%EC%8A%A4.md). 가능성 없는 이야기긴 하지만 이 프로그램이
[유료화를 시전](%EC%9E%A0%EA%B0%80%EB%9D%BC%20%EB%B0%B8%EB%B8%8C.md)한다면 우리는 내일부터
동영상을 시청 못할수도 있다. `[1]` 아래의 FFmpeg을 기반`[2]`으로 하는 프로그램 리스트를 보면 알겠지만 이건 농담이 아니다.

  

한 일화로 [NVIDIA](NVIDIA.md)와 [AMD](AMD.md)는 자사의 그래픽카드의 하드웨어 가속을 위해 FFmpeg에
'직접' 소스를 건내주고 FFmpeg이 시키는대로 수정하였다. 대부분의 멀티미디어 재생기가 FFmpeg을 기반으로 하기 때문에,
FFmpeg에서 지원만 한다면 그 효과를 당장 볼 수 있기 때문.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/FFmpeg?action=edit&section=2)]

## 2. FFmpeg에서 제공하는 것들 ¶

  * ffmpeg - 미디어 포맷 변환 도구
  * ffserver - 라이브 방송을 하는 멀티미디어 스트리밍 서버
  * libavcodec - 오디오/비디오 코덱 라이브러리
  * libavformat - 멀티미디어 컨테이너의 디먹서/먹서 라이브러리
  * libavdevice - 입출력 장치 제어 라이브러리
  * libavfilter - 미디어 필터 라이브러리
  * libswscale - 이미지 처리 라이브러리
  * libswresample - 오디오 처리 라이브러리  

[[edit](http://rigvedawiki.net/r1/wiki.php/FFmpeg?action=edit&section=3)]

## 3. 디코더 ¶

쉽게 이야기하면 동영상을 재생할때 쓰이는 코덱이다. FFmpeg의 영향력이 절대적이다. [MAC](MAC.md),
[안드로이드](%EC%95%88%EB%93%9C%EB%A1%9C%EC%9D%B4%EB%93%9C.md),
[iOS](iOS.md), [윈도우즈](%EC%9C%88%EB%8F%84%EC%9A%B0%EC%A6%88.md)에서 유명한 코덱
내장형 동영상 플레이어들은 모두 FFmpeg의 libavcodec을 기반으로 하고 있다고 봐도 무방하다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/FFmpeg?action=edit&section=4)]

### 3.1. FFmpeg을 기반으로 하는 동영상 플레이어 ¶

  * iOS : AV player, nPlayer
  * 안드로이드 : DICE player, MX player
  * 윈도우 : [다음 팟플레이어](%EB%8B%A4%EC%9D%8C%20%ED%8C%9F%ED%94%8C%EB%A0%88%EC%9D%B4%EC%96%B4.md), [곰플레이어](%EA%B3%B0%ED%94%8C%EB%A0%88%EC%9D%B4%EC%96%B4.md), [KMP](KMP.md), [MPC-HC](Media%20Player%20Classic.md)
  * 맥 : 무비스트
  * 크로스 플랫폼인 [VLC](VLC.md), [MPlayer](MPlayer.md)`[3]`  
  
여기에 적혀있는것만해도 무시무시하지 않은가? 하지만 여기에 적혀있는것들은 유명한 것들만 적힌 일부분에 불과하다(...)  

[[edit](http://rigvedawiki.net/r1/wiki.php/FFmpeg?action=edit&section=5)]

### 3.2. FFmpeg을 기반으로 하는 코덱 ¶

  * [LAVFilters](LAVFilters.md)
  * FFDshow`[4]`
  * 그리고 LAV필터와 FFDshow를 기반으로하는 수많은 통합코덱들  

[[edit](http://rigvedawiki.net/r1/wiki.php/FFmpeg?action=edit&section=6)]

## 4. [동영상인코더](%EB%8F%99%EC%98%81%EC%83%81%20%EC%9D%B8%EC%BD%94%EB%8D%94.md) ¶

이쪽은 한마디로 정리가 가능하다. [MeGUI](MeGUI.md)를 뺀 나머지 인코더 프로그램들은 모두 FFmpeg기반이라고 해도
무리가 아니다. 곰 인코더? 바닥? 다음 팟인코더? 모두 FFmpeg의 서자들이다.  
다만 2010년 쯤까지 FFmpeg의 인코딩 기능은 별로였다. 곰 인코더나 바닥, 다음 팟인코더 등이 멀티코어를 잘 지원하지 못하는 등의
이유는 바로 이것 때문이다. 하지만 2011년부터는 일취월장하여 꽤 쓸만한 수준까지 올라왔다. 물론 MEGUI의 아성을 넘보기에는 무리지만,
수많은 단계를 거쳐야하는 MeGUI에 비해 간단하면서 쓸만한 화질을 뽑아준다는 장점이 있다.  
MeGUI의 경우도 보기에 따라 FFmpeg 기반이라고 할 수 있다. mencoder를 사용하는데 이 mencoder가 FFmpeg
기반이다. 다만 FFmpeg 외 추가적으로 다른 인코딩/디코딩 라이브러리를 사용할 수 있기 때문에 FFmpeg만을 쓰는 것에 비해 더 강력한
기능을 가진다.

[[edit](http://rigvedawiki.net/r1/wiki.php/FFmpeg?action=edit&section=7)]

### 4.1. 특징 ¶

MeGUI와 비교하여 FFmpeg이 가지는 특징은 아래와 같다

  

  * FFmpeg 프로젝트 자체가 모든 영상의 디코딩/인코딩을 지향하기 때문에 추가적인 코덱의 설치가 필요없다. `[5]`
  * 멀티코어의 공식적인 지원`[6]`
  * AVIsynth의 기능을 수행하는 VF(libavfilter) 기능 내장. 단 기능은 떨어진다.
  * 쉽다.`[7]` 얼마나 쉬운지는 한 번 직접 [해보자](http://dicer.tistory.com/category/%EC%BB%B4%ED%93%A8%ED%84%B0/ffmpeg%EC%9D%B8%EC%BD%94%EB%94%A9). [다른 블로그](http://ligel.tistory.com/14) 하지만 설정할 수 있는 기능은 MeGUI보다 적다.
  * FFmpeg은 쉬운 인코딩을 위해 각종 프리셋을 포함하고 있다. 사실 아래의 인코더들을 쓰는 것보다 직접 FFmpeg을 이용해서 프리셋을 활용하는 것이 더 나은 화질을 보장한다. [CLI](CLI.md) 기반이라 어질어질 할 수도 있지만, 찾아보면 위의 블로그처럼 스크립트를 공개한 곳이 많다. 정 귀찮으면 위 블로그에 있는 배치파일을 그냥 쓰면 된다. 리플들을 보면 수정된 프리셋이 많다. 그래도 아래의 인코더들보다 화질이 훨씬 좋게 나온다.`[8]` 정 귀찮으면 아래 나오는 인코더를 써도 된다.

[[edit](http://rigvedawiki.net/r1/wiki.php/FFmpeg?action=edit&section=8)]

### 4.2. FFmpeg을 기반으로 하는 인코더 ¶

  * 제트오디오VX(무료 혹은 유료, 코원)
  * 유마일
  * 엔젤인코더
  * 샤나인코더 - 개인 개발자가 만든 인코더 임에도 불구하고, 가볍게 인코딩하는 용도로는 매우 좋다. 무료
  * Mencoder
  * [곰인코더](%EA%B3%B0%EC%9D%B8%EC%BD%94%EB%8D%94.md)
  * [팟인코더](%ED%8C%9F%EC%9D%B8%EC%BD%94%EB%8D%94.md)
  * Handbrake  

물론 이 목록 말고도, 대다수의 쉬운 인코더를 자처하는 프로그램들은 대부분 FFmpeg기반이다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/FFmpeg?action=edit&section=9)]

### 4.3. FFmpeg를 기반으로 하는 서비스 ¶

  * [니코니코 동화](%EB%8B%88%EC%BD%94%EB%8B%88%EC%BD%94%20%EB%8F%99%ED%99%94.md), [아프리카](%EC%95%84%ED%94%84%EB%A6%AC%EC%B9%B4.md) 등의 인터넷 동영상 사이트  

    * 많은 인터넷 동영상 사이트들도 ffmpeg를 사용하고 있다. 영상 파일을 다운받아서 뜯어보면 알겠지만, Lavf(libavformat)를 사용하고 있으며 영상 인코딩에도 libavcodec를 사용하고 있다. 

[[edit](http://rigvedawiki.net/r1/wiki.php/FFmpeg?action=edit&section=10)]

### 4.4. 일반적인 옵션 ¶

  * **-i `[input]`**  

    * 입력 파일을 지정한다.  

  * **-vcodec `[codec]`**, **-acodec `[codec]`**  

    * 비디오 코덱, 오디오 코덱을 지정한다. 사용할 수 있는 코덱은 ` ffmpeg -encoders ` 로 확인할 수 있다. `copy`로 지정하면 기존 스트림을 인코딩 하지 않고 복사한다.  

  * **-vf `[filter]`**, **-af `[filter]`**  

    * 비디오, 오디오에 필터를 적용한다. 리사이즈를 하거나 스피드를 바꾸거나 ass, srt 자막을 입히는 등의 처리를 할 수 있다. 자세한 것은 [ffmpeg의 필터 페이지](https://www.ffmpeg.org/ffmpeg-filters.html)를 참고하자. 참고로 자막을 입히는 건 폰트 때문에 윈도에서는 환경변수를 지정해 줘야 한다.  

  * **-b:v `[bitrate]`**, **-b:a `[bitrate]`**   

    * 비디오, 오디오의 비트레이트를 지정한다.  

  * **-y**   

    * 파일을 덮어쓸 일이 있어도 물어보지 않는다.  

  * **-re**  

    * 인코딩 속도를 1x(실시간)으로 제한한다. 로컬 파일을 ffserver로 스트리밍 시 실시간으로 feed를 전송하기 위해서 필요하다.
  

  * **-f `[container]`**   

    * 출력 포맷을 지정한다.  

  * **-t `[time]`**  

    * 지정된 시간 (초 단위)만큼 인코딩한다.  

[[edit](http://rigvedawiki.net/r1/wiki.php/FFmpeg?action=edit&section=11)]

### 4.5. 예시 ¶

위의 블로그에 나와있는 스크립트는 일반적인 TV영상에 맞춰서 된 것이고 애니메이션에는 적합하지 않은 설정이다`[9]``[10]`

  

일반 영상을 스마트폰 등에 맞추어 재인코딩 할때나 블루레이 원본 영상을 인코딩할때 `[11]`의 설정**예시**는 다음과 같다.  

    
    
    ffmpeg -y -i filename.mp4 -threads 0 -sn -vcodec libx264 -preset medium -crf 25 -tune animation -sws_flags lanczos -vf "scale=1280:ceil(1280/dar/2)*2" -acodec aac -strict experimental -ac 2 -ab 192k -async 1 outfile.mp4

"-i filename.mp4" - 입력 파일로 filename.mp4를 지정한다. 확장자를 포함시켜야 한다.  
"-vcodec libx264" - libx264를 사용하여 H.264로 인코딩. MPEG4를 쓰려면 libxvid, VP8을 쓰려면
libvpx로 설정해주면 된다. 밑은 옵션 중 libx264의 옵션을 사용하는 건 물론 달라지지만 대충 비슷하다. 필터 별 자세한 옵션은
영어가 된다면 [ffmpeg 위키](https://trac.ffmpeg.org/wiki) 참조.  
"-preset medium" - libx264의 프리셋을 이용하는것으로 very slow, slower, slow, medium,
fast, faster, veryfast 등의 옵션이 있다. ultrafast나 placebo (이렇게 느려지면 화질 개선이 플라시보 효과
이상의 무언가는 없다라는 수준) 등의 옵션도 있지만 범인들은 쓸 일 없다 (...) 당연히 slow쪽으로 갈 수록 인코딩은 느려진다.
CRF방식으로 인코딩을 할때는 용량에 관여을 하며, 비트레이트 지정으로 인코딩을 할 시 화질에 관여된다.  
"-crf 25" - 비트레이트 지정이 아닌 VBR(가변 화질우선)으로 CRF는 보통 18~30의 옵션을 쓰는데 숫자가 낮을수록 화질이
좋다. 0에서 51까지의 설정이 있고, 보통 18에서 28 정도를 쓴다. 18 정도면 눈에는 무손실처럼 보일 정도. 애니메이션은 보통
25~27의 값을 쓴다. 일반적인 비트레이트 우선 인코딩을 하고 싶다면 -vb 2000k 이렇게 지정하면 된다.  
"-tune animation" - libx264의 tune 옵션을 사용한다. animation은 화면의 색감을 애니메이션에 맞춘 프리셋.
일반적인 티비영상의 경우 film을 쓰기도 한다.  
"-sws_flags lanczos -vf "scale=1280:ceil(1280/dar/2)*2"" 화면이 720p보다 클시
lanczos란 리사이즈 필터를 이용하여 720p로 리사이즈. 리사이즈가 필요없을시 이 명령줄을 빼도 무방하다. 이 VF명령줄에 여러가지
필터를 넣을수도 있지만, tune명령어에 이미 애니메이션에 적합한 필터가 지정되어 있기 때문에 수고를 덜어준다. libass를 사용해서
자막을 하드코딩 할 수도 있다. 윈도에서 쓸 때는 환경변수 설정이 필요한 기능.  
"-acodec aac -strict experimental -ac 2 -ab 192k -async 1" - AAC코덱으로 2채널,
192kb의 비트레이트를 가지도록 음성을 인코딩한다. FFmpeg의 내장된 AAC 인코더는 아직 불안정하기 때문에 사용하기 위해서
-strict experimental 옵션을 붙여야 한다. 별로 내키지 않는다면 libfaac나 neroaac 등의 외부 AAC 코덱을
사용할 수 있다. 컴파일 설정에 따라 사용이 불가능할 수도 있다. 직접 컴파일해서 사용할 경우 컴파일 설정을 잘 한다면 프라운호퍼 소스를
이식해서 만든 고퀄 AAC 코덱을 사용할 수 있다. 이 소스가 안드로이드가 출처인데 라이센스 때문에 대놓고 ffmpeg에 포함시키지는 못하고
이런 식으로 사용할 수 있는 것.`[12]` 귀찮으면 그냥 속 편하게 오픈소스라 ffmpeg 배포판에 기본으로 포함된
[libvorbis](Ogg%20Vorbis.md)라이브러리를 쓰자(...) <del>배터리와 호환성은?</del>  
"outfile.mp4" - 출력 파일명이다. 확장자에 따라 영상 컨테이너(avi, mp4, mkv같은)를 자동으로 선택해주긴 하지만,
가급적이면 -format 옵션으로 출력 포맷을 지정해 주도록 하자.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/FFmpeg?action=edit&section=12)]

## 5. 그외 ffmpeg을 이용하는 프로그램들 ¶

  * [XBMC](XBMC.md)  

[[edit](http://rigvedawiki.net/r1/wiki.php/FFmpeg?action=edit&section=13)]

## 6. 국산 플레이어의 GPL 위반 의혹 ¶

KMPlayer, 곰플레이어, 팟플레이어 3개 플레이어의 경우 GPL 위반 의혹이 있다. 이것은 FFmpeg이 GPL과 LGPL의 이중
라이선스를 제공하고, 가이드라인을 안 지키면 GPL로 판단하기 때문이다. 갖다 쓸 때 LGPL로 해석될 경우에는 소스를 공개 안 해도
되지만, GPL이라면 전체 소스를 공개해야 한다. 이 때문에 3개 플레이어 전부 FFmpeg을 별다른 생각 없이 내장했다가 GPL 위반
의혹을 사게 되었다.

  

이 문제가 제기된 이후 소스를 공개한 것은 팟플레이어로, LGPL 라이선스와 함께 수정된 FFmpeg 소스코드를 다운받을 수 있는 주소를
제공한다. 나머지는 별다른 대응이 없다.

  

[iOS](iOS.md)의 AVPlayer의 경우 소스코드 전체를 공개하고 있다. [#다운로드
페이지](http://www.eplayworks.com/section/support/licenseAP.php?lang=kr) iOS와
[App Store](App%20Store.md) 심사의 특성상 LGPL에서 허용하는 라이브러리 다이나믹 링크로 처리할 방법이 없기
때문에 아예 소스코드 전체를 공개한 듯 하다`[13]`. 이 때문에 앱스토어에서 "무인코딩"으로 검색하면 AVPlayer 이외에도 다른 국산
플레이어가 여러 개 튀어 나온다. 물론 소스코드 공개 이런거 없다.

  

상용이든 무료든 내장 코덱을 이용하는 프로그램치고 오픈소스가 아닌 경우 GPL 위반에서 벗어나기는 불가능하다. 해당 라이센스는 포함된
프로그램 코드 전부를 원하기 때문이다. Hall of Shame에 등재되어 있지 않는 프로그램은 GPL 위반이 아니라서가 아니라 대중에게
비교적 덜 알려진 경우에 불과하다. FFmpeg에 포함된 코덱들도 라이센스 이슈에서 완전히 자유로운 것은 아니다. GPL라이센스는 비교적
법적인 재제가 심화되는 나라의 개발자들한테서 점차 기피되고 있다.  
[추가바람](%EC%B6%94%EA%B0%80%EB%B0%94%EB%9E%8C.md)

  

[[edit](http://rigvedawiki.net/r1/wiki.php/FFmpeg?action=edit&section=14)]

## 7. ffmpeg? libav? ¶

[우분투](%EC%9A%B0%EB%B6%84%ED%88%AC.md)등의 몇몇 리눅스 배포판에는 ffmpeg를 설치하면 ffmpeg대신
avconv가 설치되는데, 이는 ffmpeg의 [포크](%ED%8F%AC%ED%81%AC.md)이다. ffmpeg 안에서 파벌이 갈리고
싸움이 일어났는데, 그 결과 의견이 다른 사람들은 따로 나와서 libav 라는 새로운 포크를 만들었다. libav 쪽은 ffmpeg 쪽을
완전히 무시하고 있는 상황이지만, ffmpeg 는 자신들이 개발하는것에 더해서, libav 쪽을 계속 모니터링하면서(아무래도
오픈소스니...) libav 에서 만든것들도 좍 긁어다가 ffmpeg 에 그대로 편입시키고 있는 상황. 덕분에 왠지 ffmpeg 가
드러운것같긴 하지만, 사용자 입장에서는 ffmpeg 쪽이 기능면에서 낫다.  
자세한 것은 [#FFmpeg-libav 분쟁 기록](http://klutzy.nanabi.org/blog/2012/11/16/ffmpeg-
libav/)을 참고.

  

`\----`

  * `[1]` FFmpeg는 아니지만 실제로 스마트폰에서 로열티 문제로 코덱이 삭제되는 문제가 지속적으로 벌어지고 있다. <del>하지만 이쪽의 경우 외부 코덱을 다운받아서 설정하면 된다</del>
  * `[2]` 정확히는 FFmpeg의 일부인 libavcodec라이브러리를 주로 쓴다.
  * `[3]` FFmpeg 개발자중에는 MPlayer 개발에도 참여하는 사람이 많다. 
  * `[4]` 애시당초 FFmpeg에서 파생된 프로젝트이다.
  * `[5]` 단 FFmpeg 컴파일 시 어떤 코덱의 라이브러리를 링크하느냐 마느냐에 따라 해당 코덱의 영상 처리가 불가능한 경우도 있다.
  * `[6]` 정확히 말하면 MeGUI를 돌리는데 필수적인 AVIsynth가 멀티코어를 지원하지 않는다. 비공식적인 방법이 있지만 필터를 좀 가리기도 하고.
  * `[7]` 물론 FFmpeg은 [CLI](CLI.md)이기 때문에 GUI를 가진 MeGUI에 비해서 어려워 보일수 있으나, 막무가내 인코딩을 할때는 FFmpeg에서 제공하는 프리셋을 이용하여 노력대비 고화질을 얻을 수 있다.
  * `[8]` 이것은 인코더들이 아주 오래된 버전의 FFmpeg을 기반으로 하고 있으며, FFmpeg에서 제공하는 프리셋을 사용하지 않기 때문이다.
  * `[9]` MeGUI도 마찬가지로, 인코딩 관련글을 볼때 이 인코딩이 애니메이션에 최적화 된 것인지, 일반적인 TV영상에 최적화 된 것인지 확인해야한다.
  * `[10]` 애니메이션은 프레임수가 다르기 때문이다.
  * `[11]` 팟인코더등 인코딩 프로그램 대체
  * `[12]` 또한 DLL도 제공하는 건지 일부 FFmpeg 계열 인코더에 이걸 DLL로 포함한 경우가 있다.
  * `[13]` 사실 이것도 [KLDP](KLDP.md)에서 한차례 [논란](http://kldp.org/node/119469)이 된 끝에 이렇게 된 것.

