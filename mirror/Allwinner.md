![allwinnertech.png](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Allwinner/al
lwinnertech.png)

[PNG image (7.2 KB)]

2007년에 설립한 중국의 메이저 모바일 AP 설계사. 중국 광둥성 주하이에 본사가 있다.  
[공식 홈페이지](http://www.allwinnertech.com/en/)

## Contents

    

1. 개요 
2. 특징 
3. 주요 제품 목록 

[[edit](http://rigvedawiki.net/r1/wiki.php/Allwinner?action=edit&section=1)]

## 1. 개요 ¶

[중국](%EC%A4%91%EA%B5%AD.md)의 [AP](SoC.md) 설계사.
[ARM](ARM%20Holdings.md) 기반의 AP를 설계하는 업체이다. 동영상 재생에 강하고, 배터리 효율이 대체로 다른 중국제
AP보다 좋다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Allwinner?action=edit&section=2)]

## 2. 특징 ¶

[중국제 태블릿 컴퓨터](%EC%A4%91%EA%B5%AD%EC%A0%9C%20%ED%83%9C%EB%B8%94%EB%A6%BF%20%EC%BB%B4%ED%93%A8%ED%84%B0.md)에 락칩과 비슷한 규모로 사용되어지는 AP이다. 저사양 기기에서는 락칩보다
Allwinner의 AP가 많이 쓰이는데, 동영상 코덱 지원이 우수하고 2160p 동영상도 재생을 지원하기 때문.

  

[락칩](%EB%9D%BD%EC%B9%A9.md)과는 다른 특징이라면, 올위너는 Cortex-A9 기반의 AP가 없다. `[1]`
Cortex-A7의 사용으로, 성능은 조금 부족하지만 배터리 효율을 다른 중국제 AP보다 좋게 하려고 의도한듯. <del>그런데 배터리
효율도 기기 제조사, 펌웨어 마다 제각각이다</del>  
커널 지원도 독특한데, 락칩은 기본 최저클럭이 높게(300Mhz 이상)설정되어 있지만 올위너는 100Mhz 이하로 낮출 수 있다. 또,
오버클럭도 지원한다.

  

2011년에는 Cortex-A8 기반의 A10 등을 내놓았고, 점차 Cortex A7의 A20, A31, A31s 등을 출시하였다. A31은
발열, 배터리 효율 문제로 한때 이슈가 되었다.

  

2014년 4월 중순, 홍콩 전자쇼에서 A80 옥타코어 프로세서가 공개되었다. Cortex-A7과 Cortex-A15의 big-LITTLE
방식으로 동작하는듯. 2014년의 락칩의 RK3288과 A80의 신형 프로세서가 어떤 성능을 보여줄지 기대되는 부분.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Allwinner?action=edit&section=3)]

## 3. 주요 제품 목록 ¶

-A10  

![http://www.allwinnertech.com/uploads/140310/1-140310140405537.jpg](http://ww
w.allwinnertech.com/uploads/140310/1-140310140405537.jpg)

[[JPG external
image]](http://www.allwinnertech.com/uploads/140310/1-140310140405537.jpg)

  
2011년 출시된 싱글코어
[Cortex-A8](ARM%20Cortex-A%20%EC%8B%9C%EB%A6%AC%EC%A6%88#s-1.1.3.md) 1Ghz
프로세서. GPU는 Mali-400 싱글코어. 그래서 A10을 사용한 태블릿의 광고에는 꼭 고사양 GPU라는 말이 들어있다. 실상은 CPU가
딸려서 게임도 힘들다. 참고로, 사양이 부정확하게 표시된 기기, 예를 들어 CPU에 그냥 'Cortex-A8 1.2Ghz~1.5Ghz'
이런식으로 표시된 기기는 대부분 A10이다. 1.2, 1.5Ghz라는 것도 다 거짓광고. 1150Mhz 이상으로는 오버클럭이 힘들다.  
2160p 재생을 지원한다. 큐비보드1에도 사용되었던 프로세서.

  

-A10s  

![http://www.allwinnertech.com/uploads/140310/1-14031014042O39.jpg](http://www
.allwinnertech.com/uploads/140310/1-14031014042O39.jpg)

[[JPG external
image]](http://www.allwinnertech.com/uploads/140310/1-14031014042O39.jpg)

  
A10의 염가판. 대부분 A10과 동일하나 1080p 까지의 영상만 공식적으로 지원한다.

  

-A13  

![http://www.allwinnertech.com/uploads/140310/1-140310140343S9.jpg](http://www
.allwinnertech.com/uploads/140310/1-140310140343S9.jpg)

[[JPG external
image]](http://www.allwinnertech.com/uploads/140310/1-140310140343S9.jpg)

  
A10s와 비슷하나 [HDMI](HDMI.md)가 빠진 버전. 주로 소형 기기에 사용된다.

  

-A20  

![http://www.allwinnertech.com/uploads/140310/1-140310140319459.jpg](http://ww
w.allwinnertech.com/uploads/140310/1-140310140319459.jpg)

[[JPG external
image]](http://www.allwinnertech.com/uploads/140310/1-140310140319459.jpg)

  
2012년 12월 출시된 듀얼코어
[Cortex-A7](ARM%20Cortex-A%20%EC%8B%9C%EB%A6%AC%EC%A6%88#s-1.1.2.md)에
Mali-400 MP2가 사용됨.

  

-A23  

![http://www.allwinnertech.com/uploads/140310/1-140310140204630.jpg](http://ww
w.allwinnertech.com/uploads/140310/1-140310140204630.jpg)

[[JPG external
image]](http://www.allwinnertech.com/uploads/140310/1-140310140204630.jpg)

  
A20과 비슷하다.

  

-A31  

![http://www.allwinnertech.com/uploads/140310/1-140310135912157.jpg](http://ww
w.allwinnertech.com/uploads/140310/1-140310135912157.jpg)

[[JPG external
image]](http://www.allwinnertech.com/uploads/140310/1-140310135912157.jpg)

  
2012년 12월 출시된 쿼드코어
[Cortex-A7](ARM%20Cortex-A%20%EC%8B%9C%EB%A6%AC%EC%A6%88#s-1.1.3.md) 1.2Ghz
프로세서. GPU는 Mali-400이 아닌 SGX544 MP2가 탑재되었다. 공정은 40nm. 발열, 소비전력 문제로 상당히 말이 많다.
이전까지 우세했던 대기전력 효율도 나빠졌다는 의견이 많다. (중국 태블릿 제조사의 펌웨어 문제일 수도 있지만 대부분 같은 문제를 호소한다.)  
그런데 성능도 별로라서, 동영상 재생 이외에는 특별히 두각을 나타내는 부분이 없다. 비슷한 시기에 출시된 락칩 RK3188
[Cortex-A9](ARM%20Cortex-A%20%EC%8B%9C%EB%A6%AC%EC%A6%88#s-1.1.4.md) 쿼드코어는
비록 Mali-400 MP4를 사용하긴 했지만 CPU가 강력하여, 논리연산은 넘사벽. A31이 안투투 12000점 정도인데, RK3188은
19000점대. <del>물론 실제 성능에서의 괴리는 확실히 존재</del>  
4K를 공식 지원한다.  
레티나 태블릿에서도 사용된 프로세서이고, 아이뮤즈의 [뮤패드](%EB%AE%A4%ED%8C%A8%EB%93%9C.md)에도 사용됨.

  

-A31s  

![http://www.allwinnertech.com/uploads/140310/1-140310140045548.jpg](http://ww
w.allwinnertech.com/uploads/140310/1-140310140045548.jpg)

[[JPG external
image]](http://www.allwinnertech.com/uploads/140310/1-140310140045548.jpg)

  
A31의 염가판 프로세서. 4K를 지원하지 않고, 2160p를 지원한다. A31의 경우 1080p 에서 60프레임까지 보장하지만 A31s는
30프레임이 공식지원. 그리고 램을 1GB 까지만 지원한다. A31에서의 문제점이 다소 개선되었다.

  

-A33  

![http://www.allwinnertech.com/uploads/140603/2-1406031I04M38.jpg](http://www.
allwinnertech.com/uploads/140603/2-1406031I04M38.jpg)

[[JPG external
image]](http://www.allwinnertech.com/uploads/140603/2-1406031I04M38.jpg)

  
2014년 6월에 공개한 [CortexA7](ARM%20Cortex-A%20%EC%8B%9C%EB%A6%AC%EC%A6%88#s-1.1.3.md) 쿼드코어 프로세서.  
중보급형 기기를 겨냥한 프로세서로 공개되었다. A23과 핀이 호환되는 구조라(Pin to Pin), 기존의 A23 PCB에 바로 사용할 수
있다.  
하지만 염가판 시리즈 답게,1080p의 동영상과 1280*800까지의 해상도만 공식적으로 지원한다. 그리고 그래픽 프로세서가 Mali-400
MP2라서, 높은 성능을 기대하기에는 어려울 듯.  
하지만 28nm 공정으로, 전력 소비량 하나는 확실히 해결한 것 같다. 대기 중 AP 소모전력이 3mAh 라고 광고하니...

  

-A80  

![http://www.allwinnertech.com/uploads/140326/1-1403261Q925Q1.png](http://www.
allwinnertech.com/uploads/140326/1-1403261Q925Q1.png)

[[PNG external
image]](http://www.allwinnertech.com/uploads/140326/1-1403261Q925Q1.png)

  
2014년 4월에 공개된 옥타코어 프로세서.
[Cortex-A7](ARM%20Cortex-A%20%EC%8B%9C%EB%A6%AC%EC%A6%88#s-1.1.3.md)과
[Cortex-A15](ARM%20Cortex-A%20%EC%8B%9C%EB%A6%AC%EC%A6%88#s-1.1.6.md)의
[big.LITTLE](big.LITTLE.md) 방식으로 작동된다.  
Allwinner에서는 A80이 적용된 개발자용 보드로서 'Optimus Board' 를 공개하였다. Allwinner 관계자에 따르면,
아마 5월 말에 A80을 사용한 제품이 본격적으로 출시된다는 듯.  
RK3288과는 달리, 시대의 대세에 따라 옥타코어로 넘어갔다. 마케팅 측면에서는 쿼드코어 보다 옥타코어가 조금 더 유리할 듯.

`\----`

  * `[1]` 2012년 부터 Cortex-A9 기반의 듀얼코어 RK3066을 필두로 쭉 Cortex-A9 기반의 프로세서를 출시한 락칩과는 비교되는 부분. RK3066 세대의 락칩부터는 동영상 재생능력이 좋아져서, 올위너의 이점이 많이 퇴색되어진 경향이다.

