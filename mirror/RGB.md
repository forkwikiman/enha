![rgb.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/rgb.jpg)

[JPG image (6.45 KB)]

## Contents

    

1. 설명 
    

1.1. 디지털에서의 색 표현 방법

2. 서브컬쳐에서의 활용 
3. 관련 항목 

[[edit](http://rigvedawiki.net/r1/wiki.php/RGB?action=edit&section=1)]

## 1. 설명 ¶

[빛](%EB%B9%9B.md)의 [삼원색](%EC%82%BC%EC%9B%90%EC%83%89.md)을 뜻하는 말로,
[빨간색](%EB%B9%A8%EA%B0%84%EC%83%89.md)(Red),
[초록색](%EC%B4%88%EB%A1%9D%EC%83%89.md)(Green),
[파란색](%ED%8C%8C%EB%9E%80%EC%83%89.md)(Blue)의 합성어이다.

  

색광에서 빨간색과 초록색을 합치면 [노란색](%EB%85%B8%EB%9E%80%EC%83%89.md)(Yellow)이 되고, 초록색과
파란색을 합치면 [청록색](%EC%B2%AD%EB%A1%9D%EC%83%89.md)(Cyan)이 되며, 파란색과 빨간색을 합치면
[마젠타](%EB%A7%88%EC%A0%A0%ED%83%80.md)(Magenta)`[1]`가 된다. 그리고 세 가지 색을 모두 합치면
[흰색](%ED%9D%B0%EC%83%89.md)(White)이 되고, 반대로 세 가지 색을 모두 제외하면
[검정색](%EA%B2%80%EC%A0%95%EC%83%89.md)(Black)이 된다.

  

이런 식으로 세 가지 색상으로 모든 색을 조합시킬 수 있으며,
[텔레비전](%ED%85%94%EB%A0%88%EB%B9%84%EC%A0%84.md)이나
[컴퓨터](%EC%BB%B4%ED%93%A8%ED%84%B0.md)의
[모니터](%EB%AA%A8%EB%8B%88%ED%84%B0.md) 등 영상 장치의
[해상도](%ED%95%B4%EC%83%81%EB%8F%84.md)를 조절하는 표시 장치에 사용된다. 또한 빛을 이용하는 장치가 아닌
인쇄 매체의 경우에는 [잉크](%EC%9E%89%ED%81%AC.md)체계를 사용해 특정 색을 흡수하고 나머지를 반사하기 때문에
RGB가 아닌 [CMYK](CMYK.md)가 적용된다.

  

또한 두 가지 색상을 겹쳐서 흰색을 만들 수 있는 경우, 해당되는 두 색상을 [보색](%EB%B3%B4%EC%83%89.md)이라고
한다

  

일단 현실에서는 광점의 휘도만 적절히 조합하면 장땡이기에 CMYK에 비해 색 표현능력이 높지만, 그렇다고 모든 색을 표현할 수 있는 것은
아니다. 이를 보완하기 위해 등장한 색공간이 CIE XYZ 색공간.

  

[게이지 보존](%EA%B2%8C%EC%9D%B4%EC%A7%80%20%EB%B3%B4%EC%A1%B4.md) 중 하나인 글루온도
RGB의 색 개념이 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/RGB?action=edit&section=2)]

### 1.1. 디지털에서의 색 표현 방법 ¶

디지털에서는 각 색의 밝기를 숫자로 나타내어 표기하는데, 보통 각 색에 몇 비트씩 할당하여 표현한다. 비트 수에 따라 표현할 수 있는 색상
수가 달라진다.

  

8비트까지의 색상 표현은 [폰트](%ED%8F%B0%ED%8A%B8.md)와 비슷하게 각각의 주소 공간을 하나하나 줄 세워서 각각의
주소에 해당 색상을 하나하나 대응시키는 방법을 썼다. 이것을 [팔레트](%ED%8C%94%EB%A0%88%ED%8A%B8.md)라고
했다. 이 팔레트는 임의로 바꿀 수가 있었기에, 그래픽을 표현하는 프로그램마다 팔레트는 천차만별이었다. 심지어는 팔레트를 순간순간 바꿔
가면서 적은 표현색으로 다양한 색을 표현하는 기법도 쓰였다.

  

그러나 8비트를 넘어서면서 주소 공간이 너무 많아지자, 비트를 적당히 잘라 앞의 몇 비트는 R, 중간의 몇 비트는 G, 끝의 몇 비트는 B의
밝기를 표시하는 방법으로 바뀌었다.

  

  * 1비트 : 2개 색상만 표현 가능하다. 검정과 흰색만 표현하면 **흑백**. 그러나 2개 색상이라고 해도 하나는 거의 항상 검정만 표시하기 때문에, 남은 한 색상만 달라진다. 컴퓨터 초창기에 나온 그린 모니터나 호박색 모니터가 이런 경우다.
  * 2비트 : 과거 [CGA](CGA.md) 그래픽 카드가 사용했던 것으로, 네 가지 색상이 표현 가능했다.
  * 4비트 : 과거 [EGA](EGA.md) 그래픽 카드가 사용했던 것으로, 16색 표현이 가능했다. 일본의 PC9801 기종으로 나온 게임은 16색으로 상당히 미려한 그래픽을 구현했다.
  * 8비트 : 256색 표현이 가능. 1990년대 중반까지 많이 쓰였다.
  * 16비트 : R과 B는 5비트, G는 6비트`[2]`를 할당하여 만든 색공간으로, **하이 컬러(High Color)**라고 많이 불렸다. 65536가지 색상이 표현 가능하다. 바리에이션으로 RGB 모두 5비트를 표현하고, 나머지 1비트는 투명 여부를 표현하는 값으로 쓰인 것도 있다.
  * 24비트 : RGB를 각각 8비트씩 할당한 것. 이것을 **24비트 트루 컬러(True Color)**라고 말한다. 이렇게 표현 가능한 색상은 16,777,216가지이고, 이것은 **sRGB**라는 이름으로 국제전기표준회의의 표준으로 등재되어 있다. HTML의 색상 코드도 이것을 16진수로 표현한 값을 쓰고 있다.
  * 32비트 : 24비트 트루 컬러에 8비트의 투명값(alpha)를 추가한 것으로, **RGBA**라고 부른다.  

이외에도 48비트 딥컬러나 [포토샵](%ED%8F%AC%ED%86%A0%EC%83%B5.md) 등 전문가용 프로그램에서 사용하는
64비트 컬러(RGBA 각각 16비트 할당), 128비트 컬러(RGBA 각각 32비트 할당) 등이 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/RGB?action=edit&section=3)]

## 2. 서브컬쳐에서의 활용 ¶

빛의 삼원색이라는 공통점 때문인지 서로 많이 엮이는 3인조를 상징하는 색으로 자주 활용된다. 특히
[포켓몬스터](%ED%8F%AC%EC%BC%93%EB%AA%AC%EC%8A%A4%ED%84%B0.md)에서 많이 활용되며, 포켓몬스터
시리즈 중 가장 먼저 발매된 [적/녹/청](%ED%8F%AC%EC%BC%93%EB%AA%AC%EC%8A%A4%ED%84%B0%20%EC%A0%81/%EB%85%B9.md) 시리즈를 'RGB 시리즈'라고 하기도 한다.

  

아래는 예시. (빨강 \- 초록 \- 파랑 순으로 적는다.)

  

  * [가면라이더 시리즈](%EA%B0%80%EB%A9%B4%EB%9D%BC%EC%9D%B4%EB%8D%94%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md)  

    * [가면라이더 류우키](%EA%B0%80%EB%A9%B4%EB%9D%BC%EC%9D%B4%EB%8D%94%20%EB%A5%98%EC%9A%B0%ED%82%A4.md) : [류우키](%EB%A5%98%EC%9A%B0%ED%82%A4.md) \- [졸다](%EC%A1%B8%EB%8B%A4.md) \- [나이트](%EB%82%98%EC%9D%B4%ED%8A%B8%28%EA%B0%80%EB%A9%B4%EB%9D%BC%EC%9D%B4%EB%8D%94%20%EB%A5%98%EC%9A%B0%ED%82%A4%29.md)
    * [가면라이더 블레이드](%EA%B0%80%EB%A9%B4%EB%9D%BC%EC%9D%B4%EB%8D%94%20%EB%B8%94%EB%A0%88%EC%9D%B4%EB%93%9C.md) : [갸렌](%EA%B0%B8%EB%A0%8C.md) \- [렌겔](%EB%A0%8C%EA%B2%94.md) \- [블레이드](%EB%B8%94%EB%A0%88%EC%9D%B4%EB%93%9C%28%EA%B0%80%EB%A9%B4%EB%9D%BC%EC%9D%B4%EB%8D%94%20%EB%B8%94%EB%A0%88%EC%9D%B4%EB%93%9C%29.md)
    * [가면라이더 덴오](%EA%B0%80%EB%A9%B4%EB%9D%BC%EC%9D%B4%EB%8D%94%20%EB%8D%B4%EC%98%A4.md) : [모모타로스](%EB%AA%A8%EB%AA%A8%ED%83%80%EB%A1%9C%EC%8A%A4.md) \- [데네브](%EB%8D%B0%EB%84%A4%EB%B8%8C%28%EA%B0%80%EB%A9%B4%EB%9D%BC%EC%9D%B4%EB%8D%94%20%EB%8D%B4%EC%98%A4%29.md) \- [우라타로스](%EC%9A%B0%EB%9D%BC%ED%83%80%EB%A1%9C%EC%8A%A4.md)
    * [가면라이더 오즈](%EA%B0%80%EB%A9%B4%EB%9D%BC%EC%9D%B4%EB%8D%94%20%EC%98%A4%EC%A6%88.md) : [앙크](%EC%95%99%ED%81%AC%28%EA%B0%80%EB%A9%B4%EB%9D%BC%EC%9D%B4%EB%8D%94%20%EC%98%A4%EC%A6%88%29.md) \- [우바](%EC%9A%B0%EB%B0%94.md) \- [메즐](%EB%A9%94%EC%A6%90.md)
    * [가면라이더 위자드](%EA%B0%80%EB%A9%B4%EB%9D%BC%EC%9D%B4%EB%8D%94%20%EC%9C%84%EC%9E%90%EB%93%9C.md) : [피닉스](%ED%9B%84%EC%A7%80%ED%83%80%20%EC%9C%A0%EC%9A%B0%EA%B3%A0.md) \- [그렘린](%ED%83%80%ED%82%A4%EA%B0%80%EC%99%80%20%EC%86%8C%EB%9D%BC.md) \- [메두사](%EC%9D%B4%EB%82%98%EB%AA%A8%EB%A6%AC%20%EB%AF%B8%EC%82%AC.md)`[3]`
    * [가면라이더 가이무](%EA%B0%80%EB%A9%B4%EB%9D%BC%EC%9D%B4%EB%8D%94%20%EA%B0%80%EC%9D%B4%EB%AC%B4.md) : [바론](%EB%B0%94%EB%A1%A0%28%EA%B0%80%EB%A9%B4%EB%9D%BC%EC%9D%B4%EB%8D%94%20%EA%B0%80%EC%9D%B4%EB%AC%B4%29.md) \- [류겐](%EB%A5%98%EA%B2%90.md) \- [가이무](%EA%B0%80%EC%9D%B4%EB%AC%B4.md)
    * [가면라이더 드라이브](%EA%B0%80%EB%A9%B4%EB%9D%BC%EC%9D%B4%EB%8D%94%20%EB%93%9C%EB%9D%BC%EC%9D%B4%EB%B8%8C.md) : [하트](%ED%95%98%ED%8A%B8%28%EA%B0%80%EB%A9%B4%EB%9D%BC%EC%9D%B4%EB%8D%94%20%EB%93%9C%EB%9D%BC%EC%9D%B4%EB%B8%8C%29.md) \- [브렌](%EB%B8%8C%EB%A0%8C%28%EA%B0%80%EB%A9%B4%EB%9D%BC%EC%9D%B4%EB%8D%94%20%EB%93%9C%EB%9D%BC%EC%9D%B4%EB%B8%8C%29.md) \- [체이스](%EC%B2%B4%EC%9D%B4%EC%8A%A4%28%EA%B0%80%EB%A9%B4%EB%9D%BC%EC%9D%B4%EB%8D%94%20%EB%93%9C%EB%9D%BC%EC%9D%B4%EB%B8%8C%29.md)
  * [개구리 중사 케로로](%EA%B0%9C%EA%B5%AC%EB%A6%AC%20%EC%A4%91%EC%82%AC%20%EC%BC%80%EB%A1%9C%EB%A1%9C.md) : [기로로](%EA%B8%B0%EB%A1%9C%EB%A1%9C.md) \- [케로로](%EC%BC%80%EB%A1%9C%EB%A1%9C.md) \- [도로로](%EB%8F%84%EB%A1%9C%EB%A1%9C.md)
  * [개그 콘서트](%EA%B0%9C%EA%B7%B8%20%EC%BD%98%EC%84%9C%ED%8A%B8.md)  

    * [도찐개찐](%EB%8F%84%EC%B0%90%EA%B0%9C%EC%B0%90%28%EA%B0%9C%EA%B7%B8%20%EC%BD%98%EC%84%9C%ED%8A%B8%29.md) : [박성호](%EB%B0%95%EC%84%B1%ED%98%B8.md) \- 이종훈 - 류근일
  * [골판지 전기 시리즈](%EA%B3%A8%ED%8C%90%EC%A7%80%20%EC%A0%84%EA%B8%B0%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md)  

    * [골판지 전기 W](%EA%B3%A8%ED%8C%90%EC%A7%80%20%EC%A0%84%EA%B8%B0%20W.md) : [하나사키 란](%ED%95%98%EB%82%98%EC%82%AC%ED%82%A4%20%EB%9E%80.md) \- [하이바라 유우야](%ED%95%98%EC%9D%B4%EB%B0%94%EB%9D%BC%20%EC%9C%A0%EC%9A%B0%EC%95%BC.md) \- [오오조라 히로](%EC%98%A4%EC%98%A4%EC%A1%B0%EB%9D%BC%20%ED%9E%88%EB%A1%9C.md)
    * [골판지 전기 WARS](%EA%B3%A8%ED%8C%90%EC%A7%80%20%EC%A0%84%EA%B8%B0%20WARS.md) : [세나 아라타](%EC%84%B8%EB%82%98%20%EC%95%84%EB%9D%BC%ED%83%80.md) \- [이즈모 하루키](%EC%9D%B4%EC%A6%88%EB%AA%A8%20%ED%95%98%EB%A3%A8%ED%82%A4.md) \- [호시하라 히카루](%ED%98%B8%EC%8B%9C%ED%95%98%EB%9D%BC%20%ED%9E%88%EC%B9%B4%EB%A3%A8.md)
  * [기타프릭스](%EA%B8%B0%ED%83%80%ED%94%84%EB%A6%AD%EC%8A%A4.md)`[4]` : 넥 버튼 R - G - B
  * [나이츠 오브 더 라운드](%EB%82%98%EC%9D%B4%EC%B8%A0%20%EC%98%A4%EB%B8%8C%20%EB%8D%94%20%EB%9D%BC%EC%9A%B4%EB%93%9C.md) : [아서 왕](%EC%95%84%EC%84%9C%20%EC%99%95.md) \- [퍼시벌](%ED%8D%BC%EC%8B%9C%EB%B2%8C.md) \- [랜슬롯](%EB%9E%9C%EC%8A%AC%EB%A1%AF.md)
  * [노래의☆왕자님♪](%EB%85%B8%EB%9E%98%EC%9D%98%E2%98%86%EC%99%95%EC%9E%90%EB%8B%98%E2%99%AA.md) : [잇토키 오토야](%EC%9E%87%ED%86%A0%ED%82%A4%20%EC%98%A4%ED%86%A0%EC%95%BC.md) \- [아이지마 세실](%EC%95%84%EC%9D%B4%EC%A7%80%EB%A7%88%20%EC%84%B8%EC%8B%A4.md) \- [히지리카와 마사토](%ED%9E%88%EC%A7%80%EB%A6%AC%EC%B9%B4%EC%99%80%20%EB%A7%88%EC%82%AC%ED%86%A0.md)
  * [디지몬 테이머즈](%EB%94%94%EC%A7%80%EB%AA%AC%20%ED%85%8C%EC%9D%B4%EB%A8%B8%EC%A6%88.md)  

    * [오유민](%EC%98%A4%EC%9C%A0%EB%AF%BC.md) \- [곽소룡](%EA%B3%BD%EC%86%8C%EB%A3%A1.md) \- [은세나](%EC%9D%80%EC%84%B8%EB%82%98.md)
    * [길몬](%EA%B8%B8%EB%AA%AC.md) \- [테리어몬](%ED%85%8C%EB%A6%AC%EC%96%B4%EB%AA%AC.md) \- [레나몬](%EB%A0%88%EB%82%98%EB%AA%AC.md)
  * [러브라이브](%EB%9F%AC%EB%B8%8C%EB%9D%BC%EC%9D%B4%EB%B8%8C.md) \- [코우사카 호노카](%EC%BD%94%EC%9A%B0%EC%82%AC%EC%B9%B4%20%ED%98%B8%EB%85%B8%EC%B9%B4.md) \- [미나미 코토리](%EB%AF%B8%EB%82%98%EB%AF%B8%20%EC%BD%94%ED%86%A0%EB%A6%AC.md) \- [소노다 우미](%EC%86%8C%EB%85%B8%EB%8B%A4%20%EC%9A%B0%EB%AF%B8.md)
  * [로젠 메이든](%EB%A1%9C%EC%A0%A0%20%EB%A9%94%EC%9D%B4%EB%93%A0.md) : [신쿠](%EC%8B%A0%EC%BF%A0%28%EB%A1%9C%EC%A0%A0%20%EB%A9%94%EC%9D%B4%EB%93%A0%29.md) \- [스이세이세키](%EC%8A%A4%EC%9D%B4%EC%84%B8%EC%9D%B4%EC%84%B8%ED%82%A4.md) \- [소우세이세키](%EC%86%8C%EC%9A%B0%EC%84%B8%EC%9D%B4%EC%84%B8%ED%82%A4.md)
  * [리그 오브 레전드](%EB%A6%AC%EA%B7%B8%20%EC%98%A4%EB%B8%8C%20%EB%A0%88%EC%A0%84%EB%93%9C.md)   

    * [카타리나](%EC%B9%B4%ED%83%80%EB%A6%AC%EB%82%98%28%EB%A6%AC%EA%B7%B8%20%EC%98%A4%EB%B8%8C%20%EB%A0%88%EC%A0%84%EB%93%9C%29.md) \- [카시오페아](%EC%B9%B4%EC%8B%9C%EC%98%A4%ED%8E%98%EC%95%84%28%EB%A6%AC%EA%B7%B8%20%EC%98%A4%EB%B8%8C%20%EB%A0%88%EC%A0%84%EB%93%9C%29.md) \- [탈론](%ED%83%88%EB%A1%A0%28%EB%A6%AC%EA%B7%B8%20%EC%98%A4%EB%B8%8C%20%EB%A0%88%EC%A0%84%EB%93%9C%29.md)
    * [다리우스](%EB%8B%A4%EB%A6%AC%EC%9A%B0%EC%8A%A4%28%EB%A6%AC%EA%B7%B8%20%EC%98%A4%EB%B8%8C%20%EB%A0%88%EC%A0%84%EB%93%9C%29.md) \- [스웨인](%EC%8A%A4%EC%9B%A8%EC%9D%B8%28%EB%A6%AC%EA%B7%B8%20%EC%98%A4%EB%B8%8C%20%EB%A0%88%EC%A0%84%EB%93%9C%29.md) \- [르블랑](%EB%A5%B4%EB%B8%94%EB%9E%91%28%EB%A6%AC%EA%B7%B8%20%EC%98%A4%EB%B8%8C%20%EB%A0%88%EC%A0%84%EB%93%9C%29.md)
    * [소나](%EC%86%8C%EB%82%98%28%EB%A6%AC%EA%B7%B8%20%EC%98%A4%EB%B8%8C%20%EB%A0%88%EC%A0%84%EB%93%9C%29.md)의 일반스킬(기민함의 노래 - 인내의 아리아 - 용맹의 찬가)
    * [리산드라](%EB%A6%AC%EC%82%B0%EB%93%9C%EB%9D%BC.md)의 스킨(혈석 - 서슬여왕 - 기본)
  * [마동왕 그랑조트](%EB%A7%88%EB%8F%99%EC%99%95%20%EA%B7%B8%EB%9E%91%EC%A1%B0%ED%8A%B8.md) : [그랑조트](%EA%B7%B8%EB%9E%91%EC%A1%B0%ED%8A%B8.md) \- [윙자트](%EC%9C%99%EC%9E%90%ED%8A%B8.md) \- [아쿠아비트](%EC%95%84%EC%BF%A0%EC%95%84%EB%B9%84%ED%8A%B8.md)
  * [마법기사 레이어스](%EB%A7%88%EB%B2%95%EA%B8%B0%EC%82%AC%20%EB%A0%88%EC%9D%B4%EC%96%B4%EC%8A%A4.md) : [시도우 히카루](%EC%8B%9C%EB%8F%84%EC%9A%B0%20%ED%9E%88%EC%B9%B4%EB%A3%A8.md) \- [호우오우지 후](%ED%98%B8%EC%9A%B0%EC%98%A4%EC%9A%B0%EC%A7%80%20%ED%9B%84.md) \- [류자키 우미](%EB%A5%98%EC%9E%90%ED%82%A4%20%EC%9A%B0%EB%AF%B8.md)
  * [마법소녀 마도카☆마기카](%EB%A7%88%EB%B2%95%EC%86%8C%EB%85%80%20%EB%A7%88%EB%8F%84%EC%B9%B4%E2%98%86%EB%A7%88%EA%B8%B0%EC%B9%B4.md) : [사쿠라 쿄코](%EC%82%AC%EC%BF%A0%EB%9D%BC%20%EC%BF%84%EC%BD%94.md) \- [시즈키 히토미](%EC%8B%9C%EC%A6%88%ED%82%A4%20%ED%9E%88%ED%86%A0%EB%AF%B8.md) \- [미키 사야카](%EB%AF%B8%ED%82%A4%20%EC%82%AC%EC%95%BC%EC%B9%B4.md)
  * [미소녀전사 세일러문](%EB%AF%B8%EC%86%8C%EB%85%80%EC%A0%84%EC%82%AC%20%EC%84%B8%EC%9D%BC%EB%9F%AC%EB%AC%B8.md) : [히노 레이](%ED%9E%88%EB%85%B8%20%EB%A0%88%EC%9D%B4.md) \- [키노 마코토](%ED%82%A4%EB%85%B8%20%EB%A7%88%EC%BD%94%ED%86%A0.md) \- [미즈노 아미](%EB%AF%B8%EC%A6%88%EB%85%B8%20%EC%95%84%EB%AF%B8.md)
  * [베리베리 뮤우뮤우](%EB%B2%A0%EB%A6%AC%EB%B2%A0%EB%A6%AC%20%EB%AE%A4%EC%9A%B0%EB%AE%A4%EC%9A%B0.md) : [모모미야 이치고](%EB%AA%A8%EB%AA%A8%EB%AF%B8%EC%95%BC%20%EC%9D%B4%EC%B9%98%EA%B3%A0.md) \- [미도리카와 레타스](%EB%AF%B8%EB%8F%84%EB%A6%AC%EC%B9%B4%EC%99%80%20%EB%A0%88%ED%83%80%EC%8A%A4.md) \- [아이자와 민트](%EC%95%84%EC%9D%B4%EC%9E%90%EC%99%80%20%EB%AF%BC%ED%8A%B8.md)
  * [변신 자동차 또봇](%EB%B3%80%EC%8B%A0%20%EC%9E%90%EB%8F%99%EC%B0%A8%20%EB%98%90%EB%B4%87.md) : [또봇 R](%EB%98%90%EB%B4%87%20R.md) \- [또봇 D](%EB%98%90%EB%B4%87%20D.md) \- [또봇 C](%EB%98%90%EB%B4%87%20C.md)
  * [뽀롱뽀롱 뽀로로](%EB%BD%80%EB%A1%B1%EB%BD%80%EB%A1%B1%20%EB%BD%80%EB%A1%9C%EB%A1%9C.md) : [루피](%EB%A3%A8%ED%94%BC.md) \- [크롱](%ED%81%AC%EB%A1%B1.md) \- [뽀로로](%EB%BD%80%EB%A1%9C%EB%A1%9C.md)
  * [삼국지 시리즈](%EC%82%BC%EA%B5%AD%EC%A7%80%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md) \- [손권](%EC%86%90%EA%B6%8C.md)(오), [유비](%EC%9C%A0%EB%B9%84.md)(촉), [조조](%EC%A1%B0%EC%A1%B0.md)(위)
  * [수협](%EC%88%98%ED%98%91.md) [마스코트](%EB%A7%88%EC%8A%A4%EC%BD%94%ED%8A%B8.md) (해우리가족) : 해랑이- 해동이- 파랑이
  * [슈퍼로봇대전 J](%EC%8A%88%ED%8D%BC%EB%A1%9C%EB%B4%87%EB%8C%80%EC%A0%84%20J.md) : [페스테니아 뮤즈](%ED%8E%98%EC%8A%A4%ED%85%8C%EB%8B%88%EC%95%84%20%EB%AE%A4%EC%A6%88.md) \- [카티아 그리낼](%EC%B9%B4%ED%8B%B0%EC%95%84%20%EA%B7%B8%EB%A6%AC%EB%82%BC.md) \- [메르아 메르나 메이아](%EB%A9%94%EB%A5%B4%EC%95%84%20%EB%A9%94%EB%A5%B4%EB%82%98%20%EB%A9%94%EC%9D%B4%EC%95%84.md)
  * [아지랑이 프로젝트](%EC%95%84%EC%A7%80%EB%9E%91%EC%9D%B4%20%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8.md) : [키사라기 신타로](%ED%82%A4%EC%82%AC%EB%9D%BC%EA%B8%B0%20%EC%8B%A0%ED%83%80%EB%A1%9C.md) \- [세토 코우스케](%EC%84%B8%ED%86%A0%20%EC%BD%94%EC%9A%B0%EC%8A%A4%EC%BC%80.md) \- [에네](%EC%97%90%EB%84%A4.md)
  * [아이돌 마스터](THE%20iDOLM%40STER.md)  

    * [아마미 하루카](%EC%95%84%EB%A7%88%EB%AF%B8%20%ED%95%98%EB%A3%A8%EC%B9%B4.md) \- [호시이 미키](%ED%98%B8%EC%8B%9C%EC%9D%B4%20%EB%AF%B8%ED%82%A4.md) \- [키사라기 치하야](%ED%82%A4%EC%82%AC%EB%9D%BC%EA%B8%B0%20%EC%B9%98%ED%95%98%EC%95%BC.md)
    * [히다카 아이](%ED%9E%88%EB%8B%A4%EC%B9%B4%20%EC%95%84%EC%9D%B4.md) \- [아키즈키 료](%EC%95%84%ED%82%A4%EC%A6%88%ED%82%A4%20%EB%A3%8C.md) \- [미즈타니 에리](%EB%AF%B8%EC%A6%88%ED%83%80%EB%8B%88%20%EC%97%90%EB%A6%AC.md)
  * [언더클래스 히어로](%EC%96%B8%EB%8D%94%ED%81%B4%EB%9E%98%EC%8A%A4%20%ED%9E%88%EC%96%B4%EB%A1%9C.md) : [인](%EC%9D%B8%28%EC%96%B8%EB%8D%94%ED%81%B4%EB%9E%98%EC%8A%A4%20%ED%9E%88%EC%96%B4%EB%A1%9C%29.md) \- [아미](%EC%95%84%EB%AF%B8%28%EC%96%B8%EB%8D%94%ED%81%B4%EB%9E%98%EC%8A%A4%20%ED%9E%88%EC%96%B4%EB%A1%9C%29.md) \- [류진](%EB%A5%98%EC%A7%84%28%EC%96%B8%EB%8D%94%ED%81%B4%EB%9E%98%EC%8A%A4%20%ED%9E%88%EC%96%B4%EB%A1%9C%29.md)
  * [원피스](%EC%9B%90%ED%94%BC%EC%8A%A4%28%EB%A7%8C%ED%99%94%29.md) : [몽키 D. 루피](%EB%AA%BD%ED%82%A4%20D.%20%EB%A3%A8%ED%94%BC.md) \- [롤로노아 조로](%EB%A1%A4%EB%A1%9C%EB%85%B8%EC%95%84%20%EC%A1%B0%EB%A1%9C.md) \- [상디](%EC%83%81%EB%94%94.md)
  * [이나즈마 일레븐](%EC%9D%B4%EB%82%98%EC%A6%88%EB%A7%88%20%EC%9D%BC%EB%A0%88%EB%B8%90.md) 시리즈  

    * 이나즈마 일레븐   

      * [라이몬 나츠미](%EB%9D%BC%EC%9D%B4%EB%AA%AC%20%EB%82%98%EC%B8%A0%EB%AF%B8.md) \- [키노 아키](%ED%82%A4%EB%85%B8%20%EC%95%84%ED%82%A4.md) \- [오토나시 하루나](%EC%98%A4%ED%86%A0%EB%82%98%EC%8B%9C%20%ED%95%98%EB%A3%A8%EB%82%98.md)
      * [무카타 토모 - 무카타 마사루 -무카타 츠토무](%EB%AC%B4%EC%B9%B4%ED%83%80%20%EC%82%BC%ED%98%95%EC%A0%9C.md)
    * [이나즈마 일레븐 GO](%EC%9D%B4%EB%82%98%EC%A6%88%EB%A7%88%20%EC%9D%BC%EB%A0%88%EB%B8%90%20GO.md)   

      * [야마나 아카네](%EC%95%BC%EB%A7%88%EB%82%98%20%EC%95%84%EC%B9%B4%EB%84%A4.md) \- [세토 미도리](%EC%84%B8%ED%86%A0%20%EB%AF%B8%EB%8F%84%EB%A6%AC.md) \- [소라노 아오이](%EC%86%8C%EB%9D%BC%EB%85%B8%20%EC%95%84%EC%98%A4%EC%9D%B4.md)`[5]`
      * [미츠요시 요자쿠라](%EB%AF%B8%EC%B8%A0%EC%9A%94%EC%8B%9C%20%EC%9A%94%EC%9E%90%EC%BF%A0%EB%9D%BC.md) \- [시노야마 미츠루](%EC%8B%9C%EB%85%B8%EC%95%BC%EB%A7%88%20%EB%AF%B8%EC%B8%A0%EB%A3%A8.md) \- [이소자키 켄마](%EC%9D%B4%EC%86%8C%EC%9E%90%ED%82%A4%20%EC%BC%84%EB%A7%88.md)
      * 요시미네 미사키 - [완다 나오토](%EC%99%84%EB%8B%A4%20%EB%82%98%EC%98%A4%ED%86%A0.md) \- [나미카와 렌스케](%EB%82%98%EB%AF%B8%EC%B9%B4%EC%99%80%20%EB%A0%8C%EC%8A%A4%EC%BC%80.md)
    * [이나즈마 일레븐 GO 크로노 스톤](%EC%9D%B4%EB%82%98%EC%A6%88%EB%A7%88%20%EC%9D%BC%EB%A0%88%EB%B8%90%20GO%20%ED%81%AC%EB%A1%9C%EB%85%B8%20%EC%8A%A4%ED%86%A4.md) : [알파(Alpha(= **R**-pha))](%EC%95%8C%ED%8C%8C%28%EC%9D%B4%EB%82%98%EC%A6%88%EB%A7%88%20%EC%9D%BC%EB%A0%88%EB%B8%90%20GO%29.md) \- [감마(**G**amma)](%EA%B0%90%EB%A7%88%28%EC%9D%B4%EB%82%98%EC%A6%88%EB%A7%88%20%EC%9D%BC%EB%A0%88%EB%B8%90%20GO%29.md) \- [베타(**B**eta)](%EB%B2%A0%ED%83%80%28%EC%9D%B4%EB%82%98%EC%A6%88%EB%A7%88%20%EC%9D%BC%EB%A0%88%EB%B8%90%20GO%29.md)
    * [이나즈마 일레븐 GO 갤럭시](%EC%9D%B4%EB%82%98%EC%A6%88%EB%A7%88%20%EC%9D%BC%EB%A0%88%EB%B8%90%20GO%20%EA%B0%A4%EB%9F%AD%EC%8B%9C.md) : [노자키 사쿠라](%EB%85%B8%EC%9E%90%ED%82%A4%20%EC%82%AC%EC%BF%A0%EB%9D%BC.md) \- [모리무라 코노하](%EB%AA%A8%EB%A6%AC%EB%AC%B4%EB%9D%BC%20%EC%BD%94%EB%85%B8%ED%95%98.md) \- [소라노 아오이](%EC%86%8C%EB%9D%BC%EB%85%B8%20%EC%95%84%EC%98%A4%EC%9D%B4.md)
  * [용자 시리즈](%EC%9A%A9%EC%9E%90%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md)  

    * [용자특급 마이트가인](%EC%9A%A9%EC%9E%90%ED%8A%B9%EA%B8%89%20%EB%A7%88%EC%9D%B4%ED%8A%B8%EA%B0%80%EC%9D%B8.md)  

      * [범버즈](%EB%B2%94%EB%B2%84%EC%A6%88.md) : 버드 범버 - 라이오 범버 - 다이노 범버
    * [황금용자 골드란](%ED%99%A9%EA%B8%88%EC%9A%A9%EC%9E%90%20%EA%B3%A8%EB%93%9C%EB%9E%80.md) : 하라시마 타쿠야(팽이) - 스가누마 다이(바우) - 토키무라 카즈키(솔개)
    * [용자지령 다그온](%EC%9A%A9%EC%9E%90%EC%A7%80%EB%A0%B9%20%EB%8B%A4%EA%B7%B8%EC%98%A8.md) : [다이도우지 엔](%EB%8B%A4%EC%9D%B4%EB%8F%84%EC%9A%B0%EC%A7%80%20%EC%97%94.md) \- [사와무라 신](%EC%82%AC%EC%99%80%EB%AC%B4%EB%9D%BC%20%EC%8B%A0.md) \- [히로세 카이](%ED%9E%88%EB%A1%9C%EC%84%B8%20%EC%B9%B4%EC%9D%B4.md)
    * [용자왕 가오가이가](%EC%9A%A9%EC%9E%90%EC%99%95%20%EA%B0%80%EC%98%A4%EA%B0%80%EC%9D%B4%EA%B0%80.md) : [염룡](%EC%97%BC%EB%A3%A1.md) \- [풍룡](%ED%92%8D%EB%A3%A1.md) \- [빙룡](%EB%B9%99%EB%A3%A1.md)
  * [충격 고우라이간](%EC%B6%A9%EA%B2%A9%20%EA%B3%A0%EC%9A%B0%EB%9D%BC%EC%9D%B4%EA%B0%84.md) : [고우](%EA%B4%91%EC%9D%B8%20%EA%B3%A0%EC%9A%B0.md) \- [게키](%EA%B4%91%EC%9D%B8%20%EA%B2%8C%ED%82%A4.md) \- [간](%EA%B4%91%EC%9D%B8%20%EA%B0%84.md)
  * [캐릭캐릭 체인지](%EC%BA%90%EB%A6%AD%EC%BA%90%EB%A6%AD%20%EC%B2%B4%EC%9D%B8%EC%A7%80.md) : [란](%EB%9E%80%28%EC%88%98%ED%98%B8%EC%BA%90%EB%A6%AD%ED%84%B0%29.md) \- [수우](%EC%88%98%EC%9A%B0.md) \- [미키](%EB%AF%B8%ED%82%A4%28%EC%88%98%ED%98%B8%EC%BA%90%EB%A6%AD%ED%84%B0%29.md)
  * [케이온!](%EC%BC%80%EC%9D%B4%EC%98%A8%21.md) : [히라사와 유이](%ED%9E%88%EB%9D%BC%EC%82%AC%EC%99%80%20%EC%9C%A0%EC%9D%B4.md) \- [나카노 아즈사](%EB%82%98%EC%B9%B4%EB%85%B8%20%EC%95%84%EC%A6%88%EC%82%AC.md) \- [아키야마 미오](%EC%95%84%ED%82%A4%EC%95%BC%EB%A7%88%20%EB%AF%B8%EC%98%A4.md)
  * [크로스 앙쥬 천사와 용의 윤무](%ED%81%AC%EB%A1%9C%EC%8A%A4%20%EC%95%99%EC%A5%AC%20%EC%B2%9C%EC%82%AC%EC%99%80%20%EC%9A%A9%EC%9D%98%20%EC%9C%A4%EB%AC%B4.md) : [사라만디네](%EC%82%AC%EB%9D%BC%EB%A7%8C%EB%94%94%EB%84%A4.md) \- [카나메](%EC%B9%B4%EB%82%98%EB%A9%94%28%ED%81%AC%EB%A1%9C%EC%8A%A4%20%EC%95%99%EC%A5%AC%20%EC%B2%9C%EC%82%AC%EC%99%80%20%EC%9A%A9%EC%9D%98%20%EC%9C%A4%EB%AC%B4%29.md) \- [나가](%EB%82%98%EA%B0%80%28%ED%81%AC%EB%A1%9C%EC%8A%A4%20%EC%95%99%EC%A5%AC%20%EC%B2%9C%EC%82%AC%EC%99%80%20%EC%9A%A9%EC%9D%98%20%EC%9C%A4%EB%AC%B4%29.md)
  * [토리코](%ED%86%A0%EB%A6%AC%EC%BD%94.md)   

    * **[써니](%EC%8D%A8%EB%8B%88%28%ED%86%A0%EB%A6%AC%EC%BD%94%29.md) \- [써니](%EC%8D%A8%EB%8B%88%28%ED%86%A0%EB%A6%AC%EC%BD%94%29.md) \- [써니](%EC%8D%A8%EB%8B%88%28%ED%86%A0%EB%A6%AC%EC%BD%94%29.md)** <del>고만해 미친머리야!</del>
    * [제브라](%EC%A0%9C%EB%B8%8C%EB%9D%BC%28%ED%86%A0%EB%A6%AC%EC%BD%94%29.md) \- [코코](%EC%BD%94%EC%BD%94%28%ED%86%A0%EB%A6%AC%EC%BD%94%29.md)(두건) - [토리코](%ED%86%A0%EB%A6%AC%EC%BD%94%28%ED%86%A0%EB%A6%AC%EC%BD%94%29.md)
  * [파워퍼프걸](%ED%8C%8C%EC%9B%8C%ED%8D%BC%ED%94%84%EA%B1%B8.md) : [블로섬](%EB%B8%94%EB%A1%9C%EC%84%AC.md) \- [버터컵](%EB%B2%84%ED%84%B0%EC%BB%B5.md) \- [버블스](%EB%B2%84%EB%B8%94%EC%8A%A4.md)  

    * [파워퍼프걸Z](%ED%8C%8C%EC%9B%8C%ED%8D%BC%ED%94%84%EA%B1%B8Z.md) : [아카즈츠미 모모코](%EC%95%84%EC%B9%B4%EC%A6%88%EC%B8%A0%EB%AF%B8%20%EB%AA%A8%EB%AA%A8%EC%BD%94.md) \- [마츠바라 카오루](%EB%A7%88%EC%B8%A0%EB%B0%94%EB%9D%BC%20%EC%B9%B4%EC%98%A4%EB%A3%A8.md) \- [고토쿠지 미야코](%EA%B3%A0%ED%86%A0%EC%BF%A0%EC%A7%80%20%EB%AF%B8%EC%95%BC%EC%BD%94.md)
  * [포켓몬스터](%ED%8F%AC%EC%BC%93%EB%AA%AC%EC%8A%A4%ED%84%B0.md) : 불꽃 타입 - 풀 타입 - 물 타입  

    * [포켓몬스터 적/녹/청](%ED%8F%AC%EC%BC%93%EB%AA%AC%EC%8A%A4%ED%84%B0%20%EC%A0%81/%EB%85%B9.md) : **제목 자체**, [파이리](%EB%A6%AC%EC%9E%90%EB%AA%BD.md) \- [이상해씨](%EC%9D%B4%EC%83%81%ED%95%B4%EA%BD%83.md) \- [꼬부기](%EA%B1%B0%EB%B6%81%EC%99%95.md)
    * [포켓몬스터 금/은/크리스탈](%ED%8F%AC%EC%BC%93%EB%AA%AC%EC%8A%A4%ED%84%B0%20%EA%B8%88/%EC%9D%80.md) : [브케인](%EB%B8%94%EB%A0%88%EC%9D%B4%EB%B2%94.md) \- [치코리타](%EB%A9%94%EA%B0%80%EB%8B%88%EC%9B%80.md) \- [리아코](%EC%9E%A5%ED%81%AC%EB%A1%9C%EB%8B%A4%EC%9D%BC.md)
    * [포켓몬스터 루비/사파이어/에메랄드](%ED%8F%AC%EC%BC%93%EB%AA%AC%EC%8A%A4%ED%84%B0%20%EB%A3%A8%EB%B9%84/%EC%82%AC%ED%8C%8C%EC%9D%B4%EC%96%B4.md)  

      * [아차모](%EB%B2%88%EC%B9%98%EC%BD%94.md) \- [나무지기](%EB%82%98%EB%AC%B4%ED%82%B9.md) \- [물짱이](%EB%8C%80%EC%A7%B1%EC%9D%B4.md)
      * [그란돈](%EA%B7%B8%EB%9E%80%EB%8F%88.md) \- [레쿠쟈](%EB%A0%88%EC%BF%A0%EC%9F%88.md) \- [가이오가](%EA%B0%80%EC%9D%B4%EC%98%A4%EA%B0%80.md)
    * [포켓몬스터 디아루가/펄기아/기라티나](%ED%8F%AC%EC%BC%93%EB%AA%AC%EC%8A%A4%ED%84%B0%20DP%20%EB%94%94%EC%95%84%EB%A3%A8%EA%B0%80/%ED%8E%84%EA%B8%B0%EC%95%84.md) : [불꽃숭이](%EC%B4%88%EC%97%BC%EB%AA%BD.md) \- [모부기](%ED%86%A0%EB%8C%80%EB%B6%80%EA%B8%B0.md) \- [팽도리](%EC%97%A0%ED%8E%98%EB%A5%B4%ED%8A%B8.md)
    * [포켓몬스터 블랙/화이트](%ED%8F%AC%EC%BC%93%EB%AA%AC%EC%8A%A4%ED%84%B0%20%EB%B8%94%EB%9E%99/%ED%99%94%EC%9D%B4%ED%8A%B8.md)   

      * [뚜꾸리](%EC%97%BC%EB%AC%B4%EC%99%95.md) \- [주리비얀](%EC%83%A4%EB%A1%9C%EB%8B%A4.md) \- [수댕이](%EB%8C%80%EA%B2%80%EA%B7%80.md)
      * [팟](%ED%8C%9F%28%ED%8F%AC%EC%BC%93%EB%AA%AC%EC%8A%A4%ED%84%B0%29.md) \- [덴트](%EB%8D%B4%ED%8A%B8%28%ED%8F%AC%EC%BC%93%EB%AA%AC%EC%8A%A4%ED%84%B0%29.md) \- [콘](%EC%BD%98%28%ED%8F%AC%EC%BC%93%EB%AA%AC%EC%8A%A4%ED%84%B0%29.md)
      * [바오프](%EB%B0%94%EC%98%A4%ED%82%A4.md) \- [야나프](%EC%95%BC%EB%82%98%ED%82%A4.md) \- [앗차프](%EC%95%97%EC%B0%A8%ED%82%A4.md)
    * [포켓몬스터 SPECIAL](%ED%8F%AC%EC%BC%93%EB%AA%AC%EC%8A%A4%ED%84%B0%20SPECIAL.md) : [레드](%EB%A0%88%EB%93%9C%28%ED%8F%AC%EC%BC%93%EB%AA%AC%EC%8A%A4%ED%84%B0%20SPECIAL%29.md) \- [그린](%EA%B7%B8%EB%A6%B0%28%ED%8F%AC%EC%BC%93%EB%AA%AC%EC%8A%A4%ED%84%B0%20SPECIAL%29.md) \- [블루](%EB%B8%94%EB%A3%A8%28%ED%8F%AC%EC%BC%93%EB%AA%AC%EC%8A%A4%ED%84%B0%20SPECIAL%29.md)
  * [푸른 유성 SPT 레이즈너](%ED%91%B8%EB%A5%B8%20%EC%9C%A0%EC%84%B1%20SPT%20%EB%A0%88%EC%9D%B4%EC%A6%88%EB%84%88.md) : 베이불 - 벌디 - [레이즈너](%EB%A0%88%EC%9D%B4%EC%A6%88%EB%84%88.md)
  * [프리큐어 시리즈](%ED%94%84%EB%A6%AC%ED%81%90%EC%96%B4%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md)  

    * [Yes! 프리큐어 5](Yes%21%20%ED%94%84%EB%A6%AC%ED%81%90%EC%96%B4%205.md) : [나츠키 린](%EB%82%98%EC%B8%A0%ED%82%A4%20%EB%A6%B0.md) \- [아키모토 코마치](%EC%95%84%ED%82%A4%EB%AA%A8%ED%86%A0%20%EC%BD%94%EB%A7%88%EC%B9%98.md) \- [미나즈키 카렌](%EB%AF%B8%EB%82%98%EC%A6%88%ED%82%A4%20%EC%B9%B4%EB%A0%8C.md)
    * [스위트 프리큐어♪](%EC%8A%A4%EC%9C%84%ED%8A%B8%20%ED%94%84%EB%A6%AC%ED%81%90%EC%96%B4%E2%99%AA.md) : [트리오 더 마이너](%ED%8A%B8%EB%A6%AC%EC%98%A4%20%EB%8D%94%20%EB%A7%88%EC%9D%B4%EB%84%88.md) ([팔세토](%ED%8C%94%EC%84%B8%ED%86%A0.md) \- [바스도라](%EB%B0%94%EC%8A%A4%EB%8F%84%EB%9D%BC.md) \- [바리톤](%EB%B0%94%EB%A6%AC%ED%86%A4.md))
    * [스마일 프리큐어!](%EC%8A%A4%EB%A7%88%EC%9D%BC%20%ED%94%84%EB%A6%AC%ED%81%90%EC%96%B4%21.md)  

      * [히노 아카네](%ED%9E%88%EB%85%B8%20%EC%95%84%EC%B9%B4%EB%84%A4%28%EC%8A%A4%EB%A7%88%EC%9D%BC%20%ED%94%84%EB%A6%AC%ED%81%90%EC%96%B4%21%29.md) \- [미도리카와 나오](%EB%AF%B8%EB%8F%84%EB%A6%AC%EC%B9%B4%EC%99%80%20%EB%82%98%EC%98%A4.md) \- [아오키 레이카](%EC%95%84%EC%98%A4%ED%82%A4%20%EB%A0%88%EC%9D%B4%EC%B9%B4.md)
      * [아카오니](%EC%95%84%EC%B9%B4%EC%98%A4%EB%8B%88.md) \- [마조리나](%EB%A7%88%EC%A1%B0%EB%A6%AC%EB%82%98.md) \- [울프룬](%EC%9A%B8%ED%94%84%EB%A3%AC.md)
  * [Free!](Free%21.md) : [마츠오카 린](%EB%A7%88%EC%B8%A0%EC%98%A4%EC%B9%B4%20%EB%A6%B0.md) \- [타치바나 마코토](%ED%83%80%EC%B9%98%EB%B0%94%EB%82%98%20%EB%A7%88%EC%BD%94%ED%86%A0.md) \- [나나세 하루카](%EB%82%98%EB%82%98%EC%84%B8%20%ED%95%98%EB%A3%A8%EC%B9%B4.md)  

[[edit](http://rigvedawiki.net/r1/wiki.php/RGB?action=edit&section=4)]

## 3. 관련 항목 ¶

  * [색](%EC%83%89.md)
  * [CMYK](CMYK.md)
  * [HSB](HSB.md)
  * [Lab](Lab.md)
  * [게이지 보존](%EA%B2%8C%EC%9D%B4%EC%A7%80%20%EB%B3%B4%EC%A1%B4.md)

`\----`

  * `[1]` 보라색이 섞인 붉은색이다. 여기서 파란색과 빨간색의 밝기를 동시에 낮추면 [보라색](%EB%B3%B4%EB%9D%BC%EC%83%89.md)이 나온다.
  * `[2]` 이것은 일반적인 가시광선에서 녹색의 영역이 넓기 때문이다.
  * `[3]` 팬텀의 간부의 상징색이 옷 색깔임을 알 수 있음으로. 단 메두사가 팬텀화가 되었을 때 색깔은 파란색이 아니라 보라색이다.
  * `[4]` 클래식 및 V 계열 한정. [XG](%EA%B8%B0%ED%83%80%ED%94%84%EB%A6%AD%EC%8A%A4%26%EB%93%9C%EB%9F%BC%EB%A7%A4%EB%8B%88%EC%95%84%20XG.md)에서는 Y-옐로,P-퍼플이 추가되었다.
  * `[5]` 상징색으로 따지면 배열은 이게 맞으나 어째 미도리 쪽이 더 빨간색인 것 같다. 자세한 건 항목 참조.

