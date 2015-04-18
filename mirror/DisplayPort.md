![http://ncc.phinf.naver.net/ncc01/2012/4/9/220/img_01.jpg?width=300](http://n
cc.phinf.naver.net/ncc01/2012/4/9/220/img_01.jpg)

[[JPG external
image]](http://ncc.phinf.naver.net/ncc01/2012/4/9/220/img_01.jpg)

  
DisplayPort`[1]`

## Contents

    

1. 개요 
2. 특징 
    

2.1. 슬림포트

3. 미니 디스플레이포트 

[[edit](http://rigvedawiki.net/r1/wiki.php/DisplayPort?action=edit&section=1)]

## 1. 개요 ¶

VESA에서 정한 영상 전송 표준 커넥터이며, 약칭으로 DP라고도 부른다. HDMI와 마찬가지로 영상 신호뿐만 아니라 음성 신호도 내보낼 수
있다. 특허 사용료도 없고 `[2]`, [DVI](DVI.md)에 대해 하위 호환성도 가지고 있고, HDMI보다 대역폭도 더 높다는
여러 장점이 있음에도 불구하고, 널리 쓰이질 않는다. `[3]` 사실상 일반시장에서는 HDMI에 완전히 밀려버린 수준. 하지만 전문가용으로
널리 쓰이고 있다 Nvidia의 쿼드로나 AMD의 FirePro에는 DisplayPort만 달려있지 HDMI는 달려있지않다.

  

디스플레이 포트 1.0은 2006년 5월 3일에 승인되었다. 이후 2007년 4월 2일에 버전 1.1a, 2009년 12월 22일에 1.2가
승인되었다. 2014년 9월 15일 1.3이 승인되었다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/DisplayPort?action=edit&section=2)]

## 2. 특징 ¶

8채널 24비트/196khz Linear PCM 음성신호와 영상을 동시에 전송할 수 있다. 또한 핫 플러깅을 지원하여 장치에 플러그를 꼽으면
자동으로 감지된다.

  

디스플레이 포트 버전은 케이블에 관한 것이 아니라 디스플레이 포트의 데이터 전송을 담당하는 반도체에 관한 것이라케이블 버전에 따른 차이는
없다. 핀 20개에 선만 전부 연결되어있고 차폐만 잘되어 있다면 단자 모양이 바뀔 때 까지 계속 쓸 수 있다.

  

현재 국내에는 디스플레이 포트 1.2 인증 케이블이 거의 없다. 굳이 인증 받은걸 사고 싶다면 1.1a 케이블을 사면 된다.
[DisplayPort FAQ 2번째 항목 참조](http://www.displayport.org/faq/) FAQ에서 A
DisplayPort cable is a DisplayPort cable; 이란 말을 주목하자 선은 그냥 선이다.

  

디스플레이 포트도
[썬더볼트](Thunderbolt%28%EC%9D%B8%ED%84%B0%ED%8E%98%EC%9D%B4%EC%8A%A4%29.md)와
마찬가지로 Daisy chaining이 가능하다. 지원하는 모니터가 적을 뿐.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/DisplayPort?action=edit&section=3)]

### 2.1. 슬림포트 ¶

2012년 6월에 승인된 기술로 디스플레이 포트를 기반으로하며 모바일리티 디스플레이 포트(MyDP)라고도 불린다. 4K와 8채널 오디오
출력을 지원하며 오픈 소스에 로열티가 없기 때문에 [MHL](MHL.md)의 대안 기술로 사용된다. LG전자의 최신
[스마트폰](%EC%8A%A4%EB%A7%88%ED%8A%B8%ED%8F%B0.md)이나 [구글넥서스](%EA%B5%AC%EA%B8%80%20%EB%84%A5%EC%84%9C%EC%8A%A4.md)
[4](%EB%84%A5%EC%84%9C%EC%8A%A4%204.md) 부터 탑재되어 사용되고 있다. MHL처럼 추가로 전원을 인가하지
않아도 되는 장점이 있으나, 대신 USB OTG와의 동시 연결이 불가능하다는 치명적인 단점이 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/DisplayPort?action=edit&section=4)]

## 3. 미니 디스플레이포트 ¶

![http://bitguru.files.wordpress.com/2008/11/molexminidisplayport.gif](http://
bitguru.files.wordpress.com/2008/11/molexminidisplayport.gif)

[[GIF external
image]](http://bitguru.files.wordpress.com/2008/11/molexminidisplayport.gif)

  
일반적인 디스플레이포트에 비해 크기가 작아지고 대신 두께가 약간 두꺼워진 포트이다.`[4]` 모양이 다를 뿐 핀 개수나 케이블 특성은 같다.
노트북 등의 모바일 디바이스나, 그래픽카드에서 여러개의 디스플레이포트를 탑재할 때 사용한다.

  

[AMD](AMD.md)는 멀티 모니터 확장 기술인 **Eyefinity** 라는 기술을 보유 하고 있는데, 여러개의 모니터를 하나의
화면으로 묶어서 사용하는 것이다. 하나의 그래픽 카드가 최대 6대의 모니터까지 연결이 가능한데`[5]`, 단자의 크기와 대역폭의 문제
때문에, 일반적으로 6개의 Mini-DP 포트를 사용하여 구성되어 있다. <del>이 덕분에 미니 DP용 젠더가 Mini-VGA나 Mini-
DVI용 젠더만큼 귀하지는 않다</del> [어떻게 생겼는지 궁금하면 여기서 확인](http://www.hitechreview.com/it-
products/pc/ati-radeon-hd-5870-eyefinity-6-edition-graphics-card-is-
here/23286/)

  

참고로 [썬더볼트](%EC%8D%AC%EB%8D%94%EB%B3%BC%ED%8A%B8.md) 인터페이스는 미니디스플레이포트와 같은
단자를 사용하고 있으며 케이블도 호환이 된다. 물론 썬더볼트 인터페이스의 데이터 전송 기능은 썬더볼트를 지원하는 기기끼리에서만 사용이
가능하다.

`\----`

  * `[1]` Display Port라고 띄어쓰는 경우가 있는데 틀린 표기이다. 공식 명칭이 DisplayPort.
  * `[2]` HDMI 단자 사용 기기는 제품당 0.15$의 특허료를 지불한다. 기실 DVI란 디지털 단자가 이미 있는 컴퓨터 업계가 HDMI를 주력으로 채택하지 않고 굳이 또 DP를 만든게 이 특허료 내기 싫어서다.
  * `[3]` 그러나 2014년이후나오는 고급VGA, 모니터에서는 점차 사용하는 양이 늘어나고 있다.
  * `[4]` 두께는 숫단자가 4.5mm. 즉 USB Type-A와 높이를 맞췄다.
  * `[5]` 이는 4개의 그래픽 카드를 CF하면 한 컴퓨터에서 24개 모니터 출력이 된다는 말이다!

