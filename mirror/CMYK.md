## Contents

    

1. 일반적인 뜻 
    

1.1. 개요

1.2. 이상적인 CMY 이론과 K의 존재

1.3. 기타

1.4. 창작물에서 CMY 혹은 RYB 이론을 차용한 것들

    

1.4.1. 클리셰

1.4.2. 예시

1.5. 관련 항목

2. 가수 

[[edit](http://rigvedawiki.net/r1/wiki.php/CMYK?action=edit&section=1)]

## 1. 일반적인 뜻 ¶

![CMYK.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/CMYK.jpg)

[JPG image (447.71 KB)]

  
Cyan, Magenta, Yellow, Key

[[edit](http://rigvedawiki.net/r1/wiki.php/CMYK?action=edit&section=2)]

### 1.1. 개요 ¶

색을 구현하는 체계 중 하나. 인쇄와 사진에서의 색 재현에 사용된다. 주로
[옵셋인쇄](%EC%98%B5%EC%85%8B%EC%9D%B8%EC%87%84.md)에 쓰이는 4가지 색을 이용한 잉크체계를 뜻하며,
각각 시안(**C**yan), 마젠타(**M**agenta), 옐로(**Y**ellow), 블랙(Black = **K**ey)`[1]`을
나타낸다. 그러나 현실적인 문제 때문에 [RGB](RGB.md)나 [HSB](HSB.md)(HSV)보다 표현 가능한 색이 적다.

  

학교에서 배운 감산혼합, 즉 색의 3원색에서는 분명히 빨강, 노랑, 파랑 즉 RYB로 배웠을텐데 왜 난데없이 중간색인 CMYK를 사용하냐면,
학교에서 배운 빨강과 파랑이 사실은 부정확한 표현이기 때문이다. 색의 3원색 중 빨강은 사실은 선홍색 즉
[마젠타](%EB%A7%88%EC%A0%A0%ED%83%80.md)이고, 파랑은 사실 짙은 하늘색 즉
[시안](%EC%8B%9C%EC%95%88.md)색이다. 마젠타와 시안이 우리애게 낯설다보니 그냥 빨강과 파랑으로 퉁친 것. 노랑은
노랑 맞다.`[2]` 또한 CMY만이 아니라 K까지 끼어든 것은, 아래 서술하겠지만 잉크의 성질이 이상적이지 않기 때문.

[[edit](http://rigvedawiki.net/r1/wiki.php/CMYK?action=edit&section=3)]

### 1.2. 이상적인 CMY 이론과 K의 존재 ¶

이론상으로는 CMY 만으로도 모든 색을 나타낼 수 있어야 한다. CMY는 감산혼합을 이용하는 방법으로,
[시안](%EC%8B%9C%EC%95%88.md)(**C**yan),
[마젠타](%EB%A7%88%EC%A0%A0%ED%83%80.md)(**M**agenta),
[노란색](%EB%85%B8%EB%9E%80%EC%83%89.md)(**Y**ellow)을 섞어서 명도와 채도를 낮아지게 한다.
이론적으로는 흰 색을 제외한 모든 색을 표현할 수 있다.

  

그러나, 현실은 그리 녹록지가 않다. 현실의 CMY는 잉크를 통해 구현되는데, 잉크의 성질이 이상적이지 않기 때문이다.

  

우선 잉크의 색 구현 원리를 보자. 잉크는 빛의 삼원색인 RGB(레드,그린,블루) 중에 '특정 색'을 흡수하고 나머지를 반사하는데, 그
반사된 색이 우리가 인식하는 색이 된다. 예를 들면, 이상적인 옐로 잉크의 경우에는 RGB중 블루는 모두 흡수되고, 그린과 레드는 100%
반사되어 우리 눈에는 옐로로 보이게 되는 것이다.

  

그러나 광점의 휘도만 적절히 조절하면 장땡인 RGB와는 달리 현실의 잉크는 이상적인 잉크에 비해 흡수율과 반사율이 떨어진다는 문제가 있다.
현실의 옐로우 잉크는 푸른빛을 다소 미흡하게 흡수하며, 그린과 레드 역시 다 반사를 못하고 약간 흡수하게 된다. 이는 종이와의 문제도
섞여있으며 상당히 복잡한 문제다. 아무튼 결론을 이야기하면, 잉크의 농도가 진해지면 진해질 수록 현실의 CMY잉크는 혼합의 효과가 떨어진다!
즉, 모든 색을 섞어 나오는 가장 진한 검정색을 얻을 수가 없다는 말이다. C 100 M 100 Y 100으로 섞어보면 화면에 출력되는 건
분명히 검은색인데 실제 인쇄물로 출력해 보면 검은색이 아니라 진한 갈색 비슷한 색이 나온다.`[3]` `[4]`

  

이 때문에 특별하게 제조된 검은색 잉크인 Key black을 첨가해서 검은 영역을 담당하게 하게 된 것이 현실의 CMYK잉크체계다.
한국에서는 K를 '먹'이라고 한다.

  

K의 존재로 인해 [3차원](3%EC%B0%A8%EC%9B%90.md) 구조인 다른 색 구성법`[5]`과는 달리 **유일하게
[4차원](4%EC%B0%A8%EC%9B%90.md) 구조를 띤다.**

[[edit](http://rigvedawiki.net/r1/wiki.php/CMYK?action=edit&section=4)]

### 1.3. 기타 ¶

인쇄를 하는 작업은 반드시 CMYK 체계를 거치게 되어 있다. 이상적인 CMY는 RGB로 작업한 작업물을 완전히 소화할 수 있지만,
불행하게도 현실의 CMYK는 RGB보다 색 표현능력이 떨어진다.

  

쉽게 말하면 포토샵 등에서 RGB로 작업하던 작업물을 인쇄하게 되면 필연적으로 CMYK로 변환이 될 수밖에 없는데, 그 과정에서 일부 색이
원치 않게 변화된다는 말이다. 밝은 색일수록, 색이 옅은 미묘한 색일 수록 변형될 가능성이 높아진다. 이러한 점을 주의해야 한다.  
이 때문에 출판용 그림은 **처음부터 CMYK로 작업**해야 한다. CMYK포맷으로 작업한 출판물은 화면에 보이는 것과 거의 차이 없이
인쇄가 된다. 문제는 CMYK로는 예쁜 색 발현이 굉장히 까다롭다는 것. 분명히 팔레트에선 이 색을 찍었는데 막상 칠해보면 훨씬 탁한 색이
나올 경우가 잦다. 이 때문에 일단 칠해놓고 채도/색상 변경을 통해 보정작업을 하는 경우가 대다수.

  

특히 채도 높은 화사한 그림의 경우 색에 K가 섞이면 실제 인쇄물이 검고 탁하게 나오기 때문에`[6]` 색을 고를 때 일일히 K를 0으로
맞춰줘야 할 때도 있다. 반대로 채도가 낮은 칙칙한 그림의 경우 종이가 잉크를 잘 못받는 경우 종이가 잉크에 절어서(!) 종이가 울거나
잉크가 번져버리는 경우가 생긴다. 간단하게 테스트해보려면 집의 컬러 잉크젯 프린터를 고품질 사진출력 모드+인화지 세팅으로 한 상태에서 저급
복사용지(평량 75g/m2짜리 이하. 그냥 얇은 복사지)를 넣어서 인쇄해보자. 푹 절어서 나올것이다. 인쇄소에서도 같은 일이 일어날 수
있다. 채도가 극단적이라고 생각되는 경우에는 인쇄소측에 상의해서 잉크를 바꾸는 것도 고려해야 한다.

  

물론 잉크가 CMYK만 나오는 건 아니다. 정말로 원하면 인쇄소에 별색 추가를 주문해서 그걸로 찍을 수도 있다. 예를 들어 밝은 오렌지 계열
색상을 원하는데 도저히 CMYK잉크로는 원하는 색이 안 나올 경우 오렌지색 잉크를 인쇄기에 추가해서 별색인쇄해버리면 된다. 정말로 원하는
경우 흰색 잉크로 색지에 인쇄할 수도 있다. 물론 인쇄기에 잉크를 무한히 추가할 수는 없으니까(보통 별색은 2개 정도가 한계다) 이렇게
작업할 생각이면 인쇄소의 담당자와 반드시 상의를 해야 한다.

  

반대로 CMYK로 작업된 것을 RGB로 변환하면 손실이 없다. 인쇄를 할 작업물은 미리 프로그램 상에서 CMYK로 작업하라는 이야기. 물론
주의할 점은 그렇게 해도 모니터의 색상과 인쇄물의 색상은 또 미세한 차이가 있다. 모니터는 결국 빛을 이용한 RGB체계고, 인쇄물은 잉크를
이용한 CMYK체계기 때문.

  

한편 이미지 파일에서 CMYK 모드는 RGB에 비해 용량이 대폭 커지며, [웹브라우저](%EC%9B%B9%20%EB%B8%8C%EB%9D%BC%EC%9A%B0%EC%A0%80.md)에서 인식을 못하는 경우도 왕왕
있으므로 인터넷상에 올릴 이미지는 모드를 반드시 확인할 것.

[[edit](http://rigvedawiki.net/r1/wiki.php/CMYK?action=edit&section=5)]

### 1.4. 창작물에서 CMY 혹은 RYB 이론을 차용한 것들 ¶

볼때 가장 안정적이고 일상에서 흔히 볼 수 있는 색상 배치라
[3인체제](3%EB%8C%80%20%EC%9A%94%EC%86%8C.md)의 캐릭터에게 이 색상을 적용하는 경우가 많다.  
팬들사이에서는 '[신호등](%EC%8B%A0%ED%98%B8%EB%93%B1.md)'이라 불릴 때가 잦다.

[[edit](http://rigvedawiki.net/r1/wiki.php/CMYK?action=edit&section=6)]

#### 1.4.1. 클리셰 ¶

  * 주로 소년 만화나 마법소녀물에서 많이 볼 수 있는 [클리셰](%ED%81%B4%EB%A6%AC%EC%85%B0.md).
  * 3인조로 구성된 경우에서 많이 볼 수 있다.  

    * [주인공](%EC%A3%BC%EC%9D%B8%EA%B3%B5.md)은 마젠타 계열인 경우가 많다. 그 다음으로 옐로우.
    * 마젠타 계열 캐릭터는 [천연](%EC%B2%9C%EC%97%B0.md)이나 [열혈](%EC%97%B4%ED%98%88.md)속성을 가지고 있다.
    * 시안 계열 캐릭터는 대개 [쿨데레](%EC%BF%A8%EB%8D%B0%EB%A0%88.md)나 [츤데레](%EC%B8%A4%EB%8D%B0%EB%A0%88.md) 속성.
    * 옐로우 계열 캐릭터는 [히로인](%ED%9E%88%EB%A1%9C%EC%9D%B8.md)이나 [막내](%EB%A7%89%EB%82%B4.md)로 묘사되는 일이 많다. `[7]`
  * 이런 클리셰의 경우, [속성](%EC%86%8D%EC%84%B1.md)은 시안이 [물](%EB%AC%BC.md)or[얼음](%EC%96%BC%EC%9D%8C.md) 속성, 마젠타가 [불](%EB%B6%88.md)속성, 옐로우가 [바람](%EB%B0%94%EB%9E%8C.md)or[전기](%EC%A0%84%EA%B8%B0.md)속성인 경우가 많다.  

    * 또는 육해공을 나타내기도 한다. 이런 경우는 시안이 [바다](%EB%B0%94%EB%8B%A4.md), 마젠타가 [하늘](%ED%95%98%EB%8A%98.md), 옐로우가 [대지](%EB%8C%80%EC%A7%80.md)를 상징.
  * 적 [간부](%EA%B0%84%EB%B6%80.md)도 이런 속성을 가지는 경우가 있다. 이 경우는, [같은 색끼리의 결투](%EB%B9%84%EC%8A%B7%ED%95%9C%20%ED%83%80%EC%9E%85%EB%81%BC%EB%A6%AC%20%EB%8C%80%EA%B2%B0.md)가 생긴다.
  * 4인조로 구성되는 경우는 여기에 검은색이 더해져서 **CMYK**가 된다.  

    * [검은색](%EA%B2%80%EC%9D%80%EC%83%89.md)인 경우도 있지만, 순화시켜 [보라색](%EB%B3%B4%EB%9D%BC%EC%83%89.md)으로 표현하는 경우도 있다.
  * 클리셰까지는 아니지만 특정 이미지 색상을 가진 캐릭터들이 나오는 [만](%ED%9E%88%EB%8B%A4%EB%A7%88%EB%A6%AC%20%EC%8A%A4%EC%BC%80%EC%B9%98.md)[화](GA%20%EC%98%88%EC%88%A0%EA%B3%BC%20%EC%95%84%ED%8A%B8%20%EB%94%94%EC%9E%90%EC%9D%B8%20%ED%81%B4%EB%9E%98%EC%8A%A4.md)[들](%EC%8A%A4%EC%BC%80%EC%B9%98%EB%B6%81%28%EB%A7%8C%ED%99%94%29.md)에서 관련 드립을 치는 경우가 많다. 역으로 [전대물](%EC%A0%84%EB%8C%80%EB%AC%BC.md)드립을 치는게 클리셰.  

[[edit](http://rigvedawiki.net/r1/wiki.php/CMYK?action=edit&section=7)]

#### 1.4.2. 예시 ¶

※ 시안(푸른색)/마젠타(붉은색)/옐로우(노란색) (4인조의 경우에는 블랙 (검은색/보라색)) 순서로 작성 바람.

  

  * [가면라이더 시리즈](%EA%B0%80%EB%A9%B4%EB%9D%BC%EC%9D%B4%EB%8D%94%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md)  

    * [가면라이더 아기토](%EA%B0%80%EB%A9%B4%EB%9D%BC%EC%9D%B4%EB%8D%94%20%EC%95%84%EA%B8%B0%ED%86%A0.md) \- [아기토의 폼](%EC%95%84%EA%B8%B0%ED%86%A0%28%EA%B0%80%EB%A9%B4%EB%9D%BC%EC%9D%B4%EB%8D%94%20%EC%95%84%EA%B8%B0%ED%86%A0%29/%ED%8F%BC.md) (스톰폼/플레임폼/그랜드폼)
    * [가면라이더 카부토](%EA%B0%80%EB%A9%B4%EB%9D%BC%EC%9D%B4%EB%8D%94%20%EC%B9%B4%EB%B6%80%ED%86%A0.md) \- [가탁크](%EA%B0%80%ED%83%81%ED%81%AC.md)/[카부토](%EC%B9%B4%EB%B6%80%ED%86%A0.md)/[자비](%EC%9E%90%EB%B9%84%28%EA%B0%80%EB%A9%B4%EB%9D%BC%EC%9D%B4%EB%8D%94%20%EC%B9%B4%EB%B6%80%ED%86%A0%29.md)
    * [가면라이더 덴오](%EA%B0%80%EB%A9%B4%EB%9D%BC%EC%9D%B4%EB%8D%94%20%EB%8D%B4%EC%98%A4.md)  

      * [우라타로스](%EC%9A%B0%EB%9D%BC%ED%83%80%EB%A1%9C%EC%8A%A4.md)/[모모타로스](%EB%AA%A8%EB%AA%A8%ED%83%80%EB%A1%9C%EC%8A%A4.md)/[킨타로스](%ED%82%A8%ED%83%80%EB%A1%9C%EC%8A%A4.md)
      * [덴오의 폼](%EB%8D%B4%EC%98%A4/%ED%8F%BC.md) (로드폼/소드폼/액스폼)
    * [가면 라이더 오즈](%EA%B0%80%EB%A9%B4%20%EB%9D%BC%EC%9D%B4%EB%8D%94%20%EC%98%A4%EC%A6%88.md)  

      * **[타토바 콤보](%ED%83%80%ED%86%A0%EB%B0%94%20%EC%BD%A4%EB%B3%B4.md)**
      * [메즐](%EB%A9%94%EC%A6%90.md)/[앙크](%EC%95%99%ED%81%AC%28%EA%B0%80%EB%A9%B4%EB%9D%BC%EC%9D%B4%EB%8D%94%20%EC%98%A4%EC%A6%88%29.md)/[카자리](%EC%B9%B4%EC%9E%90%EB%A6%AC%28%EA%B0%80%EB%A9%B4%EB%9D%BC%EC%9D%B4%EB%8D%94%20%EC%98%A4%EC%A6%88%29.md)
  * [가면라이더 위자드](%EA%B0%80%EB%A9%B4%EB%9D%BC%EC%9D%B4%EB%8D%94%20%EC%9C%84%EC%9E%90%EB%93%9C.md) \- 워터 스타일/플레임 스타일/랜드 스타일
  * [개구리 중사 케로로](%EA%B0%9C%EA%B5%AC%EB%A6%AC%20%EC%A4%91%EC%82%AC%20%EC%BC%80%EB%A1%9C%EB%A1%9C.md) \- [니시자와 모모카](%EB%8B%88%EC%8B%9C%EC%9E%90%EC%99%80%20%EB%AA%A8%EB%AA%A8%EC%B9%B4.md)/[히나타 나츠미](%ED%9E%88%EB%82%98%ED%83%80%20%EB%82%98%EC%B8%A0%EB%AF%B8.md)/[앙골 모아](%EC%95%99%EA%B3%A8%20%EB%AA%A8%EC%95%84.md)/[아즈마야 코유키](%EC%95%84%EC%A6%88%EB%A7%88%EC%95%BC%20%EC%BD%94%EC%9C%A0%ED%82%A4.md)
  * [개그콘서트](%EA%B0%9C%EA%B7%B8%EC%BD%98%EC%84%9C%ED%8A%B8.md)   

    * [감사합니다](%EA%B0%90%EC%82%AC%ED%95%A9%EB%8B%88%EB%8B%A4.md) \- [이상훈](%EC%9D%B4%EC%83%81%ED%9B%88.md)/[송병철](%EC%86%A1%EB%B3%91%EC%B2%A0.md)/[정태호](%EC%A0%95%ED%83%9C%ED%98%B8.md)
    * [도찐개찐](%EB%8F%84%EC%B0%90%EA%B0%9C%EC%B0%90%28%EA%B0%9C%EA%B7%B8%20%EC%BD%98%EC%84%9C%ED%8A%B8%29.md) \- 이종훈/[박성호](%EB%B0%95%EC%84%B1%ED%98%B8.md)/곽범
    * [나는 킬러다](%EB%82%98%EB%8A%94%20%ED%82%AC%EB%9F%AC%EB%8B%A4.md) \- 빨노파(신윤승/곽범/남궁경호)
  * [괭이갈매기 울 적에](%EA%B4%AD%EC%9D%B4%EA%B0%88%EB%A7%A4%EA%B8%B0%20%EC%9A%B8%20%EC%A0%81%EC%97%90.md) \- [시에스타 자매 근위병](%EC%8B%9C%EC%97%90%EC%8A%A4%ED%83%80%20%EC%9E%90%EB%A7%A4%20%EA%B7%BC%EC%9C%84%EB%B3%91.md)(시에스타 410/시에스타 45/시에스타 00/시에스타 556)
  * [기동전함 나데시코](%EA%B8%B0%EB%8F%99%EC%A0%84%ED%95%A8%20%EB%82%98%EB%8D%B0%EC%8B%9C%EC%BD%94.md) \- [마키 이즈미](%EB%A7%88%ED%82%A4%20%EC%9D%B4%EC%A6%88%EB%AF%B8.md)/[스바루 료코](%EC%8A%A4%EB%B0%94%EB%A3%A8%20%EB%A3%8C%EC%BD%94.md)/[아마노 히카루](%EC%95%84%EB%A7%88%EB%85%B8%20%ED%9E%88%EC%B9%B4%EB%A3%A8.md)
  * [네모바지 스폰지밥](%EB%84%A4%EB%AA%A8%EB%B0%94%EC%A7%80%20%EC%8A%A4%ED%8F%B0%EC%A7%80%EB%B0%A5.md) \- [징징이](%EC%A7%95%EC%A7%95%EC%9D%B4.md)/[뚱이](%EB%9A%B1%EC%9D%B4.md)/[스폰지밥](%EB%84%A4%EB%AA%A8%EB%B0%94%EC%A7%80%20%EC%8A%A4%ED%8F%B0%EC%A7%80%EB%B0%A5%28%EB%84%A4%EB%AA%A8%EB%B0%94%EC%A7%80%20%EC%8A%A4%ED%8F%B0%EC%A7%80%EB%B0%A5%29.md)
  * [데이트 어 라이브](%EB%8D%B0%EC%9D%B4%ED%8A%B8%20%EC%96%B4%20%EB%9D%BC%EC%9D%B4%EB%B8%8C.md)  

    * [타카미야 마나](%ED%83%80%EC%B9%B4%EB%AF%B8%EC%95%BC%20%EB%A7%88%EB%82%98.md)/제시카 베일리/[엘렌 밀라 메이저스](%EC%97%98%EB%A0%8C%20%EB%B0%80%EB%9D%BC%20%EB%A9%94%EC%9D%B4%EC%A0%80%EC%8A%A4.md) (DEM사 TOP3 위저드)
    * 후지바카마 미이/하사쿠라 마이/야마부키 아이 (아이,마이,미이 트리오)
  * [듀라라라!!](%EB%93%80%EB%9D%BC%EB%9D%BC%EB%9D%BC%21%21.md) \- [류가미네 미카도](%EB%A5%98%EA%B0%80%EB%AF%B8%EB%84%A4%20%EB%AF%B8%EC%B9%B4%EB%8F%84.md)/[소노하라 앙리](%EC%86%8C%EB%85%B8%ED%95%98%EB%9D%BC%20%EC%95%99%EB%A6%AC.md)/[키다 마사오미](%ED%82%A4%EB%8B%A4%20%EB%A7%88%EC%82%AC%EC%98%A4%EB%AF%B8.md)
  * [디지몬 시리즈](%EB%94%94%EC%A7%80%EB%AA%AC%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md)  

    * [디지몬 세이버즈](%EB%94%94%EC%A7%80%EB%AA%AC%20%EC%84%B8%EC%9D%B4%EB%B2%84%EC%A6%88.md)  

      * [토마](%ED%86%A0%EB%A7%88%20H.%20%EB%86%80%EC%8A%88%ED%83%80%EC%9D%B8.md)/[유진](%EC%9C%A0%EC%A7%84%28%EB%94%94%EC%A7%80%EB%AA%AC%20%EC%84%B8%EC%9D%B4%EB%B2%84%EC%A6%88%29.md)/[최건우](%EC%B5%9C%EA%B1%B4%EC%9A%B0.md)
      * [가오몬](%EA%B0%80%EC%98%A4%EB%AA%AC.md)/[라라몬](%EB%9D%BC%EB%9D%BC%EB%AA%AC.md)/[아구몬](%EC%95%84%EA%B5%AC%EB%AA%AC.md)
    * [디지몬 크로스워즈](%EB%94%94%EC%A7%80%EB%AA%AC%20%ED%81%AC%EB%A1%9C%EC%8A%A4%EC%9B%8C%EC%A6%88.md)  

      * [바리스타몬](%EB%B0%94%EB%A6%AC%EC%8A%A4%ED%83%80%EB%AA%AC.md)/[샤우트몬](%EC%83%A4%EC%9A%B0%ED%8A%B8%EB%AA%AC.md)/[도루루몬](%EB%8F%84%EB%A3%A8%EB%A3%A8%EB%AA%AC.md)
      * [검드라몬](%EA%B2%80%EB%93%9C%EB%9D%BC%EB%AA%AC.md)/[샤우트몬](%EC%83%A4%EC%9A%B0%ED%8A%B8%EB%AA%AC.md)/[다메몬](%EB%8B%A4%EB%A9%94%EB%AA%AC.md)
  * [리그 오브 레전드](%EB%A6%AC%EA%B7%B8%20%EC%98%A4%EB%B8%8C%20%EB%A0%88%EC%A0%84%EB%93%9C.md)  

    * [케이틀린](%EC%BC%80%EC%9D%B4%ED%8B%80%EB%A6%B0%28%EB%A6%AC%EA%B7%B8%20%EC%98%A4%EB%B8%8C%20%EB%A0%88%EC%A0%84%EB%93%9C%29.md)/[바이](%EB%B0%94%EC%9D%B4%28%EB%A6%AC%EA%B7%B8%20%EC%98%A4%EB%B8%8C%20%EB%A0%88%EC%A0%84%EB%93%9C%29.md)/[이즈리얼](%EC%9D%B4%EC%A6%88%EB%A6%AC%EC%96%BC.md)
    * [트위스티드 페이트](%ED%8A%B8%EC%9C%84%EC%8A%A4%ED%8B%B0%EB%93%9C%20%ED%8E%98%EC%9D%B4%ED%8A%B8.md)의 카드뽑기(블루카드/레드카드/골드카드)
  * [마기](%EB%A7%88%EA%B8%B0%28%EB%A7%8C%ED%99%94%29.md) \- [알라딘](%EC%95%8C%EB%9D%BC%EB%94%98%28%EB%A7%88%EA%B8%B0%29.md)/[모르지아나](%EB%AA%A8%EB%A5%B4%EC%A7%80%EC%95%84%EB%82%98%28%EB%A7%88%EA%B8%B0%29.md)/[알리바바 사르쟈](%EC%95%8C%EB%A6%AC%EB%B0%94%EB%B0%94%20%EC%82%AC%EB%A5%B4%EC%9F%88.md)
  * [마법소녀 마도카☆마기카](%EB%A7%88%EB%B2%95%EC%86%8C%EB%85%80%20%EB%A7%88%EB%8F%84%EC%B9%B4%E2%98%86%EB%A7%88%EA%B8%B0%EC%B9%B4.md)  

    * [미키 사야카](%EB%AF%B8%ED%82%A4%20%EC%82%AC%EC%95%BC%EC%B9%B4.md)/[카나메 마도카](%EC%B9%B4%EB%82%98%EB%A9%94%20%EB%A7%88%EB%8F%84%EC%B9%B4.md)/[토모에 마미](%ED%86%A0%EB%AA%A8%EC%97%90%20%EB%A7%88%EB%AF%B8.md)
    * [미키 사야카](%EB%AF%B8%ED%82%A4%20%EC%82%AC%EC%95%BC%EC%B9%B4.md)/[사쿠라 쿄코](%EC%82%AC%EC%BF%A0%EB%9D%BC%20%EC%BF%84%EC%BD%94.md)/[토모에 마미](%ED%86%A0%EB%AA%A8%EC%97%90%20%EB%A7%88%EB%AF%B8.md) (**[신호등](%EC%8B%A0%ED%98%B8%EB%93%B1#S-3.md)**(3번 항목))
  * [무적코털 보보보](%EB%AC%B4%EC%A0%81%EC%BD%94%ED%84%B8%20%EB%B3%B4%EB%B3%B4%EB%B3%B4.md) \- [젤라티노](%EC%A0%A4%EB%9D%BC%ED%8B%B0%EB%85%B8.md)/[돈벼락](%EB%8F%88%EB%B2%BC%EB%9D%BD%28%EB%AC%B4%EC%A0%81%EC%BD%94%ED%84%B8%20%EB%B3%B4%EB%B3%B4%EB%B3%B4%29.md)/[보보보보 보보보](%EB%B3%B4%EB%B3%B4%EB%B3%B4%EB%B3%B4%20%EB%B3%B4%EB%B3%B4%EB%B3%B4.md)
  * [미소녀 전사 세일러 문 시리즈](%EB%AF%B8%EC%86%8C%EB%85%80%20%EC%A0%84%EC%82%AC%20%EC%84%B8%EC%9D%BC%EB%9F%AC%20%EB%AC%B8%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md) \- [미즈노 아미](%EB%AF%B8%EC%A6%88%EB%85%B8%20%EC%95%84%EB%AF%B8.md)(세일러 머큐리)/[히노 레이](%ED%9E%88%EB%85%B8%20%EB%A0%88%EC%9D%B4.md)(세일러 마스)/[아이노 미나코](%EC%95%84%EC%9D%B4%EB%85%B8%20%EB%AF%B8%EB%82%98%EC%BD%94.md)(세일러 비너스)
  * [변신 자동차 또봇](%EB%B3%80%EC%8B%A0%20%EC%9E%90%EB%8F%99%EC%B0%A8%20%EB%98%90%EB%B4%87.md) \- [또봇 Y](%EB%98%90%EB%B4%87%20Y.md)/[또봇 Z](%EB%98%90%EB%B4%87%20Z.md)/[또봇 X](%EB%98%90%EB%B4%87%20X.md)
  * [세인트 세이야](%EC%84%B8%EC%9D%B8%ED%8A%B8%20%EC%84%B8%EC%9D%B4%EC%95%BC.md) \- 마린크로스/스카이크로스/랜드크로스 ([스틸 세인트](%EC%8A%A4%ED%8B%B8%20%EC%84%B8%EC%9D%B8%ED%8A%B8.md))
  * [소닉 더 헤지혹 시리즈](%EC%86%8C%EB%8B%89%20%EB%8D%94%20%ED%97%A4%EC%A7%80%ED%98%B9%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md) \- [소닉 더 헤지혹](%EC%86%8C%EB%8B%89%20%EB%8D%94%20%ED%97%A4%EC%A7%80%ED%98%B9.md)/[너클즈 더 에키드나](%EB%84%88%ED%81%B4%EC%A6%88%20%EB%8D%94%20%EC%97%90%ED%82%A4%EB%93%9C%EB%82%98.md)/[마일즈 테일즈 파우아](%EB%A7%88%EC%9D%BC%EC%A6%88%20%ED%85%8C%EC%9D%BC%EC%A6%88%20%ED%8C%8C%EC%9A%B0%EC%95%84.md)
  * [슈퍼 마리오 시리즈](%EC%8A%88%ED%8D%BC%20%EB%A7%88%EB%A6%AC%EC%98%A4%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md) \- [루이지](%EB%A3%A8%EC%9D%B4%EC%A7%80.md)/[마리오](%EB%A7%88%EB%A6%AC%EC%98%A4%28%EB%8B%8C%ED%85%90%EB%8F%84%29.md)/[와리오](%EC%99%80%EB%A6%AC%EC%98%A4.md)/[와루이지](%EC%99%80%EB%A3%A8%EC%9D%B4%EC%A7%80.md)  

    * [페이퍼 마리오 천년의 문](%ED%8E%98%EC%9D%B4%ED%8D%BC%20%EB%A7%88%EB%A6%AC%EC%98%A4%20%EC%B2%9C%EB%85%84%EC%9D%98%20%EB%AC%B8.md) \- 마조린/비비안/마릴린 (그림자 3인조)
    * [뉴 슈퍼 마리오 브라더스 Wii](%EB%89%B4%20%EC%8A%88%ED%8D%BC%20%EB%A7%88%EB%A6%AC%EC%98%A4%20%EB%B8%8C%EB%9D%BC%EB%8D%94%EC%8A%A4%20Wii.md) \- [루이지](%EB%A3%A8%EC%9D%B4%EC%A7%80.md)`[8]`/[마리오](%EB%A7%88%EB%A6%AC%EC%98%A4%28%EB%8B%8C%ED%85%90%EB%8F%84%29.md)/노랑 [키노피오](%ED%82%A4%EB%85%B8%ED%94%BC%EC%98%A4.md)
  * **[슈퍼전대 시리즈](%EC%8A%88%ED%8D%BC%EC%A0%84%EB%8C%80%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md)**`[9]`  

    * **[태양전대 선발칸](%ED%83%9C%EC%96%91%EC%A0%84%EB%8C%80%20%EC%84%A0%EB%B0%9C%EC%B9%B8.md)** \- [사메지마 킨야](%EC%82%AC%EB%A9%94%EC%A7%80%EB%A7%88%20%ED%82%A8%EC%95%BC.md)(발 샤크)/[오오와시 류스케](%EC%98%A4%EC%98%A4%EC%99%80%EC%8B%9C%20%EB%A5%98%EC%8A%A4%EC%BC%80.md)(발 이글)/[효 아사오](%ED%9A%A8%20%EC%95%84%EC%82%AC%EC%98%A4.md)(발 팬서)
    * [초수전대 라이브맨](%EC%B4%88%EC%88%98%EC%A0%84%EB%8C%80%20%EB%9D%BC%EC%9D%B4%EB%B8%8C%EB%A7%A8.md) \- [미사키 메구미](%EB%AF%B8%EC%82%AC%ED%82%A4%20%EB%A9%94%EA%B5%AC%EB%AF%B8.md)(블루 돌핀)/[아마미야 유스케](%EC%95%84%EB%A7%88%EB%AF%B8%EC%95%BC%20%EC%9C%A0%EC%8A%A4%EC%BC%80.md)(레드 팔콘)/[오오하라 죠](%EC%98%A4%EC%98%A4%ED%95%98%EB%9D%BC%20%EC%A3%A0.md)(옐로 라이온)
    * [인풍전대 허리케인저](%EC%9D%B8%ED%92%8D%EC%A0%84%EB%8C%80%20%ED%97%88%EB%A6%AC%EC%BC%80%EC%9D%B8%EC%A0%80.md) \- [노노 나나미](%EB%85%B8%EB%85%B8%20%EB%82%98%EB%82%98%EB%AF%B8.md)(허리켄 블루)/[시나 요스케](%EC%8B%9C%EB%82%98%20%EC%9A%94%EC%8A%A4%EC%BC%80.md)(허리켄 레드)/[비토 코타](%EB%B9%84%ED%86%A0%20%EC%BD%94%ED%83%80.md)(허리켄 옐로)
    * [폭룡전대 아바레인저](%ED%8F%AD%EB%A3%A1%EC%A0%84%EB%8C%80%20%EC%95%84%EB%B0%94%EB%A0%88%EC%9D%B8%EC%A0%80.md)  

      * [산죠 유키토](%EC%82%B0%EC%A3%A0%20%EC%9C%A0%ED%82%A4%ED%86%A0.md)(아바레 블루)/[하쿠아 료우가](%ED%95%98%EC%BF%A0%EC%95%84%20%EB%A3%8C%EC%9A%B0%EA%B0%80.md)(아바 레드)/[이츠키 란루](%EC%9D%B4%EC%B8%A0%ED%82%A4%20%EB%9E%80%EB%A3%A8.md)(아바레 옐로)
      * [폭룡 트리케라톱스](%ED%8F%AD%EB%A3%A1%20%ED%8A%B8%EB%A6%AC%EC%BC%80%EB%9D%BC%ED%86%B1%EC%8A%A4.md)/[폭룡 티라노사우루스](%ED%8F%AD%EB%A3%A1%20%ED%8B%B0%EB%9D%BC%EB%85%B8%EC%82%AC%EC%9A%B0%EB%A3%A8%EC%8A%A4.md)/[폭룡 프테라노돈](%ED%8F%AD%EB%A3%A1%20%ED%94%84%ED%85%8C%EB%9D%BC%EB%85%B8%EB%8F%88.md)
    * [수권전대 게키레인저](%EC%88%98%EA%B6%8C%EC%A0%84%EB%8C%80%20%EA%B2%8C%ED%82%A4%EB%A0%88%EC%9D%B8%EC%A0%80.md) \- [후카미 레츠](%ED%9B%84%EC%B9%B4%EB%AF%B8%20%EB%A0%88%EC%B8%A0.md)(게키 블루)/[칸도 쟝](%EC%B9%B8%EB%8F%84%20%EC%9F%9D.md)(게키 레드)/[우자키 란](%EC%9A%B0%EC%9E%90%ED%82%A4%20%EB%9E%80.md)(게키 옐로)
    * [염신전대 고온저](%EC%97%BC%EC%8B%A0%EC%A0%84%EB%8C%80%20%EA%B3%A0%EC%98%A8%EC%A0%80.md)  

      * [코사카 렌](%EC%BD%94%EC%82%AC%EC%B9%B4%20%EB%A0%8C.md)(고온 블루)/[에스미 소스케](%EC%97%90%EC%8A%A4%EB%AF%B8%20%EC%86%8C%EC%8A%A4%EC%BC%80.md)(고온 레드)/[로야마 사키](%EB%A1%9C%EC%95%BC%EB%A7%88%20%EC%82%AC%ED%82%A4.md)(고온 옐로)
      * [염신 버스온](%EC%97%BC%EC%8B%A0%20%EB%B2%84%EC%8A%A4%EC%98%A8.md)/[염신 스피돌](%EC%97%BC%EC%8B%A0%20%EC%8A%A4%ED%94%BC%EB%8F%8C.md)/[염신 베아르V](%EC%97%BC%EC%8B%A0%20%EB%B2%A0%EC%95%84%EB%A5%B4V.md)
    * [특명전대 고버스터즈](%ED%8A%B9%EB%AA%85%EC%A0%84%EB%8C%80%20%EA%B3%A0%EB%B2%84%EC%8A%A4%ED%84%B0%EC%A6%88.md)  

      * [이와사키 류우지](%EC%9D%B4%EC%99%80%EC%82%AC%ED%82%A4%20%EB%A5%98%EC%9A%B0%EC%A7%80.md)(블루 버스터)/[사쿠라다 히로무](%EC%82%AC%EC%BF%A0%EB%9D%BC%EB%8B%A4%20%ED%9E%88%EB%A1%9C%EB%AC%B4.md)(레드 버스터)/[우사미 요코](%EC%9A%B0%EC%82%AC%EB%AF%B8%20%EC%9A%94%EC%BD%94.md)(옐로 버스터)
      * [고리사키 바나나](%EA%B3%A0%EB%A6%AC%EC%82%AC%ED%82%A4%20%EB%B0%94%EB%82%98%EB%82%98.md)/[치다 닉](%EC%B9%98%EB%8B%A4%20%EB%8B%89.md)/[우사다 레터스](%EC%9A%B0%EC%82%AC%EB%8B%A4%20%EB%A0%88%ED%84%B0%EC%8A%A4.md)
  * [아이돌 마스터 사이드 M](%EC%95%84%EC%9D%B4%EB%8F%8C%20%EB%A7%88%EC%8A%A4%ED%84%B0%20%EC%82%AC%EC%9D%B4%EB%93%9C%20M.md)의 타입 - 인텔리/피지컬/멘탈  

    * [JUPITER](jupiter%28%EC%95%84%EC%9D%B4%EB%8F%8C%20%EB%A7%88%EC%8A%A4%ED%84%B0%29.md) \- [이쥬인 호쿠토](%EC%9D%B4%EC%A5%AC%EC%9D%B8%20%ED%98%B8%EC%BF%A0%ED%86%A0.md)/[아마가세 토우마](%EC%95%84%EB%A7%88%EA%B0%80%EC%84%B8%20%ED%86%A0%EC%9A%B0%EB%A7%88.md)/[미타라이 쇼타](%EB%AF%B8%ED%83%80%EB%9D%BC%EC%9D%B4%20%EC%87%BC%ED%83%80.md)
    * [DRAMATIC STARS](DRAMATIC%20STARS.md) \- [사쿠라바 카오루](%EC%82%AC%EC%BF%A0%EB%9D%BC%EB%B0%94%20%EC%B9%B4%EC%98%A4%EB%A3%A8.md)/[텐도 테루](%ED%85%90%EB%8F%84%20%ED%85%8C%EB%A3%A8.md)/[카시와기 츠바사](%EC%B9%B4%EC%8B%9C%EC%99%80%EA%B8%B0%20%EC%B8%A0%EB%B0%94%EC%82%AC.md)
    * [FRAME](FRAME%28%EC%95%84%EC%9D%B4%EB%8F%8C%20%EB%A7%88%EC%8A%A4%ED%84%B0%20%EC%82%AC%EC%9D%B4%EB%93%9C%20M%29.md) \- [아쿠노 히데오](%EC%95%84%EC%BF%A0%EB%85%B8%20%ED%9E%88%EB%8D%B0%EC%98%A4.md)/[키무라 류](%ED%82%A4%EB%AC%B4%EB%9D%BC%20%EB%A5%98.md)/[신겐 세이지](%EC%8B%A0%EA%B2%90%20%EC%84%B8%EC%9D%B4%EC%A7%80.md)
    * [Beit](Beit.md) \- [타카죠 쿄지](%ED%83%80%EC%B9%B4%EC%A3%A0%20%EC%BF%84%EC%A7%80.md)/[와타나베 미노리](%EC%99%80%ED%83%80%EB%82%98%EB%B2%A0%20%EB%AF%B8%EB%85%B8%EB%A6%AC.md)/[피에르](%ED%94%BC%EC%97%90%EB%A5%B4%28%EC%95%84%EC%9D%B4%EB%8F%8C%20%EB%A7%88%EC%8A%A4%ED%84%B0%20%EC%82%AC%EC%9D%B4%EB%93%9C%20M%29.md)
    * [もふもふえん](%E3%82%82%E3%81%B5%E3%82%82%E3%81%B5%E3%81%88%E3%82%93.md) \- [오카무라 나오](%EC%98%A4%EC%B9%B4%EB%AC%B4%EB%9D%BC%20%EB%82%98%EC%98%A4.md)/[타치바나 시로](%ED%83%80%EC%B9%98%EB%B0%94%EB%82%98%20%EC%8B%9C%EB%A1%9C.md)/[히메노 카논](%ED%9E%88%EB%A9%94%EB%85%B8%20%EC%B9%B4%EB%85%BC.md)
  * [아이돌 마스터 신데렐라 걸즈](%EC%95%84%EC%9D%B4%EB%8F%8C%20%EB%A7%88%EC%8A%A4%ED%84%B0%20%EC%8B%A0%EB%8D%B0%EB%A0%90%EB%9D%BC%20%EA%B1%B8%EC%A6%88.md)의 타입 - 쿨/큐트/패션
  * [아이카츠](%EC%95%84%EC%9D%B4%EC%B9%B4%EC%B8%A0.md)   

    * [키리야 아오이](%ED%82%A4%EB%A6%AC%EC%95%BC%20%EC%95%84%EC%98%A4%EC%9D%B4.md)/[호시미야 이치고](%ED%98%B8%EC%8B%9C%EB%AF%B8%EC%95%BC%20%EC%9D%B4%EC%B9%98%EA%B3%A0.md)/[아리스가와 오토메](%EC%95%84%EB%A6%AC%EC%8A%A4%EA%B0%80%EC%99%80%20%EC%98%A4%ED%86%A0%EB%A9%94.md)/[시부키 란](%EC%8B%9C%EB%B6%80%ED%82%A4%20%EB%9E%80.md)
    * [히카미 스미레](%ED%9E%88%EC%B9%B4%EB%AF%B8%20%EC%8A%A4%EB%AF%B8%EB%A0%88.md)/[오오조라 아카리](%EC%98%A4%EC%98%A4%EC%A1%B0%EB%9D%BC%20%EC%95%84%EC%B9%B4%EB%A6%AC.md)`[10]`/[신죠 히나키](%EC%8B%A0%EC%A3%A0%20%ED%9E%88%EB%82%98%ED%82%A4.md)/[후지와라 미야비](%ED%9B%84%EC%A7%80%EC%99%80%EB%9D%BC%20%EB%AF%B8%EC%95%BC%EB%B9%84.md)
  * [아지랑이 프로젝트](%EC%95%84%EC%A7%80%EB%9E%91%EC%9D%B4%20%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8.md) \- [아마미야 히비야](%EC%95%84%EB%A7%88%EB%AF%B8%EC%95%BC%20%ED%9E%88%EB%B9%84%EC%95%BC.md)/[아사히나 히요리](%EC%95%84%EC%82%AC%ED%9E%88%EB%82%98%20%ED%9E%88%EC%9A%94%EB%A6%AC.md)/[코노하](%EC%BD%94%EB%85%B8%ED%95%98%28%EC%95%84%EC%A7%80%EB%9E%91%EC%9D%B4%20%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8%29.md)
  * [애천사전설 웨딩피치](%EC%95%A0%EC%B2%9C%EC%82%AC%EC%A0%84%EC%84%A4%20%EC%9B%A8%EB%94%A9%ED%94%BC%EC%B9%98.md) \- [타니마 유리](%ED%83%80%EB%8B%88%EB%A7%88%20%EC%9C%A0%EB%A6%AC.md)/[하나사키 모모코](%ED%95%98%EB%82%98%EC%82%AC%ED%82%A4%20%EB%AA%A8%EB%AA%A8%EC%BD%94.md)/[타마노 히나기쿠](%ED%83%80%EB%A7%88%EB%85%B8%20%ED%9E%88%EB%82%98%EA%B8%B0%EC%BF%A0.md)/[스칼렛 오하라](%EC%8A%A4%EC%B9%BC%EB%A0%9B%20%EC%98%A4%ED%95%98%EB%9D%BC%28%EC%95%A0%EC%B2%9C%EC%82%AC%EC%A0%84%EC%84%A4%20%EC%9B%A8%EB%94%A9%ED%94%BC%EC%B9%98%29.md)
  * [앵그리버드 시리즈](%EC%95%B5%EA%B7%B8%EB%A6%AC%EB%B2%84%EB%93%9C%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md) \- 블루 버드/레드 버드/옐로우 버드
  * [엘소드](%EC%97%98%EC%86%8C%EB%93%9C.md) \- [청](%EC%B2%AD%28%EC%97%98%EC%86%8C%EB%93%9C%29.md)/[이브](%EC%9D%B4%EB%B8%8C%28%EC%97%98%EC%86%8C%EB%93%9C%29.md)/[아라](%EC%95%84%EB%9D%BC%20%ED%95%9C.md)
  * [역전재판 시리즈](%EC%97%AD%EC%A0%84%EC%9E%AC%ED%8C%90%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md) \- [나루호도 류이치](%EB%82%98%EB%A3%A8%ED%98%B8%EB%8F%84%20%EB%A5%98%EC%9D%B4%EC%B9%98.md)/[미츠루기 레이지](%EB%AF%B8%EC%B8%A0%EB%A3%A8%EA%B8%B0%20%EB%A0%88%EC%9D%B4%EC%A7%80.md)/[야하리 마사시](%EC%95%BC%ED%95%98%EB%A6%AC%20%EB%A7%88%EC%82%AC%EC%8B%9C.md)  

    * [역전재판 4](%EC%97%AD%EC%A0%84%EC%9E%AC%ED%8C%90%204.md) \- [아루마지키 유우미](%EB%9D%BC%EB%AF%B8%EB%A1%9C%EC%95%84.md)/[아루마지키 잭](%EC%95%84%EB%A3%A8%EB%A7%88%EC%A7%80%ED%82%A4%20%EC%9E%AD.md)/[아루마지키 바란](%EC%95%84%EB%A3%A8%EB%A7%88%EC%A7%80%ED%82%A4%20%EB%B0%94%EB%9E%80.md)
    * [역전재판 5](%EC%97%AD%EC%A0%84%EC%9E%AC%ED%8C%90%205.md) \- [나루호도 류이치](%EB%82%98%EB%A3%A8%ED%98%B8%EB%8F%84%20%EB%A5%98%EC%9D%B4%EC%B9%98.md)/[오도로키 호우스케](%EC%98%A4%EB%8F%84%EB%A1%9C%ED%82%A4%20%ED%98%B8%EC%9A%B0%EC%8A%A4%EC%BC%80.md)/[키즈키 코코네](%ED%82%A4%EC%A6%88%ED%82%A4%20%EC%BD%94%EC%BD%94%EB%84%A4.md)
  * [원피스](%EC%9B%90%ED%94%BC%EC%8A%A4%28%EB%A7%8C%ED%99%94%29.md)  

    * <del>[몽키 D. 루피](%EB%AA%BD%ED%82%A4%20D.%20%EB%A3%A8%ED%94%BC.md)의 옷차림(청바지/붉은 조끼/노란 밀짚모자)</del>
    * [상디](%EC%83%81%EB%94%94.md)/[몽키 D. 루피](%EB%AA%BD%ED%82%A4%20D.%20%EB%A3%A8%ED%94%BC.md)/[우솝](%EC%9A%B0%EC%86%9D.md)(위스키피크 편 한정 바보 삼형제)
    * **[아오키지](%EC%95%84%EC%98%A4%ED%82%A4%EC%A7%80.md)/[아카이누](%EC%95%84%EC%B9%B4%EC%9D%B4%EB%88%84.md)/[키자루](%ED%82%A4%EC%9E%90%EB%A3%A8.md)**([해군 대장](%ED%95%B4%EA%B5%B0%20%EB%8C%80%EC%9E%A5.md), **[삼대장](%EC%82%BC%EB%8C%80%EC%9E%A5.md)**`[11]`)
    * [Dr. 인디고](Dr.%20%EC%9D%B8%EB%94%94%EA%B3%A0.md)/[스칼렛 대장](%EC%8A%A4%EC%B9%BC%EB%A0%9B%20%EB%8C%80%EC%9E%A5.md)/[금사자 시키](%EA%B8%88%EC%82%AC%EC%9E%90%20%EC%8B%9C%ED%82%A4.md)(원피스 극장판 [스트롱 월드](%EC%8A%A4%ED%8A%B8%EB%A1%B1%20%EC%9B%94%EB%93%9C.md)의 메인 악역들)`[12]`
  * [유희왕](%EC%9C%A0%ED%9D%AC%EC%99%95.md) \- [오벨리스크의 거신병](%EC%98%A4%EB%B2%A8%EB%A6%AC%EC%8A%A4%ED%81%AC%EC%9D%98%20%EA%B1%B0%EC%8B%A0%EB%B3%91.md)/[오시리스의 천공룡](%EC%98%A4%EC%8B%9C%EB%A6%AC%EC%8A%A4%EC%9D%98%20%EC%B2%9C%EA%B3%B5%EB%A3%A1.md)/[라의 익신룡](%EB%9D%BC%EC%9D%98%20%EC%9D%B5%EC%8B%A0%EB%A3%A1.md)([삼환신](%EC%82%BC%ED%99%98%EC%8B%A0.md))  

    * [유희왕 GX](%EC%9C%A0%ED%9D%AC%EC%99%95%20GX.md) \- [오벨리스크 블루](%EC%98%A4%EB%B2%A8%EB%A6%AC%EC%8A%A4%ED%81%AC%20%EB%B8%94%EB%A3%A8.md)/[오시리스 레드](%EC%98%A4%EC%8B%9C%EB%A6%AC%EC%8A%A4%20%EB%A0%88%EB%93%9C.md)/[라 옐로](%EB%9D%BC%20%EC%98%90%EB%A1%9C.md)([듀얼 아카데미아](%EB%93%80%EC%96%BC%20%EC%95%84%EC%B9%B4%EB%8D%B0%EB%AF%B8%EC%95%84.md)의 클래스)
    * [유희왕 ZEXAL](%EC%9C%A0%ED%9D%AC%EC%99%95%20ZEXAL.md) \- [V](V.md)/[III](III.md)/[IV](IV.md)([트론](%ED%8A%B8%EB%A1%A0.md))
  * [이나즈마 일레븐](%EC%9D%B4%EB%82%98%EC%A6%88%EB%A7%88%20%EC%9D%BC%EB%A0%88%EB%B8%90.md) \- [스즈노 후스케](%EC%8A%A4%EC%A6%88%EB%85%B8%20%ED%9B%84%EC%8A%A4%EC%BC%80.md)/[나구모 하루야](%EB%82%98%EA%B5%AC%EB%AA%A8%20%ED%95%98%EB%A3%A8%EC%95%BC.md)/[아후로 테루미](%EC%95%84%ED%9B%84%EB%A1%9C%20%ED%85%8C%EB%A3%A8%EB%AF%B8.md)  

    * [이나즈마 일레븐 GO 갤럭시](%EC%9D%B4%EB%82%98%EC%A6%88%EB%A7%88%20%EC%9D%BC%EB%A0%88%EB%B8%90%20GO%20%EA%B0%A4%EB%9F%AD%EC%8B%9C.md) \- [소라노 아오이](%EC%86%8C%EB%9D%BC%EB%85%B8%20%EC%95%84%EC%98%A4%EC%9D%B4.md)/[노자키 사쿠라](%EB%85%B8%EC%9E%90%ED%82%A4%20%EC%82%AC%EC%BF%A0%EB%9D%BC.md)/[모리무라 코노하](%EB%AA%A8%EB%A6%AC%EB%AC%B4%EB%9D%BC%20%EC%BD%94%EB%85%B8%ED%95%98.md)`[13]`
  * [저, 트윈 테일이 됩니다](%EC%A0%80%2C%20%ED%8A%B8%EC%9C%88%20%ED%85%8C%EC%9D%BC%EC%9D%B4%20%EB%90%A9%EB%8B%88%EB%8B%A4.md) \- [츠베 아이카](%EC%B8%A0%EB%B2%A0%20%EC%95%84%EC%9D%B4%EC%B9%B4.md)([테일 블루](%ED%85%8C%EC%9D%BC%20%EB%B8%94%EB%A3%A8.md))/[미츠카 소지](%EB%AF%B8%EC%B8%A0%EC%B9%B4%20%EC%86%8C%EC%A7%80.md)([테일 레드](%ED%85%8C%EC%9D%BC%20%EB%A0%88%EB%93%9C.md))/[신도 에리나](%EC%8B%A0%EB%8F%84%20%EC%97%90%EB%A6%AC%EB%82%98.md)([테일 옐로](%ED%85%8C%EC%9D%BC%20%EC%98%90%EB%A1%9C.md))
  * [출동!머신로보 레스큐](%EC%B6%9C%EB%8F%99%21%EB%A8%B8%EC%8B%A0%EB%A1%9C%EB%B3%B4%20%EB%A0%88%EC%8A%A4%ED%81%90.md) \- [폴리스 로보](%ED%8F%B4%EB%A6%AC%EC%8A%A4%20%EB%A1%9C%EB%B3%B4.md)(블루 사이렌즈)/[제트 로보](%EC%A0%9C%ED%8A%B8%20%EB%A1%9C%EB%B3%B4.md)(레드 윙즈)/[드릴 로보](%EB%93%9C%EB%A6%B4%20%EB%A1%9C%EB%B3%B4.md)(옐로 기어즈)
  * [포켓몬스터 시리즈](%ED%8F%AC%EC%BC%93%EB%AA%AC%EC%8A%A4%ED%84%B0.md)  

    * [제1세대](%ED%8F%AC%EC%BC%93%EB%AA%AC%EC%8A%A4%ED%84%B0%20%EC%A0%81%C2%B7%EB%85%B9.md) \- [프리저](%ED%94%84%EB%A6%AC%EC%A0%80.md)/[파이어](%ED%8C%8C%EC%9D%B4%EC%96%B4.md)/[썬더](%EC%8D%AC%EB%8D%94.md)
    * [제2세대](%ED%8F%AC%EC%BC%93%EB%AA%AC%EC%8A%A4%ED%84%B0%20%EA%B8%88%C2%B7%EC%9D%80.md) \- [스이쿤](%EC%8A%A4%EC%9D%B4%EC%BF%A4.md)/[앤테이](%EC%95%A4%ED%85%8C%EC%9D%B4.md)/[라이코](%EB%9D%BC%EC%9D%B4%EC%BD%94.md)
    * **[제4세대](%ED%8F%AC%EC%BC%93%EB%AA%AC%EC%8A%A4%ED%84%B0%20DP%20%EB%94%94%EC%95%84%EB%A3%A8%EA%B0%80%C2%B7%ED%8E%84%EA%B8%B0%EC%95%84.md)**`[14]`  

      * [아그놈](%EC%95%84%EA%B7%B8%EB%86%88.md)/[엠라이트](%EC%97%A0%EB%9D%BC%EC%9D%B4%ED%8A%B8.md)/[유크시](%EC%9C%A0%ED%81%AC%EC%8B%9C.md)
      * [디아루가](%EB%94%94%EC%95%84%EB%A3%A8%EA%B0%80.md)/[펄기아](%ED%8E%84%EA%B8%B0%EC%95%84.md)/[기라티나](%EA%B8%B0%EB%9D%BC%ED%8B%B0%EB%82%98.md)
    * [포켓몬스터 SPECIAL](%ED%8F%AC%EC%BC%93%EB%AA%AC%EC%8A%A4%ED%84%B0%20SPECIAL.md) \- [다이아몬드](%EB%8B%A4%EC%9D%B4%EC%95%84%EB%AA%AC%EB%93%9C%28%ED%8F%AC%EC%BC%93%EB%AA%AC%EC%8A%A4%ED%84%B0%20SPECIAL%29.md)/[펄](%ED%8E%84%28%ED%8F%AC%EC%BC%93%EB%AA%AC%EC%8A%A4%ED%84%B0%20SPECIAL%29.md)/[플라티나](%ED%94%8C%EB%9D%BC%ED%8B%B0%EB%82%98%20%EB%B2%A0%EB%A5%BC%EB%A6%AC%EC%B8%A0.md)
  * [케이온!](%EC%BC%80%EC%9D%B4%EC%98%A8%21.md) \- [아키야마 미오](%EC%95%84%ED%82%A4%EC%95%BC%EB%A7%88%20%EB%AF%B8%EC%98%A4.md)/[히라사와 유이](%ED%9E%88%EB%9D%BC%EC%82%AC%EC%99%80%20%EC%9C%A0%EC%9D%B4.md)/[타이나카 리츠](%ED%83%80%EC%9D%B4%EB%82%98%EC%B9%B4%20%EB%A6%AC%EC%B8%A0.md)
  * [킬라킬](%ED%82%AC%EB%9D%BC%ED%82%AC.md) \- 혼노지 사천왕 : [이누무타 호카](%EC%9D%B4%EB%88%84%EB%AC%B4%ED%83%80%20%ED%98%B8%EC%B9%B4.md)/[자쿠즈레 노논](%EC%9E%90%EC%BF%A0%EC%A6%88%EB%A0%88%20%EB%85%B8%EB%85%BC.md)/[가마고리 이라](%EA%B0%80%EB%A7%88%EA%B3%A0%EB%A6%AC%20%EC%9D%B4%EB%9D%BC.md)
  * [페르소나 시리즈](%ED%8E%98%EB%A5%B4%EC%86%8C%EB%82%98%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md)의 이미지 컬러 - [페르소나 3](%ED%8E%98%EB%A5%B4%EC%86%8C%EB%82%98%203.md)/[페르소나 5](%ED%8E%98%EB%A5%B4%EC%86%8C%EB%82%98%205.md)/[페르소나 4](%ED%8E%98%EB%A5%B4%EC%86%8C%EB%82%98%204.md)  

    * [페르소나 4](%ED%8E%98%EB%A5%B4%EC%86%8C%EB%82%98%204.md) \- [시로가네 나오토](%EC%8B%9C%EB%A1%9C%EA%B0%80%EB%84%A4%20%EB%82%98%EC%98%A4%ED%86%A0.md)/[쿠지카와 리세](%EC%BF%A0%EC%A7%80%EC%B9%B4%EC%99%80%20%EB%A6%AC%EC%84%B8.md)/[곰](%EA%B3%B0%28%ED%8E%98%EB%A5%B4%EC%86%8C%EB%82%98%204%29.md)/[타츠미 칸지](%ED%83%80%EC%B8%A0%EB%AF%B8%20%EC%B9%B8%EC%A7%80.md)
  * [프리큐어 시리즈](%ED%94%84%EB%A6%AC%ED%81%90%EC%96%B4%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md)  

    * [Yes! 프리큐어 5](Yes%21%20%ED%94%84%EB%A6%AC%ED%81%90%EC%96%B4%205.md) \- [미나즈키 카렌](%EB%AF%B8%EB%82%98%EC%A6%88%ED%82%A4%20%EC%B9%B4%EB%A0%8C.md)(큐어 아쿠아)/[나츠키 린](%EB%82%98%EC%B8%A0%ED%82%A4%20%EB%A6%B0.md)(큐어 루즈)/[카스가노 우라라](%EC%B9%B4%EC%8A%A4%EA%B0%80%EB%85%B8%20%EC%9A%B0%EB%9D%BC%EB%9D%BC.md)(큐어 레모네이드)
    * [프레쉬 프리큐어!](%ED%94%84%EB%A0%88%EC%89%AC%20%ED%94%84%EB%A6%AC%ED%81%90%EC%96%B4%21.md) \- [아오노 미키](%EC%95%84%EC%98%A4%EB%85%B8%20%EB%AF%B8%ED%82%A4.md)(큐어 베리)/[모모조노 러브](%EB%AA%A8%EB%AA%A8%EC%A1%B0%EB%85%B8%20%EB%9F%AC%EB%B8%8C.md)(큐어 피치)/[야마부키 이노리](%EC%95%BC%EB%A7%88%EB%B6%80%ED%82%A4%20%EC%9D%B4%EB%85%B8%EB%A6%AC.md)(큐어 파인)
    * [하트 캐치 프리큐어!](%ED%95%98%ED%8A%B8%20%EC%BA%90%EC%B9%98%20%ED%94%84%EB%A6%AC%ED%81%90%EC%96%B4%21.md)`[15]`  

      * [쿠루미 에리카](%EC%BF%A0%EB%A3%A8%EB%AF%B8%20%EC%97%90%EB%A6%AC%EC%B9%B4.md)(큐어 마린)/[하나사키 츠보미](%ED%95%98%EB%82%98%EC%82%AC%ED%82%A4%20%EC%B8%A0%EB%B3%B4%EB%AF%B8.md)(큐어 블로섬)/[묘도인 이츠키](%EB%AC%98%EB%8F%84%EC%9D%B8%20%EC%9D%B4%EC%B8%A0%ED%82%A4.md)(큐어 선샤인)
      * [코프레](%EC%BD%94%ED%94%84%EB%A0%88.md)/[시프레](%EC%8B%9C%ED%94%84%EB%A0%88.md)/[포프리](%ED%8F%AC%ED%94%84%EB%A6%AC.md)/[코론](%EC%BD%94%EB%A1%A0%28%ED%95%98%ED%8A%B8%20%EC%BA%90%EC%B9%98%20%ED%94%84%EB%A6%AC%ED%81%90%EC%96%B4%21%29.md)
      * [코브라자](%EC%BD%94%EB%B8%8C%EB%9D%BC%EC%9E%90.md)/[쿠모자키](%EC%BF%A0%EB%AA%A8%EC%9E%90%ED%82%A4.md)/[사소리나](%EC%82%AC%EC%86%8C%EB%A6%AC%EB%82%98.md)/[다크 프리큐어](%EB%8B%A4%ED%81%AC%20%ED%94%84%EB%A6%AC%ED%81%90%EC%96%B4.md)
    * [스위트 프리큐어♪](%EC%8A%A4%EC%9C%84%ED%8A%B8%20%ED%94%84%EB%A6%AC%ED%81%90%EC%96%B4%E2%99%AA.md) \- [쿠로카와 엘렌](%EC%BF%A0%EB%A1%9C%EC%B9%B4%EC%99%80%20%EC%97%98%EB%A0%8C.md)(큐어 비트)/[호조 히비키](%ED%98%B8%EC%A1%B0%20%ED%9E%88%EB%B9%84%ED%82%A4.md)(큐어 멜로디)/[시라베 아코](%EC%8B%9C%EB%9D%BC%EB%B2%A0%20%EC%95%84%EC%BD%94.md)(큐어 뮤즈)`[16]`
    * [스마일 프리큐어!](%EC%8A%A4%EB%A7%88%EC%9D%BC%20%ED%94%84%EB%A6%AC%ED%81%90%EC%96%B4%21.md) \- [아오키 레이카](%EC%95%84%EC%98%A4%ED%82%A4%20%EB%A0%88%EC%9D%B4%EC%B9%B4.md)(큐어 뷰티)/[히노 아카네](%ED%9E%88%EB%85%B8%20%EC%95%84%EC%B9%B4%EB%84%A4%28%EC%8A%A4%EB%A7%88%EC%9D%BC%20%ED%94%84%EB%A6%AC%ED%81%90%EC%96%B4%21%29.md)(큐어 써니)`[17]`/[키세 야요이](%ED%82%A4%EC%84%B8%20%EC%95%BC%EC%9A%94%EC%9D%B4.md)(큐어 피스)
    * [두근두근! 프리큐어](%EB%91%90%EA%B7%BC%EB%91%90%EA%B7%BC%21%20%ED%94%84%EB%A6%AC%ED%81%90%EC%96%B4.md)   

      * [히시카와 릿카](%ED%9E%88%EC%8B%9C%EC%B9%B4%EC%99%80%20%EB%A6%BF%EC%B9%B4.md)(큐어 다이아몬드)/[아이다 마나](%EC%95%84%EC%9D%B4%EB%8B%A4%20%EB%A7%88%EB%82%98.md)(큐어 하트)/[요츠바 아리스](%EC%9A%94%EC%B8%A0%EB%B0%94%20%EC%95%84%EB%A6%AC%EC%8A%A4.md)(큐어 로제타)/[켄자키 마코토](%EC%BC%84%EC%9E%90%ED%82%A4%20%EB%A7%88%EC%BD%94%ED%86%A0.md)(큐어 소드)
      * [라켈](%EB%9D%BC%EC%BC%88%28%EB%91%90%EA%B7%BC%EB%91%90%EA%B7%BC%21%20%ED%94%84%EB%A6%AC%ED%81%90%EC%96%B4%29.md)/[샤를](%EC%83%A4%EB%A5%BC%28%EB%91%90%EA%B7%BC%EB%91%90%EA%B7%BC%21%20%ED%94%84%EB%A6%AC%ED%81%90%EC%96%B4%29.md)/[란스](%EB%9E%80%EC%8A%A4%28%EB%91%90%EA%B7%BC%EB%91%90%EA%B7%BC%21%20%ED%94%84%EB%A6%AC%ED%81%90%EC%96%B4%29.md)/[다비](%EB%8B%A4%EB%B9%84%28%EB%91%90%EA%B7%BC%EB%91%90%EA%B7%BC%21%20%ED%94%84%EB%A6%AC%ED%81%90%EC%96%B4%29.md)
    * [해피니스 차지 프리큐어!](%ED%95%B4%ED%94%BC%EB%8B%88%EC%8A%A4%20%EC%B0%A8%EC%A7%80%20%ED%94%84%EB%A6%AC%ED%81%90%EC%96%B4%21.md) \- [시라유키 히메](%EC%8B%9C%EB%9D%BC%EC%9C%A0%ED%82%A4%20%ED%9E%88%EB%A9%94.md)(큐어 프린세스)/[아이노 메구미](%EC%95%84%EC%9D%B4%EB%85%B8%20%EB%A9%94%EA%B5%AC%EB%AF%B8.md)(큐어 러블리)/[오모리 유코](%EC%98%A4%EB%AA%A8%EB%A6%AC%20%EC%9C%A0%EC%BD%94.md)(큐어 허니)/[히카와 이오나](%ED%9E%88%EC%B9%B4%EC%99%80%20%EC%9D%B4%EC%98%A4%EB%82%98.md)(큐어 포춘)
    * [Go! 프린세스 프리큐어](Go%21%20%ED%94%84%EB%A6%B0%EC%84%B8%EC%8A%A4%20%ED%94%84%EB%A6%AC%ED%81%90%EC%96%B4.md) \- [카이도 미나미](%EC%B9%B4%EC%9D%B4%EB%8F%84%20%EB%AF%B8%EB%82%98%EB%AF%B8.md)(큐어 머메이드)/[하루노 하루카](%ED%95%98%EB%A3%A8%EB%85%B8%20%ED%95%98%EB%A3%A8%EC%B9%B4.md)(큐어 플로라)/[아마노가와 키라라](%EC%95%84%EB%A7%88%EB%85%B8%EA%B0%80%EC%99%80%20%ED%82%A4%EB%9D%BC%EB%9D%BC.md)(큐어 트윙클)
  * [회색도시](%ED%9A%8C%EC%83%89%EB%8F%84%EC%8B%9C.md) \- [김주황](%EA%B9%80%EC%A3%BC%ED%99%A9.md)/[하태성](%ED%95%98%ED%83%9C%EC%84%B1.md)/[허건오](%ED%97%88%EA%B1%B4%EC%98%A4.md)
  * [Fate/Zero](Fate/Zero.md) \- [세이버](%EC%84%B8%EC%9D%B4%EB%B2%84%284%EC%B0%A8%2C%205%EC%B0%A8%29.md)/[라이더](%EB%9D%BC%EC%9D%B4%EB%8D%94%284%EC%B0%A8%29.md)/[아처](%EC%95%84%EC%B2%98%284%EC%B0%A8%29.md) (성배문답에 참여한 3인의 왕)
  * [Free!](Free%21.md) \- [나나세 하루카](%EB%82%98%EB%82%98%EC%84%B8%20%ED%95%98%EB%A3%A8%EC%B9%B4.md)/[마츠오카 린](%EB%A7%88%EC%B8%A0%EC%98%A4%EC%B9%B4%20%EB%A6%B0.md)/[하즈키 나기사](%ED%95%98%EC%A6%88%ED%82%A4%20%EB%82%98%EA%B8%B0%EC%82%AC.md)
  * [GA 예술과 아트 디자인 클래스](GA%20%EC%98%88%EC%88%A0%EA%B3%BC%20%EC%95%84%ED%8A%B8%20%EB%94%94%EC%9E%90%EC%9D%B8%20%ED%81%B4%EB%9E%98%EC%8A%A4.md) ([색채전대 이로도룬져](%EC%83%89%EC%B1%84%EC%A0%84%EB%8C%80%20%EC%9D%B4%EB%A1%9C%EB%8F%84%EB%A3%AC%EC%A0%B8.md))`[18]` \- [야마구치 키사라기](%EC%95%BC%EB%A7%88%EA%B5%AC%EC%B9%98%20%ED%82%A4%EC%82%AC%EB%9D%BC%EA%B8%B0.md)/[노다 미키](%EB%85%B8%EB%8B%A4%20%EB%AF%B8%ED%82%A4.md)/[노자키 나미코](%EB%85%B8%EC%9E%90%ED%82%A4%20%EB%82%98%EB%AF%B8%EC%BD%94.md)/[오미치 미야비](%EC%98%A4%EB%AF%B8%EC%B9%98%20%EB%AF%B8%EC%95%BC%EB%B9%84.md)`[19]`/<del>[토모카네](%ED%86%A0%EB%AA%A8%EC%B9%B4%EB%84%A4.md)</del>`[20]`
  * [My Little Pony: Equestria Girls - Rainbow Rocks](My%20Little%20Pony%3A%20Equestria%20Girls%20-%20Rainbow%20Rocks.md) \- [소나타 더스크](%EC%82%AC%EC%9D%B4%EB%A0%8C%28Equestria%20Girls%29.md)/[아리아 블레이즈](%EC%82%AC%EC%9D%B4%EB%A0%8C%28Equestria%20Girls%29.md)`[21]`/[아다지오 대즐](%EC%82%AC%EC%9D%B4%EB%A0%8C%28Equestria%20Girls%29.md)
  * [GARO 어둠을 비추는 자](GARO.md) \- [쿠스가미 아그리](%EC%BF%A0%EC%8A%A4%EA%B0%80%EB%AF%B8%20%EC%95%84%EA%B7%B8%EB%A6%AC.md)(천궁기사 가이)/[자쿠즈레 타케루](%EC%9E%90%EC%BF%A0%EC%A6%88%EB%A0%88%20%ED%83%80%EC%BC%80%EB%A3%A8.md)(염인기사 젠)/[도우가이 류우가](%EB%8F%84%EC%9A%B0%EA%B0%80%EC%9D%B4%20%EB%A5%98%EC%9A%B0%EA%B0%80.md)([황금기사 가로](%ED%99%A9%EA%B8%88%EA%B8%B0%EC%82%AC%20%EA%B0%80%EB%A1%9C.md))
  * [Ib](Ib.md) \- [게리](%EA%B2%8C%EB%A6%AC%28Ib%29.md)/[이브](%EC%9D%B4%EB%B8%8C%28Ib%29.md)/[메리](%EB%A9%94%EB%A6%AC%28Ib%29.md)

[[edit](http://rigvedawiki.net/r1/wiki.php/CMYK?action=edit&section=8)]

### 1.5. 관련 항목 ¶

  * [색](%EC%83%89.md)
  * [RGB](RGB.md)
  * [HSB](HSB.md)
  * [Lab](Lab.md)
  * [YMCK](YMCK.md) \- 밴드 이름이 이 CMYK에서 따온 것이다.

[[edit](http://rigvedawiki.net/r1/wiki.php/CMYK?action=edit&section=9)]

## 2. 가수 ¶

[대한민국](%EB%8C%80%ED%95%9C%EB%AF%BC%EA%B5%AD.md)의 3인조
[힙합](%ED%9E%99%ED%95%A9.md) 그룹이다. 예전 이름은 Sunday2pm, 멤버는 데피닛, 지백, 투덱스.  

`\----`

  * `[1]` 블랙을 K로 표기하는 이유는 B로 표기하면 RGB의 블루(**B**lue)와 겹치기 때문.
  * `[2]` 빛의 3원색은 [빨강 초록 파랑 그대로의 색이 맞다.](RGB.md)
  * `[3]` 참고로 C 100 M 100 Y 100 K 100으로 섞어도 검은색이 아니다. 그리고 C 0 M 0 Y 0 K 100은 검은색이 맞긴 한데 색의 깊이가 얕다는 느낌이 든다. 인쇄업계에서는 Rich Black이라는 색을 따로 쓰는데 인쇄소가 사용하는 잉크의 제조사별로 다르지만 보통 C 91 M 79 Y 62 K 97 또는 C 96 M 70 Y 46 K 86 을 쓴다. 전자는 #010203이고, 후자는 #010b13.
  * `[4]` 모니터에서는 Black과 Rich Black 모두 R0 B0 G0 이어서 똑같아보이는데 인쇄해보면 다르다. 따라서 인쇄할 작업물은 아무리 확신이 서도 샘플 인쇄를 해봐야 한다.
  * `[5]` 단 [HSB](HSB.md)는 원기둥을 골자로 한 곡면기하
  * `[6]` 성능이 다소 떨어지는 대량인쇄용 프린터라면 더욱 그렇다. 반대로 고성능 인쇄기라면 거의 원색에 똑같은 결과를 기대할 수 있다.
  * `[7]` 반대로 덩치나 [장신](%EC%9E%A5%EC%8B%A0.md)으로 묘사되기도 한다.
  * `[8]` 이 자리에 파랑 키노피오가 들어가기도 한다. 애초에 두 명 다 선택 가능.
  * `[9]` CMY관련 색상 배치 중에서도 가장 유명하다. 여기서는 3인전대이거나 초기에 3인체재었던 전대만을 서술하기 바람.
  * `[10]` 이 자리에 [쿠레바야시 쥬리](%EC%BF%A0%EB%A0%88%EB%B0%94%EC%95%BC%EC%8B%9C%20%EC%A5%AC%EB%A6%AC.md)가 들어갈 수 있다.
  * `[11]` CMY 속성의 캐릭터 중에서도 워낙 유명한 케이스라서 그런지 아예 CMY 색을 가진 삼인방을 가리켜 **삼대장**이라고 부르는 경우가 많다.
  * `[12]` 위의 삼대장과 마찬가지로 이름에 색을 나타내는 단어가 하나씩 들어가 있는게 특징이다.
  * `[13]` 머리색은 RGB지만 이미지컬러로 따지면 CMY.
  * `[14]` 포켓몬 시리즈 중 가장 시안/마젠타/옐로우에 일치한 색상배치이다.
  * `[15]` 프리큐어 시리즈 중 가장 시안/마젠타/옐로우에 근접한 색상배치이다.
  * `[16]` 가끔 이 자리에 [미나미노 카나데](%EB%AF%B8%EB%82%98%EB%AF%B8%EB%85%B8%20%EC%B9%B4%EB%82%98%EB%8D%B0.md)(큐어 리듬)가 들어가기도 하지만, 카나데의 공색 색상은 **흰색**이다.
  * `[17]` 이 자리에는 [호시조라 미유키](%ED%98%B8%EC%8B%9C%EC%A1%B0%EB%9D%BC%20%EB%AF%B8%EC%9C%A0%ED%82%A4.md)(큐어 해피)가 들어갈수도 있지만, 클리셰에 따르면 아카네쪽이 더 가깝기 때문에 이렇게 서술한다.
  * `[18]` 사실 이건 작중 CMYK를 가지고 색채전대라며 전대물 드립을 친 것이다. 각자의 명칭은 [데셍의 레드](%ED%86%A0%EB%AA%A8%EC%B9%B4%EB%84%A4.md), [기술의 옐로](%EB%85%B8%EC%9E%90%ED%82%A4%20%EB%82%98%EB%AF%B8%EC%BD%94.md), [채색의 마젠타](%EB%85%B8%EB%8B%A4%20%EB%AF%B8%ED%82%A4.md), [효과의 시안](%EC%95%BC%EB%A7%88%EA%B5%AC%EC%B9%98%20%ED%82%A4%EC%82%AC%EB%9D%BC%EA%B8%B0.md), [보정의 모노크로](%EC%98%A4%EB%AF%B8%EC%B9%98%20%EB%AF%B8%EC%95%BC%EB%B9%84.md).
  * `[19]` K, 검정이다.
  * `[20]` 대장이라는 이유로 R, 빨강이다. 물론 다른 애들에게 까였다.
  * `[21]` M이 아닌 K에 가깝다.

