**AviSynth**

[개발자](%EA%B0%9C%EB%B0%9C%EC%9E%90.md)

AviSynth developers

정식 버전

2.5.8 (2008년 12월 30일)

개발자 버전

2.6.0 Alpha 5 (2013년 09월 18일)

[프로그래밍언어](%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20%EC%96%B8%EC%96%B4.md)

[C++](C++.md)

[운영체제](%EC%9A%B4%EC%98%81%EC%B2%B4%EC%A0%9C.md)

[Microsoft Windows](Microsoft%20Windows.md)

프로그램 종류

비선형 비디오 편집 프로그램, 프레임서버

[라이센스](%EB%9D%BC%EC%9D%B4%EC%84%BC%EC%8A%A4.md)

[GNU](GNU.md) [GPL](GPL.md)

[홈페이지](%ED%99%88%ED%8E%98%EC%9D%B4%EC%A7%80.md)

<http://avisynth.nl/index.php/Main_Page>

## Contents

    

1. 소개 
2. 기능 
    

2.1. 장점

2.2. 단점

3. AviSynth 스크립트 언어 
    

3.1. AviSynth 스크립트 언어의 특징

4. 기타 
5. 관련 항목 

[[edit](http://rigvedawiki.net/r1/wiki.php/AviSynth?action=edit&section=1)]

## 1. 소개 ¶

AviSynth는 [Microsoft Windows](Microsoft%20Windows.md)에서 구동`[1]`되는 GUI환경 비선형
비디오 편집 프로그램이다. AVI 또는 MPEG, VFW파일의 인코딩 및 영상 처리에 활용 된다. 다양한 필터를 내장 하고 있어 트리밍,
자르기, 디인터레이싱, 역 텔레시네, 색상 보정, 노이즈 제거 등이 가능하고 외부 플러그인을 추가함으로써 상용 프로그램 못지 않은 강력한
기능과 확장성을 제공한다. 밴 로디악 굴드에 의해 처음 개발되었으며 라이선스는 [GNU](GNU.md)의
[GPL](GPL.md)에 따라 배포되고 있다. 그리고 일부 필터의 기능은 v2.5.7 릴리즈 이후 버전부터 [크리에이티브 커먼즈](/
wiki/%ED%81%AC%EB%A6%AC%EC%97%90%EC%9D%B4%ED%8B%B0%EB%B8%8C%20%EC%BB%A4%EB%A8%
BC%EC%A6%88) Attribution-ShareAlike 3.0 License를 따른다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/AviSynth?action=edit&section=2)]

## 2. 기능 ¶

AviSynth는 입력된 영상을 전개해, 여러가지 필터를 걸쳐 가공한 영상을 다른 동영상 편집 소프트웨어에 건네줄 수 있다. 기본으로 다양한
영상 처리 필터를 갖추고 있고 유저가 개발한 외부 플러그 인의 추가도 가능하다.

[[edit](http://rigvedawiki.net/r1/wiki.php/AviSynth?action=edit&section=3)]

#### 2.1. 장점 ¶

  * 다양한 포맷의 동영상을 로딩할 수 있으며 외부 플러그인을 통해 지원 불가 포맷도 로딩 할 수 있다.
  * 프레임서버 프로그램으로 [동영상](%EB%8F%99%EC%98%81%EC%83%81.md)과 같이 용량이 큰 파일을 인코딩이나 디코딩시 한꺼번에 로딩하지 않고 필요한 부분만 조금씩 프로세싱 해준다.
  * 영상의 포맷변환, 크기변환, 프레임레이트 변환이 쉽다.
  * AviSynth Script인 AVS를 사용하여 임시파일이 필요없으며 즉시 편집을 지원, 다양한 비디오 편집 및 처리 방법을 제공한다. 
  * 각 프레임당 그림으로 저장이 아닌 스크립트(문자)형태로 저장할 수 있다.
  * 외부 플러그인을 통해 여러 기능을 추가할 수 있어 확장성이 대단히 우수하다.
  * 상용 프로그램 못지 않은 강력한 성능을 가졌음에도 [GNU](GNU.md) [GPL](GPL.md) 라이센스이므로 무료다.

[[edit](http://rigvedawiki.net/r1/wiki.php/AviSynth?action=edit&section=4)]

#### 2.2. 단점 ¶

  * 배우기 위한 진입 장벽이 상당히 높다.`[2]`
  * 윈도의 동영상 처리 방법에 대한 약간의 지식이 필요하다.
  * 문법 오류에 민감하고 필요한 플러그인 및 라이브러리가 제대로 설치 되지 않으면 로딩하는 것 조차 안된다.
  * 일부 필터들의 경우 하드웨어적으로 지원 가능해야 사용 할 수 있는 경우가 있다.
  * 개발된 상당수의 필터가 32비트 기반이고, 멀티스레딩 지원이 아직 미흡하다.

[[edit](http://rigvedawiki.net/r1/wiki.php/AviSynth?action=edit&section=5)]

## 3. AviSynth 스크립트 언어 ¶

AviSynth 스크립트 언어인 AviScript는 AviSynth를 프레임서버로서 사용하기 위한 인터프리터 언어이며 이를 파일형태로
지원하기 위한 확장자로 AVS가 사용된다. AVS를 확장자로 가지는 파일을 실행 하였을 때 편집에 사용된 원본의 영상과 효과를
FrameServing하여 보여주게 되며 프레임서버에서는 스크립트를 해석하여 다이렉트쇼로 인터프리팅 하게 된다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/AviSynth?action=edit&section=6)]

#### 3.1. AviSynth 스크립트 언어의 특징 ¶

AviSynth 스크립트 언어는 인터프리터의 특징을 가지고 있는데 문법이 [C언어](C%28%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20%EC%96%B8%EC%96%B4%29.md)와 유사하다. AVS의 특징을 간략히 기술하면 다음과
같다.

  

  * 대부분의 필터는 매소드 형태로 제공 되며 영상 클립을 리턴 하는 형태로 제공 된다.
  * 스크립트 변수를 사용 할 수 있다. 어떤 필터의 매소드를 임의의 변수에 저장하는 기능으로 변수명에는 길이 제한이 없고, 거의 모든 문자열을 사용 할 수 있으며, 변수명은 영어와 숫자로 선언 할 수 있다. 하지만 변수의 첫 문자로 숫자를 사용 할 수 없고 영어가 아닌 다른 문자로는 사용 불가.
  * 영상 클립을 비디오 및 오디오가 포함된, 스크립트 유형의 값으로 리턴해야 하며 클립이 액세스 할 수 있는 다양한 속성을 자체 필터로서 보유하고 있어야 한다.
  * 문자 텍스트를 나타내는 시퀀스는 문자열의 반환 가능한 텍스트중 하나를 따옴표에 의해 둘러 쌓이게 되며, 텍스트 종료 인용 부호 혹은 트리플 인용 시퀀스를 제외한 모든 문자를 사용 할 수 있다.
  * 프로그래밍 언어에서 주로 사용하는 조건문인 if 문을 지원하며, C언어와 유사한 삼항 연산자를 사용할 수 있다.
  * AviSynth 스크립트는 메모장으로도 작성 할 수 있으나 보통 AvsPmod와 같은 전용 에디터를 사용 하거나 버추얼 덥과 같은 소프트웨어를 통해 사용 하는것이 일반적이다.

[[edit](http://rigvedawiki.net/r1/wiki.php/AviSynth?action=edit&section=7)]

## 4. 기타 ¶

[Adobe](Adobe.md) [프리미어프로](%ED%94%84%EB%A6%AC%EB%AF%B8%EC%96%B4%20%ED%94%84%EB%A1%9C.md)와 같은 편집
소프트웨어에서도 AviSynth를 로드해 사용 할 수 있고, 상당수의 인코더 및 미디어 플레이어에서 AviSynth를 미디어 처리에 활용
하고 있다.`[3]` 여담으로 TV 방송이나 DVD, 블루레이의 립을 전문적으로 뜨는 대부분의 불법 릴들은 거의 100% AviSynth와
MegGUI조합을 사용 한다고 보아도 좋을 정도.  
AviSynth 2.x의 한계를 극복하고 새로운 언어를 기반으로 색공간, 사용 가능한 모델, 캐시 관리 및 매커니즘의 향상을 위해
AviSynth 3.0이 [크로스플랫폼](%ED%81%AC%EB%A1%9C%EC%8A%A4%20%ED%94%8C%EB%9E%AB%ED%8F%BC.md)으로 개발
중이었으나 2007년 8월 이후로 교착상태에 빠져 있다.`[4]`

  

[[edit](http://rigvedawiki.net/r1/wiki.php/AviSynth?action=edit&section=8)]

## 5. 관련 항목 ¶

[AviSynth/필터 일람](AviSynth/%ED%95%84%ED%84%B0%20%EC%9D%BC%EB%9E%8C.md)  
[동영상 인코더](%EB%8F%99%EC%98%81%EC%83%81%20%EC%9D%B8%EC%BD%94%EB%8D%94.md)  
[MeGUI](megui.md)  
[FFmpeg](FFmpeg.md)  
[H.26x](H.26x.md)  
[LAVFilters](LAVFilters.md)  
[프레임 더블링](%ED%94%84%EB%A0%88%EC%9E%84%20%EB%8D%94%EB%B8%94%EB%A7%81.md)

`\----`

  * `[1]` [리눅스](%EB%A6%AC%EB%88%85%EC%8A%A4.md)나 [OS X](OS%20X.md)에서도 [와인](%EC%99%80%EC%9D%B8%28%EC%86%8C%ED%94%84%ED%8A%B8%EC%9B%A8%EC%96%B4%29.md)을 이용해 구동할 수 있다.
  * `[2]` 프로그래밍 언어의 함수나 매소드, 파라메터에 대한 약간의 이해는 진입장벽을 낮추는데 상당히 도움이 된다.
  * `[3]` 심지어 오디오 재생기인 [foobar2000](foobar2000.md)에서도 컴포넌트를 추가 하는 것으로 AviSynth를 사용 할 수 있다. 단 오디오에 한해서만 동작한다.
  * `[4]` <http://forum.doom9.org/showthread.php?p=1179369#post1179369> 참고

