<del>한영 변환을 잘 못 했다가는...</del>

<http://qt-project.org/>  
[오픈소스](%EC%98%A4%ED%94%88%EC%86%8C%EC%8A%A4.md) GUI 라이브러리의 일종. '큐트'라고 읽는다.

C++, QML 기반 크로스 플랫폼 프레임워크.

GUI 라이브러리라고 하지만 실상은 통합개발환경(IDE)와 UI개발도구, 번역 작업을 위한 도구 등등에 C++ 개발에 필요한 온갖
기능을(UI, XML, 네트워크, SVG, Animation, Container Class 등등) 제공하는 거대 라이브러리.

원래 트롤텍이라는 회사에서 개발했으나 [노키아](%EB%85%B8%ED%82%A4%EC%95%84.md)가 트롤텍을 인수한 이후에는
노키아에서 관리하였으며, 2012년 8월 9일 Digia에게 넘어갔다.

라이센스는 GPLv3, LGPLv2.1, 상용 라이센스 중 하나를 골라 따를 수 있다. [GPL](GPL.md)이나
[LGPL](LGPL.md)이나 둘 다 Qt 자체의 소스코드를 변경하면서 개발한 경우 같은 라이센스에 따라 소스코드를 공개해야 되기
때문에`[1]` 마음껏 변형해서 쓰면서도 소스코드를 공개하고 싶지 않은 경우 상용 라이센스를 구입해야 된다.

Qt 3.x, Qt 4.x, Qt 5.x의 세가지 버전대가 있으며 가장 많이 사용되는 버전은 4.x와 5.x이다. 4.x 버전에는 Qt
3.x버전에 대한 지원 클래스를 포함하고 있다.

2014년 2월 최신 버전은 Qt 5.2.1과 Qt 4.8.5 이다.

기본적으로는 C++ 기반.  
C#이나 D, Java, Python, Ruby 등 많은 언어에 바인딩 되었다.  
또한 QML이라는 자체 스크립트 언어를 사용하여 빠른 개발이 가능하다.

화려하지만 이것저것 포함하고 있는 게 매우 많아 덩치가 엄청나다는 단점도 있다. 소스 패키지를 보면 4.5에 이르러서는 150메가대에 이르러
있는데 이건 같은 GUI 라이브러리인 GTK+의 그것의 몇 배에 해당된다. 게다가 버전이 올라갈수록 더 늘어나서 4.7에 와서는
200메가까지 천원돌파해 버렸다(...)

한편으로는 [윈도우즈](%EC%9C%88%EB%8F%84%EC%9A%B0%EC%A6%88.md), [Mac OSX](Mac%20OS%20X.md), [리눅스](%EB%A6%AC%EB%88%85%EC%8A%A4.md), 심비안,
[미고](%EB%AF%B8%EA%B3%A0.md) 등 여러 플렛폼에서 똑같은 코드로 프로그램을 짤 수 있는 프로그래머에겐 매우 이상적인
라이브러리이기도 했다. 하지만 2010년 10월 26일 [노키아](%EB%85%B8%ED%82%A4%EC%95%84.md)가 결국 통합
프로젝트를 폐기해 버렸다.

참고로 2011년 09월 조회 기준, 맥용 Qt 라이브러리는 800MB 이며, 리눅스용 Qt 라이브러리는 340MB 이다. 그리고, 위
문단에서 보듯 통합 프로젝트는 폐기되었는데 이상하게 통합해서 작동하도록 작성 가능하다고 한다.`[2]`

2012년 8월 9일, 노키아는 Qt를 매각해버렸다! Digia는 앞으로 Qt를 Android, iOS, Windows 8로 포팅할
예정이라고. [관련기사](http://www.theverge.com/2012/8/9/3229785/digia-nokia-qt-
acquisition)

모바일 부분에서 꽤나 강력한지 Ubuntu Mobile, MeeGo Harmattan, Jolla Sailfish 등의 신생 운영체제에 Qt
Mobile API, QML 등의 기술이 사용되고 있으며, Qt와 QML을 이용해 개발한 앱은 아이폰과 안드로이드에 비공식적으로 올릴 수
있다. 덤으로 윗 문단에서 말한 바와 같이 앞으로 공식적으로 지원 될 예정이다!

2014년 Digia 한국 지사가 생겼다고 한다. 하지만 Qt에 대한 공식적인 기술지원은 안 하고 있다.

파이썬이나 기타 언어와 연동이 된다는 점에서 C++ GUI를 MFC로만 가르치는 학교에서, 다른 학생들이 MFC로 짤동안 해당 과목을 주요
코드는 일주일만에 파이썬으로 다 짜버리고 Qt로 얹어서 A를 받은 위키러의 실화가 있다. 교수는 GUI를 MFC로만 짜라 한적 없다고
(...) <del>반칙아닌가</del> 파이썬으로 GUI를 짜는데 외부 라이브러리들이 사용감이 후지다면(...) 그냥
[PyQt](http://sourceforge.net/projects/pyqt/)로 UI를 드래그앤 드롭으로 배치하고 소스를 python
연동으로 출력한 다음, 본래 기능이랑 이어주면 끝이라서 C++ 오픈소스지만 파이썬으로도 많이 쓰는 모양.

[PyQt 생활코딩 페이지](https://opentutorials.org/module/544/4998)  
[PySide](http://qt-project.org/wiki/Category:LanguageBindings::PySide)  
[PySide 한국어 번역(일부)](http://qt-project.org/wiki/Category:LanguageBindings
::PySide-Korean)

[[edit](http://rigvedawiki.net/r1/wiki.php/Qt%28%ED%94%84%EB%A0%88%EC%9E%84%EC
%9B%8C%ED%81%AC%29?action=edit&section=1)]

### Qt가 사용된 것들 ¶

  * [KDE](KDE.md)
  * 리눅스용 오페라
  * 리눅스용 네이트온
  * 리눅스용 한글(!)
  * 리눅스용 [다음클라우드](%EB%8B%A4%EC%9D%8C%ED%81%B4%EB%9D%BC%EC%9A%B0%EB%93%9C.md)
  * [스카이프](%EC%8A%A4%EC%B9%B4%EC%9D%B4%ED%94%84.md)
  * [MeeGo](MeeGo.md)
  * [VLC](VLC.md)
  * [Virtual Box](Virtual%20Box.md)
  * [오페라(웹 브라우저)](%EC%98%A4%ED%8E%98%EB%9D%BC%28%EC%9B%B9%20%EB%B8%8C%EB%9D%BC%EC%9A%B0%EC%A0%80%29.md)
  * [마야](%EB%A7%88%EC%95%BC.md)
  * Unity 2D([우분투](%EC%9A%B0%EB%B6%84%ED%88%AC.md))
  * Mumble
  * [EA Origin](%EC%9D%BC%EB%A0%89%ED%8A%B8%EB%A1%9C%EB%8B%89%20%EC%95%84%EC%B8%A0#s-9.md)(!)
이 것들 외의 여러가지! [Qt in Use](http://qt.digia.com/Qt-in-Use/)

`\----`

  * `[1]` 단, LGPL의 경우에는 라이브러리 자체를 변경하지 않고 단순히 링크만 한 경우에는 공개 의무가 없다.
  * `[2]` 단 제한조건이 있으며 Qt 라이브러리가 설치되어 있어야 함. 당연하지만 비슷한 파인 android,Meego,Symbian,Mac OS X,iOS 들은 거의 차이 안남.

