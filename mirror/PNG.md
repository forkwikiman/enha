## Contents

    

1. 그림 파일 형식 
    

1.1. 뜻

1.2. 탄생 배경

1.3. 특징

1.4. 변형 파일 형식

1.5. 그 외

2. [ISO](ISO.md) 코드 
3. Persona Non Grata 

[[edit](http://rigvedawiki.net/r1/wiki.php/PNG?action=edit&section=1)]

## 1. 그림 파일 형식 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/PNG?action=edit&section=2)]

### 1.1. 뜻 ¶

**P**ortable **N**etwork **G**raphics의 약자로 [그림](%EA%B7%B8%EB%A6%BC.md) [파일형식](%ED%8C%8C%EC%9D%BC%ED%98%95%EC%8B%9D.md) 중 하나이다.

  

PNG는 [무손실 압축 포맷](%EB%AC%B4%EC%86%90%EC%8B%A4%20%EC%95%95%EC%B6%95%20%ED%8F%AC%EB%A7%B7.md)을 채택하였으며, 256색에 한정되던 GIF의 한계를 극복하여 32비트 트루컬러(알파채널, RGB에 각 8비트
지원)를 표현할 수 있게 되었다. 다만 네이티브 PNG는 GIF에서 제공하던 애니메이션 기능은 제공하지 못한다.

  

더불어 [GIF](GIF.md)가 제공하던 '투명 배경'은 이 형식에서도 지원된다. 엄밀히 말하자면 GIF는 특정색 한가지만 투명으로
지정하는 방법이고, PNG는 알파채널을 포함해서 완벽하게 불투명도를 지정할 수 있다. [인터넷 익스플로러](%EC%9D%B8%ED%84%B0%EB%84%B7%20%EC%9D%B5%EC%8A%A4%ED%94%8C%EB%A1%9C%EB%9F%AC.md)는 6까진 이 알파채널을
제대로 지원하지 않아 사용에 걸림돌이 되었으나`[1]` 이후 버전은 정상적으로 지원한다.

  

[JPEG](JPEG.md)가 '제이펙'으로 불리는것처럼 [PNG](PNG.md)는 '핑'이라고 불린다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/PNG?action=edit&section=3)]

### 1.2. 탄생 배경 ¶

PNG의 탄생배경은 [MP3](MP3.md)에 적용된 특허권을 피하기 위해 [OGG](Ogg%20Vorbis.md)가 개발된 것과
동일하다. 초창기 인터넷에서 그림파일들은 컴퓨서브(CompuServ)사에서 개발한 [GIF](GIF.md) 형식을 사용하고 있었다.
하지만 GIF의 핵심이 되는 LZW 알고리즘에 대하여 유니시스(Unisys)사에서 특허권을 취득하고 그 권한을 행사하기 시작하자,
프로그래머들은 이참에 GIF의 몇가지 문제점들을 해결하는 셈치고 새로운 그림 파일형식을 개발하기 시작하였고 1996년에 PNG가 발표되었다.

  

하지만 개발을 하고 발표를 했어도 초창기에는 크게 인기를 얻지 못했는데, 이유는 LZW 알고리즘에 대하여 비상용 소프트웨어의 경우에는 무료
특허 정책을 적용하여 GIF를 계속 사용할 수 있었기 때문이다. 또한 압축율이 높은 만큼 당시 컴퓨터 스펙으로는 GIF에 비해 처리속도가
느리기도 했다. [H.264](H.26x.md) 규격이 나올 당시 좌절영상이 왜 많았는지를 떠올려 보면 답이 나온다.

  

하지만 1999년에 이 정책이 폐기되면서 소프트웨어 개발자들이 대안을 찾기 시작했고, 이에 따라 PNG를 지원하는 프로그램도 점점
증가하였다. 현재는 W3C에서 표준안이 나오고([W3C 표준](http://www.w3.org/TR/PNG/)),
[ISO](ISO.md) 표준 규격([ISO 15948](http://www.iso.org/iso/iso_catalogue/catalo
gue_tc/catalogue_detail.htm?csnumber=29581), [한국어
설명](https://www.kssn.net/StdKS/KS_detail.asp?k1=X&k2=ISO/IEC%2015948&k3=1))이
나왔을 정도로 보편적인 그림파일 형식으로 자리잡은 상태다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/PNG?action=edit&section=4)]

### 1.3. 특징 ¶

등장 초기에는 같은 그림을 PNG로 압축할 경우 GIF보다 훨씬 큰 파일을 만든다고 불평을 늘어놓는 경향이 있었는데, 사실 이는 256색만
지원하는 GIF와 32비트 컬러를 지원할 수 있는 PNG의 차이 때문이다. 그리고
[어도비](%EC%96%B4%EB%8F%84%EB%B9%84.md)사의 제품이 PNG 파일에 독특한 메타데이터를 붙인다거나,
[포토샵](%ED%8F%AC%ED%86%A0%EC%83%B5.md) 구버전들이 PNG 형식의 압축 알고리즘을 잘 구현하지 못했던 까닭에
충분한 압축 효율을 발휘하지 못했던 영향도 있다. 물론 이러한 문제는 일찍이 해결되었다.`[2]`

  

[무손실 압축 포맷](%EB%AC%B4%EC%86%90%EC%8B%A4%20%EC%95%95%EC%B6%95%20%ED%8F%AC%EB%A7%B7.md)임에도 다른 무손실 포맷인 [BMP](BMP.md)·[PCX](PCX.md)·TGA 등에 비해 압축 효율이 좋은
편이어서, 사진에서 [raw](RAW%28%ED%8C%8C%EC%9D%BC%29.md) 파일을 보관할 때 이미지가 전체적으로 뭉개지는
[JPEG](JPEG.md)나 256색의 한계로 모든 것을 표현하지 못하는 [GIF](GIF.md)보다 PNG 형식을 선호하는
사람들도 있을 수는 있겠지만 PNG는 일단 [EXIF](EXIF.md)를 지원하지 못하므로 사진에는 잘 쓰이지 않는다. TIFF의 경우
LZW 알고리즘을 사용한다면 PNG와 용량이 비슷한데다 EXIF도 지원하고, [포토샵 라이트룸](%ED%8F%AC%ED%86%A0%EC%83%B5%20%EB%9D%BC%EC%9D%B4%ED%8A%B8%EB%A3%B8.md) 같이 48비트 컬러와 Prophoto RGB 같은
넓은 색공간으로 저장하는 프로그램이 많으므로 사진에서 후보정을 염두에 둔다면 거의 EXIF-TIFF 포맷을 사용하게 된다.

  

다만 과거 대부분의 웹사이트에서 업로드 할 수 있는 용량을 아주 낮게 설정해둔 경우가 많았는데, 이 경우 PNG로 압축을 할 경우 용량을
초과하는 경우가 허다했다. 현재도 그러한 경향이 남아 있기 때문에 웹상에서의 그림은 PNG 형식보다는 JPG의 비중이 더 높은 편이다. 특히
사진 같은 경우는 JPG로 어느정도 손실압축해도 그 변화를 알아차리기 힘들기 때문에 큰 문제없이 쓰인다.

  

압축 프로그램에서 사용되는 [Deflate](Deflate.md) 알고리즘을 사용하기 때문에 그 자체로 고성능 압축파일이나 마찬가지.
패턴이 반복되거나 단순한 형태의 파일을 압축할 경우 경이로운 압축률을 볼 수 있다. 지형 분석에 사용되는 고도 높이맵 데이터라든가, 게시판의
글을 캡쳐한 경우라든가.

  

웹에서 이미지에 반투명을 사용할 경우 거의 유일한 방법이다. JPG는 투명이 아예 안되고, GIF는 투명이 되지만 반투명은 안 되기
때문이다. PNG가 대중화되기 전에는 GIF의 투명기법을 사용해서 [1픽셀씩 건너서 투명과 불투명을 반복하는기법](%EC%A0%90%EB%AC%98%EB%B2%95.md)을 써서 반투명을 표현했다. 또한 원래 배경과 어우러지게 배경을
투명처리한 이미지를 배치할 때도 GIF보다 PNG가 좋다. GIF는 한 색만 투명처리되기 때문에 [도트노가다](%EB%8F%84%ED%8A%B8%20%EB%85%B8%EA%B0%80%EB%8B%A4.md)를 하지 않는 이상 필연적으로
계단 현상이 생길 수밖에 없지만, PNG는 256단계의 투명 단계(알파 채널)를 지원하기 때문에 계단 현상이 생기지 않는다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/PNG?action=edit&section=5)]

### 1.4. 변형 파일 형식 ¶

형제뻘로 애니메이션 기능을 지원하는 MNG, JPEG 압축 기능을 지원하는 JNG이 있지만 지원하는 프로그램이 적어 거의 이용되지 않는다.
구조적으로 매우 복잡해서 지원을 거의 안 한다고. 좀 더 간단하고 하위호환성도 있는(애니메이션 기능을 지원 안 해도 정지 영상은 보인다)
APNG(Animated PNG)라는 것도 있는데 공식 규격은 아니다. 표준안을 지원했지만 퇴짜맞았다.

  

![http://cfs8.tistory.com/original/15/tistory/2008/08/19/18/35/48aa93f4a69eb&f
ilename=firefox_spinfox.PNG](http://cfs8.tistory.com/original/15/tistory/2008/
08/19/18/35/48aa93f4a69eb&filename=firefox_spinfox.PNG)

[[PNG external image]](http://cfs8.tistory.com/original/15/tistory/2008/08/19/
18/35/48aa93f4a69eb&filename=firefox_spinfox.PNG)

  
위의 파이어폭스 이미지가 APNG다. 표준이 아니기에 모든 브라우저에서 움직이지는 않으며 다른 브라우저에서는 정지된 것만 보인다. (오페라
클래식 9.5, [파이어폭스](%ED%8C%8C%EC%9D%B4%EC%96%B4%ED%8F%AD%EC%8A%A4.md) 3 이상만
움직임) 지원하는 브라우저에서는 <del>폭스스핀</del>파이어폭스가 회전하는 것을 볼 수 있다. 구글 크롬에서는 플러그인을 사용해서 사용
가능하다. OS X과iOS 8에 탑재된 사파리에서는 잘 보인다. 일반 이미지 뷰어중에서는
[꿀뷰](%EA%BF%80%EB%B7%B0.md)가 5.10 버전부터 APNG 를 지원한다.

[[edit](http://rigvedawiki.net/r1/wiki.php/PNG?action=edit&section=6)]

### 1.5. 그 외 ¶

[동방탄막풍](%EB%8F%99%EB%B0%A9%ED%83%84%EB%A7%89%ED%92%8D.md)에서 유일하게 지원하는 그림
확장자이기도 하다.

  

[RPG 쯔꾸르 2000](RPG%20%EC%AF%94%EA%BE%B8%EB%A5%B4%202000.md), [RPG 쯔꾸르2003](RPG%20%EC%AF%94%EA%BE%B8%EB%A5%B4%202003.md)에서도 유일하게 지원한다.(그 이후 출시된
툴은 JPEG도 지원.)

  

[오에카키](%EC%98%A4%EC%97%90%EC%B9%B4%ED%82%A4.md)에서 사용하는 파일 포맷이기도 하다.

  

디지털 영사기에서 사용하는 [자막](%EC%9E%90%EB%A7%89.md)을 이 파일로 만들기도 한다. 디지털 영화인데 타이틀을 고유
글꼴로 만들었다면 100% 이 방식이라고 보면 된다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/PNG?action=edit&section=7)]

## 2. [ISO](ISO.md) 코드 ¶

[파푸아뉴기니](%ED%8C%8C%ED%91%B8%EC%95%84%EB%89%B4%EA%B8%B0%EB%8B%88.md)(**P**ap
ua **N**ew **G**uinea)의 [ISO 3166](ISO%203166.md)-1 코드(3자리). 2자리는 PG이다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/PNG?action=edit&section=8)]

## 3. Persona Non Grata ¶

기피인물. 자신의 나라에 주재하는 외교관을 무이유부로 거부하고 싶을때 선언한다.

  

`\----`

  * `[1]` 자바스크립트를 이용하여 인식시키는 방법이 있지만 웹브라우저가 많이 느려지는 단점이 있다.
  * `[2]` 그런데 최신 버전인 CC 2014에서 PNG로 일반 저장시 파일 크기가 비정상적으로 커지는 버그가 있으며 아직까지도 고쳐지지 않았다(...) 웹용으로 저장은 이런 현상이 없다는 것이 천만다행.

