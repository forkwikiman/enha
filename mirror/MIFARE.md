  * 상위 항목 : [교통카드](%EA%B5%90%ED%86%B5%EC%B9%B4%EB%93%9C.md)  

## Contents

    

1. 개요 
2. 종류 
3. 이용 지역 
4. 여담 

[[edit](http://rigvedawiki.net/r1/wiki.php/MIFARE?action=edit&section=1)]

## 1. 개요 ¶

[네덜란드](%EB%84%A4%EB%8D%9C%EB%9E%80%EB%93%9C.md)
[NXP반도체](NXP%EB%B0%98%EB%8F%84%EC%B2%B4.md)의 RF 기술. 이용하는 주파수는 13.56MHz로,
국제표준 규격인 ISO/IEC 14443 Type A와 **일부** 호환된다. 원래는 Mikron에서 개발한 것이라 이름도
**Mi**kron **Fare** Collecting System의 두문자어로 MIFARE가 되었는데, 이 기술을
[필립스](%ED%95%84%EB%A6%BD%EC%8A%A4.md)가 [현질](%ED%98%84%EC%A7%88.md)해서 관련
제품을 생산하기 시작했다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/MIFARE?action=edit&section=2)]

## 2. 종류 ¶

MIFARE 카드는 [스마트카드](%EC%8A%A4%EB%A7%88%ED%8A%B8%EC%B9%B4%EB%93%9C.md)의
일종이지만, 가장 처음에 등장한 MIFARE Classic 1K/4K 카드는 안테나가 달린 외장 메모리였다. 암호화같은 건 정말 팬티 한 장
걸친 수준으로만 해 놓고, 단말기에 접촉해서 정보를 읽고 쓰는 것만 가능하게 만든 것이다. 따라서 보안성이 떨어진다. 이름에서 알 수 있듯이
1K는 1,024[바이트](%EB%B0%94%EC%9D%B4%ED%8A%B8.md), 4K는 4,096바이트를 저장할 수 있다.
[유패스](%EC%9C%A0%ED%8C%A8%EC%8A%A4.md)가 MIFARE Classic 1K를 이용해서 세계 최초로 상용화된
[교통카드](%EA%B5%90%ED%86%B5%EC%B9%B4%EB%93%9C.md)다.
[대경교통카드](%EB%8C%80%EA%B2%BD%EA%B5%90%ED%86%B5%EC%B9%B4%EB%93%9C.md)도 MIFARE
Classic이다. 아예 칩셋까지 NXP 제품을 이용 중. [유패스](%EC%9C%A0%ED%8C%A8%EC%8A%A4.md)는 일부
카드만 NXP 제품이다.

  

일회용으로 쓰기엔 Classic도 오버스펙이라고 해서 MIFARE Ultralight와 MIFARE Ultralight C도 나와 있다.
Ultralight는 저장 용량도 512바이트에 암호화 없이 생으로 정보를 기록한다(...) Ultralight C는 보안을 눈꼽만큼
신경써서, 192바이트의 저장 용량에 Triple [DES](DES.md)를 올려서 나왔다. 둘 다 일회용 RF 티켓에 사용할 목적으로
개발된 것.

  

가장 대중적으로 쓰이는 것 중에 MIFARE DESFire가 있다. NFC 리더기로 읽어보면 간혹 카드 종류를 MIFARE
SmartMX라고도 읽는다. ISO/IEC 14443 표준에 맞는 모델로, 카드 내부에 8051 마이크로프로세서를 탑재하고 Triple
DES와 [AES](AES.md)를 올려서 나왔다.
[오이스터](%EC%98%A4%EC%9D%B4%EC%8A%A4%ED%84%B0.md), [OV-Chipkaart](OV-Chipkaart.md) 등에 절찬리 이용 중. 문제는 이 모델이 2011년에 해킹되었다는 것(...) 후속작으로 보안이 강화되고 DESFire와
하위호환이 되는 MIFARE DESFire EV1이 나왔다.

  

MIFARE Classic의 보안 수준이 [허접한 관계로](%EB%AC%B4%EC%9E%84%EC%8A%B9%EC%B0%A8.md),
강화된 보안 모듈을 끼워넣은 MIFARE Plus가 나왔다. 메모리는 2K/4K 두 종류로 나왔고 128비트 암호화를 지원하는 듯.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/MIFARE?action=edit&section=3)]

## 3. 이용 지역 ¶

  * [대경교통카드](%EB%8C%80%EA%B2%BD%EA%B5%90%ED%86%B5%EC%B9%B4%EB%93%9C.md)
  * [오이스터](%EC%98%A4%EC%9D%B4%EC%8A%A4%ED%84%B0.md)
  * [유패스](%EC%9C%A0%ED%8C%A8%EC%8A%A4.md)
  * [OV-Chipkaart](OV-Chipkaart.md)

[[edit](http://rigvedawiki.net/r1/wiki.php/MIFARE?action=edit&section=4)]

## 4. 여담 ¶

외국 웹에서는 상기한 모든 종류의 MIFARE 공카드를 벌크로 살 수도 있다. <del>일반인이 살 일은 대량으로
[NFC](NFC.md) 태그를 만드는 것 빼곤 없겠다만</del>

  

MIFARE, 특히 [대한민국](%EB%8C%80%ED%95%9C%EB%AF%BC%EA%B5%AD.md)에서 많이 사용한
Classic과 Ultralight가 보안성이 취약하고 복제당하기 쉽다는 단점으로 인해 [세종특별자치시](%EC%84%B8%EC%A2%85%ED%8A%B9%EB%B3%84%EC%9E%90%EC%B9%98%EC%8B%9C.md)에서는 2013년
[티머니](T-Money.md)로 [교통카드](%EA%B5%90%ED%86%B5%EC%B9%B4%EB%93%9C.md) 시스템을
전면 교체하면서 [캐시비](%EC%BA%90%EC%8B%9C%EB%B9%84.md) 이전에 나온 구형 MIFARE
[마이비](MYbi.md) [교통카드](%EA%B5%90%ED%86%B5%EC%B9%B4%EB%93%9C.md) 사용을 전면
금지했다. [광주광역시](%EA%B4%91%EC%A3%BC%EA%B4%91%EC%97%AD%EC%8B%9C.md)에서도
[한페이](%ED%95%9C%ED%8E%98%EC%9D%B4.md) 사용을 권장하는 이유다.
[롯데ATM](%EB%A1%AF%EB%8D%B0ATM.md)에서도 MIFARE [마이비](MYbi.md) 카드와
[하나로카드](%ED%95%98%EB%82%98%EB%A1%9C%EC%B9%B4%EB%93%9C.md)의 충전을 전면 중단했으며, 해당
슬롯에는 [한페이](%ED%95%9C%ED%8E%98%EC%9D%B4.md)로 대체했다.
[우리은행](%EC%9A%B0%EB%A6%AC%EC%9D%80%ED%96%89.md)도 [유패스](U-PASS.md)의 [ATM]
(/wiki/%ED%98%84%EA%B8%88%20%EC%9E%90%EB%8F%99%20%EC%9E%85%EC%B6%9C%EA%B8%88%E
A%B8%B0) 충전을 전면 삭제하고
[레일플러스](%EB%A0%88%EC%9D%BC%ED%94%8C%EB%9F%AC%EC%8A%A4.md)의 충전으로 대체했다.

