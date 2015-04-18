![Xcode.png](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Xcode/Xcode.png)

[PNG image (91.92 KB)]

## Contents

    

1. 개요 
2. 상세 
3. 버전 역사 
    

3.1. Xcode 1

3.2. Xcode 2

3.3. Xcode 3

3.4. Xcode 4

3.5. Xcode 5

3.6. Xcode 6

[[edit](http://rigvedawiki.net/r1/wiki.php/Xcode?action=edit&section=1)]

## 1. 개요 ¶

[애플](%EC%95%A0%ED%94%8C.md)의 [OS X](OS%20X.md) 및 [iOS](iOS.md) 개발 전용
[IDE](%ED%86%B5%ED%95%A9%20%EA%B0%9C%EB%B0%9C%20%ED%99%98%EA%B2%BD.md).
**엑스코드**라 읽는다. 딱 봐도 알겠지만 [OS X](OS%20X.md)용만 존재한다. 2014년 12월 현재 최신 버전은
6.1.1이다.  
2003년에 출시되어, 무려 11년의 역사를 가지고 있는 장수 IDE이다. 만약 그 전신인 Project Builder까지 연대기에 넣는다면
1988년`[1]` 출시로, 무려 26년의 역사를 자랑하는 IDE가 된다. 제작사도 애플이지만, 이 역사를 보았을 때 Xcode보다 애플
제품에 깊숙히 관여하는 IDE는 아직까지는 없다`[2]`고 보아야 한다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Xcode?action=edit&section=2)]

## 2. 상세 ¶

Apple LLVM`[3]`을 주 [컴파일러](%EC%BB%B4%ED%8C%8C%EC%9D%BC%EB%9F%AC.md)로 삼고
LLDB를 주 디버거로 이용한다. 물론 과거와의 호환성을 위해 LLVM GCC라는 이름으로 GCC의 변형판 역시 제공하고 있으나, 이는 더
이상 애플에서 **공식적으로 지원하지 않으니** 사용하지 않을 것이 권장된다`[4]`. 공식적으로 지원하는 언어는 [C](C%28%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20%EC%96%B8%EC%96%B4%29.md),
[Objective-C](Objective-C.md), [C++](C++.md), Objective-C++,
AppleScript, [자바](%EC%9E%90%EB%B0%94.md),
[파이썬](%ED%8C%8C%EC%9D%B4%EC%8D%AC.md), [루비](%EB%A3%A8%EB%B9%84.md)이며,
제3자 도구를 이용하면 [파스칼](%ED%8C%8C%EC%8A%A4%EC%B9%BC.md),
[에이다](%EC%97%90%EC%9D%B4%EB%8B%A4.md), [C#](C%23.md), [펄](%ED%8E%84%28%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20%EC%96%B8%EC%96%B4%29.md), D
언어도 사용 가능하다.

  

Xcode에 내장된 Interface Builder는 OS X에서
[Cocoa](%EC%BD%94%EC%BD%94%EC%95%84.md) 프레임워크를 가장 목적에 올바르게, 그리고 가장 아름답게
디자인할 수 있는 유일한 도구로, [Qt](QT.md)나 SDL, wxWidgets같은 크로스 플랫폼 UI 툴킷이 그 태생상 절대
따라갈 수 없는 디자인을 가능케 한다.

  

초창기의 Xcode는 버전 관리를 지원하지 않거나 svn만 맛보기 형식으로 지원하는 수준이었으나 Xcode 4의 출시와 함께
[Git](Git.md)을 내장하여 강력한 소스 코드 버전 관리가 가능하도록 하였다`[5]``[6]`.

  

간혹 애플의 개발자 프로그램에 유료로 등록해야만 Xcode를 사용할 수 있다고 잘못 알고 있기도 한데, Xcode는
[개발자](%EA%B0%9C%EB%B0%9C%EC%9E%90.md) 등록이 필요 없고`[7]` 무료이다`[8]`. 몇 백만 원을
호가하는 [MSDN](MSDN.md) 구독권을 구매해야 사용 가능한`[9]``[10]` [마이크로소프트](%EB%A7%88%EC%9D%B4%ED%81%AC%EB%A1%9C%EC%86%8C%ED%94%84%ED%8A%B8.md)의 [비주얼 스튜디오](%EB%B9%84%EC%A3%BC%EC%96%BC%20%EC%8A%A4%ED%8A%9C%EB%94%94%EC%98%A4.md)와는 다른 정책을 취하고
있다. Mac은 비싸지 않냐고 생각할 수 있지만, Mac mini정도면 저것보단 저렴한 편이고<del>모니터는?</del> 한 번 구매하면
어쨌든 쓸만한 컴퓨터 한 대 장만하는 것이니 비교가 안 된다.`[11]`

  

다만, 그래도 애플의 개발자 프로그램이 나중에는 필요하게 되는 일도 있는데, 바로
[앱스토어](%EC%95%B1%EC%8A%A4%ED%86%A0%EC%96%B4.md)를 이용할때이다. 앱스토어에 앱을 올리고자 한다면
유료 개발자 등록이 되어야하기 때문. 또한 실물 단말기를 활용할때도 유료 개발자 인증이 필요하다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Xcode?action=edit&section=3)]

## 3. 버전 역사 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/Xcode?action=edit&section=4)]

### 3.1. Xcode 1 ¶

사실상 Project Builder의 개명 버전에 가깝다. 다만, 넘어오면서 UI 변경, Code Sensing(소스 코드를 인덱스하여 자동
완성을 제공하는 기능) 추가 등이 있었다. 별로 특별한 것은 없었던 버전.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Xcode?action=edit&section=5)]

### 3.2. Xcode 2 ¶

Mac OS X Tiger의 출시와 함께 공개. Quartz Composer라는 Quartz Extreme용 시각화 프로그래밍 도구를
탑재했다. 그리고 이 때부터 애플의 개발자 문서를 IDE 자체에서 빠르게 검색할 수 있도록 하였다.  
추후 Tiger의 [Intel](Intel.md) 칩 이전에 의해 Universal 바이너리`[12]`를 생성할 수 있는 기능이
추가되었다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Xcode?action=edit&section=6)]

### 3.3. Xcode 3 ¶

Mac OS X Leopard의 출시와 함께 공개. 여러 가지 명령줄 도구`[13]`의 추가와 함께 Objective-C 2.0 지원이
추가되었으며 프로젝트 스냅샷 기능과 svn 지원으로 기초적인 소스 코드 버전 관리가 가능해졌다. 또, 운영 체제의 전반적인 64비트 전환과
함께 64비트 컴파일이 가능해졌고, [iPhone](iPhone.md)의 공개에 따라 [iPhone OS](iOS.md)용 앱을
빌드할 수 있게 되었다. 이 때 LLVM GCC 컴파일러가 스리슬쩍 더해졌다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Xcode?action=edit&section=7)]

### 3.4. Xcode 4 ¶

**"The biggest thing to happen to Xcode since Xcode`[14]`."**

  

Xcode의 화려한 변신이 행해진 첫 버전. Interface Builder가 Xcode 내부에 모듈 형태로 탑재됨에 따라 이제 개발 시에는
Xcode 하나면 켜놓으면 된다. 초기 버전은 Mac [App Store](App%20Store.md)에서 $4.99에
판매되었으나`[15]`, 항의가 거세지자 스리슬쩍 무료로 전환했다. 이 버전부터 [PowerPC](PowerPC.md) 바이너리는 일체
지원되지 않는다.

  

Xcode 4.1과 함께 Objective-C에서 [객체](%EA%B0%9D%EC%B2%B4%20%EC%A7%80%ED%96%A5%20%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D.md)의 레퍼런스 카운팅을 컴파일러가 스스로 행하는
ARC가 추가되었다.

  

Xcode 4.2에서는 Xcode 자체가 완벽하게 단일 애플리케이션으로 패키지되었다. 이전까지는 Mac App Store에서 내려받는
프로그램이 Xcode **설치** 프로그램이었으나`[16]`, 이제는 Xcode 자체를 내려받는다. 사용자는 내려받은 후 실행하면 끝. 처음
내려받았을 때나 업데이트 시 한정으로 내부 프레임워크를 시스템에 설치하는 짧은 절차를 거친다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Xcode?action=edit&section=8)]

### 3.5. Xcode 5 ¶

[2013년](2013%EB%85%84.md) 9월 18일에 정식 출시. [OS X](OS%20X.md) 10.8 마운틴라이언과
[iOS](iOS.md) 7의 SDK가 포함되었고, LLVM 컴파일러가
[A7](%EC%95%A0%ED%94%8C%20A%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md) AP를 위한 64-bit
앱을 컴파일할 수 있게 되었다. iOS 7이 기존과 UI면에서 상당히 달라진 만큼 기존의 UI와 iOS 7에 맞춘 UI를 동시에 개발하여
적용하기 쉽도록 되어있다. 원 클릭으로
[아이클라우드](%EC%95%84%EC%9D%B4%ED%81%B4%EB%9D%BC%EC%9A%B0%EB%93%9C.md)나 게임센터
서비스를 적용시킬 수 있게 되었고, 테스트 네비게이션으로 빠르

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Xcode?action=edit&section=9)]

### 3.6. Xcode 6 ¶

WWDC 2014 때 공식적으로 발표된 Xcode로, 최초로 [Swift](Swift.md)를 지원한다(!). Swift가 궁금하다면
해당문서 참조. OS X Yosemite 에서만 사용가능케했다. 그리고 새로운 **Playground** 기능을 추가했는데, 이건 놀랍게도
실시간으로 코딩을 할 수 있게해준다! 스크린샷은 애플 공홈 참조. 아직 정보가 부족함으로 추가바람.

  

Xcode 6.1 버전부터 맥용 앱을 Swift로 만들 수 있게 되었다.`[17]`

`\----`

  * `[1]` 혹은 그 이전. Project Builder가 [NeXT](NeXT.md)STEP 운영 체제의 일부분으로 배포되었으므로 운영 체제 개발 기간까지 합치면 적어도 1986년까지는 거슬러간다.
  * `[2]` 요즘 들어 iOS용 소프트웨어를 쉽게 제작할 수 있는 도구(예를 들자면 [Adobe](Adobe.md) [Flash](%EC%96%B4%EB%8F%84%EB%B9%84%20%ED%94%8C%EB%9E%98%EC%8B%9C.md))가 많이 나오고 있지만, Xcode를 성능 면에서 넘지는 못한다.
  * `[3]` 오픈 소스 프로젝트인 LLVM/Clang을 애플 내부에서 적당하게 변형한 버전. 물론 해당 프로젝트의 PM인 Chris Lattner(크리스 래트너)가 애플 직원인 만큼 가장 애플 플랫폼에 이상적으로 달라붙도록 변형되었다.
  * `[4]` 다만, 애플에서 공식적으로 지원하지 않을 뿐이지, 실제로는 LLVM 프로젝트 내에서 dragonegg라는 이름으로 활발하게 지속 중인 하위 프로젝트이다.
  * `[5]` 물론, Xcode 4의 베타는 저 Git 통합 때문에 거의 시망 수준이었다. 다른 것은 문제가 거의 없다시피 했는데 툭하면 Git과의 연동 실패로 IDE 자체가 뻗는 일이 다반사였다. 그것도 Golden Master 버전에서! 이 Git 연동은 Xcode 4.2에 들어서야 완벽해졌다.
  * `[6]` 더불어, 이 때를 기점으로 오픈 소스 프로젝트 저장소 제공 서비스인 GitHub이 Objective-C 코드로 미어터지기 시작했다.
  * `[7]` Apple ID만 있다면 Mac App Store에서 내려받을 수 있다: [#](https://itunes.apple.com/kr/app/xcode/id497799835).
  * `[8]` 사실 Xcode 4 공개 직후 며칠간 유료로 $4.99에 판매한 전적이 있긴 하다. 얼마 안 가서 무료로 풀긴 했지만, 이 때 구매했던 사람들은 상당히 황당했을 듯하다.
  * `[9]` 학생은 [DreamSpark](http://dreamspark.com)에서 무료로 내려받아 사용 가능하다. 하지만 오로지 교육용으로만 사용 가능. 졸업 후에는 구매해야 한다.
  * `[10]` Express 버전도 있는데, 이것은 기능이 제한적이다. Express 버전에 비하면 Xcode는 모든 기능을 사용 가능한 풀 패키지를 무료로 제공하는 것이다.
  * `[11]` 다만 이건 원론적인 이야기이고, 실질적으로는 엄연히 Xcode의 단점으로 꼽히는 점이기도 하다. 왜냐하면 오늘날 Xcode가 절실히 필요한 사람의 대부분은 iOS앱 개발자인데, 안드로이드앱은 오픈소스 OS에서 오픈소스 IDE(예: [이클립스](%EC%9D%B4%ED%81%B4%EB%A6%BD%EC%8A%A4.md))로도 개발이 가능하지만 iOS앱은 그렇지 않기 때문이다. 즉 iOS앱 개발을 하려는 입장에서는, Xcode의 존재는 분명히 단점 맞다. 게다가 OS X의 보급률이 MS 윈도우보다 떨어지는 것이 엄연한 사실이고, 단지 Xcode를 돌리기 위해서 맥을 사야하는 상황도 자주 발생한다. 물론 이건 정확히 말하면, Xcode의 단점이라기보다는 iOS 앱개발이 가지는 문제점이지만.
  * `[12]` PowerPC용 바이너리와 Intel용 바이너리를 모두 포함해 각 아키텍처용 Tiger에서 모두 작동하도록 한 응용 프로그램 번들.
  * `[13]` 프로그램 메모리 프로파일링 도구인 DTrace가 이 때 추가되었다.
  * `[14]` iPhone 5 홍보 문구를 패러디 한 것이다.
  * `[15]` 기존 유료 개발자 프로그램 등록자에게는 무료로 제공되었다.
  * `[16]` 실행하면 Xcode와 주변 패키지를 설치하고 자기 자신을 삭제한다.
  * `[17]` 그 전까진 iOS 앱만 만들 수 있었다.

