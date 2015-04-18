{{|이 항목은 [비쥬얼보이어드밴스](%EB%B9%84%EC%A5%AC%EC%96%BC%EB%B3%B4%EC%9D%B4%EC%96%B4%EB%93%9C%EB%B0%B4%EC%8A%A4.md)로 검색해도 들어올 수 있다.|}}

![vba.png](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/vba.png)

[PNG image (3.62 KB)]

[공식 홈페이지](http://vba.ngemu.com/)  
[다운로드 페이지(위의 페이지에서 Sourceforge로 옮겨짐)](http://sourceforge.net/projects/vba/)

약칭 VBA.`[1]` 게임보이 계열 전용
[에뮬레이터](%EC%97%90%EB%AE%AC%EB%A0%88%EC%9D%B4%ED%84%B0.md). 즉,
[게임보이](%EA%B2%8C%EC%9E%84%EB%B3%B4%EC%9D%B4.md), [게임보이컬러](%EA%B2%8C%EC%9E%84%EB%B3%B4%EC%9D%B4%20%EC%BB%AC%EB%9F%AC.md), [게임보이 어드밴스](%EA%B2%8C%EC%9E%84%EB%B3%B4%EC%9D%B4%20%EC%96%B4%EB%93%9C%EB%B0%B4%EC%8A%A4.md)용 게임들을 지원하는 에뮬레이터로 1999년에 Forgotten`[2]`이 개발하였다. 그러나 이후 VBA의 제작에서 손을
떼고 그 뒤를 VBA Team이라는 Forgotten의 형제가 만든 팀이 프로젝트를 넘겨받아 2004년부터 2006년까지 개발을 지속해왔다.
에뮬레이션 성능도 강력했지만, 메모리에서 Hex 코드, 팔레트 코드 등을 읽어 볼 수 있고
[스프라이트](%EC%8A%A4%ED%94%84%EB%9D%BC%EC%9D%B4%ED%8A%B8.md)`[3]`를 추출해낼 수 있는 등
잡다한 기능들이 많은 것으로 유명했으며 사실상 게임보이 계열용 에뮬레이터로서는 독보적인 위치에 자리 잡았다.

[Microsoft Windows](Microsoft%20Windows.md)용 버전에서 [DirectX](DirectX.md)를
이용했다보니 이것이 타 플랫폼에서 문제가 될 수 있다고 보고 그래픽 라이브러리로 SDL를 사용한 버전을 따로 만들어내기도 했으며
[GPL](GPL.md)을 따르는 [오픈소스](%EC%98%A4%ED%94%88%EC%86%8C%EC%8A%A4.md)이다 보니
다양한 플랫폼들에 포팅이 되기도 하였다. 덕분에 이를 기반으로 한 아류작들도 많이 나왔다. <del>하지만 대다수는 그냥 VBA만 쓴다는 게
함정.</del>

2004년 5월 25일에 배포된 1.7.2버전이 최신 안정화 버전으로 2005년 10월 1일에 나온 1.8.0 베타 3 버전까지 감안한다
해도 사실상 더 이상의 업데이트 없이 더 이상의 개발 진행이 없는 상황이나 어차피 게임 개발이 [닌텐도DS](%EB%8B%8C%ED%85%90%EB%8F%84%20DS.md) 이후 세대로 넘어간지라 게임보이 어드밴스용으로 더 이상 나오지
않고 사실상 돌아가지 않을 게임도 없는 수준이기에 크게 문제 될 사항은 없다. 그러나 아직까지도 VBA에 대한 개발은 포크된 다른
프로젝트들에서 뒤이어 진행되고 있어 아직은 맥이 끊어지지는 않을 듯 했으나 2015년 현재 업데이트가 되고 있는 프로젝트가 없는 상황이다.

2014년 2월 시작된 [트위치TV 채팅 포켓몬](%ED%8A%B8%EC%9C%84%EC%B9%98TV%20%EC%B1%84%ED%8C%85%20%ED%8F%AC%EC%BC%93%EB%AA%AC.md) 방송에 사용되고 있다.

[[edit](http://rigvedawiki.net/r1/wiki.php/VisualBoyAdvance?action=edit&sectio
n=1)]

## VBA기반 에뮬레이터 목록 ¶

  

[VBA2](http://code.google.com/p/gbxemu/): 이름대로 VBA의 후속이 되고자 한 듯하나 2010년 2월 23일
자 SVN 246을 끝으로 업데이트가 없다.

  

[VBA Link](http://www.vbalink.info/): 멀티플레이 기능을 추가한 VBA. LAN 연결 및 WiFi 어댑터를
지원. 현재 업데이트가 되고 있지 않다.

  

[VisualBoyAdvance GX](http://code.google.com/p/vba-wii/): VBA-M 기반으로 만들어진 게임큐브
및 Wii 전용. 2012년 7월 7일 자 2.2.8버전이 현재 최신 버전. 2013년 8월 27일자로 채널 인스톨러 1.3이 등장했다.

  

[VBA-M](http://vba-m.com/): VBA 1.8.0 버전의 포크로 2007년부터 개발을 시작했으며 업데이트로 VBA
Link와 같은 멀티플레이 기능도 추가되었다. <del>이제 아래 후술된 VBA-ReRecording의 Lua 스크립팅과 TAS 영상
기능들만 추가하면 된다.</del>

  

2013년 4월 27일 자로 1159 빌드가 나왔으며 덕분에 64비트를 지원하게 되었으나 기존 [MFC](MFC.md)로 개발되던 것을
Wxwidget으로 옮기면서 롬 실행부터 문제가 생기는 등 버그가 속출하고 있어 현재는 아직 MFC 버전을 권장한다.

  

2014년 3월 8일에 나온 1229 빌드가 현재 최신 안정화 버전으로 더 이상 업데이트가 없다.

  

[VBA-ReRecording](http://code.google.com/p/vba-rerecording/): 1.7.2 버전의 브랜치로
TAS 영상 관련 기능 특화를 목표로 삼고 있는 에뮬레이터. Lua 스크립트 관련 기능도 제공한다. 2013년 4월 14일에 나온 v23.6
svn 480이 최신 안정화 버전이며 v24 svn 480이 최신 개발 버전. <del>근데 왜 항상 개발자 버전은 버전이
24지?</del> 2014년 1월 10일자로 svn r482가 나왔으나 정식 배포되진 않고 소스만 존재하며 더 이상 업데이트가 없다.

`\----`

  * `[1]` [Visual Basic for Application](Visual%20Basic%20for%20Application.md)이 아니다!
  * `[2]` 실명은 Julian Henry Hitchcock
  * `[3]` 3번 항목

