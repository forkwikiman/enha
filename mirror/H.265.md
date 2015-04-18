![http://content.myphone.gr/photo/full/10581/h-265-etoimo-na-ferei-hd-vinteo-
se-diktya-me-chamilo-
bandwidth.jpg](http://content.myphone.gr/photo/full/10581/h-265-etoimo-na-
ferei-hd-vinteo-se-diktya-me-chamilo-bandwidth.jpg)

[[JPG external image]](http://content.myphone.gr/photo/full/10581/h-265
-etoimo-na-ferei-hd-vinteo-se-diktya-me-chamilo-bandwidth.jpg)

## Contents

    

1. 개요 
2. 4K / UHDTV 떡밥 
3. 단점 
4. 적용 

[[edit](http://rigvedawiki.net/r1/wiki.php/H.265?action=edit&section=1)]

## 1. 개요 ¶

동영상을 손실 압축하여 저장하는 [포맷](%ED%8F%AC%EB%A7%B7.md)이자 2013년 영상업계 최대의
[떡밥](%EB%96%A1%EB%B0%A5.md). [H.264](H.264.md)의 후속으로 등장했다.

  

H.265는 기술적으로 보면 복잡도가 H.264에 비해 5배 정도 늘어나고 압축률이 H.264 대비 최대 50%까지. 동일 화질(PSNR)로
따지면 대략 30%를 웃도는 정도의 압축률을 보인다.

  

HEVC를 표준화시킨 그룹은 JCT-VC 그러니까 Joint Collaborative Team on Video Coding의 약자이며 여기엔
ITU-T/ISO/IEC가 참여했는데, ITU-T는 H.시리즈 표준화, ISO/IEC에 MPEG가 있어 MPEG 시리즈를 표준화시켰다. 항상
둘이 앙숙.

  

H.264 에서는  

  * 8-pel Motion Vector Resolution
  * Adaptive Interpolation Filter
  * Motion Vector Competition 
  * Adaptive Prediction Error Coding in Spatial
  * and Frequential Domain 
  * Adaptive Quantization Matrix Selection
  
를 업데이트했다면, H.265 에선  

  * Extended Macroblock Size (EMS) 
  * Large Transform Size (LTS) 
  * Internal Bit Depth Increading (IBDI) 
  * Sample Adaptive Offset (SAO)
  * context-adaptive binary arithmetic coding (CABAC)
를 이용한다.

  

기본적으로 코딩 블록 크기를 16X16에서 64X64로 키우고, 그에 맞추어 다른 기술들의 정밀도/연산 단위를 키운 덕이 크다. 그리고
그만큼 인코딩하기 힘들어졌다.

  

포맷은 기존의 H.264를 기반으로 확장하였다. 프로필은 Main / Main 10 (10bit 영상을 위해) / Still(사진
압축용)`[1]`을 기본으로, Range extension으로서, 흑백/4:2:2/4:4:4 포맷과 12, 16비트 영상을 지원할 수 있도록
하였다.`[2]`  
덤으로, H.264 시절에 만들어진 레벨 개념에 더하여, 티어 개념이 새로 생겨 같은 레벨 영상의 영상이라도 고화질을 다룰 수 있도록
하였다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/H.265?action=edit&section=2)]

## 2. 4K / UHDTV 떡밥 ¶

기존 방송업계에선 솔직히 내부 편집할 때 매개코덱(ProRes나 DnxHD 같은)을 쓰거나 RAW를 이용해 촬영하다 보니 별문제도 없었고,
송출할 때야 당연히 1080p로 다운샘플링한 다음에 모듈레이터에 때려 박으면 볼만한 화질로 H.264 코딩되어 나가니 신경 쓸 일도 없었다.
일반 청취자들한테 치이고 [클래식덕후](%ED%81%B4%EB%9E%98%EC%8B%9D%EB%8D%95%ED%9B%84.md)들에게도
치이는 [KBS 1FM](KBS%201FM.md)과는 참 다른 분위기 (...) `[3]`

  

영화관? 영화관의 경우엔 디지털 상영하는 영화관에서 까고 말하면 SONY의 4K LCOS프로젝터나 바코의 4K 프로젝터를 설치하는 경우는
극히 드물었으며, 이것의 이용도 Dual Link HD-SDI를 2개 연결한 뒤 전용 재생기를 이용하는 편이었다.`[4]` 이게 아닌 경우는
NEC 등에서 나오는 2K 프로젝터를 이용하는 편이었고, 영화 상영이 아닌 제작과정에선 위와 같은 현실.

  

그러나 시대가 지나면서 4K 컨슈머 시장이 슬슬 발돋움 하기 시작했다. 2013년에 들어서 CES와 같은 행사에선 모두 4K 디스플레이
경쟁이 이어졌으며, 8K의 해상도를 보이는 디스플레이와 송출장비 및 카메라 등이 주요한 화제가 되었다. 물론, 모바일 분야의 경우
400ppi를 넘기는, 즉 1080p 해상도를 5인치 내에 담아내는 것에 혈안이 되어 있었었고. 이에 따라, 4K 디스플레이에서 이용 가능한
4K 영상이 필요하게 되었는데, 현실적으로 가장 이용하기 쉬운 것이 H.265였기 때문에`[5]` 이 포맷의 등장은 업계에서 상당히 민감한
반응을 만들 수밖에 없었다.

  

한마디로 말해 H.265는 H.264에 비해 50% 이상 압축률이 높다는 것. 즉, 4K 미디어를 기존의 대역폭 내에서 서비스하는 것이
가능해진다는 것이다.

  

H.265에선 영상 압축 부분에서 [비월주사](%EB%B9%84%EC%9B%94%EC%A3%BC%EC%82%AC.md)([인터레이스](
/wiki/%EC%9D%B8%ED%84%B0%EB%A0%88%EC%9D%B4%EC%8A%A4) 스캔)에 특화된 기능이 모두 제거되고
순차주사(프로그래시브 스캔)로만 영상을 저장한다. 대신 이미 나와 있는 비월주사 영상과 장비가 무척 많으므로 영상에 플래그를 두어 영상을
둘로 나누거나 짝수/홀수 필드를 모으는 식으로 비월주사 영상을 지원한다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/H.265?action=edit&section=3)]

## 3. 단점 ¶

영상코덱은 필시 압축을 할 때 여러 알고리즘을 사용하게 되는데, 압축률이 올라가는 만큼 알고리듬도 복잡해져서 H.265는 첫 등장 당시에도
소위 '좌절 영상'을 양산한 H.264에 비해 5배 이상의 연산량을 요구한다. 다만 GPU를 이용한 디코딩이나 전용 하드웨어 디코더로
재생하는 것은 가능하여 모바일의 경우 2014년 양산된 스냅드래곤 805부터, PC에서는 2009년 양산된 AMD HD5000 시리즈부터
H.265 가속이 지원되고 있으며, 실제로 openCL을 이용한 GPU 연산을 위하여 전용 코덱을 설치해 주면 듀얼코어급의 **저 사양의
CPU에서도 4K HEVC의 안정적인 재생**이 가능`[6]`하다. 다만 아직 인코딩을 실시간으로 하기는 힘들어서 전용기기가 없는 경우
생방송에는 적용하기는 어렵다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/H.265?action=edit&section=4)]

## 4. 적용 ¶

H.265를 이용한 최초의 민생용 영상 녹화기기로 2014년 11월 발매된 삼성의 미러리스 카메라
[NX1](%EC%82%BC%EC%84%B1%20NX/%EB%B0%94%EB%94%94.md)이 있다. PC에 <del>젬병</del>
문외한인 초기 리뷰어들이 삼성의 NX1 4K 동영상`[7]`은 수백만 원대의 PC로도 편집은커녕, 재생마저 불가능하다고 일갈하였으나, 알고
보니 2009년에 출시한 VGA만으로도 하드웨어 가속`[8]`으로 원활히 재생할 수 있었다. 앞으로 캠코더와
[DSLR](DSLR.md) 카메라에서 H.265의 채택은 [화질과 용량 사이의 균형](%ED%99%94%EC%A7%88%EA%B3%BC%20%EC%9A%A9%EB%9F%89%20%EC%82%AC%EC%9D%B4%EC%9D%98%20%EA%B7%A0%ED%98%95.md)을 위해 더욱 확대될 전망이다.

`\----`

  * `[1]` 이미 H.264시절에 정지 화면 압축률이 JPG2000을 넘어섰다.
  * `[2]` 일반적으로 우리가 보는 영상은 4:2:0, 8비트 포맷 영상이다.
  * `[3]` Classic FM의 경우 비록 디지털 마스터를 하지만 가정의 수신기에서 복호화한 결과까지 원음에 최대한 가깝게 튜닝하는것을 목표로 송출세팅이 되어있다. 즉, 드라마 방송처럼 대충 스케줄러에 테이프 <del>처</del>넣고 큐사인받아서 트는게 아니라 송출 엔지니어가 상시 대기하면서 장비를 조정하여 최상의 음질로 청취할 수 있도록 늘 조정하고 있다. 영상업계 이야기로 바꾸면 마스터한 원본 푸티지를 바로 보내주는 느낌.
  * `[4]` 배급사에서 HDD를 줬다.
  * `[5]` RAW 로 방송 송출할 수 있을까? 대역폭 60Gbps 주면 몰라도, 현재 공중파 방송의 대역폭은 높아봐야 30Mbps 이기 때문에 상당히 높은 압축률의 포맷이 아닌 이상 스트림을 띄울 수 없다.
  * `[6]` 보급형 4.5세대 하스웰 리프레시인 i3 4150에서, HD 4K HEVC 영상이 CPU 점유율 70% 미만으로 원활히 재생 가능했다.
  * `[7]` 해당 H.265 코덱 동영상의 해상도는 4K다. <del>일반 Full HD가 아니란 말이다.</del>
  * `[8]` 소프트웨어로 재생할 때보다 화질이 0.5%~1% 정도 떨어진다. 그 차이는 120인치 이상의 디스플레이에서 맨눈으로 구별할 수있다.<del>120인치 디스플레이를 사용하는 사람이 하드웨어 가속을 쓰긴 할까?</del>

