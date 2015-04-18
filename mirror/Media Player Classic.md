![o_1.png](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/o_1.png)

[PNG image (17.42 KB)]

  
Media Player Classic(MPC)-HC의 인터페이스

MPC-HC [홈페이지](http://mpc-hc.org/)  
MPC-BE [홈페이지](http://sourceforge.net/projects/mpcbe/)

[윈도우](%EC%9C%88%EB%8F%84%EC%9A%B0.md)에 내장된 Windows Media Player가 7.0 버전 이후로
이것저것 잡다한 기능을 많이 추가함으로서 쓸데없이 무거워지고 미디어 재생기 본연의 기능에 충실하지 못한 것에 불만을 가진 것에서 개발이
시작되었다. 초기 제작자는 Gabest.

[DirectX](DirectX.md) 기능을 사용하기 때문에, Windows용으로만 제작되고 있다. 제작자인 Gabest는 6.4.9
버전 이후로 개발을 중단했으나, Doom9 포럼 커뮤니티에서 버그 수정 및 기능 강화 버전인 **M**edia **P**layer
**C**lassic-**H**ome **C**inema(이하 MPC-HC) 를 계속해서 내놓고 있다. 기존 내장 코덱을 가진 버전은
MPC-BE 프로젝트에서 계승하고 있으며, MPC-BE는 MPC-HC에 비해 상대적으로 인터페이스가 수려하다.

MPC-HC 프로그램 외형은 Windows Media Player 6.4 버전의 모습이랑 같다.

순수한 미디어 재생기로서의 높은 성능과 다양한 미디어 지원, 그리고 64bit 지원이 장점. 그리고 내장 필터들을 따로 받아 다른 미디어
재생기에 쓸 수도 있다. 특정 렌더러에서의 자막표시도 지원한다.

H.264/AVC 코덱과 VC-1 코덱 그리고 최신 베타 빌드에선 MPEG-2 코덱의 DXVA 모드도 지원. 한글도 지원한다.

그리고 [오픈소스](%EC%98%A4%ED%94%88%EC%86%8C%EC%8A%A4.md)인 만큼 플레이어와 내장 필터의 빠른
업데이트도 장점.

MPC-HC의 진정한 장점은 극강의 화질을 자랑하지만, 성능도 많이 잡아먹는 [madVR](madVR.md)이라는 렌더러와 조합이 아주
좋다. madVR이 나온 이후로 MPC-HC를 사용하는 사람들은 대부분 저 madVR을 사용하기 위한 것이라 보면 된다.

화질과 사운드를 중시하는 유저들은 MPC-HC + [madVR](madVR.md) \+
[LAVFilters](LAVFilters.md) \+ xy-VSFilter + ReClock 조합을 많이 사용하였는데, 이제는
MPC-HC 에서 기존 코덱을 버리고 LAVFilters 를 내장코덱으로 사용하고 있기때문에 LAVFilters 는 따로 설치할 필요가
없어졌다. 정확히는 개발팀이 분리되면서 자체 코덱을 유지할 능력이 없어져서 LAVFilters에 의존하는 것. 이 조합은 거의 모든 포맷을
다 재생 가능하며, 화질면에서도 매우 우수하고 xy-VSFilter를 통해 보다 개선된 자막표현이 가능하며, ReClock은 윈도우를 통해야
하는 Direct Sounnd 대신 사운드 장치를 직접 제어하는 WASAPI`[1]`를 사용할 수 있게 해준다. 다만, ReClock이
32비트 버전밖에 없기때문에 위 조합을 사용하려면 MPC-HC와 [LAVFilters](LAVFilters.md), madVR, xy-
VSFilter도 32비트 버전을 사용해야 한다. 귀찮다면 미국의 포럼 하루히쨩에서 제공하는 [Kawaii Codec
Pack](http://haruhichan.com/KCP)을 받으면 전부 포함되어 있다. <del>오오 양덕후 오오오</del> 물론, 여러
설정 필요없이 편의성이 우선인 경우라면 그냥 팟플/곰플/KMP 코덱팩으로 재생하는 게 더 나은 선택이다.

[madVR](madVR.md) \+ [LAVFilters](LAVFilters.md) 를 사용한다면 영상재생 자체는 저것들이
전부 담당하며 플레이어 자체는 사실상 자막 플레이어 겸 UI 도구 정도로 전락하기때문에 굳이 MPC-HC 가 아니더라도 팟플레이어처럼 코덱을
선택할 수 있는 플레이어를 쓴다면 한번 손수 적용해볼 것을 추천한다. 어차피 옵션 몇 단계만 거치면 바로 적용할 수 있고 화면 깨질 걱정도
거의 없어지니 충분히 남는 장사다. 물론, MPC-HC 에서 [LAVFilters](LAVFilters.md) 를 내장코덱으로 사용한
이후부터는 [madVR](madVR.md) 정도만 추가로 설치하면 되므로 오히려 MPC-HC 쪽이 삽질이 적은 편이다.

최신 베타 버전의 소스 코드는 공개되어있지만 컴파일을 할 줄 모르거나 귀찮다고 생각되는 사람들은
[여기](http://xhmikosr.1f0.de/mpc-hc/)로 가보자.

`\----`

  * `[1]` Windows Audio Session API의 약자로, MS 에서 사운드장치 제어를 위해 제공하는 최신 API이다.

