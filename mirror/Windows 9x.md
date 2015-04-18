**[Microsoft Windows 버전 일람표](Microsoft%20Windows/%EB%B2%84%EC%A0%84.md)**

**DOS 병행 시절**

**DOS 계열**
**[9x](Windows%209x.md) 계열**
**NT 계열**

[Windows 1.x](Microsoft%20Windows/%EB%B2%84%EC%A0%84#s-1.1.md)

[Windows 95](Windows%2095.md)

[Windows NT 3.x](Windows%20NT#s-3.1.1.md)

[Windows 2.x](Microsoft%20Windows/%EB%B2%84%EC%A0%84#s-1.2.md)

[Windows 98](Windows%2098.md)

[Windows NT 4.0](Windows%20NT%204.0.md)

[Second Edition](Windows%2098#s-2.md)

[Windows 3.1](Windows%203.1.md)

[Windows Me](Windows%20Me.md)

[Windows 2000](Windows%202000.md)

**DOS 단종 이후**

**서버용**
**클라이언트용**
**휴대기기**

[Windows Server 2003](Windows%20Server%202003.md)

[Windows XP](Windows%20XP.md)

[Windows Embedded Compact](Windows%20Embedded%20Compact.md) (CE)

[Windows Server 2008](Windows%20Server%202008.md)

[Windows Vista](Windows%20Vista.md)

[Windows Mobile](Windows%20Mobile.md)

[Windows Server 2008 R2](Windows%20Server%202008%20R2.md)

[Windows 7](Windows%207.md)

[Windows Phone](Windows%20Phone.md)

[Windows Server 2012](Windows%20Server%202012.md)

[Windows 8](Windows%208.md)

[Windows RT](Windows%208.md)

[Windows Server 2012 R2](Windows%20Server%202012%20R2.md)

[Windows 8.1](Windows%208.1.md)

[Windows 8.1 RT](Windows%208.1.md)

[Windows 10 Server](Windows%2010%20Server.md)

[Windows 10](Windows%2010.md)

  

## Contents

    

1. 개요 
2. 내부 구조 및 부팅과정 
    

2.1. 기반 버전

3. 흥망 
4. [그래도 Windows 9x는 돈다.](%EA%B7%B8%EB%9E%98%EB%8F%84%20%EC%A7%80%EA%B5%AC%EB%8A%94%20%EB%8F%88%EB%8B%A4.md)

[[edit](http://rigvedawiki.net/r1/wiki.php/Windows%209x?action=edit&section=1)
]

## 1. 개요 ¶

[Windows 95](Windows%2095.md) 시리즈, [Windows 98](Windows%2098.md)/SE,
[Windows Me](Windows%20Me.md)라는 크게 이 세가지를 통틀어서 말하는 것을 의미한다. 전부 버전이 Windows
4라 Windows 4.x라고도 한다.`[1]` 아무튼 NT 커널이 가정용 시장도 맡기 시작한 [WindowsXP](Windows%20XP.md)까지 가정용 시장을 담당하였다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Windows%209x?action=edit&section=2)
]

## 2. 내부 구조 및 부팅과정 ¶

구조는 이전의 Windows 1.x ~ 3.x와 동일하게 여전히 [MS-DOS](MS-DOS.md) 안에서 돌아가는 구조였다. 부팅할때
도스가 먼저 뜨고 그 다음에 윈도우 셸이 뜨고 시스템을 종료하면 컴퓨터가 같이 꺼지는 식으로 해서 외형적인 존재만 숨긴 것이다. 다만 그냥
윈도셸로 보기엔 구조적으로 약간 차이가 있다. 이 때문에 6.x 버전대의 도스에서는 저 3가지 윈도우를 돌릴 수 없다.`[2]`

  

부팅과정을 조금 더 구체적으로 설명하자면 우선 일반적인 [MS-DOS](MS-DOS.md)의 부팅 과정을 밟기 시작하여
Logo.sys를 불러들이면서 부팅 로고가 뜨고`[3]` IO.SYS가
[레지스트리](%EB%A0%88%EC%A7%80%EC%8A%A4%ED%8A%B8%EB%A6%AC.md)를 불러들이고`[4]` 리얼모드를
설정한 후 드라이버를 불러들인 뒤에 Win.com이 실행되고`[5]` 가상 장치 드라이버를 점검하고 불러들이고 하면서 이 과정이 끝나면
보호모드로 전환된다. 동적 가상 장치 드라이버를 모두 불러들이면 본격적으로 [GUI](GUI.md) 환경을 구축하기 시작하며 로그온이
있다면 로그온 과정을 거치고 시작 프로그램 및 RunOnce`[6]` 레지스트리의 시작 프로그램을 모두 불러들임으로써 끝나게 된다.

  

[Windows 98](Windows%2098.md)까지는 시스템 종료에서 다시 도스로 빠져 나갈 수 있었다. 이후 [WindowsMe](Windows%20Me.md)는 일정 부분 도스의 영향력에서 벗어나고자 시도했기 때문에 자연히 이 옵션이 빠지게 되었다.
<del>그리고 Win Me는 그 댓가로 정말로 **많은 것**을 잃어야 했다.</del>

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Windows%209x?action=edit&section=3)
]

### 2.1. 기반 버전 ¶

앞서 말했다 싶이 Windows 9x는 이래저래 차이가 있다고 해도 결국은 도스 기반인지라 [윈도우를책임질](%EB%BF%8C%EB%BF%8C%EB%BF%A1.md) 도스가 필요하였다. 아래는 해당 윈도 버전과 그 기반 도스 버전을
요약한 표이다.

  

윈도우 버전

도스 버전

[Windows 95](Windows%2095.md)

7.0

[Windows 95](Windows%2095.md) OSR2, [Windows 98](Windows%2098.md)/SE

7.1

[Windows Me](Windows%20Me.md)

8.0

  
상기한 특징으로 인하여 해당 윈도우의 도스 파일만 추출해 별도의 도스로 만든 것도 있었다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Windows%209x?action=edit&section=4)
]

## 3. 흥망 ¶

Windows 9x 계의 첫 시작을 끊은 [Windows 95](Windows%2095.md)의 경우에는 **IT 계의 혁명**이라는
수식어와 함께 좋은 스타트를 끊었다.`[7]` 이후 [Windows 98](Windows%2098.md) 또한 한참 이후에 출시된
[Windows XP](Windows%20XP.md)와 한때 시장 양분을 했을 정도의 인기를 구사하였다.`[8]` 그런데 마지막은
[Windows Me](Windows%20Me.md)로 장식하면서... [안습](%EC%95%88%EC%8A%B5.md).

  

다만 MS가 Windows 9x의 끝을 별로 좋지 않게 마무리한 것은 이 시기 쯤 [넵튠](%EB%84%B5%ED%8A%A0.md)을
넘어 [Windows XP](Windows%20XP.md) 베타 버전을 뿌리고 있을 시기였으므로 [WindowsMe](Windows%20Me.md)는 [MS-DOS](MS-DOS.md) 안에서 뽑을수 있는 한계치까지 뽑아낸 피날레격 작품
정도로만 의의를 두었을 것이라고 추측되고 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Windows%209x?action=edit&section=5)
]

## 4. [그래도 Windows 9x는 돈다.](%EA%B7%B8%EB%9E%98%EB%8F%84%20%EC%A7%80%EA%B5%AC%EB%8A%94%20%EB%8F%88%EB%8B%A4.md) ¶

산업현장 등에서는 비용, 호환성 문제 때문에 여전히 많은 곳에서 애용되고 있다. 특히 [ISA](ISA.md) 기반의 I/O 제어를
하고 있는 곳이라면 하드웨어 직접 제어가 차단되어 있다는 [Windows NT](Windows%20NT.md) 계열의 특정상`[9]`
OS 교체에 어려움이 있기에 이런 장소에서는 여전히 사용될 것으로 보인다.

  

[EZ2DJ](EZ2DJ.md), [EZ2AC](EZ2AC.md)`[10]`,
[네오드럼](%EB%84%A4%EC%98%A4%EB%93%9C%EB%9F%BC.md)`[11]`의 경우에도 Windows 9x 계열
운영체제를 사용하고 있다.

`\----`

  * `[1]` Windows 95(4.0), Windows 98(4.1), Windows ME(4.9)
  * `[2]` 예를 들어 9x의 [IO.SYS](IOSYS.md)의 경우 기존 도스의 IO.SYS와 MSDOS.SYS의 기능을 모두 수행한다. 여기에는 기존까지 config.sys와 autoexec.bat가 수행하는 기능까지 포함되어 있어서 이 두 파일에 별도의 수정을 하지 않아도 최적의 환경으로 부팅이 가능한 것이다.
  * `[3]` 이는 MSDOS.SYS에 해당 파일을 불러들이도록 설정되어 있기 때문이다. [MS-DOS](MS-DOS.md) 부팅 과정을 지나면서 같이 불러들여진 것으로 MSDOS.SYS 파일 내용중 Logo=1을 Logo=0으로 수정하면 로고를 끌수 있었다.
  * `[4]` 만약 없다면 확장자 da0의 백업 파일을 불러들여 내부적으로 [Ctrl CV](Ctrl%20CV.md)를 먼저 한다.
  * `[5]` [더블스페이스](%EB%8D%94%EB%B8%94%EC%8A%A4%ED%8E%98%EC%9D%B4%EC%8A%A4.md)가 설정되어 있다면 이거 이전에 더블스페이스 설정을 먼저 불러들인다.
  * `[6]` 이름에 맞게 여기 있는 시작 프로그램은 한번 불러들이면 다음 부팅에선 실행되지 않는다.
  * `[7]` 이 시기 쯤 가정용 PC 보급률도 오르기 시작하였다.
  * `[8]` 이건 98 자체가 특출나서 라기보다는 서로의 기반이 달라 발생하는 호환성 문제 등 해결해야 할 문제도 있었고 XP의 경우 테마 기능도 있는 등 당시 PC 사양의 업그레이드 주기 등도 고려해야 한다. 여기에 출시 초기의 경우 안정성 검증도 필요하였다. 정착에 필요한 모든 검증 및 과정이 끝난 이후에는 당연히 XP가 빠르게 자리를 채웠다.
  * `[9]` 프로그램을 써서 개방할 수는 있다.
  * `[10]` 영문판 [Windows 98](Windows%2098.md) SE
  * `[11]` [영문 Windows 95를 사용하다가](http://board5.dcinside.com/zb40/zboard.php?id=16&page=61&sn1=&divpage=3&sn=off&ss=on&sc=on&select_arrange=reg_date&desc=desc&no=173948) 현재 최신작인 뉴 패러다임의 경우 외형상 한글 [Windows 95](Windows%2095.md)로 추정되고 있다.

