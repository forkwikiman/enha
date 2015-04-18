## Contents

    

1. 전자 문서 형식 
    

1.1. 개요

1.2. 버전별/규격별 차이

    

1.2.1. PDF 1.x

1.2.2. PDF/X, PDF/A, PDF/E

1.2.3. 그 외

1.3. pdf 뷰어 목록

2. [Warhammer 40,000](Warhammer%2040%2C000.md)의 [행성 방위군(Planetary Defence Force)](%ED%96%89%EC%84%B1%20%EB%B0%A9%EC%9C%84%EA%B5%B0.md)
3. 확률밀도함수 

[[edit](http://rigvedawiki.net/r1/wiki.php/PDF?action=edit&section=1)]

# 1. 전자 문서 형식 ¶

  * [컴퓨터 관련 정보](%EC%BB%B4%ED%93%A8%ED%84%B0%20%EA%B4%80%EB%A0%A8%20%EC%A0%95%EB%B3%B4.md)  

[[edit](http://rigvedawiki.net/r1/wiki.php/PDF?action=edit&section=2)]

## 1.1. 개요 ¶

![pdf.png](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/PDF/pdf.png)

[PNG image (27.87 KB)]

  

Portable Document Format 라는 뜻으로, [Adobe](Adobe.md)가 1993년에 개발한 전자 문서 형식이자,
국제 표준([ISO](ISO.md)) 문서 형식.

  

[Adobe](Adobe.md)사에서 제작된 [포스트스크립트](%ED%8F%AC%EC%8A%A4%ED%8A%B8%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8.md) 기반의 전자 문서 형식. 어느 환경에서나 동일한 결과물을 보여주기 위해
개발되었으며`[1]`, 그림과 [글꼴](%EA%B8%80%EA%BC%B4.md)을 포함한 여러 객체를 포함할 수 있다. 파일 내에 모든
정보를 포함하는게 필수는 아니며(보통은 [글꼴](%EA%B8%80%EA%BC%B4.md)정보를 제외하는 경우가 많음.) 해당 정보를 각
장치에서 모두 지원하지 않으면 관련 정보 표현에 있어 왜곡이 발생할 수 있다.

  

구조가 공개되어있으며, 사용권을 다양하게 부여할 수 있다. 체크박스, 글상자, 라디오 버튼 등을 문서에 삽입하면 기초적인 인터페이스로서
상호작용도 가능하다. 현재는 3D 오브젝트와 애니메이션등을 지원하기도 한다.

  

이미 [미국](%EB%AF%B8%EA%B5%AD.md)에서 [마이크로소프트](%EB%A7%88%EC%9D%B4%ED%81%AC%EB%A1%9C%EC%86%8C%ED%94%84%ED%8A%B8.md) 워드와 함께 실질적인 표준(de facto standard) 문서로
자리잡은 상태이다. 한 예로써 IB에 제출하는 모든 서류는 원본 파일과 인쇄판을 같이 내야되는데 이때 원본 파일의 형식은 반드시 PDF로
제출해야 한다. 어떤 OS에 어떤 상황에서도 컴퓨터만 작동하면 볼 수 있기 때문. 간단히 말하자면 어느 컴퓨터에서나 똑같이 볼 수 있는
다기능 문서 양식이다. 또한 출판과 출력을 위한 PDF의 전신 [포스트스크립트](%ED%8F%AC%EC%8A%A4%ED%8A%B8%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8.md)와 같은 그래픽모델을 공유하고 있고, [포스트스크립트](%ED%8F%AC%EC%8A%A4%ED%8A%B8%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8.md)와 달리 인덱스와 동적데이터 구조
등을 염두해두고 개발되었기에 전자책 같은 다양한 매체에 쓰인다.

  

2008년 7월 2일에 [ISO](ISO.md)(International Organization for Standardization)
국제표준으로 인정받았으며, 인정 받는 과정에서 표준 제정과 관련한 권한이 [ISO](ISO.md)로 이관되어, 더이상
[Adobe](Adobe.md)에서 관리하지 않는다.  
(ISO 32000-1, Document management – Portable document format – Part 1: PDF
1.7)

  

[한국](%ED%95%9C%EA%B5%AD.md)에서는 대체로 찬밥신세를 면치 못하고 있다. 생각보다 사용처가 제한적인 편. 여러 가지
이유가 있는데 가장 큰 이유는 한국 전자문서의 대세는 [Microsoft Windows](Microsoft%20Windows.md)
\+ [아래아 한글](%EC%95%84%EB%9E%98%EC%95%84%20%ED%95%9C%EA%B8%80.md) 조합이라는 것이다.
덕분에 '어느 환경에서나 동일한 결과물'을 보여줘야 할 필요성이 떨어지는 점도 있으며 윈도우즈 8 이전까지 기본적으로 PDF로 인쇄하는
기능을 지원하지 않았기 때문에`[2]`(맥OS는 OS 단계에서 기본 지원하지만, 한국은 맥 사용 비중이 매우 낮음을 감안하자) PDF 리더를
따로 설치하는 것도 귀찮을 뿐더러 Adobe사의 공식 리더가 그렇게 빠른 편이 아니기 때문에`[3]` 한국인들의
<del>[복돌이](%EB%B3%B5%EB%8F%8C%EC%9D%B4.md)</del>습성과는 안 맞는 편이라는 의견도 있고, 한글과
워드 및 기타 사무용 문서 솔루션에 비해 PDF 문서에 대한 사회적인 교육이 덜 된 점도 무시하기 힘들다. 편집이 안되는 점 때문에 아예
불완전한 문서로 생각하는 사람도 있다.

  

이제는 웬만한 프로그램이나 하드웨어의 도움말도 PDF로 나오게 되면서 제공하는 CD/DVD에 어도비 리더 정도의 프로그램은 제공하고 있다.
그러나 일반인 중에서 PDF 파일을 직접 제작할 수 있는 사람은 가뭄에 콩 나듯. <del>그리고 가장 널리 사용된다는 모 PDF 편집기의
가격이 터무니없이 비싸기도 하고</del>

  

가장 널리 사용되는 PDF 파일 제작·편집 프로그램은 [Adobe](Adobe.md)사의 [AdobeAcrobat](Adobe%20Acrobat.md) 제품군이다. 현존하는 PDF 파일 관련 프로그램중에서 가장 다양한 기능을 가지고
있고, 특히 PDF파일의 편집이 어느정도 가능(파일 제작자가 설정한 권한상에 문제가 없고 제작한 프로그램과의 호환성 문제가 없을 경우로
한정되지만)하기에 그 위치는 어느정도 보장되고 있다. 다만 비싸다. 환율에 따라 변동은 있지만 정가 기준으로 Acrobat X
Standard가 50만원대, Acrobat X Pro가 80만원대 가격을 형성하고 있다. 그 대신 [MS워드](MS%20%EC%9B%8C%EB%93%9C.md)를 사용하면 그만한 돈을 쓰지 않고도 작성이 가능한데, 저장할 때 PDF 혹은
XPS로 저장하기를 누르면 끝이다. 단 워드를 이용해 수정 등은 되지 않기에 따로 .doc 파일을 보관해둬야 한다.

  

아래는 PDF파일 형식을 만든 어도비사의 관련 소개 페이지. 이런 업체관련 페이지가 다 그렇듯, 자화자찬이 좀 있다. 적당히 필터링할것.
[Adobe PDF](http://www.adobe.com/kr/products/acrobat/adobepdf.html)

  

[[edit](http://rigvedawiki.net/r1/wiki.php/PDF?action=edit&section=3)]

## 1.2. 버전별/규격별 차이 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/PDF?action=edit&section=4)]

### 1.2.1. PDF 1.x ¶

PDF파일 내부적으로 사용된 기능에 따라 규격에 대한 버전이 존재한다. 리더 프로그램이나 PDF파일 관련 기기등에서 해당 파일을 지원하는지
결정하는 기준이된다.

  

  * PDF 1.3 : 투명도 지원 X / 레이어 지원 X / 멀티바이트 글꼴`[4]` 지원 X / 40비트 RC4보안
  * PDF 1.4 : **투명도 지원 O** / 레이어 지원 X / **멀티바이트 글꼴 지원 O** / 128비트 RC4보안
  * PDF 1.5 : 투명도 지원 O / 레이어 지원 O`[5]` / 멀티바이트 글꼴 지원 O / 128비트 RC4보안
  * PDF 1.6 & PDF 1.7 : 투명도 지원 O / 레이어 지원 O / 멀티바이트 글꼴 지원 O / 128비트 RC4보안 및 128비트 AES(Advanced Encryption Standard) 보안  

보다 자세한 정보는 아래에서 확인이 가능하다.  
[Acrobat X Pro 제품
도움말](http://help.adobe.com/ko_KR/acrobat/pro/using/WS25210BC7-2345-4e30-A05C-
80903A3B36EE.html)

  

[[edit](http://rigvedawiki.net/r1/wiki.php/PDF?action=edit&section=5)]

### 1.2.2. PDF/X, PDF/A, PDF/E ¶

용도에 따른 국제 표준 형식. 각각의 용도에 따라 크게 세가지가 있다.

  

  * PDF/X : 인쇄기기용 PDF파일의 표준형식 PDF/X-1a(PDF 1.3 가장 널리 사용됨), PDF/X‑3, PDF/X-4(PDF 1.4가 사용되어서 투명도 및 멀티바이트 글꼴 지원)까지 있으며, 인쇄기기나 RIP프로그램에서의 지원 범위에 따라 최종 출력물 품질에 미치는 영향이 크다. 
  * PDF/A : 장기 보관용 전자문서 형식. PDF/A‑1a 및 PDF/A‑1b 형식이 존재.
  * PDF/E : 엔지니어링 문서 상호 교환 형식. 현재는 PDF/E-1이 유일  

[[edit](http://rigvedawiki.net/r1/wiki.php/PDF?action=edit&section=6)]

### 1.2.3. 그 외 ¶

[ISO](ISO.md) 표준이 되기 이전부터 관련 기술의 대부분이 개방되어 있는 상태이기 때문에 다양한 업체에서 PDF파일 제작
솔루션이 제작 및 공급이 되고 있다. 따라서 한글 2007/2010 및 MS Office 2007/2010에서 자체적인 PDF변환 기능이
제공되기도 한다.

  

그림 파일을 그대로 PDF 문서로 만들어버리는 일이 잦아서 용량이 크다`[6]`는 편견이 있는데, 실제로는 전혀 그렇지 않다. 제대로만
만들면 생각보다 크기가 줄어드는 일도 있다. 예를 들어 같은 내용을 담은 [포스트스크립트](%ED%8F%AC%EC%8A%A4%ED%8A%B8%EC%8A%A4%ED%81%AC%EB%A6%BD%ED%8A%B8.md)(Postscript, .ps)파일을 PDF 파일로 변환하면
크기가 대략 1/2로 줄어든다. 문서에 포함된 그림 파일을 압축해서 저장하면 이보다 더 줄어들 수도 있다.`[7]``[8]`  
[어도비 일러스트레이터](%EC%96%B4%EB%8F%84%EB%B9%84%20%EC%9D%BC%EB%9F%AC%EC%8A%A4%ED%8A%B8%EB%A0%88%EC%9D%B4%ED%84%B0.md)의 ai파일을 읽어야하는데 해당 소프트웨어가 없으면, ai파일의 확장자를
pdf로 바꾸면 PDF리더로 파일이 열리기도 한다. 단, 저장 옵션`[9]`에 따라 안 될수도 있음.

  

[어도비 포토샵](%EC%96%B4%EB%8F%84%EB%B9%84%20%ED%8F%AC%ED%86%A0%EC%83%B5.md)에서는
확장자 변경 없이 그냥 열린다. 멀티 페이지 지원까지 하므로 문서의 여러 페이지 중 필요한 부분만 선택해서 불러들일수 있다. 스캔이나 캡춰
없이 문서를 그대로 포토샵으로 가져오는 기능이 되겠다. 사실 포토샵의 .psd 파일도 PDF 파일과 구조가 같다고 한다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/PDF?action=edit&section=7)]

## 1.3. pdf 뷰어 목록 ¶

  * [Adobe Reader](Adobe.md)
  * [별PDF](http://www.startools.co.kr/home/)
  * evince
  * okular
  * Foxit Reader
  * 미리보기 (Preview)
  * nespdf  

[추가바람](%EC%B6%94%EA%B0%80%EB%B0%94%EB%9E%8C.md)

[[edit](http://rigvedawiki.net/r1/wiki.php/PDF?action=edit&section=8)]

# 2. [Warhammer 40,000](Warhammer%2040%2C000.md)의 [행성 방위군(Planetary DefenceForce)](%ED%96%89%EC%84%B1%20%EB%B0%A9%EC%9C%84%EA%B5%B0.md) ¶

  

[[edit](http://rigvedawiki.net/r1/wiki.php/PDF?action=edit&section=9)]

# 3. 확률밀도함수 ¶

Probability Density Function

  

"확률밀도함수"의 영어식 표현. 확률밀도함수는 확률이나 통계 관련 과목에서 매우 중요하게 취급되는 개념이므로, 영어 원서로 공부한다면 책
속에서 PDF라는 약어 표현을 매우 많이 볼 수 있다.

  

`\----`

  * `[1]` 장치, 응용프로그램 독립적
  * `[2]` 8에서 지원하지만, 터치 인터페이스에 최적화된 Style UI용 뷰어이다.
  * `[3]` Adobe 리더는 PDF 리더중 최고의 퀄리티를 자랑하지만 동시에 가장 무겁고 느린 리더기이다. 타사 혹은 오픈소스로 제작한 가벼운 리더기들도 많이 존재하지만 한국에선 PDF 사용하는 사람 자체가 적기 때문에 관심 있는 사람도, 아는 사람도 별로 없다.
  * `[4]` 한글이나 중국어, 일본어 서체등이 대표적인 멀티바이트 글꼴이다. 즉 PDF 1.3에서는 정상적인 한글텍스트 등의 지원이 안된다.
  * `[5]` 일러스트나 인디자인 같은 프로그램에서 제작된 레이어가 사용된 PDF파일이 여기에 해당
  * `[6]` 스캐너나 복합기 설치 프로그램에서 기본 유틸로 제공되는 기능에 스캔한 데이타로 PDF파일 생성 기능이 있는 경우가 많다.
  * `[7]` 이미지 처리 옵션 설정에 따라 화질이 저하 될 수 있다. 주의요망
  * `[8]` PDF파일은 압축 포멧이 아니므로 용량이 항상 줄어들지는 않는다. 단지 변환 설정과 원본 데이타에 따라 용량이 감소할 수도 있을 뿐이다.
  * `[9]` 저장할 때 "PDF 호환 파일 만들기(Create PDF Compatible File)"라는 옵션이 있다.

