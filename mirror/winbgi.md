[Upload new Attachment "[a-z" on the "UploadFile"](http://rigvedawiki.net/r1/w
iki.php/UploadFile?action=UploadFile&rename=%5Ba-z)]![http://www.cppfrance.com
/gdi/c/10907.cs.jpg?align=center](http://z1.enha.kr/http://www.cppfrance.com/g
di/c/10907.cs.jpg)

[winbgim으로 작성된 팩맨 게임 소스](http://www.cppfrance.com/codes/DEVCPLUSPLUS-PACMAN-
AVEC-GRAPHIC-WINBGIM_10907.aspx)`[1]`

## Contents

    

1 개요

2 특징

제작

볼랜드

플랫폼

윈도우

장르

그래픽 API

<http://winbgim.codecutter.org/>

## 1 개요 ¶

  

BGI(Borland Graphic Interface, 볼랜드 그래픽 인터페이스)의 윈도우 버전. 볼랜드 [C++](C%20++.md) 5.x 이후부터 탑재된 그래픽 API.

  

과거의 그래픽 프로그래밍 기법은 가장 대중적인 [IBM](IBM.md) PC에서는 인터럽트 모드를 통해 직접 그래픽 램에 접근하여
모니터에 주사하는 굉장히 불편한 방법이다. 하지만, 동시에 프로그래머가 하드웨어에 접근이 가능하기 때문에 API나 라이브러리를 사용할 때
보다 최적화 할 수는 있다. 좀 더 편한 그래픽 작업을 위해 볼랜드는 자사의 터보 C/C++에 BGI라는 이름으로 그래픽 API를
포함시켰다. 도스 시대를 지나 윈도우 시대로 접어들면서 윈도우 환경에서도 컴파일 가능하도록 만든 것이 Winbgi 이다.

  

더불어 나이 지긋한 프로그래머라면 다들 알만한 conio.h(콘솔 Input/Output) 라는 비정규 헤더파일도 포함시켰다. stdio.h
을 대체하면서 좀 더 사용하기 편하고 유용한 함수들(대표적으로 getch()라든가)이 포함되었다. 한 때는 엄청나게 사용했지만 지금은
GCC와 호환이 안되니 주의. 쓴다면 컴파일 에러가 난다.  

## 2 특징 ¶

  

최대 장점은 '사용하기 쉽다'이다. 다른 그래픽 API인 [OpenlGL](OpenlGL.md)과
[다이렉트X](%EB%8B%A4%EC%9D%B4%EB%A0%89%ED%8A%B8X.md)와 비교해 보면, 초기화하는데 코딩이 몇줄
차이가 나는지 확연히 드러난다. 가장 최신 버전인 Winbgim 은 'initwindow()' 한 줄이면 충분하다. 이게 얼마나
획기적인가하면 그나마 쉽다고 알려진 [GLUT](GLUT.md)(OpenGL Utility Toolkit)마저도 10줄 이상이
필요하다.

  

하지만 쓰기 쉬운 만큼 3D 기능은 거의 지원하지 않는다. 이론적으론 3D 엔진을 구현할 수 있기는 하지만 설령 구현한다고 하더라도 매우
느릴것이다. 애초에 2D 그래픽 인터페이스로 개발된 만큼 3D은 고려하지 않았을 뿐더러, 2D 그래픽 역시, 현재의 그래픽 API들과
비교해봐도 기본적인 기능만 지원한다. 도스 버전 BGI는 640x480이라는 심히 [골룸](%EA%B3%A8%EB%A3%B8.md)한
해상도까지 지원했으며 16색밖에 표현할수 없었다. 당시에도 상당한 제약이였기 때문에 많은 도스 게임 개발자들은 VGA 인터럽트를 통해
256색을 구현했다. VGA 모드의 심각한 점은 해상도가 320x200으로 더욱 좁아진다는 것과 페이지가 단 한개 밖에 없다는 점이다.
덕분에 개발자들은 갖은 편법을 동원하여 페이지 비스무리한 것을 무려 4개나 발견하는데 성공한다.

  

현재 볼랜드사는 winbgi에 대한 공식적인 지원을 중단한 상태이며, 가장 최신의 버전은 [마이크로소프트](%EB%A7%88%EC%9D%B4%ED%81%AC%EB%A1%9C%EC%86%8C%ED%94%84%ED%8A%B8.md) 비주얼 C ++ 6.0 에서 컴파일 가능하다.
그 이후 버전인 .net 버전에서는 링커와 충돌이 일어난다. 충돌이 발생하는 라이브러리를 링커에서 제외시키면 쓸 수는 있지만 그래도 여전히
불안정하다. 대신, 미국 [콜로라도](%EC%BD%9C%EB%A1%9C%EB%9D%BC%EB%8F%84.md) 대학교 컴퓨터 공학과
교수인 마이클 메인(Michael Main)박사가 수업의 교재로 사용하기 위해 GCC와 호환이 되는 Winbgim이라는 그래픽 API로
새롭게 재탄생시켰다. 이 버전은 winbgi의 모든 기능을 지원할 뿐만 아니라, 윈도우 그래픽 유저 인터페이스 구현을 위해 여러가지 기능을
추가하였다. 더불어 conio.h에 있던 비정규 함수들도 몇가지 추가하였다. 예를 들면 delay(), kbhit().
[대인배](%EB%8C%80%EC%9D%B8%EB%B0%B0.md)스럽게도 수업을 듣는 학생뿐만 아니라, 다른 개발자들을 위해서 친히
학교 서버에 소스와 바이너리 파일, 그리고 메뉴얼 까지 올려서 배포하고 있다.

  

[Visual Studio 버전](http://www.cs.colorado.edu/~main/bgi/)  
[GCC 버전](http://www.cs.colorado.edu/~main/bgi/dev-c++/)

  
  
  

  

`\----`

`[1]` 사실상 winbgim으로 할 수 있는 모든 것을 보여준다. 스프라이트도 구현된다.

