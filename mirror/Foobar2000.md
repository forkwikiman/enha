![main-alternate.png](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/main-
alternate.png)

[PNG image (98.79 KB)]

  
기본 인터페이스

## Contents

    

1. [개요](%EA%B0%9C%EC%9A%94.md)
2. 특징 
    

2.1. 다양한 파일 포맷 지원

2.2. 오디오 출력 옵션

2.3. 컴포넌트

2.4. 파일과 태그 관리

2.5. UI 편집

2.6. 포터블 버전 지원

2.7. 지역화 미지원

3. 외부링크 

[[edit](http://rigvedawiki.net/r1/wiki.php/Foobar2000?action=edit&section=1)]

## 1. [개요](%EA%B0%9C%EC%9A%94.md) ¶

![Xchange_3_6_0h_by_Br3tt.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Xc
hange_3_6_0h_by_Br3tt.jpg)

[JPG image (49.2 KB)]

  
Foobar2000의 테마 중 하나

  

[윈앰프](%EC%9C%88%EC%95%B0%ED%94%84.md)의 핵심 개발 인력으로 알려진 인물인, 피터 파블롭스키가 개발한
윈도우용 프리웨어 오디오 플레이어. [유니코드](%EC%9C%A0%EB%8B%88%EC%BD%94%EB%93%9C.md)를 지원한다.

  

윈도우용 오디오 플레이어로서 단순한 인터페이스와 음악 파일의 메타데이터 지원,
컴포넌트([플러그인](%ED%94%8C%EB%9F%AC%EA%B7%B8%EC%9D%B8.md))을 이용한 기능확장, 데이터베이스기능,
리플레이게인등을 지원한다. 메인 프로그램의 소스는 비공개이지만 플러그인 개발을 위한 SDK는 소스가 공개되어있다.

[[edit](http://rigvedawiki.net/r1/wiki.php/Foobar2000?action=edit&section=2)]

## 2. 특징 ¶

<del>컴포넌트에서 시작해서 컴포넌트로 끝나는 프로그램</del>

[[edit](http://rigvedawiki.net/r1/wiki.php/Foobar2000?action=edit&section=3)]

### 2.1. 다양한 파일 포맷 지원 ¶

MP3, AAC, OGG, FLAC, CD 등 자주 쓰이는 대부분의 포맷을 재생할 수 있으며, 기본 지원 포맷이 아닌 경우 디코더 컴포넌트
설치를 통해 재생할 수 있다.

[[edit](http://rigvedawiki.net/r1/wiki.php/Foobar2000?action=edit&section=4)]

### 2.2. 오디오 출력 옵션 ¶

출력 장치를 설정할 수 있으며, WASAPI나 ASIO를 지원한다. 이 경우 출력 비트를 설정하거나 디더링의 유무를 정할 수 있다.

[[edit](http://rigvedawiki.net/r1/wiki.php/Foobar2000?action=edit&section=5)]

### 2.3. 컴포넌트 ¶

컴포넌트라 불리는 DLL 파일을 추가함으로써 기능을 더할 수 있다. UI 기능를 추가하거나 외부 VST를 사용할수도 있으며 음향효과를 위한
DSP를 설치할 수도 있다. 리샘플러나 채널 믹서, IIR Filter와 같은 음향 관련 컴포넌트부터 아이튠즈의 커버플로우까지 다양한 종류가
있다. [알송 가사 플러그인](http://dlunch.net/blog/category/programs/alsong-lyric-
plugin/)도 있을 정도. 특히 제3자 컴포넌트 개발이 활발하다. foobar 2000의 강력한 기능은 여기서 나온다.<del>다만
그만큼 램을 더 먹는다.</del>

[[edit](http://rigvedawiki.net/r1/wiki.php/Foobar2000?action=edit&section=6)]

### 2.4. 파일과 태그 관리 ¶

Media Library 방식으로 사용하면 많은 파일과 그 태그를 쉽게 관리할 수 있다. 파일복사나 이동은 기본이고 아이튠즈처럼 장르,
아티스트, 앨범 범주를 지원하는 패널을 통해 관리할 수도 있다. 또한, 컴포넌트를 통해 freedb나
[MediaBrainz](http://musicbrainz.org/)에서 클릭 한두번으로 태그를 받아올 수도 있다. 포맷 변환도 가능하며,
공개 CLI 인코더를 사용하기 위한 인터페이스도 갖추고 있다. 인코딩에 VST나 DSP를 적용할 수 있다는게 특징. 당연히
ReplayGain도 지원한다.

  

다양한 컴포넌트를 사용한다면 아주 편리한 파일 관리가 가능하다. 예를 들면, 폴더에 새로 추가된 파일을 필터를 통해 확인하고, 태그와
앨범커버를 찾아서 입히고, 컨버터를 통해 포맷을 변환하여 아이튠즈 등 다른 프로그램으로 보내는 작업을 단축키만 몇 번 눌러서 할 수 있다.  
이걸 오래 쓰다보면 푸바가 음악 플레이어가 아닌 음악 파일 변환기가 되는 진기한 장면을 볼 수 있다.

[[edit](http://rigvedawiki.net/r1/wiki.php/Foobar2000?action=edit&section=7)]

### 2.5. UI 편집 ¶

![K-2.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Foobar2000/K-2.jpg)

[JPG image (155.82 KB)]

  

간단하게 플레이어만 사용가능하기도 하지만 여러가지 플러그인을 추가하여, 맨 위 스크린샷의 메뉴, 버튼, 앨범목록, 재생목록 등을 모두
뜯어고칠 수 있다. 이런 각각의 UI 요소들을 패널이라 부르는데, 배치를 바꾸는 것은 물론이고 컴포넌트를 설치하여 패널을 추가할 수도 있다.
마음에 드는 것이 없으면 종결자인 WSH panel을 설치해서 스크립트로 하나하나 짜서 넣을 수도 있다. 또한,
TitleFormatting을 이용하면 어떤 파일이 어떤 형식이고, 몇 번 재생되었고, 어디에 저장되어 있고, 태그 버전은 몇인지 등 수많은
정보를 파라미터와 함수를 사용해 재생목록 등에 커스터마이징해서 뿌릴 수도 있다.

  

이런 설정 작업이 귀찮다면, 컴포넌트와 기타 설정을 포함한 테마팩을 덮어씌우기만 하면 간단하다. 공식 포럼이나
[DeviantArt](http://foo-nation.deviantart.com/), 구글링을 이용해 보자.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Foobar2000?action=edit&section=8)]

### 2.6. 포터블 버전 지원 ¶

설치시에 일반 버전과 포터블 버전을 선택해서 설치할 수 있다. 포터블 버전은 파일형식 연결 설정을 프로그램 내부에서 지원하지 않는다는 점을
빼면 일반 버전과 아무런 차이가 없다. 입맛대로 이런저런 설정 등을 해서 개인화하기 쉬운 반면, 자체적인 설정 내보내기/가져오기 기능을
지원하지 않기 때문에 쌩으로 쓸 것이 아니면 포터블 버전이 관리하기 편하다. <del>물론 쌩으로 쓸 것이면 푸바를 쓰지 않겠지.</del>

[[edit](http://rigvedawiki.net/r1/wiki.php/Foobar2000?action=edit&section=9)]

### 2.7. 지역화 미지원 ¶

따로 언어팩이란 게 없고, 지원할 계획도 없다고 한다. 다만 튜토리얼 문서를 번역하는 것은 상관 없다는 듯.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Foobar2000?action=edit&section=10)]

## 3. 외부링크 ¶

  * 웹페이지: <http://www.foobar2000.org/>
  * 포럼: <http://forums.foobar2000.org/>

