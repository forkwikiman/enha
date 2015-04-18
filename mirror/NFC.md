  * [동음이의어](%EB%8F%99%EC%9D%8C%EC%9D%B4%EC%9D%98%EC%96%B4.md)
  * [NFL](NFL.md) 산하 National Football Conference를 찾아오신 분은 NFL 항목으로 가십시오.  

## Contents

    

1. Near Field Communication 
    

1.1. 기능

1.2. RFID와의 차이점

1.3. [대한민국](%EB%8C%80%ED%95%9C%EB%AF%BC%EA%B5%AD.md)에서는

1.4. 설정

    

1.4.1. 유의사항

1.5. 이용 기기

2. Not From Concentrate 

[[edit](http://rigvedawiki.net/r1/wiki.php/NFC?action=edit&section=1)]

# 1. Near Field Communication ¶

  

![http://upload.wikimedia.org/wikipedia/en/c/c3/NFC-N-Mark-
Logo.png](http://upload.wikimedia.org/wikipedia/en/c/c3/NFC-N-Mark-Logo.png)

[[PNG external image]](http://upload.wikimedia.org/wikipedia/en/c/c3/NFC-N
-Mark-Logo.png)

  

[휴대전화](%ED%9C%B4%EB%8C%80%EC%A0%84%ED%99%94.md) 등 NFC 기능을 탑재한 전자기기들이 근거리
무선통신을 할 수 있게 하는 기술. [FeliCa](FeliCa.md), [MIFARE](MIFARE.md) 등 기존의 [RF표준 기술](RFID.md)들을 이용해서 [노키아](%EB%85%B8%ED%82%A4%EC%95%84.md),
[필립스](%ED%95%84%EB%A6%BD%EC%8A%A4.md)(지금은
[NXP반도체](NXP%EB%B0%98%EB%8F%84%EC%B2%B4.md)),
[소니](%EC%86%8C%EB%8B%88.md) 등이 개발했다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/NFC?action=edit&section=2)]

## 1.1. 기능 ¶

기존의 RF 기기들이 지원하던 [모바일카드](%EB%AA%A8%EB%B0%94%EC%9D%BC%EC%B9%B4%EB%93%9C.md)와
[교통카드](%EA%B5%90%ED%86%B5%EC%B9%B4%EB%93%9C.md)를 대체할 전자지불 서비스는 당연히 가능하다. 또
[블루투스](%EB%B8%94%EB%A3%A8%ED%88%AC%EC%8A%A4.md)처럼 파일도 전송할 수 있고, 박물관의 전시물 안내
서비스처럼 NFC 태그 가까이에 가져다 대면 자동으로 특정 동작을 수행하는 기능도 할 수 있다. 응용 서비스 중에 그나마 알려진 것으로는
지갑 휴대폰 기능을 이용한 [e-AMUSEMENT PASS](e-AMUSEMENT%20PASS.md)나
[ALL.Net](ALL.Net.md)등이 있다. 다만, 모바일Suica 앱이 있어야 사용이 가능한데, 이게 일본 국내에 출시된
단말기만 실행이 가능하도록 제한되어 있어서 국내에서는 보통 정상적으로 사용이 불가능하다`[1]`

  

추가로 요즘 별별 사업을 다 하는 [구글](%EA%B5%AC%EA%B8%80.md)은 구글 월렛이라고
[안드로이드](%EC%95%88%EB%93%9C%EB%A1%9C%EC%9D%B4%EB%93%9C%28OS%29.md) 스마트폰의 NFC
기능을 이용한 결제 서비스를 오픈했는데[#](http://www.google.com/wallet/index.html), 당연히 한국에서는
사용할 수 없다. 서비스 실시중인 [미국](%EB%AF%B8%EA%B5%AD.md)에서도
[마스타카드](%EB%A7%88%EC%8A%A4%ED%83%80%EC%B9%B4%EB%93%9C.md) PayWave만 지원하는듯.

  

또한 안드로이드 5.0 (롤리팝) 이후 기능인 smart lock기능에서 자신이 등록한 nfc를 접촉할시 암호를 입력하지 않고 바로
홈화면으로 갈 수 있는 기능이 생겼다.

  

NFC 태그에 접촉하면 핸드폰이 매너모드로 전환하거나, [Wi-Fi](Wi-Fi.md)를 켜거나, 취침 모드로 들어가는 등의 지정한
동작을 수행하도록 할 수도 있다. 그런데 NFC 태그의 가격이 아직까지는 안드로메다급. 오픈마켓에서 10장에 13000원~20000원 정도
한다. [구글 플레이](%EA%B5%AC%EA%B8%80%20%ED%94%8C%EB%A0%88%EC%9D%B4.md) 스토어에는 각
NFC/RF카드의 정보를 읽어주는 앱이 수두룩하게 올라와 있으며, 한국산 앱 중에는
[티머니](%ED%8B%B0%EB%A8%B8%EB%8B%88.md)나
[캐시비](%EC%BA%90%EC%8B%9C%EB%B9%84.md), 16자리 표준형 카드 대부분을 지원하는 교통카드 잔액확인 앱도
있다. [#](https://play.google.com/store/apps/details?id=kr.co.smavis.st) 좀 더
기술적인 내용을 알고 싶으면 [이
앱](https://play.google.com/store/apps/details?id=com.nxp.taginfolite)을 설치해 보자.

  

NFC시장이 이동통신사 중심으로 돌아가다 보니 유통사업자들은 NFC를 무시하고 다른 길을 모색해온지 오래다. 카드를 읽히면 그만인 신용카드에
비해 단말기를 일일이 켜서 사용한다는 것이 까다롭다는 지적도 많았다. 더욱이 스마트폰을 쓰면서 신용카드가 없다는 것도 상상하기 힘든
것이고... 같은 이유로 사용률이 줄어든 [QR코드](QR%EC%BD%94%EB%93%9C.md)와 같은 전철을 밟을 것으로 여겨진다.
[애플](%EC%95%A0%ED%94%8C%28%EA%B8%B0%EC%97%85%29.md)은 다들 알다시피 원래부터 NFC에 별
관심이 없었고 대신 [iOS](iOS.md) 7에 추가된 iBeacon(아이비콘) 기능을 전폭적으로 지원하고 있다.`[2]` [아이튠즈스토어](%EC%95%84%EC%9D%B4%ED%8A%A0%EC%A6%88%20%EC%8A%A4%ED%86%A0%EC%96%B4.md)
를 이용하는 사용자들을 자연스럽게 모바일 결제 시장으로 돌리겠다는 의도로 보여진다. 이와 비슷하게
[구글](%EA%B5%AC%EA%B8%80.md)도 2013년부터 NFC 시장에서 발을 빼는 모습을 보이고 있어서, NFC의 미래는
불투명하다고 볼 수 있겠다. 2014년에 와서는 NFC 시장 자체가 다 크지도 못하고 설익은 채로 저무는 듯한 분위기이다.

  

2014년 여름에는 애플이 아이비콘과 NFC를 접목할 수도 있다는 루머가 있었다. 그리고 실제로 후속 모델인 [아이폰6](%EC%95%84%EC%9D%B4%ED%8F%B0%206.md)와 [아이폰6+](%EC%95%84%EC%9D%B4%ED%8F%B0%206+.md), 그리고 [애플워치](%EC%95%A0%ED%94%8C%20%EC%9B%8C%EC%B9%98.md)에 NFC를 지원하고 기존 자사 플랫폼인 패스북과
연동된 애플 페이(Apple Pay)라는 결제 기능을 도입했다. 본인 확인의 경우 5s부터 탑재된 터치 아이디(지문 인식 홈버튼)를
사용한다.

  

애플 페이가 보안이나 사용 용이성 측면에 있어 구글 월렛 등의 다른 NFC 결제 방식보다 강력하고 여러 기업들로부터 도입에의 환영을 받는
것은 사실이나, 다른 형태의 결제 방식 도입을 추진하고 있는 미국의 일부 대형 유통업체들은 NFC 리더기를 매장에서 모조리 치워버리는 등
의외로 강경하게 대응하고 있기도 하다. 그덕분에 NFC 결제를 사용해왔던 다른 사용자들 또한 졸지에 낭패를 보게 됐다는 소식이 전해졌다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/NFC?action=edit&section=3)]

## 1.2. RFID와의 차이점 ¶

[RFID](RFID.md)가 [NFC](NFC.md)보다 수신 범위가 길다. NFC는 고작 10cm정도이다. 그리고
[RFID](RFID.md)는 단방향 통신이고, NFC는 양방향 통신이다. RFID는 태그와 리더기의 역할이 고정되어 있다. 예를 들어
교통카드의 경우 태그의 역할로서 정보를 내주는 역할(출력)만 수행한다. 버스에 부착된 카드리더기는 교통카드(태그)에서 정보를 읽는 역할을
수행한다. 반면 NFC는 상황에 따라 태그와 리더기의 역할을 변경할 수 있다. 예를 들어 NFC 기능이 내장된 스마트폰의 경우 교통카드
기능을 사용할 땐 태그로서의 역할을 수행하는 것이고, NFC 태그`[3]`에 갖다대거나 다른 교통카드의 잔액을 확인할 때는 리더기의 역할을
수행하는 것으로 볼 수 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/NFC?action=edit&section=4)]

## 1.3. [대한민국](%EB%8C%80%ED%95%9C%EB%AF%BC%EA%B5%AD.md)에서는 ¶

[대한민국](%EB%8C%80%ED%95%9C%EB%AF%BC%EA%B5%AD.md)에서는 NFC 맛도 아니고 NFC 향 첨가(...)
수준의 서비스만 사용할 수 있는 실정. 그나마도 외산폰들은 NFC 탑재라도 통신사들의 농간으로 인해
[모바일카드](%EB%AA%A8%EB%B0%94%EC%9D%BC%EC%B9%B4%EB%93%9C.md)와 [모바일티머니](T-Money.md)/[캐시비](%EC%BA%90%EC%8B%9C%EB%B9%84.md) 등 그나마 있는 NFC 향 첨가
수준의 서비스조차 이용할 수 없다. 그 이유는 몇가지가 있는데, NFC 결제 정보를 저장하는 SE(Secure Element)가 스마트폰마다
다르기 때문이다. 구글 넥서스의 경우 이 정보를 별도의 내장 칩`[4]`에 저장하는 반면 국내 스마트폰들은 NFC USIM`[5]`에
저장한다. SE가 내장된 마이크로 SD카드도 있다.<del>하지만 마이크로SD방식은 듣보잡이고 잘 안 쓴다</del>  
그런데 소니의 엑스페리아 시리즈는 우리나라 기기들처럼 NFC USIM**도** SE로 사용하기 때문에, 국내 NFC유심을 끼우면 [티머니](
/wiki/T-Money#s-2.5)·[캐시비](%EC%BA%90%EC%8B%9C%EB%B9%84#s-2.10.md)`[6]`를 쓸 수
있다. 물론 오프라인 충전·결제만. 아래 서술할 내용과 같이 타사유심기변으로 쓰는 셈이기 때문에 [모바일티머니](T-Money#s-2.5.md)·[모바일캐시비](%EC%BA%90%EC%8B%9C%EB%B9%84#s-2.10.md) 앱이나
[모바일카드](%EB%AA%A8%EB%B0%94%EC%9D%BC%EC%B9%B4%EB%93%9C.md),
[뱅크월렛](%EB%B1%85%ED%81%AC%EC%9B%94%EB%A0%9B.md) 앱은 못 쓴다. 굳이 쓰려면 아래 서술할 내용과
같이 원 통신사 단말기로 주카드를 설정해 놓으면 주카드로만 쓸 수 있다.  
그리고 윈도우폰의 경우에도 오프라인 결제(티머니 등)는 사용 가능하다.`[7]` 하지만 앱이 없기 때문에 잔액은 폰에서 확인불가.  
<del>개발 덕후들은</del>자세한 건 이런 걸 참고하라.[Smart 2013 Conference](http://www.iaria.org
/conferences2013/filesSMART13/Urien_Talk_smart2013.pdf) [SmartCard
API](http://code.google.com/p/seek-for-android/)

  

구글 넥서스 시리즈의 경우, 구글이 구글 월렛에 우리나라 서비스를 추가한다면 어느 정도 가능성은 있을 지도?[#](https://www.sk
smarttouch.com/web/main/nop/mainPage)[#](http://readme.skplanet.com/?p=3028)

  

![s_2014_04_66_2.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/NFC/s_2014_
04_66_2.jpg)

[JPG image (218.66 KB)]

  

[지하철](%EC%A7%80%ED%95%98%EC%B2%A0.md) 역 등에서 NFC기능을 이용한
[영화](%EC%98%81%ED%99%94.md) [광고](%EA%B4%91%EA%B3%A0.md)를 하는 경우도 있다.
스마트폰의 NFC(읽기쓰기)를 활성화 한 뒤 광고판에 폰을 대라는 표시가 있는데 이렇게 하면 스마트폰으로 해당 광고의 예고편을 볼 수 있다.
<del>데이터 요금은 덤</del> <del>한 번 해볼까 하며 태깅하러 다가서면 공익근무요원이 호각을 불며 물러나라고 지시한다</del>

  

[[edit](http://rigvedawiki.net/r1/wiki.php/NFC?action=edit&section=5)]

## 1.4. 설정 ¶

[안드로이드](%EC%95%88%EB%93%9C%EB%A1%9C%EC%9D%B4%EB%93%9C%28OS%29.md)를 이용하는
기기에서는 설정 - 무선 및 네트워크 - 더 보기 - NFC 에서 NFC 설정을 할 수 있다.  

  * "**NFC (카드모드)**"는 NFC 카드 에뮬레이션을 켠다는 것을 의미한다. [UbiTouch](UbiTouch.md)나 [모바일카드](%EB%AA%A8%EB%B0%94%EC%9D%BC%EC%B9%B4%EB%93%9C.md), [교통카드](%EA%B5%90%ED%86%B5%EC%B9%B4%EB%93%9C.md)`[8]`를 쓰려면 국내폰 기준으로 "**NFC(카드모드)**"만 체크하면 된다. 아래 것들은 체크하지 않아도 된다!
  * "**NFC 읽기쓰기·P2P 수신**"는 각종 NFC 태그를 인식하겠다는 것을 뜻한다. 태그 인식`[9]`이나 파일 주고받기를 이용하려면 이것도 켜야 한다. 교통카드 기능이 있는 카드나 출입카드를 휴대폰 가까이 가져다댔을 때 "뚜-두둥" 하는 소리가 나는 것이 바로 "**NFC 읽기쓰기·P2P 수신**"가 켜져 있기 때문이다. 거슬린다면 이걸 체크하지 않으면 된다. [코레일](%EC%BD%94%EB%A0%88%EC%9D%BC.md)에서 나온 레일머니 앱은 이 모드로 세팅하고 NFC 안테나에 [레일플러스](%EB%A0%88%EC%9D%BC%ED%94%8C%EB%9F%AC%EC%8A%A4.md) 실물 카드를 갖다 대서 충전하는 방식이다.
  * "**NFC 송신·Android Beam**"는 [블루투스](%EB%B8%94%EB%A3%A8%ED%88%AC%EC%8A%A4.md)나 Wi-Fi Direct처럼 파일 주고받기 기능을 쓰겠다는 것을 뜻한다. 폰을 마주대면 전송할 파일을 선택할 수 있다.  

[[edit](http://rigvedawiki.net/r1/wiki.php/NFC?action=edit&section=6)]

### 1.4.1. 유의사항 ¶

  * "NFC (카드모드)"를 이용하려면 국내용 NFC단말기+**NFC 유심**이 필요하다. **금융유심이 아니라 NFC 유심**이다. [구글 넥서스](%EA%B5%AC%EA%B8%80%20%EB%84%A5%EC%84%9C%EC%8A%A4.md) 시리즈같은 외국 폰들은 [모바일카드](%EB%AA%A8%EB%B0%94%EC%9D%BC%EC%B9%B4%EB%93%9C.md)나 [뱅크월렛](%EB%B1%85%ED%81%AC%EC%9B%94%EB%A0%9B.md), 모바일[티머니](%ED%8B%B0%EB%A8%B8%EB%8B%88.md)를 쓸 수 없다.
  * NFC 읽기쓰기·P2P 송수신, Android Beam은 NFC 단말기라면 모두 다 되는 기능으로, **USIM과는 전혀 관계가 없다**. 없어도 그만, 5,500원짜리 통신전용유심이라도 그만이다.  
즉, 넥서스 시리즈도 위에 서술한 플라스틱교통카드 잔액 [조회
앱](https://play.google.com/store/apps/details?id=kr.co.smavis.st)을 쓰는 데 전혀 문제가
없으며, 국내 단말기에 NFC유심을 꽂지 않아도 NFC tag읽기·쓰기나 파일 송·수신에 전혀 문제가 없다는 뜻이다.  
몇몇 정신나간 AS센터 직원들은 NFC유심을 안 끼우면 NFC 읽기쓰기도 안 된다는 <del>헛소리</del>개드립을 치기도 하니까 속지
말자.

  * 위 설정 구분은 국내 단말기 기준으로, [USIM](USIM.md) SE 기반 카드 에뮬레이션을 쓰지 않는 외국 단말기에선 "**NFC**"가 곧 "**NFC 읽기쓰기·P2P 수신**"라는 점에 조심할 필요가 있다. 혼동할 염려가 있으니 주의.
  * 또한 **NFC (카드모드)**`[10]`만 켤 경우에는 배터리를 추가로 소모하지 않는다. "[GPS](GPS.md)"를 켜 놓아도 실제로 GPS를 사용하고 있을 때만`[11]` 배터리를 소모하는 것처럼 [교통카드](%EA%B5%90%ED%86%B5%EC%B9%B4%EB%93%9C.md)나 [모바일카드](%EB%AA%A8%EB%B0%94%EC%9D%BC%EC%B9%B4%EB%93%9C.md) 결제시에만 잠깐 배터리를 극소량 소모할 뿐이다.
  * 반대로 **NFC 읽기쓰기·P2P수신**이나 **Android Beam**을 켜면 [블루투스](%EB%B8%94%EB%A3%A8%ED%88%AC%EC%8A%A4.md)나 [Wi-Fi](Wi-Fi.md)마냥 주기적으로 주파수를 스캔하는 데에 배터리를 소모하니 필요할 때만 켜는 것이 배터리 절약에 도움이 된다.  
대부분 단말기는 화면이 꺼져 있을 땐 NFC 읽기쓰기를 꺼 버린다. 또, 몇몇 [갤럭시S4](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20S4.md)는 화면이 꺼지면 "NFC (카드모드)"도 꺼버려서 화면을 켜야
티머니가 찍힌다고. 스테미나모드를 켠 소니 엑스페리아 단말기도 이러한 현상을 보인다. <del>뭥미?</del>

  * **NFC (카드모드)**의 경우, 타사유심기변을 하면 주카드 변경이 되지 않아 타사유심기변하기 전에 설정한 주카드만 쓸 수 있으니 유의해야 한다. 쉽게 말하자면, [뱅크월렛](%EB%B1%85%ED%81%AC%EC%9B%94%EB%A0%9B.md)([유비터치](%EC%9C%A0%EB%B9%84%ED%84%B0%EC%B9%98.md))을 신한s20통장, [모바일카드](%EB%AA%A8%EB%B0%94%EC%9D%BC%EC%B9%B4%EB%93%9C.md)를 우리v체크카드, [교통카드](%EA%B5%90%ED%86%B5%EC%B9%B4%EB%93%9C.md)를 [티머니](%ED%8B%B0%EB%A8%B8%EB%8B%88.md)로 설정한 상태라면 유심기변을 원복하기 전에는 주구장창 해당 카드만 쓸 수 있다는 것이다. SKT의 티머니 NFC유심을 KT 기계에 끼우면 [티머니](T-Money.md)로만 쓸 수 있고, [캐시비](%EC%BA%90%EC%8B%9C%EB%B9%84.md)로 바꿀 수 없다는 뜻이다.  
무슨 말이냐면, 예를 들어 KT용 갤4에 SKT NFC유심을 끼운 상태에선 sktusimservice.apk, tca.apk,
smartcardservice.apk, seioagent.apk`[12]`가 없다며 NFC(카드모드) 관련 앱이 실행이 안 되기 때문. 앱을
실행시켜야 다른 카드를 선택할 수 있는데 앱을 실행시킬 수 없어서 주카드로 설정해 놓은 해당 카드만 계속 쓸 수 있다. 그러니 타사유심기변을
할 경우 주의할 것.  
물론, 위 문단에서 설명한 대로 **NFC(카드모드)**에만 체크하면 오프라인에서 아무 문제없이 결제가 되기 때문에,
[뱅크월렛](%EB%B1%85%ED%81%AC%EC%9B%94%EB%A0%9B.md)이나
[모바일카드](%EB%AA%A8%EB%B0%94%EC%9D%BC%EC%B9%B4%EB%93%9C.md)를 하나만 쓴다면(즉,
뱅크월렛(유비터치) 앱을 실행시킬 일이 없는 사용자라면) 별 문제를 못 느낄 수도 있다.  

[[edit](http://rigvedawiki.net/r1/wiki.php/NFC?action=edit&section=7)]

## 1.5. 이용 기기 ¶

한국에 출시된 기기 중 NFC를 이용할 수 있는 휴대전화의 목록은 다음과 같다.

  

  * [구글 넥서스](%EA%B5%AC%EA%B8%80%20%EB%84%A5%EC%84%9C%EC%8A%A4.md) \- 모두 읽기쓰기·P2P만 된다. 대한민국에서 서비스하는 NFC 카드모드는 안 됨.  

    * [넥서스 S](%EB%84%A5%EC%84%9C%EC%8A%A4%20S.md)
    * [갤럭시 넥서스](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20%EB%84%A5%EC%84%9C%EC%8A%A4.md)
    * [넥서스 7](%EB%84%A5%EC%84%9C%EC%8A%A4%207/1%EC%84%B8%EB%8C%80.md)
    * [넥서스 4](%EB%84%A5%EC%84%9C%EC%8A%A4%204.md)
    * [넥서스 10](%EB%84%A5%EC%84%9C%EC%8A%A4%2010.md)
    * [넥서스 7 2013](%EB%84%A5%EC%84%9C%EC%8A%A4%207/2%EC%84%B8%EB%8C%80.md)
    * [넥서스 5](%EB%84%A5%EC%84%9C%EC%8A%A4%205.md)
    * [넥서스 6](%EB%84%A5%EC%84%9C%EC%8A%A4%206.md)
    * [넥서스 9](%EB%84%A5%EC%84%9C%EC%8A%A4%209.md)  

  * [삼성 갤럭시](%EC%82%BC%EC%84%B1%20%EA%B0%A4%EB%9F%AD%EC%8B%9C.md)  

    * [애니콜](%EC%95%A0%EB%8B%88%EC%BD%9C.md) 코비 N - 유일한 비 스마트폰으로 출시 시기도 가장 빠르다
    * [갤럭시 S II](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20S%20II.md) \- 다른 폰들은 배터리 커버에 안테나가 달려 있는데 반해 S 시리즈들은 기존 피처폰시절 금융RF폰처럼 배터리에 안테나가 달려 있다.
    * [갤럭시 S II LTE](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20S%20II%20LTE.md)
    * [갤럭시 S II HD LTE](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20S%20II%20HD%20LTE.md)
    * [갤럭시 노트](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20%EB%85%B8%ED%8A%B8.md)
    * [갤럭시 R 스타일](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20R%20%EC%8A%A4%ED%83%80%EC%9D%BC.md)
    * [갤럭시 S III](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20S%20III.md)
    * [갤럭시 노트 II](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20%EB%85%B8%ED%8A%B8%20II.md)
    * [갤럭시 그랜드](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20%EA%B7%B8%EB%9E%9C%EB%93%9C.md)
    * [갤럭시 팝](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20%ED%8C%9D.md)
    * [갤럭시 S4](%EA%B0%A4%EB%9F%AD%EC%8B%9C%20S4.md) 등 이후 모델  

  * [팬택 베가](%ED%8C%AC%ED%83%9D%20%EB%B2%A0%EA%B0%80%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md)  

    * [베가 레이서](%EB%B2%A0%EA%B0%80%20%EB%A0%88%EC%9D%B4%EC%84%9C.md)
    * [베가 No.5](%EB%B2%A0%EA%B0%80%20No.5.md)
    * [베가 LTE](%EB%B2%A0%EA%B0%80%20LTE.md)
    * [베가 LTE M](%EB%B2%A0%EA%B0%80%20LTE%20M.md)
    * 베가 LTE EX
    * [베가 레이서 2](%EB%B2%A0%EA%B0%80%20%EB%A0%88%EC%9D%B4%EC%84%9C%202.md)
    * [베가 S5](%EB%B2%A0%EA%B0%80%20S5.md)
    * [베가 R3](%EB%B2%A0%EA%B0%80%20R3.md)
    * [베가 No.6](%EB%B2%A0%EA%B0%80%20No.6.md) 등 이후 모델  

  * [KT테크](KT%ED%85%8C%ED%81%AC.md)  

    * [테이크 타키](%ED%85%8C%EC%9D%B4%ED%81%AC%20%ED%83%80%ED%82%A4.md)
    * [테이크 HD](%ED%85%8C%EC%9D%B4%ED%81%AC%20HD.md)
    * [테이크 핏](%ED%85%8C%EC%9D%B4%ED%81%AC%20%ED%95%8F.md)
    * [테이크 LTE](%ED%85%8C%EC%9D%B4%ED%81%AC%20LTE.md)  

  * [LG 옵티머스](LG%20%EC%98%B5%ED%8B%B0%EB%A8%B8%EC%8A%A4.md)  

    * [프라다폰 3.0](%ED%94%84%EB%9D%BC%EB%8B%A4%ED%8F%B0%203.0.md)
    * [옵티머스 LTE](%EC%98%B5%ED%8B%B0%EB%A8%B8%EC%8A%A4%20LTE.md)
    * [옵티머스 LTE TAG](%EC%98%B5%ED%8B%B0%EB%A8%B8%EC%8A%A4%20LTE%20TAG.md)
    * [옵티머스 뷰](%EC%98%B5%ED%8B%B0%EB%A8%B8%EC%8A%A4%20%EB%B7%B0.md)
    * [옵티머스 3D 큐브](%EC%98%B5%ED%8B%B0%EB%A8%B8%EC%8A%A4%203D%20%ED%81%90%EB%B8%8C.md)
    * [옵티머스 LTE II](%EC%98%B5%ED%8B%B0%EB%A8%B8%EC%8A%A4%20LTE%20II.md)
    * [옵티머스 L7](%EC%98%B5%ED%8B%B0%EB%A8%B8%EC%8A%A4%20L%281%EC%84%B8%EB%8C%80%29#s-2.3.md)
    * [옵티머스 G](%EC%98%B5%ED%8B%B0%EB%A8%B8%EC%8A%A4%20G.md)
    * [옵티머스 뷰 II](%EC%98%B5%ED%8B%B0%EB%A8%B8%EC%8A%A4%20%EB%B7%B0%20II.md)
    * [옵티머스 G Pro](%EC%98%B5%ED%8B%B0%EB%A8%B8%EC%8A%A4%20G%20Pro.md) 등 이후 모델  

  * [블랙베리](%EB%B8%94%EB%9E%99%EB%B2%A0%EB%A6%AC.md)  

    * [블랙베리 볼드 9900](%EB%B8%94%EB%9E%99%EB%B2%A0%EB%A6%AC%20%EB%B3%BC%EB%93%9C.md) \- 대한민국에서 서비스하는 모바일카드 불가
    * [블랙베리 Q5](%EB%B8%94%EB%9E%99%EB%B2%A0%EB%A6%AC%20Q5.md)/[블랙베리 Q10](%EB%B8%94%EB%9E%99%EB%B2%A0%EB%A6%AC%20Q10.md) \- 원 통신사 단말기에서 앱을 실행시켜 주카드를 설정해 놓으면 해당 주카드로 오프라인에서만 사용 가능.  

  * [소니](%EC%86%8C%EB%8B%88.md) \- 원 통신사 단말기에서 앱을 실행시켜 주카드를 설정해 놓으면 해당 주카드로 오프라인에서만 사용 가능.  

    * [엑스페리아 Z1](%EC%97%91%EC%8A%A4%ED%8E%98%EB%A6%AC%EC%95%84%20Z1.md)
    * [엑스페리아 Z1 컴팩트](%EC%97%91%EC%8A%A4%ED%8E%98%EB%A6%AC%EC%95%84%20Z1.md)
    * <del>[엑스페리아 Z2](%EC%97%91%EC%8A%A4%ED%8E%98%EB%A6%AC%EC%95%84%20Z2.md)</del>
    * <del>[엑스페리아 Z3](%EC%97%91%EC%8A%A4%ED%8E%98%EB%A6%AC%EC%95%84%20Z3.md)</del>
    * <del>[엑스페리아 Z3 컴팩트](%EC%97%91%EC%8A%A4%ED%8E%98%EB%A6%AC%EC%95%84%20Z3%20%EC%BB%B4%ED%8C%A9%ED%8A%B8.md)</del>
    * Z2의 경우 4.4.4로 판올림하면 NFC 카드모드에 이상이 생겨 카드모드가 아예 안 된다는 보고가 나오고 있다. 더욱 불행한 사실은 Z3는 출시당시부터 4.4.4라는 점. <del>소니 개갞끼</del>  

  * [애플](%EC%95%A0%ED%94%8C%28%EA%B8%B0%EC%97%85%29.md) \- 애플페이 전용.  

    * [아이폰 6](%EC%95%84%EC%9D%B4%ED%8F%B0%206.md)
    * [아이폰 6 플러스](%EC%95%84%EC%9D%B4%ED%8F%B0%206%20%ED%94%8C%EB%9F%AC%EC%8A%A4.md)
    * [애플 워치](%EC%95%A0%ED%94%8C%20%EC%9B%8C%EC%B9%98.md)  

그 밖의 이용할 수 있는 기기

  

  * [닌텐도](%EB%8B%8C%ED%85%90%EB%8F%84.md)  

    * [amiibo](amiibo.md) \- 닌텐도에서 발매한 게임 연동 피규어. 아래의 기기들은 사실상 이걸 사용하기 위해 NFC 기능이 들어간 것이다.
    * [닌텐도 3DS](%EB%8B%8C%ED%85%90%EB%8F%84%203DS.md) \- 자체적으로는 NFC 기능을 지원하지 않으나 별도의 어댑터를 연결하여 사용할 수 있다.
    * [New 닌텐도 3DS](New%20%EB%8B%8C%ED%85%90%EB%8F%84%203DS.md) \- 구형과 달리 NFC 리더를 내장하고 있다. [2014년](2014%EB%85%84.md) [12월 9일](12%EC%9B%94%209%EC%9D%BC.md)부터 이를 이용해 교통카드를 통한 [닌텐도 eShop](%EB%8B%8C%ED%85%90%EB%8F%84%20%EB%84%A4%ED%8A%B8%EC%9B%8C%ED%81%AC#s-3.3.md) 잔액 추가기능을 이용할 수 있다.
    * [Wii U](Wii%20U.md)  

  * [삼성 NX](%EC%82%BC%EC%84%B1%20NX.md) 시리즈 카메라 - 최근 모델의 바디에 NFC 태그가 내장되어 스마트폰에 인식시키면 삼성 모바일링크 어플리케이션과 기기의 Wi-Fi Direct 기능을 작동시킨다.

`\----`

  * `[1]` [e-AMUSEMENT PASS](e-AMUSEMENT%20PASS.md)의 경우는 사용은 가능하지만 카드 번호가 매번 태그할때마다 랜덤으로 생성, [ALL.Net](ALL.Net.md)계열은 인식조차 되지 않는다. 이 방법으로 카드 번호를(1회용) 발급받아서 **안쓰는 카드 데이터를 옮겨버리면서 동시에 삭제할 수 있다.** 국내에서 가동중인 터치형 카드리더기를 채용한 [비마니 시리즈](%EB%B9%84%EB%A7%88%EB%8B%88%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md) 전부 가능. 다만 NFC를 실행시켜도 생각보다 인식이 잘 안될 수 있으며, 네트워크가 연결되어 있어야 한다. 리플렉에서는 잘 인식되는데 유비트나 사볼에서는 인식이 안되는 경우가 자주 있으니 NFC기능이나 핸드폰을 껏다 켜보자. 또한 이것은 국내판만 가능하며 일본에서는 인식은 되나 계정생성이 되지 않는다.
  * `[2]` 아이비콘은 NFC와 달리 [블루투스](%EB%B8%94%EB%A3%A8%ED%88%AC%EC%8A%A4.md) 기반이다.
  * `[3]` NFC와 NFC 태그의 차이에 주의하자. NFC 태그 = RFID 태그라고 생각하면 된다.
  * `[4]` <http://nelenkov.blogspot.kr/2012/08/accessing-embedded-secure-element-in.html>
  * `[5]` 일반 유심과의 차이는 금융정보를 저장하기 위한 메모리용량이 추가되었고 스마트폰의 NFC 통신칩과 직접 연결되기 위한 SWP용 핀이 있다. 6번 핀.
  * `[6]` 원 통신사 단말기에서 모바일캐시비·월렛 앱을 실행해 캐시비를 주교통카드로 선택하고 다시 그 유심을 엑스페리아 시리즈에 꽂는 식으로
  * `[7]` 다른 기능의 경우 확인바람
  * `[8]` 즉, NFC 향 첨가 수준의 서비스(...)
  * `[9]` 상기 언급한 캐시비·티머니 잔액 조회 앱 포함
  * `[10]` 물론 국내 폰 기준
  * `[11]` 상단의 알림 표시줄 왼쪽에 GPS아이콘이 점멸(깜빡깜빡)하거나 켜졌을 때
  * `[12]` 모두 통신사 프리로드 앱이다. 이 중 seioagent.apk는 구글플레이에 등록되어 있는 상태.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/NFC?action=edit&section=8)]

# 2. Not From Concentrate ¶

비농축과즙. 즉, 과일 그대로를 착즙해서 만든 쥬스다.

