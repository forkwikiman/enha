Microsoft Foundation Classes.  
<del>Myeong-dong Fried Chicken([명동](%EB%AA%85%EB%8F%99.md) [프라이드치킨](%ED%94%84%EB%9D%BC%EC%9D%B4%EB%93%9C%20%EC%B9%98%ED%82%A8.md))</del>  
<del>[폴아웃시리즈](%ED%8F%B4%EC%95%84%EC%9B%83%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md) 플레이어라면
마이크로 퓨전 셀</del>  
<del>[댄스 댄스 레볼루션](%EB%8C%84%EC%8A%A4%20%EB%8C%84%EC%8A%A4%20%EB%A0%88%EB%B3%BC%EB%A3%A8%EC%85%98.md)에서는 [Marvelous FullCombo](%EC%97%91%EC%84%A4%EB%9F%B0%ED%8A%B8.md)</del>

[MSDN의 MFC 페이지](http://msdn.microsoft.com/en-us/library/d06h2x6e.aspx)

## Contents

    

1. 개요 
2. 사용 목적 
3. 단점? 
    

3.1. 하지만...

4. 대안 

[[edit](http://rigvedawiki.net/r1/wiki.php/MFC?action=edit&section=1)]

## 1. 개요 ¶

[Microsoft Windows](Microsoft%20Windows.md) 운영체제 환경에서 작동하는 [GUI](GUI.md)
프로그램을 C++언어를 사용하여 개발할 수 있도록 [Win32 API](Win32%20API.md)의 핸들`[1]`과
[C언어](C%EC%96%B8%EC%96%B4.md) 함수들을 C++ 언어의 클래스화 한 라이브러리 이다. **Visual
C++**이라고 하면 이 MFC를 말하는 것이다. 윈도 환경에서 [COM](COM.md)(Component Object Model)
개발을 위한 라이브러리인 [ATL](ATL.md)(Active Template Library)과 CString등의 기반 클래스를
공유하는 등 매우 밀접한 관련이 있다.

  

<del>윈도우즈환경에서 C++ 개발자라면 좆구린줄 알면서도 이를 악물고 써야 하는 물건</del>`[2]`

  

윈도우즈 환경에서 시스템을 제어하려면 [Win32 API](Win32%20API.md)를 필수적으로 써야 하는데`[3]`, 이 물건은
단순히 윈도우즈라는 운영체제의 여러 기능들을 노출시켜주는 **C 함수**들의 집합일 뿐이기 때문에, GUI를 작성하는 등의 고차원적인 작업을
할때에는 필연적으로 코드 노가다가 들어간다. 그리고 최신의 윈도 컨트롤과 같은 고차원적인 기능들은 Win32 API가 아닌 COM
라이브러리로만 쓸 수 있기때문에, WinAPI 만으로는 한계가있다. 그래서 이걸 그나마 좀 편하게 클래스 형태로 쓸수 있도록 해주는 물건이
바로 이것.

  

Microsoft [Visual Studio](Visual%20Studio.md)의 유료 버전에는 기본으로 포함되어 있다. 무료인
'Express' 버전에는 MFC와 ATL이 포함되지 않는다.

  

Viusal Studio 2013 Communiy Edtion 에 포함되었다!

[[edit](http://rigvedawiki.net/r1/wiki.php/MFC?action=edit&section=2)]

## 2. 사용 목적 ¶

[Microsoft Windows](Microsoft%20Windows.md) 환경에서 실행되는 GUI 프로그램 개발을 위해 사용한다.
C언어 API인 Win32 API를 사용할 수도 있지만 생산성의 문제로 MFC를 사용하는 경우가 대다수이다. C++언어는 C언어에 비해
생산성이 상당히 높으면서도 C언어의 강력한 기능을 사용할 수 있기 때문.

  

MS에서 개발하는 프로그램 중 [Microsoft Office](Microsoft%20Office.md)나 윈도 운영체제 자체 등 일반
사용자에게 제공되는 제품은 MFC를 사용하지 않는다. MFC를 사용하여 개발된 것 중 가장 유명한 것은 [VisualStudio](Visual%20Studio.md) 6.0에 포함되어 있는 Visual C++ 6.0 IDE일 것이다. 하지만 닷넷이
발표되면서 현재의 Visual Studio는 닷넷의 WPF로 개발되고 있다.

  

사실 MFC를 사용하는 가장 큰 이유는 Visual Studio에 포함되어 있기 때문이라는 말이 있다. 더 좋은 라이브러리들이
존재하지만(혹은 존재를 잘 몰라서) 굳이 찾지 않고 포함되어 있는것을 사용한다는 것. 근거 없는 말이 아닌 것이, 타인에게 작업물을
전달한다거나, 라이브러리를 GUI 예제 프로그램과 함께 외부 공개한다거나 할 때에는 MFC의 경우 비주얼 스튜디오 버전만 맞춰주면 보통 별
문제가 없지만, 비주얼 스튜디오에서 기본지원하지 않는 외부 기술을 사용했을 경우에는 그것에 대한 설치와 설정방법도 함께 제공해야 하는데
이것이 귀찮기 때문이다. <del>이게 뭐예요? 이거 안깔고 하면 안돼요? 시키는대로 했는데 왜 안 돼요? 아오</del> 그렇다고
Win32 API를 직접 사용해 GUI 예제를 제공하는 것은 더 귀찮고.

[[edit](http://rigvedawiki.net/r1/wiki.php/MFC?action=edit&section=3)]

## 3. 단점? ¶

  * 순수하게 C언어로 Win32 API를 사용하여 개발한 프로그램에 비하면 무겁다. 물론 [Qt](Qt%28%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8C%ED%81%AC%29.md)나 GTK+와 비교한다면야...<del>하지만 [반디소프트](%EB%B0%98%EB%94%94%EC%86%8C%ED%94%84%ED%8A%B8.md)에서는 무겁다고 까인다</del>`[4]`
  * ATL과 공유되는 CString, CList 등의 클래스는 매우 강력하지만, GUI를 위하여 제공되는 기능은 Win32 API의 매우 얇은 Wrapper 정도이다. 게다가 MFC로 개발한다고 해서 Win32 API를 쓰지 않을 수도 없다.
  * Visual C++ 2008 Feature Pack에서 추가된 리본 인터페이스는 [Microsoft Office](Microsoft%20Office.md)와 비교해 보면 매우 엉성하고 조잡한 티가 난다. 이는 해당 클래스들이 MS에서 제작된 것이 아니라 타사(<http://www.bcgsoft.com/>에서 제작한것을 MS가 구입하여 포함시켰기 때문이다.
  * GUI 디자인 기능이 매우 허접하다. 직접 UI를 그려서 설계할 수 있는 부분은 "윈도 리소스"라는 매우 특이한 형식으로 처리되는 **다이얼로그(대화상자)**만 가능하며, 일반적인 화면은 직접 코드로 구현해야 한다. VB6.0이나 닷넷의 WinForm/WPF, Qt의 QtDesigner등과 비교하면 이뭐병 소리가 절로 나온다.  

[[edit](http://rigvedawiki.net/r1/wiki.php/MFC?action=edit&section=4)]

### 3.1. 하지만... ¶

C++ 언어와 윈도 운영체제에 대한 이해가 있다면 못 써먹을 정도의 물건은 아니다. MFC는 C++ 라이브러리이며, 윈도 운영체제를 다루기
위한 것이므로 이 둘에 대한 선행 학습이 이루어져야 한다.

  

하지만 MFC의 클래스/함수/변수들의 네이밍 센스, Visual Studio가 자동 생성해주는 Template들의 구조는 정말 최악이다.
그런 코드들에 물들면 돌이킬 수 없는 결과가...

  

[[edit](http://rigvedawiki.net/r1/wiki.php/MFC?action=edit&section=5)]

## 4. 대안 ¶

윈도우 응용프로그램을 만들기 위해 반드시 Win32 API 또는 MFC를 사용해야 하는것은 아니다.

  

  * 만들고자 하는 응용프로그램이 매우 간단한 UI만 가지고 있는가? 그렇다면 **WTL**을 고려해보자. MS에서 C++의 템플릿 기능을 사용하여 Win32 API를 C++ 클래스로 구현한 ATL의 확장 라이브러리이다. [홈페이지](http://wtl.sourceforge.net/)  

  * C++언어를 사용하여 강력한 기능과 UI를 빠른 시간안에 개발하고 싶은가?   

    * 그렇다면 **[Qt](Qt%28%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8C%ED%81%AC%29.md)**라이브러리를 사용해 보자. 
    * [Qt](Qt%28%ED%94%84%EB%A0%88%EC%9E%84%EC%9B%8C%ED%81%AC%29.md)는 Linux, Mac, 윈도우를 모두 지원하는 C++ 라이브러리로, 단순한 GUI라이브러리가 아니라 자체적으로 네트워크, 파일 및 DB처리, XML지원, 강력한 String 클래스 등 방대한 기능들을 가지고 있다. 
    * 당연히 윈도 시스템 함수를 호출하는 것도 가능하다.`[5]`
    * 한번만 써보면 MFC의 다이얼로그 편집기는 쓰레기로 보이게 될 GUI Designer를 제공하며, 비주얼스튜디오와 훌륭히 연동된다. [홈페이지](http://qt-project.org/)
    * [닷넷](%EB%8B%B7%EB%84%B7.md)의 WPF와 비슷한 QtQuick을 제공한다.[QML을 시작합니다.](http://blog.qt.digia.com/blog/category/qml_start/)   

  * GTK+나 wxWidgets 등도 훌륭한 대안이 될 것이다.  

  * C++ Builder는 델파이와 같은 훌륭한 개발 환경을 가지고 있으며, C++을 이용하여 동일한 편의성을 누릴 수 있다.  

  * 다른 언어는 어떤가? 반드시 C++을 사용할 필요가 없다면?  

    * 오브젝트 파스칼(델파이)은 매우 훌륭하게 디자인 된 개발환경으로, 역시 강력한 GUI개발도구를 지원하며 또한 Native 컴파일 되는 언어이다.
    * 최근 MS가 열심히 밀어주고 있는 닷넷 플랫폼에는 **윈폼**과 **WPF**의 두가지 GUI 라이브러리가 포함되어 있다. 또한 C#은 C++은 비교도 되지 않는 높은 생산성을 자랑하는 언어이다. 기존 윈도용 C/C++ 프로젝트나 라이브러리와의 연동도 수월하므로 일단 핵심 코드는 그대로 둔 채 껍데기부터 차차 교체할 수도 있다. 닷넷 프레임워크로 개발된 프로그램의 대표작이라면 [비주얼 스튜디오](%EB%B9%84%EC%A3%BC%EC%96%BC%20%EC%8A%A4%ED%8A%9C%EB%94%94%EC%98%A4.md)중 2008 이후의 버전들`[6]`을 들 수 있을것이다. 커다란 용량의 닷넷 런타임 배포가 부담스럽다면, 개인적으로 사용하는 프로그램의 개발에서부터 활용해 보자. 또한 웹 인스톨러 등을 이용하거나 인스톨러가 닷넷 설치 웹사이트를 띄워주는 등의 방법으로 배포에 대한 부담을 줄일 수도 있다. 어차피 윈도 7부터는 닷넷 프레임워크 3.5가, 윈도 8부터는 4.5가 기본적으로 포함돼 있기도 하고, [ATI 카탈리스트](%EC%B9%B4%ED%83%88%EB%A6%AC%EC%8A%A4%ED%8A%B8%28%EC%86%8C%ED%94%84%ED%8A%B8%EC%9B%A8%EC%96%B4%29.md) 컨트롤 센터처럼 장치 드라이버 관련 유틸리티가 닷넷 기반으로 개발되기도 하는 등, 완전히 닷넷이란 것과 담을 쌓다가 갑자기 설치해야 되는 일은 많이 줄어들었다. <del>"아니 이거 닷넷 깔아야 돼? 안 써 그럼."(...) 하던 시절도 있긴 했지만.</del>
    * [Java](Java.md)는 AWT와 Swing이라는... 아니 이건 좀 아닌것 같다. 잊어버리자(...).  

      * Java에는 SWT`[7]`, SwingX등의 GUI 툴킷이 존재하며, [Qt](QT.md)와 GTK, wx4j`[8]` 등의 라이브러리도 사용 가능하다.
    * [Python](Python.md), [Ruby](Ruby.md), [Lua](Lua.md)등 고 생산성 스크립트 언어들은 GUI 구현을 위해 Tcl/Tk, Qt, GTK+등 다양한 라이브러리와 연결 기능을 제공한다.

`\----`

  * `[1]` 운영체제에서 제공하는 객체(C++의 객체와는 조금 다르다)를 다루기 위한 일종의 ID
  * `[2]` 반드시 그런것은 아니다. 조금만 눈을 돌려보면 대안은 차고 넘친다. <del>다만 기존 코드가 MFC로 되어 있는 경우가 많을 뿐.</del>
  * `[3]` 아래에서 서술되는 Qt등의 라이브러리도 윈도용 버전은 Win32 API를 기반으로 개발된 것이다.
  * `[4]` 반디집 설명에 **MFC**와 같은 **무거운 라이브러리**를 사용하지 않아 프로그램이 작고 빠르고 가볍습니다.라고 되어있다.
  * `[5]` 이 경우에는 당연히 리눅스 등에서는 사용 불가능하다.
  * `[6]` WPF로 개발되었다.
  * `[7]` Eclipse 개발을 위해 사용된다. [홈페이지](http://www.eclipse.org/swt/). 
  * `[8]` wxWidgets의 Java 바인딩이다. [홈페이지](http://wx4j.sourceforge.net/). 

