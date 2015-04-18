## Contents

    

1. Home Trading System 
    

1.1. 개요

1.2. 금융사별 HTS

2. [How to Survive](How%20to%20Survive.md)

[[edit](http://rigvedawiki.net/r1/wiki.php/HTS?action=edit&section=1)]

# 1. Home Trading System ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/HTS?action=edit&section=2)]

## 1.1. 개요 ¶

![http://img.daewoodirect.com/online/vi_020502_01.gif](http://img.daewoodirect
.com/online/vi_020502_01.gif)

[[GIF external image]](http://img.daewoodirect.com/online/vi_020502_01.gif)

  
출처: KDB대우다이렉트

  

HTS란 개인 투자자가 객장에 나가지 않고, 집이나 사무실에서 주식과 파생상품 등 금융 투자 거래를 할 수 있는 프로그램인
'홈트레이딩시스템'을 뜻한다. 인터넷에 접속된 컴퓨터를 이용해 매매는 물론 정보 검색까지 할 수 있다.
[한국거래소](%ED%95%9C%EA%B5%AD%EA%B1%B0%EB%9E%98%EC%86%8C.md)
[유가증권시장](%EC%9C%A0%EA%B0%80%EC%A6%9D%EA%B6%8C%EC%8B%9C%EC%9E%A5.md)과
파생상품시장에서는 50% 이상, [코스닥](%EC%BD%94%EC%8A%A4%EB%8B%A5.md)에서는 거래의 90% 이상이 HTS를
통해 이루어진다. 즉 [펀드](%ED%8E%80%EB%93%9C.md)를 제외한 금융투자의 필수품.

  

홈트레이딩시스템(HTS)의 효시는 지난 1980년대 말과 90년대 초반 9인치 화면 모니터나 TV를 전용선에 연결시켜 단순히 주식시세 조회만
할 수 있는 기능만 제공된 '가정용 투자정보 시스템'이라고 할 수 있다.

  

온라인 주문이 가능하게 된 것은 인터넷 통신환경이 본격화하기 시작한 97년이후로 98,99년 증시 활황과 더불어 온라인 주식거래 인구가
폭발적으로 늘어나자 증권사들의 온라인거래 수수료율 인하와 함께 다양한 HTS프로그램을 선보였다.
[대신증권](%EB%8C%80%EC%8B%A0%EC%A6%9D%EA%B6%8C.md)의 사이보스(CYBOS)를 최초의 HTS로 공인하고
있다.

  

결국 증권사간 HTS의 차별화 경쟁이 촉발됐고 초고속 통신망 보급이 확산되면서 불과 2년 새 더욱 빠르고 안정화된 시스템으로 변화했다.

  

갈수록 늘어가는 홈트레이더들의 요구에 맞추기 위해 계속 기능 개선을 하다보니, 대부분의 HTS는 '기관투자자용' 수준까지 올라가고 있다는
평가를 받고 있다. 실제로 2004년만 해도 기관투자자들의 트레이딩 툴은 일반 증권사/선물사 고객용과 큰 차이가 없었다.

  

[블래스트씨앤알](http://blastcnr.com/01_be/01_02.php)(舊 스톡피아)이라는 회사가 개인투자자용 HTS에 대해
매년 평가를 하고 있다.

  

초기에는 시세를 보여주고 주문을 하는 기능밖에 없었지만, 2000년대 중반부터 각종 지표 분석부터 매매시점까지 판단하는 상담까지 하고 있다.
특히 각 종목의 등락에 따른 매매 조건을 입력해 놓으면 자동적으로 매매를 진행하는 [시스템 트레이딩](%EC%8B%9C%EC%8A%A4%ED%85%9C%20%ED%8A%B8%EB%A0%88%EC%9D%B4%EB%94%A9.md) 기능이 중점적으로 개발되고 있다.

  

[대신증권](%EB%8C%80%EC%8B%A0%EC%A6%9D%EA%B6%8C.md)에서 시스템 트레이딩을 위해서 [MicrosoftWindows](Microsoft%20Windows.md)의 [COM](COM.md) 서버를 이용 [비주얼베이직](BASIC.md)과 [C++](C++.md), DHTML 등의 프로그래밍 툴로 마치 나만의 HTS 같은 것을 만들 수
있는 시세 가공 [API](API.md)를 공개하고 있고, 다른 금융투자회사에서도 [DDE](DDE.md) 등을 이용 [MS엑셀](MS%20%EC%97%91%EC%85%80.md) 같은 소프트웨어에 시세 및 매매주문 데이터를 연동할 수 있다. 그런데
2012년에 [한국거래소](%ED%95%9C%EA%B5%AD%EA%B1%B0%EB%9E%98%EC%86%8C.md)와
[코스콤](%EC%BD%94%EC%8A%A4%EC%BD%A4.md)에서 이와 같은 시세 재분배가 업무규정 위반이라고 발표하면서 이런
서비스가 불투명해질 뻔했으나 곧 정리되었다. 즉 시세 데이터를 직접 다루고 싶으면 공짜로 쓰지 말고
[코스콤](%EC%BD%94%EC%8A%A4%EC%BD%A4.md)에 시세 이용료를 내라는 말이었다.

  

한국의 일반 HTS가 시장 정보를 수신하는 통신 과정은 대략 다음과 같다.  
[한국거래소](%ED%95%9C%EA%B5%AD%EA%B1%B0%EB%9E%98%EC%86%8C.md) 매매시스템에서 매매 체결 또는
호가 접수→한국거래소 시장정보 분배 서버에서 호가 정렬 등 가공→[증권사](%EC%A6%9D%EA%B6%8C%EC%82%AC.md)
또는 [선물회사](%EC%84%A0%EB%AC%BC%ED%9A%8C%EC%82%AC.md) 원장 서버에서 자신의 매매 정보를
가공→증권사 또는 선물회사 시장정보 분배 서버→HTS

  

주문을 송신하는 과정도 시세분배 과정을 제외한 역순이라 보면 된다.

  

2009년에는 [코스콤](%EC%BD%94%EC%8A%A4%EC%BD%A4.md)의 증권사용 미들웨어인 PowerBase 서비스용
데이터센터에 입주한 일부 증권,선물사가 0.004초정도 접속이 빠르다는 사실이 밝혀져 매매시스템 접속의 형평성 논란이 시작되었다.

  

[스마트폰](%EC%8A%A4%EB%A7%88%ED%8A%B8%ED%8F%B0.md)이 대중화됨에 따라
[스마트폰](%EC%8A%A4%EB%A7%88%ED%8A%B8%ED%8F%B0.md)과
[태블릿](%ED%83%9C%EB%B8%94%EB%A6%BF.md)용 HTS 앱도 많다. 기능은 시세조회와 매매주문 위주.

  

개인투자자가 많이 사용하는 HTS로는 [키움증권](%ED%82%A4%EC%9B%80%EC%A6%9D%EA%B6%8C.md)의 영웅문이
있다.  
[FX마진](FX%EB%A7%88%EC%A7%84.md)용으로는 러시아에서 만든 MetaTrader가 인기가 많다.

  

미국이나 유럽, 일본등 해외에서 쓰이는 HTS`[1]`는 의외로 한국의 HTS들보다 성능이 뒤떨어진다. 단, FX마진의 MetaTrader만
제외하고...

[[edit](http://rigvedawiki.net/r1/wiki.php/HTS?action=edit&section=3)]

## 1.2. 금융사별 HTS ¶

[대신증권](%EB%8C%80%EC%8B%A0%EC%A6%9D%EA%B6%8C.md)

U-Cybos

[대신증권](%EB%8C%80%EC%8B%A0%EC%A6%9D%EA%B6%8C.md) 크레온

크레온

[대우증권](%EB%8C%80%EC%9A%B0%EC%A6%9D%EA%B6%8C.md)

Qway NEO

[대우증권](%EB%8C%80%EC%9A%B0%EC%A6%9D%EA%B6%8C.md) 다이렉트

다이렉트

[미래에셋증권](%EB%AF%B8%EB%9E%98%EC%97%90%EC%85%8B%EC%A6%9D%EA%B6%8C.md)

카이로스

[BS투자증권](BS%ED%88%AC%EC%9E%90%EC%A6%9D%EA%B6%8C.md)

QFIT

[삼성증권](%EC%82%BC%EC%84%B1%EC%A6%9D%EA%B6%8C.md)

POP

[신한금융투자](%EC%8B%A0%ED%95%9C%EA%B8%88%EC%9C%B5%ED%88%AC%EC%9E%90.md)

신한아이

[신한금융투자](%EC%8B%A0%ED%95%9C%EA%B8%88%EC%9C%B5%ED%88%AC%EC%9E%90.md) S-Lite

S-Lite

[NH투자증권](NH%ED%88%AC%EC%9E%90%EC%A6%9D%EA%B6%8C.md)

Mug

[NH투자증권](NH%ED%88%AC%EC%9E%90%EC%A6%9D%EA%B6%8C.md) TX

TX

[이트레이드증권](%EC%9D%B4%ED%8A%B8%EB%A0%88%EC%9D%B4%EB%93%9C%EC%A6%9D%EA%B6%8C.md)

X-ing

[유안타증권](%EC%9C%A0%EC%95%88%ED%83%80%EC%A6%9D%EA%B6%8C.md)

MyNet W

[키움증권](%ED%82%A4%EC%9B%80%EC%A6%9D%EA%B6%8C.md)

영웅문

[하나대투증권](%ED%95%98%EB%82%98%EB%8C%80%ED%88%AC%EC%A6%9D%EA%B6%8C.md) 피가로

Hi-Five

[하이투자증권](%ED%95%98%EC%9D%B4%ED%88%AC%EC%9E%90%EC%A6%9D%EA%B6%8C.md)

싸이칸

[한국투자증권](%ED%95%9C%EA%B5%AD%ED%88%AC%EC%9E%90%EC%A6%9D%EA%B6%8C.md)

eFriend

[한국투자증권](%ED%95%9C%EA%B5%AD%ED%88%AC%EC%9E%90%EC%A6%9D%EA%B6%8C.md) 뱅키스

eFriend

[현대증권](%ED%98%84%EB%8C%80%EC%A6%9D%EA%B6%8C.md)

You First

[KB투자증권](KB%ED%88%AC%EC%9E%90%EC%A6%9D%EA%B6%8C.md)

Plustar

[삼성선물](%EC%82%BC%EC%84%B1%EC%84%A0%EB%AC%BC.md)

FuturesNet S

[KR선물](KR%EC%84%A0%EB%AC%BC.md)

SilKRoad

[[edit](http://rigvedawiki.net/r1/wiki.php/HTS?action=edit&section=4)]

# 2. [How to Survive](How%20to%20Survive.md) ¶

  * [스팀](%EC%8A%A4%ED%8C%80.md)에서 구매할 수 있는 호러 생존 액션 RPG 게임 [How to Survive](How%20to%20Survive.md) 의 약자. 자세한 것은 해당 항목 참조.  

`\----`

  * `[1]` HTS는 한국에서만 쓰는 표현이지만(뜻이 주택매매체계가 되어 버리는 문제가...)... 영미계에서는 트레이딩 플랫폼, 일본에서는 트레이딩 툴 이라고 하기도...

