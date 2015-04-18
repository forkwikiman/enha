## Contents

    

1. 설명 
2. 내부 코덱 종류 

[[edit](http://rigvedawiki.net/r1/wiki.php/OGG?action=edit&section=1)]

## 1. 설명 ¶

Xiph.Org 재단에서 개발하고 있는 [오픈소스](%EC%98%A4%ED%94%88%EC%86%8C%EC%8A%A4.md) 컨테이너
포맷이다.

  

[확장자](%ED%99%95%EC%9E%A5%EC%9E%90.md)는 .ogv, .oga, .ogx, .ogg, .spx 등이 있다.

  

본래 OGG하면 음악 포맷인 [Vorbis](Vorbis.md)가 유명하지만, 그외에도 동영상이나 자막 포맷 등 여러가지 포맷이
존재한다. OGG는 이 모든것의 껍질에 해당하는 컨테이너 포맷이다.

  

원래는 Vorbis 빼면 [듣보잡](%EB%93%A3%EB%B3%B4%EC%9E%A1.md)에 가까웠지만`[1]``[2]`,
HTML5가 이 OGG를 공식적으로 지원하면서 앞으로 성장이 기대되는 포맷이다.

  

특정 기업에서 특허권을 행사중이라 상업용으로 활용할 때 로열티를 지불해야 하는 [MP3](MP3.md)와는 달리, ogg는 오픈소스라
자유롭게 사용할 수 있다. 한때는 이 사항이 **OGG파일로 된 음악에는 저작권이 없다**는 식으로 잘못 퍼져서, "저작권이 없는 ogg로
올립니다~" 라는 멘트와 함께 ogg로 인코딩된 음악을 업로드하는 사람들이 꽤 있었다. <del>그리고 그들은 [법무법인과 즐거운한때](%EA%B0%95%EC%A0%9C%EC%A0%95%EB%AA%A8.md)를 보냈다.</del> 확장자가 무료 배포용이라고 해도
일단 그 음악 자체의 저작권이 죽는건 아니니까 주의하자. 포장 디자인이 무료 배포가 가능하다고 해서 안에 들어있는 제품까지 무료 배포가
되는건 아니란 말씀. <del>그러니까, 콜라병이 공짜라도 콜라는 공짜가 아닌 셈</del>

[[edit](http://rigvedawiki.net/r1/wiki.php/OGG?action=edit&section=2)]

## 2. 내부 코덱 종류 ¶

  * 오디오  

    * [손실 압축 포맷](%EC%86%90%EC%8B%A4%20%EC%95%95%EC%B6%95%20%ED%8F%AC%EB%A7%B7.md)  

      * [Vorbis](Vorbis.md)
      * [Speex](Speex.md) \- 음성통화용도의 포맷으로, 알게모르게 많이 쓰이는 코덱. 대표적으로 [XBOX360](XBOX360.md)의 음성채팅, [아이폰](%EC%95%84%EC%9D%B4%ED%8F%B0.md)의 [Siri](Siri.md)에 쓰인다. 바로 아래항목의 opus코덱은 이 speex를 대체하기 위하여 나온것
      * [Opus](Opus.md) \- 2012년 개발된 따끈따끈한 코덱. 확장자는 .ogg 이외에 .opus를 쓸 수 있다. Xiph.Org을 포함한 오픈소스 그룹, [마이크로소프트](%EB%A7%88%EC%9D%B4%ED%81%AC%EB%A1%9C%EC%86%8C%ED%94%84%ED%8A%B8.md), [브로드컴](%EB%B8%8C%EB%A1%9C%EB%93%9C%EC%BB%B4.md), [구글](%EA%B5%AC%EA%B8%80.md), [모질라](%EB%AA%A8%EC%A7%88%EB%9D%BC.md)재단 등등에서 공동제작한 [오픈소스](%EC%98%A4%ED%94%88%EC%86%8C%EC%8A%A4.md) 코덱이다. 본래 스카이프같은 인터넷전화나 화상회의등에서 쓰이는 G.7xx나 Speex코덱을 대체`[3]`하는 용도였는데 [AAC](AAC.md)와 [Vorbis](Vorbis.md) 뺨때릴만한 음질을 자랑하는 괴물이 되었다(...) 최대 512kb/s의 비트레이트를 자랑하여 음악감상용으로도 손색이 없다. 2013년 6월 현재 ffmpeg에서 인코딩이 가능하며, 음악재생 프로그램은 [foobar2000](foobar2000.md)이 지원을 하고, 동영상 코덱팩인 Lavfilter나 K-lite codec pack, 다음 [팟플레이어](%ED%8C%9F%ED%94%8C%EB%A0%88%EC%9D%B4%EC%96%B4.md)역시 지원한다.`[4]`[소개(한글)](http://hacks.mozilla.or.kr/2012/11/its-opus-it-rocks-and-now-its-an-audio-codec-standard/)
    * [무손실 압축 포맷](%EB%AC%B4%EC%86%90%EC%8B%A4%20%EC%95%95%EC%B6%95%20%ED%8F%AC%EB%A7%B7.md)  

      * [FLAC](FLAC.md)
      * [OggPCM](OggPCM.md)
  * 비디오  

    * [손실 압축 포맷](%EC%86%90%EC%8B%A4%20%EC%95%95%EC%B6%95%20%ED%8F%AC%EB%A7%B7.md)  

      * [Theora](Theora.md)`[5]`
      * [Tarkin](Tarkin.md)
      * [Dirac](Dirac.md)
    * [무손실 압축 포맷](%EB%AC%B4%EC%86%90%EC%8B%A4%20%EC%95%95%EC%B6%95%20%ED%8F%AC%EB%A7%B7.md)  

      * [OGGUVS](OGGUVS.md)
  * 기타  

    * [Writ](Writ.md)

`\----`

  * `[1]` Xiph.Org에서 제작한 [FLAC](FLAC.md)코덱도 유명하지만, 확장자가 OGG보단 flac를 많이 쓴다.
  * `[2]` Speex코덱또한 많이 쓰이지만, 얜 일반적인 음원에 쓰이는 코덱이 아니라서 대중적인 인지도가 낮다
  * `[3]` 64kb/s 이하의 저비트레이트에서 쓰인다.
  * `[4]` .opus가 아닌 .ogg로 해줘야 재생된다.
  * `[5]` 이놈이 HTML5에서 [구글](%EA%B5%AC%EA%B8%80.md)과 [모질라](%EB%AA%A8%EC%A7%88%EB%9D%BC.md)재단이 밀고 있는 WebM에 들어가는 코덱이다.

