## 목차

    

1. 개요 
2. 요구사양 

![https://s3.amazonaws.com/wordpressprod/blog/wp-content/uploads/2014/06
/front-view.jpg?width=550](https://s3.amazonaws.com/wordpressprod/blog/wp-
content/uploads/2014/06/front-view.jpg)

[[JPG external image]](https://s3.amazonaws.com/wordpressprod/blog/wp-
content/uploads/2014/06/front-view.jpg)

  
제스쳐기반 [HID](HID.md) 기기.

[[편집](http://rigvedawiki.net/r1/wiki.php/Myo?action=edit&section=1)]

## 1. 개요 ¶

  

[Thalmic Labs](https://www.thalmic.com/)에서 개발한 제스쳐기반 [HID](%EC%9D%B8%EA%B0%84%20%EC%9D%B8%ED%84%B0%ED%8E%98%EC%9D%B4%EC%8A%A4%20%EC%9E%A5%EC%B9%98.md)기기로
팔찌/아대 모양으로 되어있어서 팔에 끼워서 사용한다. 발음은 마이오로 근육을 뜻하는 그리스어 접두어에서 따왔다. 작동 원리는 센서를 이용해
근육의 전기 신호를 읽어내어 어떤 제스쳐를 취하고 있는지 알아내는 것이다.

  

![https://s3.amazonaws.com/wordpressprod/blog/wp-content/uploads/2013/08/arm_a
nd_signal.jpg?width=550](https://s3.amazonaws.com/wordpressprod/blog/wp-
content/uploads/2013/08/arm_and_signal.jpg)

[[JPG external image]](https://s3.amazonaws.com/wordpressprod/blog/wp-
content/uploads/2013/08/arm_and_signal.jpg)

▲작동원리를 설명하는 이미지.

  

2013년에 일반에 공개되어 2014년 9월 현재까지
[예약주문](https://www.thalmic.com/en/myo/preorder/)을 받고 있으며 가격은 $149.99 이다. 본래
2013년 말에 출시 예정이었으나 이런 새로운 기기들이 대부분 그렇듯 몇차례 미뤄졌었다. 출시를 두차례로 나눠서 하는데, 어느정도 개발
역량이 있는 사람들을 대상으로 한 Myo 개발자 키트(Developer Kit)는 2014년 7월에, 일반 사용자들을 위한 Myo 최종
버전(Final Unit)은 개발자 키트가 모두 배포되고 난 뒤 9월에 출시한다고
한다[#(영문)](https://www.thalmic.com/blog/unveiling-final-design-myo-armband/).
개발자 키트와 최종버전의 차이는 하드웨어적인 차이는 없고 딸려오는 펌웨어 등의 소프트웨어 차이만 있다.

  

2013년 말부터 Myo Alpha Unit 이라는 프로토타입을 선정된 개발자들에게 배포하고 있다. 이는 [LeapMotion](Leap%20Motion.md)이 했던것 처럼 출시 이후 사용자들을 위한 앱을 미리 준비하기 위함으로 보인다.

  

소프트웨어에 따라 두개의 Myo를 동시에 이용할 수 있다고도 하며, 이 때문인지 한개만 주문했을때 하나 더 주문해보는게 어떻냐고 메일이
오기도 한다.

  

2014년 6월 11일(한국시간 기준)에 발표한 [보도자료](https://www.thalmic.com/press/thalmic-labs-
unveils-final-design-myo-armband/)와 [블로그](https://www.thalmic.com/blog
/unveiling-final-design-myo-armband/)에 따르면 기존 알파버전 기기와는 전혀 다르게 디자인을 새로하다시피 하여
변경했으며 일부 외형 스펙`[1]`등이 더 좋아졌다.

  

2014년 9월 말 현재 아직도 개발자 키트를 배포하고 있어 일반 버전의 출시가 본래 예정되어 있던 2014년 9월보다 늦어질 가능성이 매우
높다. 2014년 7월부터 개발자 키트를 배송하고 있지만 매일 처리되는 수량이 적고, 배송지에 관계 없이 주문한 순서대로 배송하는 것이
아니라 북미 지역 주문자에게 우선적으로 배송하고 있어서 북미 지역이 아닌 주문자는 받기까지 한참 걸릴 것으로 예상되고 있다. 배송 상태에
관해 문의하는 사람이 하도 많았는지 배송 현황을 확인할 수 있는
[페이지](https://www.thalmic.com/en/myo/shipping/)를 만들었다. 그런데 2014년 10월 4일 현재 배송
시작 2~3개월이 지난 시점에서 최종 버전은 시작도 안했고 개발자 키트도 30%만 배송을 한 상황이다.

  

한국으로 보내지는 주문은 4~6주가 걸리며, 사정상 추적할 수 있는 송장 번호 등을 제공할 수 없다고 한다.

  

[[편집](http://rigvedawiki.net/r1/wiki.php/Myo?action=edit&section=2)]

## 2. 요구사양 ¶

구체적인 요구사양은 아직 나오지 않았으나 지원하는 OS로는 [윈도우](Microsoft%20Windows.md), Mac [OSX](OS%20X.md), [iOS](iOS.md), 그리고 [안드로이드](%EC%95%88%EB%93%9C%EB%A1%9C%EC%9D%B4%EB%93%9C%28%EC%9A%B4%EC%98%81%EC%B2%B4%EC%A0%9C%29.md)가 있고 연결은
[블루투스](%EB%B8%94%EB%A3%A8%ED%88%AC%EC%8A%A4.md) 4.0 Low Energy를 이용한다고 한다.

  

전원은 자체 내장 리튬이온 배터리로, 충전은 Micro-USB 케이블로 가능하다고 한다.

`\----`

  * `[1]` 접촉면이 알파유닛에선 [구리](%EA%B5%AC%EB%A6%AC.md)였으나 최종 버전에서는 의학용 [스테인레스](%EC%8A%A4%ED%85%8C%EC%9D%B8%EB%A0%88%EC%8A%A4.md) 스틸로 바뀌었고 디자인이 변경되면서 재질도 바꾸는 등의 변화가 있었고, 그로인해 중량도 25% 가량 더 가벼워지고 두께도 50% 가까이 얇아지는 효과가 있었다.

