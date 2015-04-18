![http://www.blogcdn.com/www.tuaw.com/media/2009/07/opencl.jpg](http://z2.enha
.kr/http://www.blogcdn.com/www.tuaw.com/media/2009/07/opencl.jpg)

[[JPG external
image]](http://www.blogcdn.com/www.tuaw.com/media/2009/07/opencl.jpg)

  
Open Computing Language, OpenCL

한글명칭은 개방형 범용 병렬 컴퓨팅 프레임워크이며, OpenCL을 지원하는 장비는 [CPU](CPU.md)든
[GPU](GPU.md)든 혹은 그 이외의 연산 장비든 모두 가져다 동시에 쓸 수 있다. 개발자는 [AppleInc](%EC%95%A0%ED%94%8C%28%EA%B8%B0%EC%97%85%29.md). 개발자라 덩달아 이 이름의 상표권도
가지고 있다. 애플은 이걸 어느 정도 틀을 잡아놓고 [nVIDIA](nVIDIA.md), [AMD](AMD.md),
[인텔](%EC%9D%B8%ED%85%94.md) 등과 같이 다듬어서 OpenGL 등을 개발하는 크로노스 그룹에 맡긴다. 그후 크로노스
그룹은 열심히 노력해서 1.0을 개발하였고, 1.0은...

당연하게도 [Mac OS X](Mac%20OS%20X.md) 스노우 레오파드와 같이 공개되었다.

애플은 OpenCL 1.0을 공개하면서 이렇게 말했다.  

> Snow Leopard further extends support for modern hardware with Open Computing
Language (OpenCL), which lets any application tap into the vast gigaflops of
GPU computing power previously available only to graphics applications. OpenCL
is based on the C programming language and has been proposed as an open
standard.

  
한글 번역은 다음과 같다.  

> 스노우 레오파드는 OpenCL로 현대 하드웨어에 대한 지원을 확장하였습니다. 이전에는 GPU의 방대한 기가플롭스 계산 능력을 그래픽
애플리케이션에만 사용해 왔지만, OpenCL을 통하여 이제 어떠한 응용 프로그램에서도 끌어와 쓸 수 있습니다. OpenCL은 C 프로그래밍
언어에 기반하고 있으며, 개방형 표준으로 제안되었습니다.

  
OpenCL은 나온 지가 얼마 되지 않아, 많이 알려져 있지 않다. OpenCL은 공개 규격(API)일뿐이지 소스가 공개된 게 아니며,
구현은 전적으로 개발사의 몫이긴 하지만, CUDA는 nVIDIA 하드웨어에서만 동작한다는 단점을 가지고 있어 장래가 기대된다고 보는 사람도
있다. 최근 [AMD](AMD.md)측과 인텔 측에선 OpenCL을 밀고 있는데, 그러나 아직(2013년 8월 기준) AMD의 경우
관련 카탈리스트 드라이버가 정식으로 안 나온 상태`[1]`. 인텔의 경우에도 SDK를 설치하여 개발 및 구동이 가능하나`[2]`, 리눅스에서
사용하기는 좀 난처하다.`[3]`

Mac OS X의 경우, 10.6 Snow Leopard부터 기본적으로 OpenCL을 지원하고 있으며, 따라서 별도의 SDK/드라이버 설치
등이 필요하지 않다. 다만 1.1이 나왔음에도 불구하고 버전이 계속 1.0에 머물러 있으므로 굳이 1.1을 사용하고 싶다면 별도로 드라이버
및 SDK를 설치해야 한다. 또한 일부 헤더 파일을 include할 때 다소 차이가 있다.

GPU만 제어하는 CUDA에 비해 여러 가지 장비를 동시에 관리해야 하므로, 아무래도 명령어가 많이 길어지고 초기화 과정도 하나하나 다 해
줘야 하는 결점이 있다. 코드 길이가 CUDA 코드에 비해 압도적으로 길고, 명령어가 많아서 아무래도 처음 배우는 사람들에게는 문턱이 높다.
대신 여러 장비를 동시에 통제할 수 있고, 그 방법 또한 CUDA보다 세련된 면이 있다.

PyOpenCL이라는 [파이썬](%ED%8C%8C%EC%9D%B4%EC%8D%AC.md) wrapper를 사용하여 편리하고 간결하게
사용할 수 있다. 관심이 있다면 찾아서 배워 보자.

iOS 6에선 잘하면 OpenCL이 등장할 가능성이 크다. 일단, 그 증거로 애플이 iOS 4.3 베타에선 힌트를 숨겨놓더니, iOS 5에선
아예 OS 비밀 프레임워크 디렉토리 안에 OpenCL 프레임워크를 넣어놨기 때문(...) <del>만약 된다면, 보고있냐 구글! 그리고
엔비디아!가 되겠지만...</del>

2013년 8월 31일 현재 최신 버전은 OpenCL 1.2 이다. 그리고 NVIDIA, AMD 각각 SDK 를 제공한다.
([NVIDIA](NVIDIA.md) 는 [CUDA](CUDA.md) 툴킷에 포함하여 제공, [AMD](AMD.md) 는
자체 IDE 를 제작함)

그리고 OpenCL 을 소스가 공개돼서는 안 되는 상용 프로젝트에 사용할 때 문제가 있다. OpenCL 은 호환성 확보를 위해 Online
Complie 이라는 방법을 사용하는데 소스 코드를 불러와 그걸을 즉석에서 컴파일하여 바이너리를 만드는 방식이다. 문제는, 이 것 때문에
소스 코드 공개를 막을 방법이 없다! 소스코드를 어떤 방법으로든 난독화를 하더라도(암호화, 압축 등) 소스를 컴파일하여 바이너리를 만드는 그
함수엔 반드시 원본 소스를 집어넣어야 하기 때문에 이 함수만 잘 추적한다면 원본 소스를 통째로 도둑맞게 된다. 그렇다고 미리 컴파일된
바이너리를 로드하는 방법을 쓰자니, 각 아키텍처에 맞게 컴파일된 바이너리라 호환성을 보장할 수 없다. 이 상황에서 유일한 방법은 [각각아키텍처마다 일일이 바이너리를 만드는 것](%EB%85%B8%EA%B0%80%EB%8B%A4.md)이다.

이 부분을 개선해달라고 개발자들이 요청하고 있으니 다음 개정판을 기다려보자.

`\----`

  * `[1]` 베타로는 나왔지만, 안정 버전으론 나오지 않았다
  * `[2]` 인텔의 경우 아직(13년 8월) CPU only로밖에 나오지 않았다. 조만간 내장 GPU를 지원할 예정이라고 한다.
  * `[3]` 정확히는, 일부 버전의 리눅스를 제외하고는 지원이 안 되거나, 되더라도 불안불안하다.

