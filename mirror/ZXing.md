## Contents

    

1. 개요 
2. 구성 
3. 알고리즘 
4. 기타 
5. 바깥고리 

[[edit](http://rigvedawiki.net/r1/wiki.php/ZXing?action=edit&section=1)]

## 1. 개요 ¶

구글에서 제공하는 오픈소스로 Zebra Crossing의 약자. QR코드 스캔 어플리케이션의 대다수가 이 어플리케이션을 이용했다고 해도
과언이 아닐정도로 널리 쓰이고 있는 코드다. 다양한 바코드를 인식할 수 있다. 인식할 수 있는 바코드 종류는 총 15 가지.

  
  

[[edit](http://rigvedawiki.net/r1/wiki.php/ZXing?action=edit&section=2)]

## 2. 구성 ¶

\- 이미지 디코딩 라이브러리  
\- 테스트 코드`[1]`  
\- 안드로이드 클라이언트  
\- 아이폰 클라이언트  

[[edit](http://rigvedawiki.net/r1/wiki.php/ZXing?action=edit&section=3)]

## 3. 알고리즘 ¶

기본적인 흐름은 다음 형식을 따른다.  

\- 카메라를 연 후 프리뷰를 가동한다.  
\- 카메라로부터 지속적으로 영상을 받아들인다. `[2]`  
\- 영상에서 밝기값만 추출`[3]`하여 이를 기반으로 이진화를 수행한다.`[4]`  
\- Detector 클래스를 통해 QR코드 영역을 찾아냈다.  
\- 찾아낸 영역을 Decoder 클래스를 통해 해석한다.  
\- 결과 값과 결과 영상을 리턴  
\- 결과 값을 분석하여 URL일 경우 탭하면 인터넷으로 연결되도록 한다.  
\- 화면에 결과 영상과 결과 값을 출력한다.  

말 자체는 간단하게 했지만 QR코드 패턴을 찾아내서 데이터에 저장하는게 말처럼 쉽지만은 않다.  
이미지 매트릭스나 QR코드정보를 저장하는 매트릭스는 Hashtable과 Vector를 이용하는 듯.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ZXing?action=edit&section=4)]

## 4. 기타 ¶

  * **카메라 해상도가 고정**되어있다. 때문에 QR 스캔에 있어 카메라 성능은 의미가 없다.   

[[edit](http://rigvedawiki.net/r1/wiki.php/ZXing?action=edit&section=5)]

## 5. 바깥고리 ¶

[ZXing 공식 페이지](https://github.com/zxing/zxing)

`\----`

  * `[1]` 에뮬레이터에서 카메라 촬영이 안되므로 샘플 이미지를 통해 스캔할 수 있도록하는 코드.
  * `[2]` 단, 바코드를 스캔하여 결과를 보여주는 동안에는 영상 수입을 중단한다.
  * `[3]` 카메라에서 얻는 영상은 YCbCr포맷이기 때문에 여기서 Y(명도)만 빼오면 된다.
  * `[4]` 한마디로 흑백으로 바꾼다는 소리

