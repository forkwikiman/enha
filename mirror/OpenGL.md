![http://www.opengl.org/img/opengl-4-logo.gif?align=right](http://www.opengl.o
rg/img/opengl-4-logo.gif)

[[GIF external image]](http://www.opengl.org/img/opengl-4-logo.gif)

## Contents

    

1. 개요 
2. 종류 
    

2.1. OpenGL

2.2. OpenGL ES

2.3. WebGL

[홈페이지](http://www.opengl.org/)

[[edit](http://rigvedawiki.net/r1/wiki.php/OpenGL?action=edit&section=1)]

## 1. 개요 ¶

OpenGL은 2D, 3D 그래픽 라이브러리로 가장 광범위하게 사용되고 있다. 그래픽쪽을 배울 때에는 꼭 접하게 된다.
[DirectX](DirectX.md)의 [라이벌](%EB%9D%BC%EC%9D%B4%EB%B2%8C.md) 격. 초창기에는
MS에서도 OpenGL을 지원했었다. 그러다가, 독자솔루션인 DirectX를 내놓으면서 MS는 OpenGL은 전문가 산업용, DirectX는
가정용 컴퓨터 게임 그래픽용이라는 기믹을 만들어 퍼뜨렸는데 존 카멕이 OpenGL이 DirectX보다 훨씬 편리하게 게임에 사용이 가능하다고
직접 코드를 보이면서 글을 올렸고, MS는 존 카멕이 사용하기 힘들다면 다른 누구에게도 힘든게 맞다며 꼬리를 내렸다. 그러나, 이후
OpenGL은 거듭된 병크를 터뜨렸고`[1]` DirectX는 크게 발달하여 결국 역전이 되었다. 존 카멕도 얼마 전 이제는 DirectX가
낫다고 발언한 상황. 저 병크의 원인으로 MS의 음모론을 이야기하는 사람도 있는데, OpenGL 위원회에 MS 측 사람이 껴있긴 했지만 딱
한 명밖에 없어서 가능성은 희박하다. 그리고, 만약 저 한 명으로 인해 저런 병크를 터뜨린 거라면 그건 그냥 OpenGL 쪽이 무능하다는
얘기밖에 안된다.

  

어쨌건 지금은 OpenGL도 절치부심해서 빠르게 발전하고 있으며, 특히나 모바일 게임시장이 뜨고 MS가 거기서 지지부진한 상황에서 상당한
분발을 보여주고 있다.

  

어지간한 [그래픽 카드](%EA%B7%B8%EB%9E%98%ED%94%BD%20%EC%B9%B4%EB%93%9C.md)라면 [둘 다지원하는](%EC%96%91%EB%8B%A4%EB%A6%AC.md) 경우가 많다. DirectX는 **사실상
[윈도우즈](%EC%9C%88%EB%8F%84%EC%9A%B0%EC%A6%88.md) 전용이므로** 타
[운영체제](%EC%9A%B4%EC%98%81%EC%B2%B4%EC%A0%9C.md)([OS X](OS%20X.md),
[우분투](%EC%9A%B0%EB%B6%84%ED%88%AC.md) 등)를 쓴다면 유일한 그래픽 라이브러리이기도 하다. 2010년대
시점에서는 [일반인](%EC%9D%BC%EB%B0%98%EC%9D%B8.md) 시각으로 [그놈이그놈](%EA%B7%B8%EB%86%88%EC%9D%B4%20%EA%B7%B8%EB%86%88.md)이나... [WindowsPhone](Windows%20Phone.md)을 제외한 모바일
[운영체제](%EC%9A%B4%EC%98%81%EC%B2%B4%EC%A0%9C.md), 특히
[안드로이드](%EC%95%88%EB%93%9C%EB%A1%9C%EC%9D%B4%EB%93%9C%28OS%29.md))에서는
[메이저](%EB%A9%94%EC%9D%B4%EC%A0%80.md)다.

  

최신 버전은 [2013년](2013%EB%85%84.md) [7월 22일](7%EC%9B%94%2022%EC%9D%BC.md)
발표된 4.4 버전이며, DirectX에 주력하는 [AMD](AMD.md)와는 대조적으로 [nVIDIA](nVIDIA.md)가
밀고 있는 녀석이다.<del>그런데 왠지 AMD가 더 성능이 잘나온다</del> `[2]`

  

OpenGL은 크게 GL, GLU로 나눠져 있다. GL은 기본적인 함수들이 구현되어 있고, GLU는 좀 더 편히 사용할 수 있도록 함수가
짜여 있다.

  

사실 OpenGL을 실제로 화면에 나타내려면 추가로 라이브러리를 사용해야 하는데, <del>이때 사용하는 것이
glut이다.</del>`[3]` 이 외에도 SDL등과 연동해서 사용하기도 하는데 대부분 크로스플랫폼을 지원한다.

  

대부분의 3D 그래픽이 그렇지만, OpenGL도 사용하려면 어느 정도 수학과 친해져야 한다. 물론, 기본적인 내용에서는 요구하는 수학이
기초적인 공대수준의 선형대수학과 미분기하학 정도로 그리 높지는 않지만, 컴퓨터 공학과 특성상 저쪽과 별 관련없는 이산수학을 제외하면
대학레벨의 수학을 거의 배우지 않는 경우가 많기도 하고, 특히나 신기술이 추가되면서 요구하는 수학수준도 점점 올라가는 추세이다.

  

관련 교재와 서적으로는 Red Book과 Blue Book(레퍼런스 매뉴얼), Orange Book, Superbible이 대표적이다.

  

[애플](%EC%95%A0%ED%94%8C%28%EA%B8%B0%EC%97%85%29.md)이 매우 사랑하여`[4]` [OSX](OS%20X.md)의 모든 시스템 그래픽은 OpenGL로 **항상 가속**되어 표시된다.?`[5]` <del>근데 그걸 아는
사람들이 [인텔](%EC%9D%B8%ED%85%94.md) [그래픽감속기](%EA%B7%B8%EB%9E%98%ED%94%BD%20%EC%B9%B4%EB%93%9C.md)를 달아서 팔았어?</del>
그러나 [WWDC](WWDC.md) 2014에서 Metal을 새로 공개하면서 [iOS](iOS.md)용 앱들은 OpenGL에서
자유로워질 것으로 보인다. 한 전문가는 이를 두고 애플이 OpenGL에 강타를 날린 것이라고 비유했다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/OpenGL?action=edit&section=2)]

## 2. 종류 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/OpenGL?action=edit&section=3)]

### 2.1. OpenGL ¶

[추가바람](%EC%B6%94%EA%B0%80%EB%B0%94%EB%9E%8C.md)

  

[[edit](http://rigvedawiki.net/r1/wiki.php/OpenGL?action=edit&section=4)]

### 2.2. OpenGL ES ¶

임베디드 시스템 등에서 사용할 수 있게 몇 가지 잘 사용되지 않는 함수를 제거한 API. 안드로이드 시스템과 iOS에서 그래픽 가속을 위해
사용된다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/OpenGL?action=edit&section=5)]

### 2.3. WebGL ¶

OpenGL 가속을 플러그인의 도움 없이 표시할 수 있게 해 주는 API.

  

[인터넷 익스플로러](%EC%9D%B8%ED%84%B0%EB%84%B7%20%EC%9D%B5%EC%8A%A4%ED%94%8C%EB%A1%9C%EB%9F%AC.md)(10 이하 제외, 11도 완전히 지원하지는 못하고 있다), [사파리](%EC%82%AC%ED%8C%8C%EB%A6%AC%28%EC%9B%B9%20%EB%B8%8C%EB%9D%BC%EC%9A%B0%EC%A0%80%29.md), [크롬](/wiki
/%ED%81%AC%EB%A1%AC%28%EC%9B%B9%20%EB%B8%8C%EB%9D%BC%EC%9A%B0%EC%A0%80%29)`[6]
`, [모질라 파이어폭스](%EB%AA%A8%EC%A7%88%EB%9D%BC%20%ED%8C%8C%EC%9D%B4%EC%96%B4%ED%8F%AD%EC%8A%A4.md), [오페라](%EC%98%A4%ED%8E%98%EB%9D%BC%28%EC%9B%B9%20%EB%B8%8C%EB%9D%BC%EC%9A%B0%EC%A0%80%29.md) 등이 이를 지원한다.

  

`\----`

  * `[1]` 사실 병크라고 하기는 뭣한 게 오늘날 기준으로 보면 맞는 길이다. 하지만, 당시 하드웨어 성능으로 보면 틀린 길이었고 덕분에 쉐어를 많이 잃게 되었다.
  * `[2]` [AMD GPU 일람](AMD%20GPU%20%EC%9D%BC%EB%9E%8C.md)에서 최신에 속하는 HD 7000번대 시리즈가 OpenGL 4.3까지인데, [nVIDIA GPU 일람](nVIDIA%20GPU%20%EC%9D%BC%EB%9E%8C.md)에서 그다지 최신이라고 할 수 없는 400번대 시리즈가 OpenGL 4.4을 지원한다. 그런데 [2014년](2014%EB%85%84.md) [4월 26일](4%EC%9B%94%2026%EC%9D%BC.md)자에 업뎃된 [드라이버](%EC%B9%B4%ED%83%88%EB%A6%AC%EC%8A%A4%ED%8A%B8%28%EC%86%8C%ED%94%84%ED%8A%B8%EC%9B%A8%EC%96%B4%29.md)로, HD 5000번대 이후의 전 기종이 OpenGL 4.4를 지원하게 됐다. <del>[야 신난다](%EC%95%BC%20%EC%8B%A0%EB%82%9C%EB%8B%A4.md)</del>
  * `[3]` 해당 라이브러리는 1996년(!) 이후로 업데이트된 적이 없다. OpenGL 공식 위키에서 대안으로 FreeGLUT나 GLFW 등을 추천하고 있으니 관심있는 위키러는 찾아보도록 하자. <del>디바이스 컨텍스트에 관한 지식을 쌓은 후 네이티브하게 구현해버려도 상관은 없지만 그러면 크로스플랫폼과는 영영 이별인지라(...)</del>
  * `[4]` 사실 윈도우 이외의 OS 에서는 다른 선택지가 없다. [맨틀](%EB%A7%A8%ED%8B%80.md)이 있긴하지만 아직 제대로 공개되진 않은 상황
  * `[5]` Mac OS X 이후에 등장한 [Windows Vista](Windows%20Vista.md), [Windows 7](Windows%207.md), [Windows 8](Windows%208.md) 등도 UI에 그래픽 가속을 하게 되었다.
  * `[6]` 모바일 포함. 자세한 정보는 Chrome Experience 참조.

