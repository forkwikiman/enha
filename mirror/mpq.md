MPQ(MoPaQ)

## Contents

    

1. MPQ란? 
2. MPQ 압축이 사용된 게임 
3. MPQ 개조 
4. MPQ 개조를 통한 MOD 명작품들 
    

4.1. 스타크래프트

    

4.1.1. 건담크래프트

4.1.2. 포켓몬크래프트

4.1.3. 폴른 엔젤

4.2. 워크래프트

4.3. 기타 다른 작품

5. 개조를 통한 문제점 
6. MPQ를 통해 알 수 있는 것들 
7. 보안 문제 

[[edit](http://rigvedawiki.net/r1/wiki.php/mpq?action=edit&section=1)]

# 1. MPQ란? ¶

MPQ 포맷이란 "MoPaQ"으로 불리며 블리자드에서 직접 개발한 데이터 압축 포맷이다. 대개 모든 게임 회사에서 독자적으로 데이터 압축
포맷을 만들어 데이터 파일들의 단일화와 게임 데이터의 안정성, 보안성(게임의 무단 수정 방지를 위한)을 목적으로 한다. **<del>지만
이미 털린지 오래</del>** (대표적으로 [수도꼭지](%EB%B0%B8%EB%B8%8C%20%EC%BD%94%ED%8D%BC%EB%A0%88%EC%9D%B4%EC%85%98.md)의 GCF 포맷) 사실 유명 게임사들은 자체적으로 압축 포맷을 만들어 그 안에 게임
데이터들을 몽땅 집어 넣는다. [이드 소프트웨어](%EC%9D%B4%EB%93%9C%20%EC%86%8C%ED%94%84%ED%8A%B8%EC%9B%A8%EC%96%B4.md)가 [둠시리즈](%EB%91%A0%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md)에서 이러한 방식(WAD파일)을 정립시켰으며,
요즘 나오는 게임들은 전부 이런 방식이다. 심지어 [성진국](%EC%9D%BC%EB%B3%B8.md)의
[에로게-무](%EC%97%90%EB%A1%9C%EA%B2%8C.md)도 이런 방식을 쓰는 게임들이 있다. <del>하지만 나온지 얼마
안되어 모두 뜯기고 뜯겨버린다.</del>

  

[히어로즈 오브 더 스톰](%ED%9E%88%EC%96%B4%EB%A1%9C%EC%A6%88%20%EC%98%A4%EB%B8%8C%20%EB%8D%94%20%EC%8A%A4%ED%86%B0.md)부터는 근 20년 동안 써온 MPQ파일을 버리고 새로이 개발한
CASC(Content Addressable Storage Container) 압축 방식이 사용된다. 기존 MPQ 포맷보다 유지, 보수,
속도, 확장성 면에서 비약적으로 발전된 포맷이라고 한다. [월드 오브 워크래프트](%EC%9B%94%EB%93%9C%20%EC%98%A4%EB%B8%8C%20%EC%9B%8C%ED%81%AC%EB%9E%98%ED%94%84%ED%8A%B8.md)도 [드레노어의 전쟁군주](/
wiki/%EB%93%9C%EB%A0%88%EB%85%B8%EC%96%B4%EC%9D%98%20%EC%A0%84%EC%9F%81%EA%B5%
B0%EC%A3%BC)부터는 이 압축방식을 사용한다고 한다.
<http://www.inven.co.kr/webzine/news/?news=107573>

  

[[edit](http://rigvedawiki.net/r1/wiki.php/mpq?action=edit&section=2)]

# 2. MPQ 압축이 사용된 게임 ¶

\- [디아블로](%EB%94%94%EC%95%84%EB%B8%94%EB%A1%9C.md)  
\- [워크래프트 2](%EC%9B%8C%ED%81%AC%EB%9E%98%ED%94%84%ED%8A%B8%202.md) (배틀넷
에디션)  
\- [스타크래프트](%EC%8A%A4%ED%83%80%ED%81%AC%EB%9E%98%ED%94%84%ED%8A%B8.md)  
\- [디아블로 2](%EB%94%94%EC%95%84%EB%B8%94%EB%A1%9C%202.md)  
\- [워크래프트 3](%EC%9B%8C%ED%81%AC%EB%9E%98%ED%94%84%ED%8A%B8%203.md)  
\- [월드 오브 워크래프트](%EC%9B%94%EB%93%9C%20%EC%98%A4%EB%B8%8C%20%EC%9B%8C%ED%81%AC%EB%9E%98%ED%94%84%ED%8A%B8.md)  
\- [스타크래프트2](%EC%8A%A4%ED%83%80%ED%81%AC%EB%9E%98%ED%94%84%ED%8A%B8%202.md)  
\- [디아블로 3](%EB%94%94%EC%95%84%EB%B8%94%EB%A1%9C%203.md)

<del>(어차피 블리자드 게임일 뿐이잖아!!!)</del>  

\- 로드 오브 매직`[1]`  

[[edit](http://rigvedawiki.net/r1/wiki.php/mpq?action=edit&section=3)]

# 3. MPQ 개조 ¶

구글 검색을 통하여 MPQ 관련 도구(WinMPQ 등등)를 받아서 MPQ 파일의 내부를 편집할 수 있다. 블리자드 게임의
[MOD](MOD.md)를 만들 생각이라면 해당 게임의 데이터가 어떠한 파일들로 이루어져있는지, 해당 파일이 무슨 역할을 하는지, 해당
파일의 편집을 위해선 어떠한 프로그램을 이용해야할지를 알아야 한다. **<del>당연한가</del>**

  

3가지를 제대로 꿰뚫고 있다면 절대로 개조는 [어렵지않아요~](%EC%82%AC%EB%A7%88%EA%B7%80%20%EC%9C%A0%EC%B9%98%EC%9B%90.md), 또한 개조의
묘한 중독에 빠져들게 된다.`[2]`

  

[[edit](http://rigvedawiki.net/r1/wiki.php/mpq?action=edit&section=4)]

# 4. MPQ 개조를 통한 MOD 명작품들 ¶

  

최고조로 유행했던 때는 **스타드래프트**`[3]`를 통해 사용자가 직접 스타크래프트1의 데이터를 수정하던 시절이었다.`[4]`

  

[[edit](http://rigvedawiki.net/r1/wiki.php/mpq?action=edit&section=5)]

## 4.1. 스타크래프트 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/mpq?action=edit&section=6)]

### 4.1.1. 건담크래프트 ¶

![gundam.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/mpq/gundam.jpg)

[JPG image (220.47 KB)]

  

[[edit](http://rigvedawiki.net/r1/wiki.php/mpq?action=edit&section=7)]

### 4.1.2. 포켓몬크래프트 ¶

![http://img.blog.yahoo.co.kr/ybi/1/29/ca/photoshop0909/folder/3/img_3_95_0?12
71038187.jpg?width=570&height=410](http://img.blog.yahoo.co.kr/ybi/1/29/ca/pho
toshop0909/folder/3/img_3_95_0?1271038187.jpg)

[[JPG external image]](http://img.blog.yahoo.co.kr/ybi/1/29/ca/photoshop0909/f
older/3/img_3_95_0?1271038187.jpg)

  
<del>[넌 내꺼야</del>!](%ED%8F%AC%EC%BC%93%EB%AA%AC%EC%8A%A4%ED%84%B0.md)

  

[[edit](http://rigvedawiki.net/r1/wiki.php/mpq?action=edit&section=8)]

### 4.1.3. 폴른 엔젤 ¶

이를 응용하여 바다건너 [쌀국](%EB%AF%B8%EA%B5%AD.md)에선 스타크래프트 비공식 확장팩`[5]`이 만들어져 나오기도
했다. 놀라운 점은 완성도도 어느 정도 있으며 게임의 미션, 게임의 인물묘사(메뉴버튼 밑의 그림), 음악등을 순수 제작하였다는 것. (자세한
얘기는 [엔하위키 Fallen Angel 참조](Fallen%20Angel.md))

  

![http://images1.wikia.nocookie.net/__cb20071221062509/lotc/images/thumb/a/a4
/Fallenangel-title.jpg/500px-Fallenangel-title.jpg](http://images1.wikia.nocoo
kie.net/__cb20071221062509/lotc/images/thumb/a/a4/Fallenangel-title.jpg/500px-
Fallenangel-title.jpg)

[[JPG external image]](http://images1.wikia.nocookie.net/__cb20071221062509/lo
tc/images/thumb/a/a4/Fallenangel-title.jpg/500px-Fallenangel-title.jpg)

  
  

[[edit](http://rigvedawiki.net/r1/wiki.php/mpq?action=edit&section=9)]

## 4.2. 워크래프트 ¶

워크래프트 3 데이터를 개조해 스타크래프트를 3D화한 프로젝트 레볼루션<del>([절대 이게 아니다](%EB%93%9C%EB%9E%98%EA%B3%A4%EB%B3%BC%20%EC%97%90%EB%B3%BC%EB%A3%A8%EC%85%98.md))</del>

  

![http://www.freewebs.com/deathlord3000/shotty3.jpg?width=570&height=410](http
://www.freewebs.com/deathlord3000/shotty3.jpg)

[[JPG external image]](http://www.freewebs.com/deathlord3000/shotty3.jpg)

  
<del>우와아...</del>

  

[워크래프트 3](%EC%9B%8C%ED%81%AC%EB%9E%98%ED%94%84%ED%8A%B8%203.md)를
[스타크래프트](%EC%8A%A4%ED%83%80%ED%81%AC%EB%9E%98%ED%94%84%ED%8A%B8.md)의 모든
내용으로 바꿔치운 것이기 때문에 [블리자드 엔터테인먼트](%EB%B8%94%EB%A6%AC%EC%9E%90%EB%93%9C%20%EC%97%94%ED%84%B0%ED%85%8C%EC%9D%B8%EB%A8%BC%ED%8A%B8.md)으로 부터 저작권 문제를 걸지 않을까 우려가
있었지만 [스타크래프트](%EC%8A%A4%ED%83%80%ED%81%AC%EB%9E%98%ED%94%84%ED%8A%B8.md)
CD, [워크래프트 3](%EC%9B%8C%ED%81%AC%EB%9E%98%ED%94%84%ED%8A%B8%203.md) CD에서
파일을 받아서 설치하는 방식, 그러니까 이 두 게임 CD가 있어야 설치가 되도록하여 아무런 문제가 되지 않았다.

[[edit](http://rigvedawiki.net/r1/wiki.php/mpq?action=edit&section=10)]

## 4.3. 기타 다른 작품 ¶

저 멀리 [쌀국](%EB%AF%B8%EA%B5%AD.md)의 CampaignCreations.org 라는 사이트를 방문하게 되면 폴른
엔젤을 비롯 다양한 스타크래프트 MOD를 볼 수 있다.
[CampaignCreations(영문)](http://www.campaigncreations.org)

  

아래 사이트는 워크래프트3 사이트.  
[Warcraft III Campaigns(영문)](http://www.wc3c.net)

  

디아블로2의 MOD도 존재한다. 네이버에 전문 카페도 존재하나.. 활성화 상태는 <del>안습</del>인 듯  
[네이버 디아블로2 모드카페](http://cafe.naver.com/modcafe)

  
  

[[edit](http://rigvedawiki.net/r1/wiki.php/mpq?action=edit&section=11)]

# 5. 개조를 통한 문제점 ¶

아무래도 블리자드가 직접 만든 것이 아닌 아마추어들이 제작하였기 때문에 게임 구동에 있어서 불안정하였다. 건담크래프트같은 경우 게임 중 튕길
때가 많았다. 민감한 데이터를 잘못 수정할 시 그렇다. 또한 배틀넷을 통한 멀티플레이에 충돌을 일으키는 경우가 있다. (한쪽은 MOD,
한쪽은 정식버전일 경우 등)

  

또한, 스타크래프트 2 같은 경우 MPQ를 수정할 경우 로그인 자체가 안 되는 경우가 있다. (...)

  

[[edit](http://rigvedawiki.net/r1/wiki.php/mpq?action=edit&section=12)]

# 6. MPQ를 통해 알 수 있는 것들 ¶

해당 게임의 정식판에 나오지 않은 유닛`[6]`이나 미션, 정보, 혹은 다음 패치 때 나오게 될 중요한 정보를 미리 볼 수 있는 경우가
있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/mpq?action=edit&section=13)]

# 7. 보안 문제 ¶

[월드 오브 워크래프트](%EC%9B%94%EB%93%9C%20%EC%98%A4%EB%B8%8C%20%EC%9B%8C%ED%81%AC%EB%9E%98%ED%94%84%ED%8A%B8.md)가 출시되기 전 세대들의 작품(스타크래프트1, 디아블로2, 워크래프트3)들의 경우 일부
MPQ 파일에(stardat.mpq, d2sfx.mpq, d2char.mpq, war3.mpq, war3x.mpq 등) 사용자의
[시디키](%EC%8B%9C%EB%94%94%ED%82%A4.md)`[7]` 정보가 저장되어 있다. 이를 악용한 외국의 프로그래머들이
MPQ 내부에 접근하여 시디키만 추출하는 프로그램을 제작/배포하였다. 덕분에 한동안 PC방 폐인, 중고딩들이 집에서 배틀넷을 즐기기 위해
PC방에서 시디키 추출 프로그램을 통해 시디키를 유출`[8]`시켜 자신의 집에서 사용하거나 와레즈에 등록하는 등 대량으로 시디키가 유출되어
친구들과 PC방에서 배틀넷 플레이를 위해 접속하는 순간.. **"이 시디키는 이미 사용 중입니다."** 메시지를 자주 볼 수
있었다.`[9]` <del>[야신난다!](%EC%95%BC%20%EC%8B%A0%EB%82%9C%EB%8B%A4%21.md)</del>

  

이러한 문제를 해결하기 위해 [스타크래프트2](%EC%8A%A4%ED%83%80%ED%81%AC%EB%9E%98%ED%94%84%ED%8A%B8%202.md)`[10]`부터는
계정 등록제를 통해 자신의 계정에 게임 시디키를 등록하여 게임을 등록하고, 게임을 설치할 땐 시디키가 필요없게 되었다. 대신 해당 게임의
시디키가 등록된 계정을 로그인 해야 게임을 이용할 수 있다. 이런 통합과정을 통해 블리자드의 모든 게임들이 계정에 등록되어 있는 상태에서
핵을 쓰다 계정을 정지 당하면...
<del>[망했어요](%EB%A7%9D%ED%96%88%EC%96%B4%EC%9A%94.md)</del>

`\----`

  * `[1]` Lords of Magic. 판타지 배경의 턴제/실시간 전략 시뮬레이션으로서 '97년도에 [시에라 엔터테인먼트](%EC%8B%9C%EC%97%90%EB%9D%BC%20%EC%97%94%ED%84%B0%ED%85%8C%EC%9D%B8%EB%A8%BC%ED%8A%B8.md)에서 발매했다. 때문에 이 작품만은 블리자드와 무관하면서도 MPQ 포맷을 사용한 유일한 케이스라고 말할 수 있다. <del>근데, 시에라가 [액티비전-블리자드](%EC%95%A1%ED%8B%B0%EB%B9%84%EC%A0%84-%EB%B8%94%EB%A6%AC%EC%9E%90%EB%93%9C.md)에 흡수돼버렸잖아, 블자 아니면 [안 될 거야 아마](%EC%95%88%20%EB%90%A0%20%EA%B1%B0%EC%95%BC%20%EC%95%84%EB%A7%88.md)</del>
  * `[2]` 사용자가 해당 파일에 맞는 도구를 통해 내용을 수정한 후 다시 MPQ로 봉인하면 사용자가 원하는 대로 수정이 가능하다.
  * `[3]` 스타크래프트 MOD 도구였다. 이 도구를 이용해 만들어진 대표적인 MOD로는 건담크래프트, 포켓몬크래프트 등이 있다.
  * `[4]` 이 시기엔 MPQ를 직접 개조했다고 하긴 좀 그렇다. 스타드래프트를 통해 만들어진 EXE파일을 로드하는 방식이였다.
  * `[5]` 미국 NexusCore 에서 제작한 스타크래프트: 폴른 엔젤 등이 있다. 그러나 이 것도 시리즈의 일부분일 뿐...
  * `[6]` 스타크래프트의 경우 Independent Starport 등, 데이터 상으로만 존재하는 숨겨진 정보들이 존재한다.
  * `[7]` 대규모 멀티플레이어 서비스인 배틀넷을 이용하기 위한 코드를 말한다. 윈도우의 제품번호같은 개념
  * `[8]` 엄연한 절도 행위다.
  * `[9]` PC방에서 제대로 배틀넷을 이용할 수 없을 정도였다.
  * `[10]` 블리자드는 외국에서는 와우부터, 국내에서는 스타크래프트 2부터 계정등록제를 사용하기 시작했다. 그 이유는 와우의 클라이언트 배포 방식이 다르기 때문이다. 외국에서는 패키지 게임 사듯이 클라이언트 패키지를 구입, 시디키를 계정에 등록해서 사용해야 하지만 국내에서는 클라이언트를 무료로 배포한다. 이 때문에 와우는 국내에서는 시디키 등록 과정이 필요없다.

