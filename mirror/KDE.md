  * [동음이의어](%EB%8F%99%EC%9D%8C%EC%9D%B4%EC%9D%98%EC%96%B4.md)

## Contents

    

1. 오픈소스 데스크탑 환경 K Desktop Environment 
    

1.1. 개요

1.2. 기본 구성요소와 특징

1.3. KDE/Qt 어플리케이션

    

1.3.1. Konqueror

1.3.2. Rekonq

1.3.3. Dolphin

1.3.4. Kontact

1.3.5. Kate

1.3.6. Okular

1.3.7. Kile

1.3.8. Gwenview

1.3.9. Amarok

1.3.10. SMPlayer

1.3.11. Marble

1.3.12. KTorrent

1.3.13. KOffice

1.3.14. KDevelop

2. 게임회사 Konami Digital Entertainment 

[[edit](http://rigvedawiki.net/r1/wiki.php/KDE?action=edit&section=1)]

# 1. 오픈소스 데스크탑 환경 K Desktop Environment ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/KDE?action=edit&section=2)]

## 1.1. 개요 ¶

![http://kde.org/announcements/4.8/screenshots/plasma-
desktop-4.8.png&width=600](http://kde.org/announcements/4.8/screenshots
/plasma-desktop-4.8.png)

[[PNG external image]](http://kde.org/announcements/4.8/screenshots/plasma-
desktop-4.8.png)

  

[공식 사이트](http://www.kde.org/)

  

KDE는 **K** **D**esktop **E**nvironment의 약자로, 독일을 중심으로 한 인터내셔널 팀이 개발하는 오픈소스
데스크탑 환경이다. [Qt](QT#s-4.md) 라이브러리 위에서 돌아간다.

  

기능이 매우 많고 사용자에게 제공되는 옵션이 매우 많다는 점이 특징이다. 그만큼 시간을 좀 들이면 정말 예쁘고 자신에게 알맞는 데스크탑
환경을 구현할 수 있다는 강점이 있다. 물론 기능과 옵션이 워낙 많아 데스크탑이 무겁다거나, UI가 직관적이지 않다는 비판을 받기도 한다.
그러나 KDE 4.X 에 들어와서 기능을 많이 희생하지 않으면서도 UI가 많이 깔끔해진데다가`[1]` KDE 4.11 출시 이후 속도도 크게
향상되면서 이런 비판의 목소리는 줄어들고 있다.

  

Gnome3가 사용자에게 필요한 옵션만 제공한다는 정책 하에 개발되었고 언뜻 보면 합리적인 이야기였던데다 Gnome2까지의 평이 꽤 좋았기
때문에 사용자들에게 최대한 많은 옵션을 제공하자는 KDE의 사상은 그다지 고평가되진 않았었으나,UX의 적용이 UI 스타일의 흥행요소를 넘어
UI 자체의 생명력이 되어버린 지금 UX적인 사상으로 보았을때는 오히려 오픈소스에 제일 잘 맞는것이 아닌가 하는 이야기가 있다.사용자층이
윈도우처럼 매우 많은것도 아니라 사용자경험 축적이 비교적 힘들고 맥처럼 UI 하나에 온갖 입력장치의 특허권을 움켜쥐고 인력을 많은 돈을
주면서 확보해 따로이 연구를 하는것도 어려운 상황에서 `[2]`차라리 사용자에게 최대한의 선택권을 주는것이 오픈소스라는 프로그램 특성
측면에서는 옳은것이 아닌가 해서 나온 이야기가 아닌가 싶다.

  

위의 Gnome3가 나왔을때 많은 비판을 받았던 이유도 무겁다던가 Gnome2와 좀 다르다던가 등의 여러 사유도 있지만 가장 큰 것은 UI가
마음에 안든다였다. UX적인 측면에서만 본다면 사용자에게 필요한걸 노출시킨다는 방향성을 코어 개발진이 잡아서 제시해야 하는데,그 방향성을
조금이라도 잘못 잡을 경우 일어나는 일이 어떤것인지 개략적으로 알 수 있게 해주는 대목이라고 할 수 있겠다.`[3]``[4]``[5]`

  

QT5에서 [타블렛](%ED%83%80%EB%B8%94%EB%A0%9B.md)`[6]`입력이 안되는 버그가 있어 이후 와콤 타블렛의
정식지원을 하지 않을거 같다는 이야기가 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/KDE?action=edit&section=3)]

## 1.2. 기본 구성요소와 특징 ¶

KDE의 구성요소로는 우선 Plasma desktop과 윈도우 매니저인 Kwin이 있다. Qt를 사용하고 KDE 핵심부에 깊숙히 들어앉아
있기 때문에 Kwin만 따로 추출해 사용하는 경우는 거의 없지만, 거의 모든 것을 제공한다고 할 수 있을 정도로 다기능이다.
Translucency(Real transparency라고도 한다.), 20개까지 되는 가상 데스크탑에, 심지어 타일링까지 지원하며, 그 외
오만 가지 아이캔디 효과도 지원한다. 처음 KDE를 실행하면 상당히 보수적(?)이며 썰렁하지만, 옵션 창을 하나하나 뒤져 보면 거의 모든
것을 다 바꿀 수 있을 정도로 유동적이다. 바탕화면에도 물론 날씨, 폴더뷰, 달력, 트위터, 페이스북, 일일만화, 기타 등등 다양한 위젯을
놓고 쓸 수 있다. 기본적으로 Air 데스크탑 테마를 사용하는데, 샤워실 유리처럼 뿌옇게 투명하다. 이것도 역시 맘대로 바꿀 수 있다.
**느리고 무거워!**라는 사용자가 많았지만, 버전 4.6부터 매우 빠릿빠릿해졌다.

  

또다른 중요한 특징 중 하나는 GNOME의 Bonobo에 대응되는 Kpart인데, KDE 어플리케이션을 다른 어플리케이션에 임베딩하여 사용
가능하다. GNOME에 비해 상당히 적극적으로 써먹고 있기 때문에, 웹 브라우저/파일 매니저/에디터 등에서 터미널 에뮬레이터인
Konsole을 임베딩하여 사용하기도 하고, 뷰어나 에디터 역시 다른 어플리케이션에 임베딩시키는 등 어플리케이션간의 소통(?)이 매우
원활하다. 설계할 때부터 독립된 어플리케이션이라기보다는 데스크탑 환경의 일부여서 가능한 일이고, 이런 것이 잘 되어 있을수록 보통 통합이 잘
되어 있다고 할 수 있다.

  

그 외에도 거의 모든 단축키를 비롯해서 세팅을 뒤져 보면 GUI 상에서 못 고치는 게 거의 없다. 그리고, 그만큼 옵션이 많고
복잡하다.`[7]` 요즘 유행하는 Semantic desktop에도 열심인데, Nepomuk으로 유저의 모든 데이터를 자동으로 검색해 정리해
놓고 쉽게 찾을 수 있도록 한다. 다만, GNOME에서 사용하는 Zeitgeist`[8]`처럼 "어제 마지막에 들었던 음악 켜" 이런 식으로
찾으면 안된다.`[9]` 어쨌건 디폴트로 켜져 있고, 유저의 홈 디렉토리에 있는 자료들을 Strigi를 이용해서 주기적으로 인덱싱하는데,
이게 I/O뿐 아니라 CPU를 엄청나게 사용한다. 홈 디렉토리에 자료가 적다면 바로바로 끝나니 상관없지만, 자료가 많을 경우는 퍼포먼스에 큰
문제가 된다. 이것으로 인해 문제가 있다면, 완전히 끌 필요는 없고 세팅에서 인덱싱할 디렉토리만 다 꺼주면 된다. 이제부터 KDE에서 주로
사용하는 KDE/Qt 어플리케이션들을 알아보자.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/KDE?action=edit&section=4)]

## 1.3. KDE/Qt 어플리케이션 ¶

[GNOME](GNOME.md)을 비롯한 다수의 리눅스 데스크탑 환경 및 어플리케이션은 Gtk 툴킷을 사용하는 반면, KDE는 오픈소스
진영에서 Qt 프레임워크를 이용하는 몇 안되는 데스크탑 환경이다`[10]`. KDE 어플리케이션은 타 데스크탑 환경의 어플리케이션들에 비해
기능이 뛰어난 것들이 많고, 데스크탑 환경자체로 비교해 봐도 KDE 쪽이 어플리케이션 간의 긴밀한 조합을 허용하여 서로 잘 통합돼 있지만,
이는 반대급부로 다른 단점을 낳는다.

  

대다수의 오픈소스 어플리케이션들은 특정 데스크탑에 종속되지 않아도 대부분 Qt보다는 Gtk 툴킷을 사용하여 만들어진다. 그리고 이들은 같은
Gtk 툴킷을 사용하여 만든 GNOME이나 [Xfce](Xfce.md) 등의 데스크탑 환경에서 별 문제 없이 사용이 가능하나, KDE
환경에서 사용하려면 일단 Gtk 라이브러리를 설치하여 의존성을 해결해야 하고, 실제 사용 시에도 KDE/Qt 앱들에 비해 그래픽이나 폰트가
상당히 이질적이다.`[11]` Gtk 툴킷을 사용한 어플리케이션 중에는 [Emacs](Emacs.md)나 [모질라 파이어폭스](/wik
i/%EB%AA%A8%EC%A7%88%EB%9D%BC%20%ED%8C%8C%EC%9D%B4%EC%96%B4%ED%8F%AD%EC%8A%A4)
, [크롬(웹 브라우저)](%ED%81%AC%EB%A1%AC%28%EC%9B%B9%20%EB%B8%8C%EB%9D%BC%EC%9A%B0%EC%A0%80%29.md) 같은 킬러 앱들도 여럿 있기 때문에 KDE 유저들에겐 짜증나는 일이 아닐 수 없다. <del>KDE/Qt에는
Amarok과 VLC가 있어요 으헣헣</del>`[12]` 물론 QtCurve나 해당 어플리케이션에서 제공하는 테마나 플러그인 등을 이용하면
네이티브 KDE/Qt 앱과 비슷하게 보이게 할 수 있다. 그러나, 그냥 깔면 되는 것과 깔고 나서 이러저러한 설정을 따로 해 줘야 하는 것의
차이는 크다.

  

다행이라면, GNOME이나 Xfce 등 타 데스크탑에 종속된 앱 중에는 KDE 유저들이 간절히 바라는 킬러 앱이란 게 딱히 없다.`[13]`
데스크탑이 제공하는 어플리케이션으로만 따지면 KDE는 이미 다른 웬만한 데스크탑 환경보다 우위에 있다.

  

리눅스 쪽에서 독일 하면, [openSUSE](%EC%98%A4%ED%94%88%EC%88%98%EC%84%B8.md)와 KDE를 가장
먼저 떠올린다.`[14]` 라틴 어원의 단어들에서 영어에서 C로 쓰이는 것을 독어에서는 K로 바꾸어 쓰는 경우가 많은데,`[15]`
비슷하게, KDE 관련 패키지의 이름을 지을 때도 이렇게 영단어를 가져다가 C를 K로 바꿔서 프로그램 이름을 붙이는 경우가 많고, KDE
어플리케이션임을 강조할 때는 **K**Player처럼 아예 영단어 앞에 K를 대놓고 갖다붙이기도 한다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/KDE?action=edit&section=5)]

### 1.3.1. Konqueror ¶

![Konqueror600.png](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/KDE/Konqueror
600.png)

[PNG image (168.09 KB)]

  

콘커러는 KDE에서 가장 중요한 어플리케이션 중 하나로, KDE 올드비들은 콘커러 때문에 KDE를 쓴다는 사람도 많을 정도이다. 간단히
말하자면 유니버설 브라우저이다. 웹 브라우징, 파일 매니저, PDF 뷰어, 포토 뷰어 등 뭔가 읽고 보는 거는 이걸로 다 된다고 보면
간단하다. 거기다가, 사진에서 보이듯이 콘커러 내에서 화면을 마음대로 분할할 수 있다. 워낙 기능이 많다보니 KDE는 복잡하고 어렵다는
편견을 만들어낸 주범 중 하나이지만, KDE 유저들의 사랑을 듬뿍 받고 있다.

  

콘커러에겐 영광이고 KDE에겐 불행인 한 가지는, 콘커러가 바로 KDE의 주력 웹 브라우저면서 동시에 주력 파일 매니저 중 하나라는 것이다.
파일 매니저 부분은 솔직히 문제가 없고 오히려 매우 우수하다고까지 볼 수 있지만, 웹 브라우징 측면에서는 조금 다르다. 콘커러 입장에서는
주력 웹 브라우저가 될 수 있을 수준의 웹 브라우징 능력을 갖고 있다고 콧대를 높일 수도 있겠는데, KDE 입장에서는 대안이 없어서
쓴다고밖에 할 수 없다. 위에서 나열한 Gtk 킬러 앱에 웹 브라우저가 2개나 포함된 것은 우연이 아니다. KDE 유저들이 가장 간절히
바라는 것 중 하나가 파폭 수준의 KDE/Qt 웹 브라우저이다.

  

하지만, 키보드 단축키를 애용하는 고급유저들을 위한 기능만은 오히려 더 우수하다고 볼수도 있는데, 기본 디폴트상태로 hjkl 의 vi-
style 스크롤을 지원한다. 물론, 파폭에도 vimperator 등의 확장기능이 존재하기때문에, 겨우 이정도로 키보드 브라우징이 가능하다고
이야기하는것은 아니고...키보드 브라우징을 할때 가장 짜증나는 부분은, 바로 링크 찾아 누르기이다. 웹페이지에 여러가지 링크가 있을때
마우스를 안쓴다는 가정하에 Tab 으로 순서대로 링크를 돌며 원하는 링크를 선택하는것은 그야말로 PITA 인데, 여기서 콘커러는 빛을
발한다. ctrl 키만 한번 쳐주면, 웹상의 모든 링크(물론, 링크가 너무 많으면 안되겠지만, 웬만한 웹페이지 수준의 웹페이지에서는 문제가
없다.) 아래에 키보드 단축키가 뜨고 해당 단축키만 탁 쳐주면 그 링크로 이동이 가능한 엽기수준에 가까운 기능이 탑재되어있다. 마우스를 전혀
안쓴다 가정할때, 이보다 더 편한 웹브라우저는 찾기 힘들다.

  

콘커러는 자체적으로 만들어 쓰던 [KHTML](KHTML.md) 렌더링 엔진을 이용하는데, 애플사는 바로 이 KHTML을 포크하여
[웹키트](%EC%9B%B9%ED%82%A4%ED%8A%B8.md) 프로젝트를 진행했고, 이는 현재 사파리나 구글 크롬 브라우저에
쓰이고 있다. 그런데, 웹키트는 쌩쌩 잘 돌아가는데 그 모체인 KHTML은 덜그럭거리면서 돌아간다. 콘커러에서도 QtWebkit 을 이용하여
웹브라우징을 할 수는 있지만, KHTML에 비해 안정성이나 웹 페이지 호환성에서 떨어진다.<del>이 부분은 다른 데도 아니고, 웹 환경에서
갈라파고스 반도임을 자랑하는 한국이라 더더욱 중요한 부분이다.</del> 결국, 그냥 KHTML 을 잡고 사는 것이 낫다. 여하튼,
영문사이트로 한정할 경우, 별 문제 없이 주력 웹브라우저로 사용이 가능하긴 하다. 그러나...

  

[[edit](http://rigvedawiki.net/r1/wiki.php/KDE?action=edit&section=6)]

### 1.3.2. Rekonq ¶

![http://rekonq.kde.org/sites/rekonq.kde.org/files/images/Rekonq-0.6.0.png](ht
tp://rekonq.kde.org/sites/rekonq.kde.org/files/images/Rekonq-0.6.0.png)

[[PNG external image]](http://rekonq.kde.org/sites/rekonq.kde.org/files/images
/Rekonq-0.6.0.png)

Rekonq로 본 KDE홈페이지  
[공식 홈페이지](http://rekonq.kde.org/)  
Rekonq는 [웹키트](%EC%9B%B9%ED%82%A4%ED%8A%B8.md)를 기반으로한 [KDE](KDE.md)의 [웹브라우저](%EC%9B%B9%20%EB%B8%8C%EB%9D%BC%EC%9A%B0%EC%A0%80.md)다.  
Kubuntu 10.10에서 Konqueror를 밀어내고 기본 웹 브라우저가 되었다.  
<del>Rekonq에 차이고 Dolphin에 차이는 불쌍한 Konqueror</del>

  

[[edit](http://rigvedawiki.net/r1/wiki.php/KDE?action=edit&section=7)]

### 1.3.3. Dolphin ¶

![Dolphin600.png](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/KDE/Dolphin600.
png)

[PNG image (22.38 KB)]

  

KDE4에서 새로 등장한 파일 매니저로, 콘커러를 제끼고 기본 파일 브라우저가 되었다. 콘커러만큼은 아니지만, 기능이 많은 파일 관리자인데,
대부분의 기능이 렌치버튼 아래의 메뉴에 들어가 있어 컨커러보다 깔끔하고 단순해보이는 UI를 가지고 있다. 참고로, KDE를 이용한 우분투
버전인 쿠분투에서는 콘커러를 아예 없애 버렸다.`[16]` 웹 브라우저는 새로 등장한 [Rekonq](Rekonq.md)를,
파일매니징은 돌핀을 디폴트로 정해 놓았다.

  

돌핀과 콘커러가 흔히 비교 대상이 되곤 하는데, 돌핀은 분명 콘커러에 비해 기능이 적다. 돌핀은 KDE 팀이 KDE4로 들어오며 조금 더
깔끔하고 사용하기 쉬운 UI를 추구하는 흐름에 따라 나온 애플리케이션이기 때문이다. 지나치게 많다는 비판을 듣던 옵션 수를 줄이기 위해서
기능을 일부 쳐냈던 것. 하지만 아무리 기능이 적다고 해도 돌핀은 Thunar, Nautilus 등 타 데스크탑의 파일 관리자에 비해선
월등히 기능이 많다.

  

한편 콘커러가 KDE 올드비 사이에서 많은 팬들을 거느리고 있기 때문에, 돌핀이 등장하자 콘커러가 우선순위에서 밀리게 되는 것 아니냐는
우려를 표하는 사람들이 많다. 현재 개발팀은 돌핀이 콘커러를 대체하기 위한 프로그램이 아니며, KDE를 설치하면 둘 다 설치되니 원하는 것을
선택해서 쓰라는 입장이다. 올드비들에 비해 KDE를 새로 접하는 사람들은 돌핀을 선호하는 경향이 있다.

  

여담이지만 digikam이란 프로그램의 윈도우판을 설치하면 같이 딸려서 설치된다.파일매니징을 digikam 내에서 하게 될 경우엔 돌핀이
튀어나온다는 이야기.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/KDE?action=edit&section=8)]

### 1.3.4. Kontact ¶

![Kontact600.png](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/KDE/Kontact600.
png)

[PNG image (116.02 KB)]

  

이것도 일종의 KDE 킬러 앱인데, KDE PIM(Personal Information Manager) Suite라고도 한다. 위에서 얘기한
Kpart를 적극적으로 이용하여, 개인정보관리에 해당하는 거의 모든 것을 한 군데 모아둔 짬뽕이라 할 수 있다. 메일 클라이언트, 뉴스
리더, 메모장, 달력, 주소록등을 다 모아 놨다. 그런데, 도저히 개인 사용자용이라 보기 힘들 정도로 온갖 기능을 다 넣어 놔서 정말
복잡하다. 여기에 자체적으로 PIM 데이터를 관리하는 데이터베이스를 내장한 Akonadi 서버라는 것까지 돌리고 있으니...할 말이 없다.
게다가, 여러 가지 어플리케이션을 한군데 몰아넣다보니 옵션의 홍수 속에서 허우적거리다 포기하고 썬더버드를 설치하는 사람이 많다. 역시
독일에서 개발한 Kolab 그룹웨어 서버도 지원하는데 이건 문서가 독어로밖에 없다.(...) 여러 모로 기능적인 측면에서도, 난해함이라는
측면에서도 KDE의 정점을 찍는 어플리케이션이다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/KDE?action=edit&section=9)]

### 1.3.5. Kate ¶

![Kate600.png](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/KDE/Kate600.png)

[PNG image (28.31 KB)]

  

GNOME 데스크탑 환경의 gedit과 경쟁하는 에디터이다. 터미널 임베딩도 되고, [Vi](Vi.md) 키맵도 지원하기 때문에 여러
모로 기능은 많다. gedit은 위에서 말한 노틸러스 파일매니저처럼 처음 기능은 미비하지만, 온갖 외부 플러그인으로 중무장하면 Kate와
맞짱뜰 만한 수준으로 변신이 가능하다. 하지만, Kate 의 강점은 그것뿐이 아니다. KDE 데스크탑 환경에서 Kate는 Kpart를 통해
다른 어플리케이션으로 임베딩이 가능하다. 덕분에, 여러 가지 다른 프로그램들에서도 Kate를 에디터 파트로 사용할 수 있고, 실제로 KDE
쪽 문서나 소스 에디팅 관련 어플리케이션은 기본적으로 Kate를 임베딩하여 사용하는 어플리케이션들이 많다. 즉, KDE 환경에서는 다른
프로그램을 사용하여 문서 에디팅을 해도 단축키를 새로 익히거나 할 필요가 없다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/KDE?action=edit&section=10)]

### 1.3.6. Okular ¶

![Okular600.png](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/KDE/Okular600.pn
g)

[PNG image (125.65 KB)]

  

문서 뷰어이다. 만화부터 시작해서 거의 다 볼 수 있고, 리눅스쪽 문서 뷰어 중에서는 최고라는 평도 자주 듣는 관계로, 자세한 설명은
**필요없다**.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/KDE?action=edit&section=11)]

### 1.3.7. Kile ¶

![Kile600.png](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/KDE/Kile600.png)

[PNG image (113.47 KB)]

  

[TeX](TeX.md) 에디터이다. 오픈소스쪽에서 기능의 다양함과 세팅의 디테일한 면에서는 알아주는 TeX 전용 에디터이다. 참고로,
Kile을 만들었던 개발자가 Kile을 떠나서 Texmaker를 만들었는데, 이것은 KDE에 종속되지 않은 Qt 어플리케이션이다. 개발자가
같았던 관계로 인터페이스도 비슷하니, 혹시 GNOME 환경에서 사용하고 싶은 사람은 Texmaker를 알아보자.`[17]` 참고로, Kile
역시 다른 사람이 메인테이너로 활동하고 있기 때문에, 독자적으로 계속 개발되고 있다. 기본적으로, Okular 와 Konsole, Kate를
임베딩하여 사용한다.<del>끝없는 재활용 정신</del>

  

[[edit](http://rigvedawiki.net/r1/wiki.php/KDE?action=edit&section=12)]

### 1.3.8. Gwenview ¶

![Gwenview600.png](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/KDE/Gwenview60
0.png)

[PNG image (243.77 KB)]

  

포토 뷰어이다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/KDE?action=edit&section=13)]

### 1.3.9. Amarok ¶

![Amarok600.png](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/KDE/Amarok600.pn
g)

[PNG image (168.44 KB)]

  

오디오 플레이어. 리눅스 오디오플레이어 순위 설문조사하면 단골로 1위하는 어플리케이션이니만큼, 자세한 설명은 필요없다고 본다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/KDE?action=edit&section=14)]

### 1.3.10. SMPlayer ¶

![SMPlayer600.png](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/KDE/SMPlayer60
0.png)

[PNG image (212.15 KB)]

  

<del>영상 내용이 신경쓰이면 지는거다</del>

  

이것도 리눅스 쪽에서는 말이 필요없는 최고의 [MPlayer](MPlayer.md) 프론트엔드이다. KDE 어플리케이션은 아니지만,
Qt 어플리케이션이라 문제없이 사용가능하다. 이외에 [VLC](VLC.md) 역시 Qt 어플리케이션이다. KDE 어플리케이션중에는
[KMPlayer](KMPlayer.md)와 KPlayer`[18]` 등의 MPlayer 프론트엔드가 존재하는데, KDE
어플리케이션으로서 콘커러등에 임베딩시켜 사용이 가능한 장점이 있지만, 순수 프론트엔드로서의 기능 면에서는 아무래도 SMPlayer에 비해
떨어진다. 이외에 MPlayer가 아닌 [xine](xine.md)을 백엔드로 하는 [Kaffeine](Kaffeine.md)도
비디오 플레이어로 많이 쓰인다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/KDE?action=edit&section=15)]

### 1.3.11. Marble ¶

![Marble600.png](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/KDE/Marble600.pn
g)

[PNG image (449.48 KB)]

  

많은 찬사를 받는 어플리케이션 중 하나이다. 그냥 여러 가지 지구본들이 있고, 이리저리 돌리면서 찾아보는 건데, 인터넷과 연동돼서 매우
자세한 곳까지 확대해서 볼 수 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/KDE?action=edit&section=16)]

### 1.3.12. KTorrent ¶

![KTorrent600.png](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/KDE/KTorrent60
0.png)

[PNG image (62.05 KB)]

  

기능도 많고 세팅도 디테일하게 할 수 있으며, 오만 가지 플러그인에 스크립트도 지원하는 강력한 토렌트 클라이언트이다. KDE에서 토렌트
클라이언트는 KTorrent만 믿고 가자.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/KDE?action=edit&section=17)]

### 1.3.13. KOffice ¶

![http://www.koffice.org/wp-content/uploads/2009/05/multiple_master_slides-
489x350.png](http://www.koffice.org/wp-content/uploads/2009/05
/multiple_master_slides-489x350.png)

[[PNG external image]](http://www.koffice.org/wp-content/uploads/2009/05
/multiple_master_slides-489x350.png)

  

[오픈오피스](%EC%98%A4%ED%94%88%EC%98%A4%ED%94%BC%EC%8A%A4.md)와
[리브레오피스](%EB%A6%AC%EB%B8%8C%EB%A0%88%EC%98%A4%ED%94%BC%EC%8A%A4.md) 의 대항마격인
KDE 의 오피스 수트이다. 현재는 Calligra Suite 라는 이름으로 새로이 개발중인데, 아직 베타 버전이고 정식 버전은 등장하지
않았다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/KDE?action=edit&section=18)]

### 1.3.14. KDevelop ¶

![http://scr3.golem.de/screenshots/1005/KDevelop4.0/kdevelop_0.png](http://scr
3.golem.de/screenshots/1005/KDevelop4.0/kdevelop_0.png)

[[PNG external
image]](http://scr3.golem.de/screenshots/1005/KDevelop4.0/kdevelop_0.png)

  

강력한 통합개발환경. 현존하는 리눅스 IDE중에서는 가장 완성도가 높다.  
C/C++외에도 Java, Ruby등등 다양한 통합개발환경을 지원한다. QT개발환경과 궁합이 잘 맞는다.  
[Eclipse](Eclipse.md)로 C/C++개발환경 만들려 삽질하지말고 이것을 쓰자.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/KDE?action=edit&section=19)]

# 2. 게임회사 Konami Digital Entertainment ¶

[코나미](%EC%BD%94%EB%82%98%EB%AF%B8.md) 항목 참조

`\----`

  * `[1]` KDE 3 시절까지 KDE를 사용하던 사람들이 KDE 4 초기에 엄청난 UI 변화와 많은 버그를 견디지 못하고 이탈한 경우도 많으니, 새로운 UI는 사용자에 따라 호불호가 갈리는 듯하다. 현재 버그는 많이 줄어들었다.
  * `[2]` KDE를 위시한 리눅스 UI 팀들이 이런걸 안한다는건 아니다.단지 타 기업의 UI 팀에 비해서는 체계적인 데이터를 쌓는 등의 작업은 어렵다는 뜻이다.실제로 그나마 GUI 철학이나 디자인요소의 가이드라인이라도 문서로 존재하는 Gnome3에 비해 KDE는 그런 부분의 문서화는 상당히 부실하다.
  * `[3]` 물론 이후 그놈3을 기반으로 뜯어고친 유니티가 이런 비판을 다 흡수해(..) 버리면서 상대적으로 비판자체는 좀 덜하게 되었으나 그놈 3 자체를 그대로 적용시킨 배포판이 얼마 없다는것을 상기하면 별로 좋은 상태는 여전히 아니다.인기가 좋은 리눅스민트나 우분투같은 배포판은 여전히 UI를 뜯어고쳐 적용시키고 있으며 비판받는 유니티마저도 UI가 마음에 안든다기보단 불안정하고 무거워서 비판받는것임을 생각해보자.
  * `[4]` 다만 본 문단만 보고 Gnome3에 대해 판단하는 것은 매우 편협한 시각으로 이어지므로 주의가 필요하다. 그놈 쉘은 익스텐션을 이용해 기능을 수정, 추가 또는 제거(!)할 수 있으며, 유저의 피드백을 받아가며 UI요소에 상당한 양의 수정을 가하고 있다. 또한 Gnome3에 기반한 데스크톱 환경이 우후죽순처럼 나타나는 현상은 그 자체로 Gnome3의 모듈화와 확장성이 뛰어나다는 반증이기도 하다.
  * `[5]` 덧붙여서 우분투는 Gnome3의 UI를 뜯어고쳐 적용한 적이 없다. 우분투에 적용된 Unity가 Gnome3의 변종처럼 오해되곤 하는데, Unity는 Gnome3보다는 Gnome2와 공유하는 코드가 더 많다. 당장 적용된 WM만 봐도 Metacity가 아니라 Compiz다. 착각하지 말자. 게다가 우분투 그놈 리믹스는 Gnome3에 최소한의 수정을 가해서 우분투에 적용하는 것을 목표로 삼고 있다. 다만 Unity도 Unity8로 넘어가면서 QT와 Mir/XMir 기반으로 갈아타며 GTK와의 코드 공유가 상당히 줄어들 예정이기에, 선술된 Unity에 대한 설명은 Unity8이 적용되기 이전의 우분투, 즉 Ubuntu Desktop Edition의 13.10 또는 그 이전 버전에 대해서만 참이다.
  * `[6]` 타블렛 PC의 타블렛 말고 와콤 등지의 회사에서 나오는 그림용 입력장치.
  * `[7]` 희귀한 리눅스 그래픽 작업자(..)들은 때문에 KDE를 조금 더 선호하기도 하는데,이유는 상당히 단순하게도 KDE쪽의 타블렛 GUI가 윈도우에 거의 비등하게 옵션을 제공하기 때문.유니티 등에서 근래에 지원해주기 시작한 와콤 타블렛 GUI도 있기는 하나 듀얼모니터 환경에서 여러가지 에로사항을 아직 해결하지 못했기 때문에 그런 부분에서 KDE는 확실한 우위를 가지고 있다.단 설치시 이상한 에러들을 뿜어내 삽질하게 만드는건..리눅스 사용자의 필연이니 어쩔 수 없을것이다(..)또 국내 개인 사용자 대상으로 많이 쓰이는건 데비안 계열 배포판들인데 KDE를 사용한 배포판중 듀얼모니터가 제대로 잡히는 배포판이 생각보다 별로 없다.듀얼모니터 타블렛 사용때문에 쓰는 KDE인데 못잡으면(..)여기 쓰기엔 한도끝도 없지만 멀티미디어 작업을 위해 리눅스를 운용하면 서버나 일반사용자와는 여러가지로 다른 필요성이 많아지기에(ex : 미디 작업시 반드시 써야하는 jack은 관리자 권한으로 실행 안하면 스타트 자체가 안되며 VSTi의 경우 관리자권한으로 불러와야만 되는 DAW가 많다)배포판 선택에 여러 에로사항을 만드는 경우가 많다.
  * `[8]` 독일어로, 직역하면 시간정신, 의역하면 시대정신쯤 된다. 
  * `[9]` KDE에서도 Nepomuk에 더해 Zeitgeist를 사용할 거라고 들었다.
  * `[10]` 우분투가 11.04버전 부터 GNOME 대신 기본으로 돌리고 있는 Unity 또한 Gtk가 아닌 Qt 기반이다.
  * `[11]` 반대로, 이것은 GNOME 환경에서 KDE 애플리케이션을 실행하도 마찬가지이다.
  * `[12]` 역으로 이는 Gnome/Gtk 측의 문제이기도 하다. 리눅스 데스크탑 라이브러리가 크게 Qt와 Gtk로 양분되어 있<del>고 서로 Editor war 비슷한 전쟁을 치르고 있</del>기 때문에, 둘 중 하나만 사용하던 유저가 어떤 프로그램 하나만 깔자고 라이브러리 하나를 통째로 깔아야 하는 상황이 발생한다.
  * `[13]` Emacs나 파이어폭스같은 것들은 비록 Gtk 툴킷을 사용했지만, 특정 데스크탑에 종속되지 않은 독립적인 어플리케이션이기에 겉모습만 수정하면 문제없이 사용가능하다. 하지만, 특정 데스크탑에 종속된 어플리케이션의 경우, 해당 데스크탑 내에서 다른 어플리케이션들과 긴밀한 관계를 가질 가능성이 있고, 이렇게 되면 문제는 더 커진다.
  * `[14]` 그리고, 대부분의 메이저 리눅스 배포판들이 [GNOME](GNOME.md)을 기본으로 채택하고 있는 것과 달리, openSUSE의 디폴트 데스크탑 환경은 KDE이다.
  * `[15]` Communication => Kommunikation이고, Conversation => Konversation, Command => Kommando, Condition => Kondition 등
  * `[16]` 물론, 원하면 수동으로 인스톨해서 깔 순 있다.
  * `[17]` 다른 데스크탑 환경에서 사용할경우, KDE 의존보다는 Qt 의존이 낫다. Kile 인스톨하면 콘커러, Konsole 등이 의존으로 다 따라온다. 
  * `[18]` KPlayer 는 현재 장기간 업데이트가 되지 않고 있기때문에 데드 프로젝트라고 볼 수 있다. 

