  * 관련 항목 : [게리 모드](%EA%B2%8C%EB%A6%AC%20%EB%AA%A8%EB%93%9C.md)
  * [TTT 공식 홈페이지](http://ttt.badking.net/)  

![Example.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Trouble_20In_20Ter
rorist_20Town/Example.jpg)

[JPG image (29.04 KB)]

  

**한 유저의 TTT 가이드영상.**

  * 수상 쩍으면, 탄창을 비워라.(갈겨라)
  * 언제나 탈출로를 확보하라.
  * 무죄인끼리 싸우도록 둬라.
  * C4를 찾기 못하는곳에 둬라.
  * 함정 방을 조심하라.
  * 프롭(물건)을 믿지마라.
  * GM_Construct 맵에서 플레이하지마라.`[1]`  
  

[게리 모드](%EA%B2%8C%EB%A6%AC%20%EB%AA%A8%EB%93%9C.md)의 인기 게임모드 중 하나로, **Bad
King Urgrain**`[2]`이 제작한 [마피아](%EB%A7%88%ED%94%BC%EC%95%84.md) 게임 비슷한
게임모드이다. [게리 모드](%EA%B2%8C%EB%A6%AC%20%EB%AA%A8%EB%93%9C.md)의 Lua 프로그래밍 언어를
사용하였으며, [카운터 스트라이크: 소스](%EC%B9%B4%EC%9A%B4%ED%84%B0%20%EC%8A%A4%ED%8A%B8%EB%9D%BC%EC%9D%B4%ED%81%AC%3A%20%EC%86%8C%EC%8A%A4.md)의
[캐릭터](%EC%BA%90%EB%A6%AD%ED%84%B0.md)와 [무기](%EB%AC%B4%EA%B8%B0.md) 모델을
사용한다. [카운터 스트라이크: 소스](%EC%B9%B4%EC%9A%B4%ED%84%B0%20%EC%8A%A4%ED%8A%B8%EB%9D%BC%EC%9D%B4%ED%81%AC%3A%20%EC%86%8C%EC%8A%A4.md)와 [게리모드](%EA%B2%8C%EB%A6%AC%20%EB%AA%A8%EB%93%9C.md) 둘 다 설치되어있어야 하며, 그렇지 않으면
[보라돌이](%EB%B3%B4%EB%9D%BC%EB%8F%8C%EC%9D%B4.md) 현상이 극심하게 발생한다. TTT 모드는 [게리모드](%EA%B2%8C%EB%A6%AC%20%EB%AA%A8%EB%93%9C.md) 내에 _기본적으로 내장_되어 있다.

2010년 [게리 모드](%EA%B2%8C%EB%A6%AC%20%EB%AA%A8%EB%93%9C.md) Fretta Contest에서
**최우수작**으로 선정되었다. 2등은 Dogfight Arcade, 3등은 Prop Hunt.

## Contents

    

1. TTT란? 
2. 게임 플레이 
    

2.1. Haste Mode <del>빡친시간</del>

2.2. 시체 확인

2.3. 특수 상점

3. 아이템 
    

3.1. 공용 아이템(배신자,탐정)

    

3.1.1. 방탄복 (Body Armour)

3.1.2. 레이더 (Radar)

3.1.3. 텔레포터 (Teleporter)

3.2. 트레이터 전용 아이템

    

3.2.1. 칼 (Knife)

3.2.2. C4

3.2.3. 라디오 (Radio)

3.2.4. 위장기 (Disguiser)

3.2.5. 소음 권총 (Slienced Pistol)

3.2.6. 교란기 (Decoy)

3.2.7. 발화 권총 (Flare Gun)

3.2.8. 뉴턴 런처 (Newton Launcher)

3.2.9. 폴터가이스트 (Poltergeist)

3.3. 탐정 전용 아이템

    

3.3.1. DNA 스캐너 (DNA Scanner)

3.3.2. 의료 기기 (Health Station)

3.3.3. 비쥬얼라이저 (Visualizer)

3.3.4. 쌍안경 (Binoculars)

3.3.5. UMP .45 프로토타입 (UMP .45 Prototype)

3.3.6. 해체 킷 (Defuser)

4. 클래스 
    

4.1. 무죄인 (Innocent)

4.2. 배신자 (Traitor)

4.3. 탐정 (Detective)

[[edit](http://rigvedawiki.net/r1/wiki.php/Trouble%20In%20Terrorist%20Town?act
ion=edit&section=1)]

## 1. TTT란? ¶

일반적으로 _마피아 게임_이라 불린다. 3가지 클래스가 존재하며 이들 속에서 각자의 역할을 완수하는것이 목표이다.

  

일반적으로 대다수가 선정되는 **무죄인**과 무죄인의 대장 격인 **탐정**, 겉보기에는 무죄인이지만 속은 <del>시뻘겋게</del> 다른
**배신자**가 있다.

  

**배신자**는 라운드 시간 내에 **몰래 죽이든 대놓고 죽이든** 배신자 외 나머지 플레이어를 [올킬](%EC%98%AC%ED%82%AC.md)해야 한다. 일반적으로 가만히 있으면 평범한 무죄인으로 보이지만, 대놓고 무죄인들을 죽이다가 **발각**되면, **자신이 _범인_으로 지목되어** 무죄인들과 탐정들에게서 맹추격을 받는다. 채팅기능과 보이스기능, 퀵라디오 기능으로 빠르게 의사전달이 가능하기 때문에 치밀한 계획과 재빠른 행동이 중요하다.  
(탐정과 배신자는 특수 물품을 크레딧(Credit)을 이용해 **C** 키를 눌러 특수 상점에서 구매할 수 있다.)

  

한국 [게리모드](%EA%B2%8C%EB%A6%AC%EB%AA%A8%EB%93%9C.md)서버 중 몇개가 TTT서버로 구동중이며,
사람이 많이 몰리는 편이다.

  

일반적으로 통용되는 기본 룰로는 **프리킬`[3]` 금지**(배신자라는 증거 없이 사살했을 경우), **탐정명령 복종**(해괴한 명령이나
너무 심한 수준 외), **위협사격 금지**(탐정에게 대부분 해당) 등이 있다. (서버마다 차이가 있을수 있음)  
기본 룰과 서버마다 걸려있는 서버 룰을 지키지 않으면 _밴_ 당하기 일쑤이니 한번 쯤은 MOTD를 보는것이 좋다.

[[edit](http://rigvedawiki.net/r1/wiki.php/Trouble%20In%20Terrorist%20Town?act
ion=edit&section=2)]

## 2. 게임 플레이 ¶

게임의 라운드가 시작되면, 모든 플레이어는 클래스를 부여받는다. 일반적으로 탐정은 6명마다 1명씩, 배신자는 3명마다 1명씩 부여되는것으로
알려져있다. 라운드가 시작되면 각각 클래스는 <del>서로를 죽이고 숨기는</del> 플레이를 할 수 있게 된다.

  

무죄인은 탐정과 협력하여 라운드시간이 끝날때까지 생존해야하며, 탐정은 진짜 무죄인을 찾아내고 배신자를 죽여야한다. 배신자는 배신자 빼고 그냥
[싹쓸이](%EC%8B%B9%EC%93%B8%EC%9D%B4.md)하면 된다.

  

**라운드가 끝나면**, 어떤 클래스가 이겼는지 뜨고, 누가 누구를 언제,어떻게 죽였는지 표시되며, 잘못된 사살도 표시된다.(프리킬 등), 각각 사람마다 부여된 클래스도 모조리 표시된다. **단,** 시간 초과로 무죄인이 승리했을때는 **죽은 사람 외**의 배신자는 누구인지 표시되지 않는다. <del>연기 실력을 감추기 위한 것이었다</del>

[[edit](http://rigvedawiki.net/r1/wiki.php/Trouble%20In%20Terrorist%20Town?act
ion=edit&section=3)]

### 2.1. Haste Mode <del>빡친시간</del> ¶

![AR.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Trouble_20In_20Terroris
t_20Town/AR.jpg)

[JPG image (15.39 KB)]

기본적으로 정해진 라운드 시간 외에도, **Haste Mode**(간단하게 연장시간)라고 해서 배신자가 무죄인이나 탐정을 죽이면 몇십초씩
라운드 시간이 연장되는데, 무죄인과 탐정에게는 기본 라운드시간만 표시되고, 배신자에게는 **라운드시간+Haste Mode 시간**이 된다.
(10초마다 기본 라운드시간, Haste Mode 시간이 번갈아 표시된다. 뭔가 [구라](%EA%B5%AC%EB%9D%BC.md)를
칠때 유용하다.)

  

Haste Mode 시간이 되면, 무죄인과 탐정의 시간표시에는 **OVER TIME**이라고 표시되면서, <del>끝없이</del> 게임이
계속 진행된다. 끝나는 시간은 배신자만 알 수 있으므로, 이 시간에는 최대한 조심해야 한다.

[[edit](http://rigvedawiki.net/r1/wiki.php/Trouble%20In%20Terrorist%20Town?act
ion=edit&section=4)]

### 2.2. 시체 확인 ¶

누군가 죽으면, 시체가 남는다. 이는 [발화권총](%EB%B0%9C%ED%99%94%20%EA%B6%8C%EC%B4%9D.md)(Flare Gun)으로 없애지 않는 이상, 맵에서
계속 존재하게 된다.  
_아무도 조사하지 않은 시체_에 대고 'E' 키를 누르면, 시체의 신원이 모든사람에게 알려짐과 동시에 시체의 상세한 정보가 표시된다.
**탐정**이 시체를 조사하면 모든 사람이 **Tab 키를 눌러 스코어보드**에서 시체의 상세 정보를 알 수 있게 된다.  

![01.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Trouble_20In_20Terroris
t_20Town/01.jpg)

[JPG image (155.85 KB)]

  
시체에 대고 'ALT+E' 를 누르면, 몰래 조사할 수 있으며, _아무도 조사하지 않은 시체_라 하더라도 아무에게도 알리지 않고 조용히 자기
혼자 시체의 상세정보를 볼 수 있다.

  

<del>시체가 떡하니 길거리에 있다면, 일단 주위를 둘러보자, [함정](%ED%95%A8%EC%A0%95.md)일 수
있다.</del>

[[edit](http://rigvedawiki.net/r1/wiki.php/Trouble%20In%20Terrorist%20Town?act
ion=edit&section=5)]

### 2.3. 특수 상점 ¶

![Shop.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Trouble_20In_20Terror
ist_20Town/Shop.jpg)

[JPG image (40.33 KB)]

  
기본적으로 배신자와 탐정은 **C** 키를 눌러 상점에서 특수 물품을 구매할 수 있다. 단, 특정 물품은 **재고**가 있어 몇 번 이상
구매하면 더 이상 살수 없게 제한되어있다. 서버마다 [애드온](%EC%95%A0%EB%93%9C%EC%98%A8.md)을 추가하여
[아이템](%EC%95%84%EC%9D%B4%ED%85%9C.md)을 추가할 수 있다.  
배신자는 클래스 지정시 _크레딧 2개_(배신자가 혼자라면 3개), 탐정은 _크레딧 3개_가 주어진다.

  

크레딧을 갖고 있던 사람이 **사망**하면, 그 시체를 조사해서 크레딧을 가져올 수 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Trouble%20In%20Terrorist%20Town?act
ion=edit&section=6)]

## 3. 아이템 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/Trouble%20In%20Terrorist%20Town?act
ion=edit&section=7)]

### 3.1. 공용 아이템(배신자,탐정) ¶

[방탄복](%EB%B0%A9%ED%83%84%EB%B3%B5.md),[레이더](%EB%A0%88%EC%9D%B4%EB%8D%94.md) 등 이 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Trouble%20In%20Terrorist%20Town?act
ion=edit&section=8)]

#### 3.1.1. 방탄복 (Body Armour) ¶

![001.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Trouble_20In_20Terrori
st_20Town/001.jpg)

[JPG image (5.84 KB)]

  
몸에 맞는 총기류의 데미지를 30% 줄여주며, 무한의 내구도를 자랑한다. 착용시 <del>자기가 시체가 되었을경우</del> 시체를 조사할때
**방탄복 착용 여부**가 표시된다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Trouble%20In%20Terrorist%20Town?act
ion=edit&section=9)]

#### 3.1.2. 레이더 (Radar) ¶

![002.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Trouble_20In_20Terrori
st_20Town/002.jpg)

[JPG image (5.13 KB)]

  
30초마다 1회씩 HUD에 모든 사람의 위치를 표시한다. 배신자의 경우 탐정,무죄인 구분도 가능하다. 배신자는 **위장기** 아이템을
사용하면 레이더에서 표시되지 않게 할 수 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Trouble%20In%20Terrorist%20Town?act
ion=edit&section=10)]

#### 3.1.3. 텔레포터 (Teleporter) ¶

![003-1.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Trouble_20In_20Terro
rist_20Town/003-1.jpg)

[JPG image (17.62 KB)]

  
지정한 위치로 텔레포트 시켜준다.

  

원하는 위치에서 텔레포터를 들고 오른쪽 클릭을 하면 위치가 지정된다.  
원할때마다 텔레포터를 들고 왼쪽 클릭을 하면 **1초 만에** 원하는 위치로 텔레포트 된다.

  

**단,** 텔레포트 시마다 바닥에 하얀 자국이 남으며, 텔레포트 소리가 크게 들린다. _위급할때만 쓰자._

  

<del>텔레포트 하는데 그 자리에 누군가 있다면 텔포킬을 시킬수 있다.</del>

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Trouble%20In%20Terrorist%20Town?act
ion=edit&section=11)]

### 3.2. 트레이터 전용 아이템 ¶

트레이터는 사살이 주 목적인 물품이 대다수이다. 대부분 서버에서는 트레이터 전용 물품을 **이노인증**을 하지 않고 사용하면 _트레이터로
간주하여 **즉살**한다._ 유념.  
[칼](%EC%B9%BC.md), [C4](C4.md)폭탄,
[라디오](%EB%9D%BC%EB%94%94%EC%98%A4.md)`[4]`, 위장기, 소음 권총, 교란기 등 이 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Trouble%20In%20Terrorist%20Town?act
ion=edit&section=12)]

#### 3.2.1. 칼 (Knife) ¶

![004-1.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Trouble_20In_20Terro
rist_20Town/004-1.jpg)

[JPG image (37.79 KB)]

  
보통 두방을 찌르면 사살할 수 있다. 완전 무음이며, 오른쪽 마우스를 눌러 **던질수도 있다.** <del>실패하면 목숨은
장담못한다</del> 한국서버 대부분은 한방으로 데미지를 변경해놓았다. 누구든지 가까이에만 있다면 한방에 보낼수 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Trouble%20In%20Terrorist%20Town?act
ion=edit&section=13)]

#### 3.2.2. C4`[5]` ¶

![005-1.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Trouble_20In_20Terro
rist_20Town/005-1.jpg)

[JPG image (38.89 KB)]

  
바닥에 **드롭한상태**로 쓰거나, **벽에 부착한 상태**로 쓸수있다. 45초부터 10분까지 시간을 조절할 수 있으며, **타이머가
길수록** 타이머 _소리의 주기_와 _소리크기_가 줄어들고, _폭파범위_가 증가한다. 해체시 6개의 선 중 1개를 골라야한다. 실패하면
[펑](%ED%8E%91.md). (해체실패시 폭발범위는 타이머 종료시 폭발범위보다 작다)  
그 **방법**을 알아내는 방법은, C4를 설치한 배신자를 죽인 후, 시체 상세정보에 있는
_[쪽지](%EC%AA%BD%EC%A7%80.md)_를 확인하면 된다. (어느것이 가짜선이라고 적혀있다.)  
혹은, 탐정이 특수상점에서 살 수 있는 **해체 킷**을 사용하면 _단번에_ 해체가 가능하다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Trouble%20In%20Terrorist%20Town?act
ion=edit&section=14)]

#### 3.2.3. 라디오 (Radio) ¶

![006-1.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Trouble_20In_20Terro
rist_20Town/006-1.jpg)

[JPG image (38.83 KB)]

  
어느 지점에 설치후에, 배신자가 C키를 눌러 메뉴에서 원하는 소리버튼을 클릭하면, **라디오에서 그 소리가 재생된다.** 이를 이용해 낚아서
<del>찜쪄</del> 죽일수도 있다.

  

_DNA가 남지 않는 아이템이다._

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Trouble%20In%20Terrorist%20Town?act
ion=edit&section=15)]

#### 3.2.4. 위장기 (Disguiser) ¶

![007.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Trouble_20In_20Terrori
st_20Town/007.jpg)

[JPG image (4.82 KB)]

  
<del>긴장타라 1대1이다 를 선언하기 위한 도구</del>

  

누군가 자신을 조준했을때, 이름이 표시되지 않게한다. 타겟을 지정후 퀵라디오로 알리려고 해도 __위장기를 착용한 사람__이라고 뜬다.
**레이더**에도 표시되지 않는다. 사살된 후 시신을 조사하면 위장기 착용 여부가 표시된다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Trouble%20In%20Terrorist%20Town?act
ion=edit&section=16)]

#### 3.2.5. 소음 권총 (Slienced Pistol) ¶

![008-1.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Trouble_20In_20Terro
rist_20Town/008-1.jpg)

[JPG image (42.21 KB)]

  
말 그대로 소음 권총이다. 소리가 별로 없으며, **헤드샷 2방**이면 사살이 가능하다.  
정확도가 꽤나 높아 중,장거리에서도 요긴하게 쓸 수 있다. 별로 잘 쓰이진 않는다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Trouble%20In%20Terrorist%20Town?act
ion=edit&section=17)]

#### 3.2.6. 교란기 (Decoy) ¶

![009-1.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Trouble_20In_20Terro
rist_20Town/009-1.jpg)

[JPG image (43.45 KB)]

  
만약 탐정이 DNA을 이용해 자신을 추적한다면, 이 교란기 하나면 탐정을 낚을 수 있다.  
자신의 DNA와 다른 배신자가 남긴 DNA를 추적하면 이 교란기의 위치가 표시된다. **교란기를 파괴하면** DNA스캐너에는 원래 DNA의
주인의 위치가 표시된다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Trouble%20In%20Terrorist%20Town?act
ion=edit&section=18)]

#### 3.2.7. 발화 권총 (Flare Gun) ¶

![010-1.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Trouble_20In_20Terro
rist_20Town/010-1.jpg)

[JPG image (36.46 KB)]

  
**시체를 태울 수 있다.** 총 4발.

  

시체에 쏘면 약 6~8초간 불타다가 시체가 사라진다. _바닥에는 검은 탄 자국이 남는다_ 산 사람에게 쏘면 그대로 불이 붙고 물에 들어가지
않는 이상 체력이 30정도 깎일때까지 불붙은 인간이 된다.

  

_물에서는 아무리 쏴도 불이 붙지 않는다_

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Trouble%20In%20Terrorist%20Town?act
ion=edit&section=19)]

#### 3.2.8. 뉴턴 런처 (Newton Launcher) ¶

![011-1.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Trouble_20In_20Terro
rist_20Town/011-1.jpg)

[JPG image (11.62 KB)]

  
**중력빔을 발사해서 물체나 사람을 밀 수 있다.**

  

아슬아슬하게 걸쳐져 있는 사람에게 쏘면 안성맞춤이다. **왼쪽클릭**시 단발로 나가며, **오른쪽클릭**시 충전할 수 있다. 완전충전 상태로
발사하면 꽤 멀리까지 날라간다. (특히 점프상태면 [로켓](%EB%A1%9C%EC%BC%93.md)수준으로 날라간다.)

  

쏠때 파란색 빔과 [하프라이프 2](%ED%95%98%ED%94%84%EB%9D%BC%EC%9D%B4%ED%94%84%202.md)의
**AR2 라이플** 발사 소리가 나기때문에 숨어서 하거나 _바로 뒤에서_ 하면 좋다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Trouble%20In%20Terrorist%20Town?act
ion=edit&section=20)]

#### 3.2.9. 폴터가이스트 (Poltergeist) ¶

![011-3_1.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Trouble_20In_20Ter
rorist_20Town/011-3_1.jpg)

[JPG image (57.48 KB)]

  
프롭을 **미쳐 날뛰게** 할 수 있다.

  

어떤 프롭에 대고 쏘면, 프롭에 어떤 공이 붙는다. 그 프롭은 랜덤한 방향으로 날라다닌다. 그 데미지는 꽤 아프다. 특히 **큰
물건**일수록 대부분 죽는다. 몇번 튕기다가 나중에는 터진다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Trouble%20In%20Terrorist%20Town?act
ion=edit&section=21)]

### 3.3. 탐정 전용 아이템 ¶

탐정은 수색이 주 목적인 물품이 대다수이다. 가끔 이노인증을 한 무죄인에게 특정 아이템을 하사해주는 **좋은** 탐정들이 있다.  
(혹은 DNA스캐너를 버그로 마구마구 복제해서 뿌리기도 한다.)

[[edit](http://rigvedawiki.net/r1/wiki.php/Trouble%20In%20Terrorist%20Town?act
ion=edit&section=22)]

#### 3.3.1. DNA 스캐너 (DNA Scanner) ¶

![012-1.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Trouble_20In_20Terro
rist_20Town/012-1.jpg)

[JPG image (3.8 KB)]

  

![thereyou.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Trouble_20In_20Te
rrorist_20Town/thereyou.jpg)

[JPG image (58.42 KB)]

  
<del>배신자들이 이 글을 싫어합니다.</del>

  

탐정에게는 **기본적으로 제공**된다. DNA가 존재하는 시체에 사용하면 근처에 있었던 사람의 DNA를 추출할 수 있다. 이는 _아이템_에도
적용된다. (각종 무기,C4 폭탄 등)  
DNA가 남으려면 중거리 안에서 사살해야 DNA가 남는다. **최대한 근접거리에서 사살할수록 DNA 유지시간이 길어진다.**

  

추출된 DNA는 DNA 스캐너에 계속 남아있게된다. DNA를 추적하면 해당 사람의 위치를 알아낼 수 있다. _그러나 반드시 DNA에서 나온
사람이 범인이라는 확정은 없다._

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Trouble%20In%20Terrorist%20Town?act
ion=edit&section=23)]

#### 3.3.2. 의료 기기 (Health Station) ¶

![012-3.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Trouble_20In_20Terro
rist_20Town/012-3.jpg)

[JPG image (41 KB)]

  
전자레인지 모델을 사용하는 아이템. **사용하면 체력이 올라가는 구급킷**이다.

  

서버마다 다르지만, 사용하고 있으면 초당 30HP씩 체력을 회복받는다. 초기 의료기기의 **회복 한도**는 200HP.  
그 한도를 다 소모하면 더 이상 사용할수 없다. 하지만 몇초당 1HP씩 재충전되니 시간만 있다면 다시 회복받는것도 문제는 아니다.

  

_**사용시 DNA가 묻는다.**_ 이를 이용해 탐정들은 **의료기기 사용금지**를 명령하고 자신 외 사용한 사람을 **DNA스캐너**를
이용해 쫓기도 한다. 이동이 불가능하고 바닥에 놓을수만 있어서 대부분 특정 장소에 놓는 편이다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Trouble%20In%20Terrorist%20Town?act
ion=edit&section=24)]

#### 3.3.3. 비쥬얼라이저 (Visualizer) ¶

![012-4.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Trouble_20In_20Terro
rist_20Town/012-4.jpg)

[JPG image (22.25 KB)]

  
주울 수 있으며, 바닥에 놓으면 **근처에 파란 원 형태의 빔이 형성된다.**

  

시체 근처에 비쥬얼라이저를 놓으면, 파란 전자기장이 _그를 죽인사람의 위치, 죽은사람의 위치와 총알궤적을 표시한다._ (사용무기, 살인자
신원 등은 확인할 수 없다.)  
대부분 탐정들은 증거확보나 명분을 얻기위해 사용한다.

[[edit](http://rigvedawiki.net/r1/wiki.php/Trouble%20In%20Terrorist%20Town?act
ion=edit&section=25)]

#### 3.3.4. 쌍안경 (Binoculars) ¶

![013-1.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Trouble_20In_20Terro
rist_20Town/013-1.jpg)

[JPG image (26.62 KB)]

  
**멀리에 있는 시체**를 확대해서 시체를 상세하게 _조사_할 수 있다. 멀리 있는 시체를 조사하는데 약 3~4초 정도가 소요된다. 시체 조사 외에도 장거리 상황을 살펴볼때도 유용하다.

  

<del>하필 모델이 돌돌말린 휴지다</del>

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Trouble%20In%20Terrorist%20Town?act
ion=edit&section=26)]

#### 3.3.5. UMP .45 프로토타입 (UMP .45 Prototype) ¶

![014-1.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Trouble_20In_20Terro
rist_20Town/014-1.jpg)

[JPG image (62.11 KB)]

  
얼핏보면 그냥 기관단총이지만, **명중할 때 마다 전기충격**을 주는 좋은 효과가 있다.  
데미지는 많이 약하지만, 반동이 매우 낮고 명중률도 좋은데다가 명중할 때 마다 **에임을 다른데로 돌려버린다.**  
_특히 헤드샷이면 효과가 크다. 춤추는 모습을 볼 수 있다._

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Trouble%20In%20Terrorist%20Town?act
ion=edit&section=27)]

#### 3.3.6. 해체 킷 (Defuser) ¶

![015-1.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Trouble_20In_20Terro
rist_20Town/015-1.jpg)

[JPG image (28.61 KB)]

  
**C4를 0.00000001초만에 해체할 수 있다.**

  

그냥 해체킷을 들고 작동중인 [C4](C4.md)폭탄에 클릭만 하면 _바로 해체된다._  
보통 급할때 구입하거나, 믿을만한 무죄인에게 선물로 준다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Trouble%20In%20Terrorist%20Town?act
ion=edit&section=28)]

## 4. 클래스 ¶

TTT에는 3가지 클래스가 존재하며, 라운드 시작시 각각 특정비율로 클래스가 부여된다.

[[edit](http://rigvedawiki.net/r1/wiki.php/Trouble%20In%20Terrorist%20Town?act
ion=edit&section=29)]

### 4.1. 무죄인 (Innocent) ¶

![ttt-innocent.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Trouble_20In_
20Terrorist_20Town/ttt-innocent.jpg)

[JPG image (16.04 KB)]

  
<del>온갖 프리킬의 주범</del>

  
  

TTT모드에서 대부분 되는 클래스. <del>무죄인이 되면 보이스로 다들 푸념을 늘어놓는다</del>  
하단 HUD에 **Innocent 글자**와 **초록색 배경**으로 표시된다.

  

배신자에게서 살아남아야 하는것이 주 목표, 라운드 시간이 끝나기 전까지 살아남아야 한다. 탐정에게서
[신뢰](%EC%8B%A0%EB%A2%B0.md)를 얻어 엄호를 받으면 좋다. 신뢰를 얻는 **제일 좋은 방법**은 _배신자를 죽이는
것._  
정말 배신자를 죽였다면 탐정에게 **푸짐한 엄호혜택과 함께 가끔씩 특전 아이템을 받을 수 있다!** (그러나 가끔 배신자끼리 짜고서 배신자가
배신자를 죽이고는 **이노 인증**`[6]`이라고 하는 경우가 있다.)

[[edit](http://rigvedawiki.net/r1/wiki.php/Trouble%20In%20Terrorist%20Town?act
ion=edit&section=30)]

### 4.2. 배신자 (Traitor) ¶

![ttt-traitor.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Trouble_20In_2
0Terrorist_20Town/ttt-traitor.jpg)

[JPG image (15.39 KB)]

  
**TTT의 꽃.**

  
  

대부분 유저가 되고싶어하는 클래스.  
하단 HUD에 **Traitor 글자**와 **빨간색 배경**으로 표시된다.

  

배신자들끼리 팀채팅이 가능하다. 기본 채널외 **배신자 전용 채널**로 대화할 수 있다. 서로 크레딧을 **송수신** 할 수 있으며,
크레딧이 넘치는 사람이 부족한 사람에게 크레딧을 마구마구 퍼줄수도 있다.  
탐정과 무죄인을 모조리 죽이는것이 주 목표이며, 상점에서 특수 아이템을 구입할 수 있다.

[[edit](http://rigvedawiki.net/r1/wiki.php/Trouble%20In%20Terrorist%20Town?act
ion=edit&section=31)]

### 4.3. 탐정 (Detective) ¶

![ttt-detective.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Trouble_20In
_20Terrorist_20Town/ttt-detective.jpg)

[JPG image (13.38 KB)]

  
<del>늘 털리는 불쌍한 탐정</del>

  
  

무죄인과 연합하여 배신자에 대항하는 클래스.  
하단 HUD에 **Detective 글자**와 **파란색 배경**으로 표시된다.

  

배신자들과 마찬가지로 탐정끼리 **팀채팅**이 가능하다. 마찬가지로 **크레딧 송수신**도 가능하다. 탐정의 주 목표는 트레이터를 모조리
사살하는것, 그리고 제한시간까지 버티는 것이다. 특수 아이템을 구입할 수 있다.

  

대부분 배신자들의 _제거 1순위_이기 때문에 늘 라운드타임 중간쯤에 가면 탐정은 다 죽어있다. <del>에효</del>

`\----`

  * `[1]` 이 맵에선 떨어져있는 무기가 없고, 숨을 곳도 없고 맵이 사실상 개방되어 있기 때문에, 탐정과 배신자가 특수상점에서 아이템을 사서 서로 싸운다, 무죄인은 빠루를 들고 근접전을 펼치고, 배신자들은 여유롭게 잉여들을 학살하는 꼴불견(...)이 연출된다. GM_Flatgrass 맵도 마찬가지
  * `[2]` [하프라이프 2](%ED%95%98%ED%94%84%EB%9D%BC%EC%9D%B4%ED%94%84%202.md)의 인기 모드였던 [Zombie Master](Zombie%20Master.md)의 [개발자](%EA%B0%9C%EB%B0%9C%EC%9E%90.md)라고 알려져있다.
  * `[3]` 영어권 서버에서는 'RDM(Random DeathMatch)'라고 하니 거기에서 할꺼면 알아두자.
  * `[4]` 특정 사운드를 원격으로 낼 수 있다, 유도할때 쓰인다
  * `[5]` 일부 서버는 패스워드를 쓰기도 한다
  * `[6]` 무죄인이라는 것이 확실하다고 할때 말한다

