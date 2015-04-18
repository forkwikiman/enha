  * [영어](%EC%98%81%EC%96%B4.md):digital multiplex
  * [약칭](%EC%95%BD%EC%B9%AD.md):DMX(Digital MultipleX)  

## Contents

    

1. 개요 
2. 방식 
3. 주 사용처 
4. 어떻게 하면 쓸 수 있나. 
    

4.1. 마스터 구입

4.2. 슬레이브 구입

4.3. 장비 연결

4.4. 장비 설정

4.5. 스테이지 설정

4.6. 구축 완료

5. 래퍼겸 배우 

[[edit](http://rigvedawiki.net/r1/wiki.php/DMX?action=edit&section=1)]

# 1. 개요 ¶

  

옛날 옛적 dimmer`[1]` 를 좀 더 편리하게 제어할 수 없을까 란 생각에서부터 출발하여, 지금은 모든 조명과 부수장비가 사용하는
인터페이스로서 당당하게 International Standard 가 된 규격이다.

  

본래 DMX 뒤에는 사용 가능한 정보의 양을 나타내는 숫자가 따라가지만, 어차피 대부분의 장비가 DMX 512, 심지어 싸구려
[스트로브](%EC%8A%A4%ED%8A%B8%EB%A1%9C%EB%B8%8C.md) 싸이키마저 DMX 512 를 완전 지원하므로 역시
DMX 512 기준으로 설명한다. 물론, 대부분이 하위규격이랑 똑같은 감이 없지않아 많으므로 크게 혼란이 있진 않을 것이다.

  

참고로, 그래서 지금 쓰는 규격은 정확하게 E1.11 - 2008, USITT DMX512-A 라는 스텐다드다. `[2]`

  

[[edit](http://rigvedawiki.net/r1/wiki.php/DMX?action=edit&section=2)]

# 2. 방식 ¶

  

DMX 는 [데이지 체인](%EB%8D%B0%EC%9D%B4%EC%A7%80%20%EC%B2%B4%EC%9D%B8.md)`[3]`형태의
전기 연결을 사용하며, EIA-485`[4]`전압이 신호로 흐른다. 게다가, 다른 통신선로와 달리 DMX 는 조명을 제어하는데 중점적으로
되어 있어서, 1개의 기기간 링크는 최대 1.2Km 까지 연결되도록 규정하고 있다. 또한, 포트는 모두 절연되어야 하는데, 사용처가 엄청나게
높은 전력의 조명이나 그런 쪽이면 그라운드 루프`[5]`가 발생하기 때문이다. 접속 형식은 인터넷 연결선 형식과 XLR(오디오기기
연결형식)이 있는데 1구골에 1정도가 RJ-45 형식이니, 그냥 하나만 된다 치면 속편하다. 가끔 독자규격의 기기도 나오는데, 굳이 필요하지
않으면 호환성을 위해 다른 기기를 찾는것도 좋다.

  

DMX 512 의 내부 전송속도는 256kbaud 인데, 이것저것 붙다보면 많이 느려진다. 기계에서 수신하여 처리하면 대략 0.001초가
소요된다. FTTH 를 생각해보면 간단한데, CSMA 로 동작하는 FTTH 특성상, 1개의 1.125Gbps 광케이블에 32가구의 수용자
모뎀과 연결된다. 이 때, 여러 수용가의 신호가 난립하는 FTTH 의 전송속도는 엄청나게 낮아진다.`[6]` DMX는 마커 뒤에 기계별로
쭈루루루루룩 가는 타입이지만, 여전히 기계수 늘어날수록 느려지기 마련이다.

  

DMX 512 도 해상도의 차이가 있다.  
8bit 지원 기기가 있는가 하면, 16bit 지원기기도 있다.`[7]`  
그런데 신경 안쓰고 살아도 잘돌아가니 너무 민감하게 반응하진 말것.`[8]`

  

[[edit](http://rigvedawiki.net/r1/wiki.php/DMX?action=edit&section=3)]

# 3. 주 사용처 ¶

DMX 의 시초가 시초이니만큼, 조명이 쓰이는 모든 곳에서 표준 인터페이스로 단단히 자리잡고 있다. 비록 전광판과 같은 고대역폭이 필요한
곳은 HD-SDI DualLink 등으로 수십 Gbps 의 속도를 확보하나, 간단한 조명 신호들은 모두 사용 가능하다. LED컨트롤러도
DMX 를 사용할 수 있다. 물론, DMX 지원 기기는 생각보다 비싸다.`[9]` 무빙 라이트도 가능하고, DMX 드라이 스모그
제네레이터`[10]` DMX 스모커`[11]` DMX 레이저 프로젝터`[12]`심지어 DMX CO2 솔레노이드와 DMX FireArt
Trigger 도 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/DMX?action=edit&section=4)]

# 4. 어떻게 하면 쓸 수 있나. ¶

  

[[edit](http://rigvedawiki.net/r1/wiki.php/DMX?action=edit&section=5)]

## 4.1. 마스터 구입 ¶

먼저, 싸게  

![http://westcoastradio.co.uk/images/dmx%20controller.jpg](http://westcoastrad
io.co.uk/images/dmx%20controller.jpg)

[[JPG external
image]](http://westcoastradio.co.uk/images/dmx%20controller.jpg)

  
이런 스텐드얼론 기계(35만원 정도)를 구입하거나

  

![http://img.diytrade.com/cdimg/742380/10364086/0/1252292962/DMX_USB_interface
_DMX_controller.jpg](http://img.diytrade.com/cdimg/742380/10364086/0/125229296
2/DMX_USB_interface_DMX_controller.jpg)

[[JPG external image]](http://img.diytrade.com/cdimg/742380/10364086/0/1252292
962/DMX_USB_interface_DMX_controller.jpg)

  
컴퓨터와 연결 가능한 인터페이스 변환기(30만원 정도)를 구입한다.

  

둘 다 마음에 안들면,  

![http://img.alibaba.com/img/pb/852/363/297/297363852_590.jpg](http://img.alib
aba.com/img/pb/852/363/297/297363852_590.jpg)

[[JPG external
image]](http://img.alibaba.com/img/pb/852/363/297/297363852_590.jpg)

  
컴퓨터에 연결 가능한 기계를 산다.`[13]`

  
  

[[edit](http://rigvedawiki.net/r1/wiki.php/DMX?action=edit&section=6)]

## 4.2. 슬레이브 구입 ¶

마스터를 구입했으면, 슬레이브로 연결 가능한 기계를 산다.  

![http://cachepe.samedaymusic.com/media/quality,85/PUNCHLEDPRORight-3114fa5539
a369227983b93d02173389.jpg](http://cachepe.samedaymusic.com/media/quality,85
/PUNCHLEDPRORight-3114fa5539a369227983b93d02173389.jpg)

[[JPG external image]](http://cachepe.samedaymusic.com/media/quality,85
/PUNCHLEDPRORight-3114fa5539a369227983b93d02173389.jpg)

  
고즈넋하게 색상과 밝기를 바꾸는 PAR 조명도,  

![http://image.made-in-china.com/2f0j00kClQcMSbLiqB/Violet-Laser-Light-DMX-
Light-Laser-Show.jpg](http://image.made-in-china.com/2f0j00kClQcMSbLiqB
/Violet-Laser-Light-DMX-Light-Laser-Show.jpg)

[[JPG external image]](http://image.made-in-china.com/2f0j00kClQcMSbLiqB
/Violet-Laser-Light-DMX-Light-Laser-Show.jpg)

  
화려한 레이저도,

  

어떤 것이라도 DMX 라는 인터페이스면 연결 가능하다.

  
  

[[edit](http://rigvedawiki.net/r1/wiki.php/DMX?action=edit&section=7)]

## 4.3. 장비 연결 ¶

![http://www.wahlberg.dk/Portals/0/products/Motion/250_DCmotor_controller_70w_
S/website/DC_controller_DMX-stik.jpg](http://www.wahlberg.dk/Portals/0/product
s/Motion/250_DCmotor_controller_70w_S/website/DC_controller_DMX-stik.jpg)

[[JPG external image]](http://www.wahlberg.dk/Portals/0/products/Motion/250_DC
motor_controller_70w_S/website/DC_controller_DMX-stik.jpg)

  
이렇게 생긴 부분끼리 연결한다. out 은 in 에 꼽아야 한다.

  

DMX 의 체널을 설정한다. 1개의 레일은 각 수신 시작 넘버를 가지며, 사용하는 기계가 점유하는 체널 수 만큼 밀어내게 된다. 만약 4개의
14체널 무빙라이트 가 있으면, 첫 기기는 0으로, 다음 기기는 14, 다음 기기는 28 등으로 설정한다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/DMX?action=edit&section=8)]

## 4.4. 장비 설정 ¶

컴퓨터 연결이면 이런 화면  

![http://www.djkit.com/images/products/cue001_in1.jpg](http://www.djkit.com/im
ages/products/cue001_in1.jpg)

[[JPG external image]](http://www.djkit.com/images/products/cue001_in1.jpg)

  

![http://www.djsuperstore.co.uk/pimages/224366-2.jpg](http://www.djsuperstore.
co.uk/pimages/224366-2.jpg)

[[JPG external image]](http://www.djsuperstore.co.uk/pimages/224366-2.jpg)

  
을 불러오고 기기에서 사용중이면 새로운 장비 설정을 만든다.

  

각 조명에서 점유하는 체널 수, 각 체널별 동작 특성을 설정한다. 무빙라이트 구입시 가장 튼튼한 종이에 적혀있는게, 기기의 무개와 크기,
출력 그리고 DMX 체널 셋팅방법과 체널별 동작이다.  

![http://www.특수램프.kr/bemarket/imgs/save/upload/b003_402.jpg](http://www.%ED%8A
%B9%EC%88%98%EB%9E%A8%ED%94%84.kr/bemarket/imgs/save/upload/b003_402.jpg)

[[JPG external image]](http://www.%ED%8A%B9%EC%88%98%EB%9E%A8%ED%94%84.kr/bema
rket/imgs/save/upload/b003_402.jpg)

  
이런 식으로 적혀있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/DMX?action=edit&section=9)]

## 4.5. 스테이지 설정 ¶

각 기기의 장면설정으로 들어가, 현재 접속중인 장비의 프리셋을 모두 불러온다.`[14]`  
각 처음 연출과 끝 연출을 입력하여, 기기들이 제대로 연결되었는지 확인한다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/DMX?action=edit&section=10)]

## 4.6. 구축 완료 ¶

축하드립니다. 기계의 설정이 완료되셨습니다. 이제부턴 마음껏 장면들을 만들어보세요. =) 는
[개뿔](%EA%B0%9C%EB%BF%94.md)이고, 일단 이까지 오기 엄청나게 힘들다. 이후 프로그램 짜기 등등이 있는데, 이
다음부턴 동영상 강의를 첨부한다.

  

width="425" height="349"><param name="movie" value="http://www.youtube.com/v/S
vs<del>6XgRIY?version=3&hl=ko_KR"></param><param name="allowFullScreen"
value="true"></param><param name="allowscriptaccess"
value="always"></param><embed
src="http://www.youtube.com/v/Svs</del>6XgRIY?version=3&hl=ko_KR"
type="application/x-shockwave-flash" width="425" height="349"
allowscriptaccess="always" allowfullscreen="true"></embed></object>  
시리즈물이니, 계속 보면 된다.

  

기초강의를 다 수강하였으면, 본격적으로 좀 더 어려운 것을 사용해보도록 하자.

  

width="425" height="349"><param name="movie"
value="http://www.youtube.com/v/d6dvRc4MbAE?version=3&hl=ko_KR"></param><param
name="allowFullScreen" value="true"></param><param name="allowscriptaccess"
value="always"></param><embed
src="http://www.youtube.com/v/d6dvRc4MbAE?version=3&hl=ko_KR"
type="application/x-shockwave-flash" width="425" height="349"
allowscriptaccess="always" allowfullscreen="true"></embed></object>

  

마지막으로, 컴퓨터 프로그램을 이용하는 분들은 이것도 된다.

  

width="425" height="349"><param name="movie"
value="http://www.youtube.com/v/szLmAPW39uE?version=3&hl=ko_KR"></param><param
name="allowFullScreen" value="true"></param><param name="allowscriptaccess"
value="always"></param><embed
src="http://www.youtube.com/v/szLmAPW39uE?version=3&hl=ko_KR"
type="application/x-shockwave-flash" width="425" height="349"
allowscriptaccess="always" allowfullscreen="true"></embed></object>

  

[[edit](http://rigvedawiki.net/r1/wiki.php/DMX?action=edit&section=11)]

# 5. 래퍼겸 배우 ¶

[DMX(래퍼)](DMX%28%EB%9E%98%ED%8D%BC%29.md) 항목 참조.

`\----`

  * `[1]` 조광기. 읽으면 dimmer 라는 것으로, 사이리스터를 이용한 phase shift control 을 사용해 조명의 밝기를 조정하는 기계다.
  * `[2]` A 의 의미는 [비동기식 전송](%EB%B9%84%EB%8F%99%EA%B8%B0%EC%8B%9D%20%EC%A0%84%EC%86%A1.md) 이라는 의미이다. DMX 는 필연적으로 비동기전송을 할 수 밖에 없는데, 뒤에 이유가 나온다.
  * `[3]` 기계가 일렬로 쭈우우우우욱 연결된 모습을 연상하자. 혹은 고리모양으로 해도 된다. DMX는 대신 약간 차이가 있는데, 대상 기계에 in, out이 있으면, 마스터엔 out 만 있다. 또한 DMX엔 링크당 제한이 있어 필요시 분기기를 쓰게된다. 계속 읽어보자.
  * `[4]` RS-485의 프로토콜이 아니라, 하드웨어 접속 규격. 전송전압은 알다시피 ±5V.
  * `[5]` 신호가 접지를 타고 다시 시그널로 들어오는 현상 혹은 노이즈가 접지를 타고 시그널로 들어오는 현상.
  * `[6]` 신호 교란에 의함.
  * `[7]` 중간은 없다.
  * `[8]` 한바퀴 돌아가는데 256 단계로 끊어져 보인다거나 조명의 밝기를 천천히 올리는데 천천히 올라가는게 아니라 ""뚝뚝 끊어져"" 올라가는 게 눈에 보일 뿐이다.
  * `[9]` 인터페이스가 비싼게 아니라 그 이하 제품에 DMX 를 달아봐야 쓸데가 없어서 안달릴 뿐이다. 아니면 집적 만들어도 된다.
  * `[10]` 바닥에 깔리는 안개를 만드는 기계. 드라이 아이스와 점성이 있는 드라이 스모그액을 사용하여 잘 증산하지 않는 뿌연 안개를 만든다. 흡입해도 안전함.
  * `[11]` 대기를 뿌옇게 만드는 기계. 스모크액을 태워 연기를 만드는 것으로, 위로 떠오르는 연기를 만들어낸다. 그렇다고 위에 모이진 않으며, 잘 섞여 전체적으로 뿌옇게 되는것이 목적. 조명 효과를 극대화 할 수 있다.
  * `[12]` 사실 이쪽은 ILDA 라는 전용 인터페이스가 있다. 물론 국제규격이니 집적 만들어 써도 잘들러붙는다.
  * `[13]` 440만원 한다. 대신, 2048 extended 체널 지원으로, 연결가능 기기는 엄청나게 더 늘어났다. dimmer 전용 기능도 있음
  * `[14]` 그 전에 프리셋 다 짜두고. 참고로, 순서가 맞아야 제대로 동작한다.

