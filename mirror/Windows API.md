이 항목에서는 [Microsoft Windows](Microsoft%20Windows.md) 운영체제의 응용 프로그램을 제작하는 데
사용되는 [API](API.md)에 대해 설명한다.

## Contents

    

1. 개요 
2. 특징 
    

2.1. 하드웨어 독립적

2.2. 동적 링크 라이브러리

2.3. 메시지 처리

2.4. 핸들

2.5. 리소스

3. [Hello, Windows 프로그램](Hello%2C%20world%21.md)
    

3.1. 메시지 박스

3.2. 윈도우

[[edit](http://rigvedawiki.net/r1/wiki.php/Windows%20API?action=edit&section=1
)]

## 1. 개요 ¶

Windows API는 [Microsoft Windows](Microsoft%20Windows.md)에서 사용하는
[C언어](C%EC%96%B8%EC%96%B4.md) 기반의 [API](API.md)이다. 기본적으로는 C언어 기반이지만,
[C++](C++.md)에서도 사용 가능하다. 윈도우에서 실행되는 모든 종류의 어플리케이션들은 내부적으로 전부 이 윈도우 API함수를
호출하는 형태로 바뀌어지게 된다.`[1]`

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Windows%20API?action=edit&section=2
)]

## 2. 특징 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/Windows%20API?action=edit&section=3
)]

### 2.1. 하드웨어 독립적 ¶

과거의 [MS-DOS](MS-DOS.md) 환경에서는 프로그래머가 시스템에 연결된 장치의 종류를 모두 알아야 했다. 가령
[한/글](%ED%95%9C/%EA%B8%80.md) 같은 위드프로세서를 만들어야 한다고 가정해 보자. 문제가 되는 것은 모니터랑
프린터인데, 과거에는 이 그래픽 출력 장치 및 프린터에 대한 제어 코드를 일일이 만들어 주어야 했다.`[2]` 만약 회사나 학교에서 사용
중인 워드 프로세서가 [아래아한글](%EC%95%84%EB%9E%98%EC%95%84%20%ED%95%9C%EA%B8%80.md)이고, 지원하는 프린터가 정해져
있다고 생각해 보자. 누군가가 외국에서 프린터 좋은 거 있다고 해서 사 왔는데, 아래아 한글에서 지원하지 않는 프린터라면 [더 이상의 자세한설명은 생략한다](%EB%8D%94%20%EC%9D%B4%EC%83%81%EC%9D%98%20%EC%9E%90%EC%84%B8%ED%95%9C%20%EC%84%A4%EB%AA%85%EC%9D%80%20%EC%83%9D%EB%9E%B5%ED%95%9C%EB%8B%A4.md).  
그러나 Windows 환경에서는 그러한 하드웨어 제어 코드는 [장치드라이버](%EB%93%9C%EB%9D%BC%EC%9D%B4%EB%B2%84#s-3.md)가 가져가게 되며, 문자 출력은
DrawText 또는 TextOut 함수 호출로 한큐에 끝내게 된다. 꼭 문자 출력뿐만 아니라 거의 모든 게 이런 식으로 하드웨어의 종류에
영향을 받지 않는다.  
거꾸로 윈도우 환경으로 넘어오면서 하드웨어 인터럽트를 직접 건드려 제어하는 방식의 프로그래밍 기법은 완전히 사장되었다. 그도 그럴 것이,
윈도우에서는 하나의 운영체제 위에 여러 개의 프로세스가 작동하는 멀티태스킹 및 멀티스레딩 환경이기 때문.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Windows%20API?action=edit&section=4
)]

### 2.2. 동적 링크 라이브러리 ¶

윈도우는 기본적으로 꼭 필요한 기능들을 정적 라이브러리 형태가 아닌 DLL 형태로 만들어 윈도우 운영체제 안에 내장시켜 놓았는데, 보통
C:\Windows\system32 경로에 가 보면 이런 DLL들을 찾아볼 수 있다. 프로그램이 실행될 때 동적으로 불려오는 DLL의
특징상, 프로그램을 한 번 짜 놓으면 윈도우 버전이 올라가면서 윈도우 DLL이 개선되는 경우 그에 맞게 프로그램 기능도 개선되게 된다.
<del>하지만 호환성이 문제</del>  
자주 사용하는 DLL은 다음과 같다.  

  * kernel32.dll : 메모리 관리, 파일 입/출력, 프로그램 로드/실행 등 기본적인 기능이 내장되어 있다.
  * gdi32.dll : 화면/프린터의 그래픽 출력을 관리한다.
  * user32.dll : 윈도우`[3]`, 대화 상자, 메뉴 등을 관리한다.  

[[edit](http://rigvedawiki.net/r1/wiki.php/Windows%20API?action=edit&section=5
)]

### 2.3. 메시지 처리 ¶

[MS-DOS](MS-DOS.md)환경이나 콘솔 응용 프로그램에서는 프로그램의 실행 흐름이 프로그래머가 작성한 코드에 따라서
움직였다면, 윈도우에서는 프로그램 외부에서 발생하는 이벤트들을 메시지의 형태로 프로그램에게 알려 준다. 하드웨어 이벤트`[4]`가 발생하면,
윈도우의 시스템 메시지 큐에 이것이 쌓이게 되고, 시스템 메시지 큐에 들어온 메시지를 운영체제가 해당하는 윈도우의 메시지 큐에 넣어 준다.
프로그램은 while문을 돌면서 계속 메시지를 읽어서, switch-case해서 어떤 메시지가 오면 어떻게 처리한다는 로직을 기술하는 형태를
가진다.  
메시지가 전달될 때는 단순히 메시지 뿐만 아니라, 메시지를 받을 윈도우가 어떤 것인지와, 그 메시지에 딸려 오는 부가적인 정보도 같이
날아오게 된다.`[5]`

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Windows%20API?action=edit&section=6
)]

### 2.4. 핸들 ¶

핸들(HANDLE)은 윈도우에서 오브젝트에 붙여 주는 숫자로, 가상 메모리의 주소일 수도 있고, 시스템이 전역으로 식별하기 위해 붙인 번호일
수도 있다. 어떤 오브텍트는 주소의 의미를, 어떤 오브젝트는 번호의 의미를 갖는다.`[6]` 핸들은 각각의 윈도우, 브러시, 펜, 파일,
프로세스, 스레드 등 거의 모든 오브젝트에 붙게 된다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Windows%20API?action=edit&section=7
)]

### 2.5. 리소스 ¶

윈도우 프로그램을 짜다 보면 메뉴, 대화 상자(다이얼로그 박스), [아이콘](%EC%95%84%EC%9D%B4%EC%BD%98.md),
[비트맵](%EB%B9%84%ED%8A%B8%EB%A7%B5.md) 이미지, 커서 등을 많이 사용한다. 그러나 얘네들은 메모리 용량을
많이 잡아먹기 때문에 프로그램이 메모리에 올라올 때 얘네들이 메모리에 전부 다 올라와버리면 메모리가 터져나가게(...) 된다. 그렇기 때문에
이런 것들은 리소스로 취급하며, 리소스 컴파일러를 통해 프로그램 코드와는 별개로 컴파일되고, 이들을 사용할 때는 LoadMenu,
LoadIcon, LoadBitmap, LoadCursor 등의 함수를 통해 메모리에 로드하는 과정을 거치게 된다. 프로그램 실행 중
사용하지 않는 리소스는 메모리에서 자동으로 내려간다.

  
  

[[edit](http://rigvedawiki.net/r1/wiki.php/Windows%20API?action=edit&section=8
)]

## 3. [Hello, Windows 프로그램](Hello%2C%20world%21.md) ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/Windows%20API?action=edit&section=9
)]

### 3.1. 메시지 박스 ¶

이 프로그램은 아무 아이콘도 없고, 확인 버튼이 하나 존재하는 메시지 박스에 "Hello, Windows"를 출력한다.  

    
    
    #include <Windows.h>#include <tchar.h>int APIENTRY _tWinMain(HINSTANCE hInstance, HINSTANCE hPrevInstance, LPTSTR lpCmdLine, int nCmdShow){    MessageBox(NULL, TEXT("Hello, Windows!"), TEXT("Hello"), MB_OK);    return 0;}

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Windows%20API?action=edit&section=1
0)]

### 3.2. 윈도우 ¶

이 프로그램은 흰색 바탕의 클라이언트 영역의 정중앙에 "Hello, Windows"를 출력하는 윈도우를 하나 띄운다.  

    
    
    #include <Windows.h>#include <tchar.h>LRESULT CALLBACK WndProc(HWND, UINT, WPARAM, LPARAM);int APIENTRY _tWinMain(HINSTANCE hInstance, HINSTANCE hPrevInstance, LPTSTR lpCmdLine, int nCmdShow){    static TCHAR szAppName[] = TEXT("HELLOWINDOWS");    HWND hWnd;    MSG msg;    WNDCLASS wndclass;    wndclass.style = CS_HREDRAW | CS_VREDRAW;    wndclass.lpfnWndProc = WndProc;    wndclass.cbClsExtra = 0;    wndclass.cbWndExtra = 0;    wndclass.hInstance = hInstance;    wndclass.hIcon = LoadIcon(NULL, IDI_APPLICATION);    wndclass.hCursor = LoadCursor(NULL, IDC_ARROW);    wndclass.hbrBackground = (HBRUSH)GetStockObject(WHITE_BRUSH);    wndclass.lpszMenuName = NULL;    wndclass.lpszClassName = szAppName;    if (!RegisterClass(&wndclass))    {           MessageBox(NULL, TEXT("This program requires Windows 2000 or upper."),            szAppName, MB_OK | MB_ICONERROR);return 0;    }    hWnd = CreateWindow(szAppName, TEXT("Hello Windows Application"),        WS_OVERLAPPEDWINDOW, CW_USEDEFAULT, CW_USEDEFAULT,        CW_USEDEFAULT, CW_USEDEFAULT, NULL, NULL, hInstance, NULL);    ShowWindow(hWnd, nCmdShow);    UpdateWindow(hWnd);    while (GetMessage(&msg, NULL, 0, 0))    {        TranslateMessage(&msg);        DispatchMessage(&msg);    }    return msg.wParam;}LRESULT CALLBACK WndProc(HWND hWnd, UINT message, WPARAM wParam, LPARAM lParam){    HDC hDC;    PAINTSTRUCT ps;    RECT rect;    switch (message)    {    case WM_CREATE:        return 0;    case WM_PAINT:        hDC = BeginPaint(hWnd, &ps);        GetClientRect(hWnd, &rect);        DrawText(hDC, TEXT("Hello, Windows!"), -1, &rect,            DT_SINGLELINE | DT_CENTER | DT_VCENTER);        EndPaint(hWnd, &ps);        return 0;    case WM_DESTROY:        PostQuitMessage(0);        return 0;    }    return DefWindowProc(hWnd, message, wParam, lParam);}

`\----`

  * `[1]` [MFC](MFC.md), [비주얼 베이식](%EB%B9%84%EC%A3%BC%EC%96%BC%20%EB%B2%A0%EC%9D%B4%EC%8B%9D.md), [델파이](%EB%8D%B8%ED%8C%8C%EC%9D%B4.md), 등 윈도우에서 사용할 수 있는 모든 라이브러리는 실행 시 전부 내부적으로 어떻게든 변환을 거치게 된다.
  * `[2]` 모니터 출력의 경우 허큘리스, CGA, EGA, VGA ... 그리고 프린터의 경우 각각의 프린터에 대한 제어 코드를 일일이 다 만들어서 위드프로세서 프로그램 안에 내장시켜 주어야 했다.
  * `[3]` "창"의 의미로 사용되는 그 윈도우를 의미한다
  * `[4]` 사용자가 키보드를 누르거나 마우스를 움직였다거나, 기타 여러 가지의 자잘한 이벤트를 의미한다.
  * `[5]` WPARAM과 LPARAM이 여기서 나온다.
  * `[6]` 특정 종류의 오브젝트를 가리키는 핸들이 주소인지 번호인지는 마이크로소프트에서 공식적으로 문서화하지 않았다. 즉 언제든 바뀔 수 있다.

