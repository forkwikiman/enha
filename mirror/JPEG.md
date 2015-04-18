## Contents

    

1. 뜻 
2. 특징 
    

2.1. 정보 손실

2.2. 작은 용량

2.3. 이중 압축

2.4. 순차 주사

2.5. Motion JPEG

3. 유용한 웹 사이트 
4. 그 외 
    

4.1. 웹 문화

[[edit](http://rigvedawiki.net/r1/wiki.php/JPEG?action=edit&section=1)]

## 1. 뜻 ¶

Joint Photograph Experts Group의 약자로 [그림](%EA%B7%B8%EB%A6%BC.md) [파일형식](%ED%99%95%EC%9E%A5%EC%9E%90.md) 중 하나.

  

정지 화상을 위해서 만들어진 손실 압축, 무손실 압축(JPEG 9.1부터) 방법 표준이다. 이 표준은 [ISO](ISO.md)와
ITU-T에서 제정하였다.([ISO 10918-1](http://www.iso.org/iso/iso_catalogue/catalogue_tc
/catalogue_detail.htm?csnumber=10918), [한국어 설명](https://www.kssn.net/StdKS/KS_
detail.asp?k1=X&k2=ISO/IEC%2010918-1_2001&k3=1))

  

JPEG를 사용하는 파일 형식들도 보통 JPEG 이미지라 불리며, .jpg, .jpeg, .jpe 등의
[확장자](%ED%99%95%EC%9E%A5%EC%9E%90.md)를 사용한다.

  

JPEG 표준은 이미지가 어떻게 연속된 바이트로 바뀌는 지만을 규정한다. 독립 JPEG 그룹(Independent JPEG Group;
IJG)에서 만든 JPEG의 확장인 JFIF(JPEG File Interchange Format)는 JPEG 스트림을 저장과 전송에 적합한
형태로 담는 이미지 파일 형식이다. [디지털카메라](%EB%94%94%EC%A7%80%ED%84%B8%20%EC%B9%B4%EB%A9%94%EB%9D%BC.md)의 사진 저장
방식으로는 다른 확장인 EXIF JPEG 형식이 더 자주 사용된다. 일반적으로 JPEG 파일이라고 할 때는 JFIF 형식이거나 EXIF
JPEG 형식을 가리키지만, JNG와 같은 JPEG 기반의 다른 파일 형식도 존재한다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/JPEG?action=edit&section=2)]

## 2. 특징 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/JPEG?action=edit&section=3)]

### 2.1. 정보 손실 ¶

JPEG/JFIF는 웹 상에서 사진 등의 화상을 보관하고 전송하는 데 가장 널리 사용되는 파일 형식이다. 압축 과정은 YIQ모델로 변환 →
Macroblock화 → 8×8블록화 → DCT변환 → 양자화`[1]` → 지그재그 스캐닝 → 엔트로피 코딩의 단계를 거친다. 이 중에서
**양자화 과정이 유일하게 되돌릴 수 없는 과정**으로, 이 과정에서 일부 데이터가 소실된다. 때문에 이 압축 방법은 인물이나 풍경 사진에는
쓸만할지 몰라도, 문자, 선, 세밀한 격자 등 고주파 성분이 많은 이미지의 변환에서는 [GIF](GIF.md)나
[PNG](PNG.md)에 비해 불리하며, 나쁜 품질을 보이는 경우가 많다. JPEG 표준에도 비손실 압축 방법이 정의되어 있지만 특허
문제와 압축률 등의 이유로 잘 사용되지는 않으며, 비손실 압축 형식을 쓰려는 사람은 [PNG](PNG.md) 등의 비손실 압축을
지원하는 포맷을 많이 사용한다.

  

[사진](%EC%82%AC%EC%A7%84.md)을 압축할 목적으로 개발한
[알고리즘](%EC%95%8C%EA%B3%A0%EB%A6%AC%EC%A6%98.md)이기 때문에 복잡한 패턴과 색상이 포함될수록 손실을
[눈](%EB%88%88.md)으로 감지하기 어려워진다. 쉬운 예로 단색이나 뚜렷한 윤곽선을 가지는 그래픽을 JPEG 압축하면 색이
뭉개지며 흩뿌려지거나 윤곽선 주위에 노이즈가 낀다.

  

**과감하게** 손실시키면서 압축하기 때문에 [그림판](%EA%B7%B8%EB%A6%BC%ED%8C%90.md)에서 [BMP](BMP.md)나 [GIF](GIF.md) 확장자 파일을 이 포맷으로 재저장하면 아름답게 도트가 뭉개지고 색이 갈변하는 것을 볼 수 있다.(...)`[2]` 그리고 [DSLR](DSLR.md)을 사용하는 사람들은 JPEG보다는 [raw](RAW%28%ED%8C%8C%EC%9D%BC%29.md) 이미지를 사용하고, 인쇄 출판 계통쪽 사람들은 [TIFF](TIFF.md), [EPS](EPS.md) 확장자를 많이 쓰는 편. JPEG로 저장할 때 최상 퀄리티로 설정해두면 그만큼 압축률은 떨어지지만 손실도 적어지는데, 아무리 높은 퀄리티로 해도 손실이 없어지진 않는다. 

  

JPEG를 쓸 때 빨간색이 들어가는 이미지라면 다른 포맷을 쓰는 것이 좋다. 빨간색이 특히 잘 무너진다.

  

JPEG로 저장된 파일을 불러와서 편집하고, 다시 JPEG 형식으로 저장하면 그림이 한 층 더 뭉개진다(…). 따라서 JPEG로 그림을
보관하는 경우에는 편집을 대비해서 원본을 별도로 보관할 필요가 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/JPEG?action=edit&section=4)]

### 2.2. 작은 용량 ¶

작은 용량 덕분에 각종 웹 사이트들이 가장 좋아하는 업로드 확장자중 하나이다. 특히 대부분 국내 웹 사이트들은 이미지 업로드시 강제적으로
JPEG나 GIF 혹은 PNG 형식 파일만 업로드 하게 지정해놓고 있다. 이유는 딱 하나. 용량이 작으니까.`[3]` 그 중에서도 JPG
확장자를 제일 선호하는듯 싶다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/JPEG?action=edit&section=5)]

### 2.3. 이중 압축 ¶

손실 압축을 하는데도, 한 번 더 (무손실)압축할 수 있는 프로그램이 있다. ([Winzip](Winzip.md),
[Stuffit](Stuffit.md), [PackJPG](PackJPG.md)) 단, 고유 파일형식을 사용하기 때문에 똑같은
프로그램이 없으면 압축 해제가 안된다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/JPEG?action=edit&section=6)]

### 2.4. 순차 주사 ¶

순차 주사(Progressive)를 지원한다. 이걸 쓸 경우 웹상에서 로딩 방식이 달라지고`[4]`
[포토샵](%ED%8F%AC%ED%86%A0%EC%83%B5.md) 기준으로 파일 용량이 10%가량 줄어드는 장점이 있다. 다만 저장할
때마다 세팅을 일일이 해야 하는 귀찮음이 있다(...)

  

[[edit](http://rigvedawiki.net/r1/wiki.php/JPEG?action=edit&section=7)]

### 2.5. Motion JPEG ¶

이 JPEG 기술을 이용해서 나온 [동영상](%EB%8F%99%EC%98%81%EC%83%81.md) 파일 포맷이 Motion
JPEG로, [퀵타임 플레이어](%ED%80%B5%ED%83%80%EC%9E%84%20%ED%94%8C%EB%A0%88%EC%9D%B4%EC%96%B4.md)에서 처음 채용했다. MPEG과는 달리, 여러 프레임간 압축을 하지 않기 때문에 MPEG보다 더 용량이 높다.

  

의외로 여러 군데서 쓰였는데, [플레이스테이션](%ED%94%8C%EB%A0%88%EC%9D%B4%EC%8A%A4%ED%85%8C%EC%9D%B4%EC%85%98.md)의 동영상 포맷으로 사용되었으며, 현재 극장용 디지털 영화 포맷으로 사용되고 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/JPEG?action=edit&section=8)]

## 3. 유용한 웹 사이트 ¶

만일 JPEG로 인한 화질 저하가 없으면서, 파일 용량을 줄이길 원한다면 <http://www.jpegmini.com> 이 사이트에서
변환하면 된다. 사진 크기나 기타 다른 변환 없이 용량만 줄여준다. 다만, 업로드 시 JPEG 확장자만 지원한다. <del>그 말인 즉슨,
변환 할 파일도 이미 화질을 손실해버릴 수밖에 없는 의미..?!</del>

  

위 사이트랑은 정반대로, 화질이 손실되는 확장자라는 걸 조크로 삼아 이미지 화질을 확 내리는 [needs more
jpeg](http://needsmorejpeg.com/) 라는 사이트도 존재한다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/JPEG?action=edit&section=9)]

## 4. 그 외 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/JPEG?action=edit&section=10)]

### 4.1. 웹 문화 ¶

  * [Dcinside](Dcinside.md)에선 주로 [jyp](%EB%B0%95%EC%A7%84%EC%98%81.md) 혹은 jp[gee](gee.md)라 불리고 있다. 
  * [Dcinside](Dcinside.md)에서 시작된 것인데, 언젠가부터 글 제목 뒤에 ****.jpg라고 붙어있는 글들이 생겨나기 시작했다.(ex : 혐짤.jpg) 이것은 그 게시물의 내용이 그림이 주가 된다는 것을 제목에서부터 전달하려고 만들어진 것이다. 물론 이를 이용해서 [낚시](%EB%82%9A%EC%8B%9C.md)를 하는 경우도 많다.<del>확장자라 쓰고 조회수 높이는 주문이라 읽는다.</del>
  * 영미권에서는 JPEG를 '제이펙'이라고 읽는다.   
  
  
  
  
  
  

`\----`

  * `[1]` Quantumization, 계수화라고도 한다.
  * `[2]` 그림판을 열어 빨간색으로 선을 쭉 그은뒤 저장해보자. 갈색이 된다.
  * `[3]` 보안적인 이유도 있다. 웹셸이나 XSS 등 서버나 클라이언트에 악영향을 주는 파일의 업로드를 원천적으로 차단하기 위함이다.
  * `[4]` 저해상도의 이미지를 앞서 보여준 다음 점점 해상도를 높이는 방식으로 로딩된다.

