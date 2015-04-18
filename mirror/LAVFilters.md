## Contents

    

1. 소개 
2. 특징 
3. 적용법 

[[edit](http://rigvedawiki.net/r1/wiki.php/LAVFilters?action=edit&section=1)]

## 1. 소개 ¶

[공식 홈페이지](https://github.com/Nevcairiel/LAVFilters/releases)  
유명한 [FFmpeg](FFmpeg.md)에서 디코딩 기능만을 빼와 만든
[오픈소스](%EC%98%A4%ED%94%88%EC%86%8C%EC%8A%A4.md) 통합 오디오, 동영상 코덱.  
2013년 현재 유료코덱, 무료코덱 통틀어서 패왕이라고 불리는 코덱이다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/LAVFilters?action=edit&section=2)]

## 2. 특징 ¶

  * 광범위한 호환성 - 상용 코덱인 리얼미디어 코덱과 퀵타임 코덱을 제외한 나머지 거의 모든 코덱을 지원한다. 또한 내장 스플리터를 포함하고 있기때문에, 비슷한 오픈소스 코덱인 ffdshow보다 호환성이 더욱 폭넓다.`[1]`  

  * 쉬운 설정법 - ffdshow가 Geeks을 위한 하드코어한 설정을 자랑한다면, LAV filter는 비교적 손쉬운 설정을 지향한다.  

  * 가볍다. - 사실 일반적으로 사람들이 많이 찾는 통합코덱팩의 경우 ffdshow를 기반으로 하여, 이 코덱이 이 지원하지 못하는 몇 가지 코덱과 스플리터, 그리고 광고프로그램(...)을 버무려 놓은 것에 불과하다. 하지만 위쪽에 서술했듯이 리얼 미디어와 퀵타임을 제외하곤 재생불가한 것은 거의 없다. 또한 통합코덱이 쓸데없이 과도하게 많은 코덱을 설치하여 일어나는 코덱끼리의 충돌현상이 일어나지 않는다.  

  * 신기술의 적용이 빠르다. - yadif 디인터레이싱, DXVA, Intel Quicksync, Nvidia Cuvid 등 CoreAvc나 Cyberlink Power DVD같은 상용코덱에서나 지원하던 옵션들을 모두 지원한다. 또한 스플리터로 유명한 할리 미디어 스플리터 같은 경우 TrueHD, DTS-HD, [mkv](mkv.md)같은 최신 기술을 지원하지 못하는 반면, `[2]` LAVFilter에 포함되어있는 스플리터는 모두 지원한다.  

[[edit](http://rigvedawiki.net/r1/wiki.php/LAVFilters?action=edit&section=3)]

## 3. 적용법 ¶

[LAVFilters](http://code.google.com/p/lavfilters/)와 [리얼
미디어](http://software.naver.com/software/summary.nhn?softwareId=MFS_103886) 코덱
<del>근데 리얼미디어는 옛~날 [야동](%EC%95%BC%EB%8F%99.md)에나 쓰이던 녀석이잖아</del>, [퀵타임
코덱](http://software.naver.com/software/summary.nhn?softwareId=MFS_103882)`[3]`
세 개만 설치하면 못 돌리는 동영상은 없다고 봐도 무방하다. 쓰는 사람이 극히 드물겠지만(...) 윈도우 미디어 플레이어를 쓴다면 자막표시를
위한 [vsfilter](http://code.google.com/p/xy-vsfilter/wiki/Downloads?tm=2) 정도가
필수품.

  

  * [MPC-HC](Media%20Player%20Classic.md) \- <del>MPC-HC에 들어있는 자체코덱은 이 코덱만 뽑아서 쓸 사람이 있을 정도로 LAVFilters에 비견될 만큼 훌륭한 코덱이기 때문에, 굳이 LAVFilters를 따로 쓸 필요는 없다. 단지 LAVFilters를 이용하는 것은 MAD-VR과의 조합으로 극상의 화질조합을 낼 때 쓰는 것.</del> MPC-HC v1.7.0부터 LAV Filters를 내장하기 시작했다. `[4]`  

  * [다음 팟플레이어](%EB%8B%A4%EC%9D%8C%20%ED%8C%9F%ED%94%8C%EB%A0%88%EC%9D%B4%EC%96%B4.md)  

    * LAVFilters를 이용한 저사양을 위한 하드웨어 가속 - [링크](http://beautifulmirinae.tistory.com/2285) 그래픽카드를 이용한 가속법이므로, 그래픽카드의 성능이 떨어진다면, 하드웨어 가속부분을 none으로 놓자.
    * [madVR](madVR.md)+LAVFilters - MPC-HC의 경우와 마찬가지로 극상의 화질을 기대할 수 있는 설정법 [설정법1](http://horro.tistory.com/15) [설정법2](http://varins.com/394).`[5]`
단 설정법1 링크에 있는 LAVFilters는 구 버전이다. 위의 공식 홈페이지에 가서 최신 버전으로 설치를 하면 된다.  

  * [곰플레이어](%EA%B3%B0%ED%94%8C%EB%A0%88%EC%9D%B4%EC%96%B4.md)나 [KMP](KMP.md) 같은 경우, LAV필터와의 호환성이 그다지 안 좋다고 알려져 있다. 사실 KMP 같은 경우는 나온지도 오래돼서 윈도우 7과의 호환성도 그다지 좋지 않고.

`\----`

  * `[1]` ffdshow는 스플리터를 포함하지 않기 때문에, flv같은 윈도우에서 기본적으로 지원하지 못하는 확장자는 재생하지 못한다.
  * `[2]` 통합코덱이 지저분해지는 이유 중 하나이다.
  * `[3]` 아이튠즈를 쓴다면 포함되어 있기 때문에 따로 깔 필요없다.
  * `[4]` 정확히는 개발팀이 분리되면서 자체 코덱을 유지할 능력이 없어져서 LAVFilters에 의존하는 것, 기존 내장 코덱을 가진 버전은 MPC-BE 프로젝트에서 계승하고 있다.
  * `[5]` 설정법은 작성자의 동영상 재생 시스템을 기준으로 작성된 것이므로, 이를 참고하여 각자 자신의 시스템에 맞도록 설정하는 것이 필요하다.

