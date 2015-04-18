## Contents

    

1. 소개 
2. 단점 
3. ALZ를 풀기위한 노력들 

[[edit](http://rigvedawiki.net/r1/wiki.php/ALZ?action=edit&section=1)]

## 1. 소개 ¶

  

[이스트소프트](%EC%9D%B4%EC%8A%A4%ED%8A%B8%EC%86%8C%ED%94%84%ED%8A%B8.md) 에서 만든
압축 포맷. 대부분의 압축 포맷이 자체 알고리즘을 사용하는데 반하여, ALZ 포맷은 [BZIP2](BZIP2.md)의 변형 알고리즘과
[Deflate](Deflate.md)알고리즘을 사용한다. 포맷 자체도 [ZIP](ZIP.md)포맷과 거의 유사하지만, 초기의
[ZIP](ZIP.md) 포맷이 파일 크기를 저장하는 필드를 4바이트로 고정하여 4GB이상의 파일을 처리하지 못하는 반면, ALZ
포맷은 파일 크기 저장 필드를 가변으로 처리할 수 있도록 개선하여 4GB 이상의 파일도 처리할 수 있으며, 분할 파일에 대한 처리 기능도
추가 되었다. (물론 요즘 ZIP 포맷은 4GB 이상의 파일도 처리가 가능하고, 분할 압축은 원래 잘 지원했다.)

  

ALZ 포맷이 처음 소개된 것은 알집 4.9 버전부터 이며, 이때는 BZIP2 알고리즘을 변형(?)한 알고리즘을 사용하였다. 아마도 ZIP
포맷 보다는 나은 포맷이라는 것을 주장하고 싶어서 Deflate 압축 알고리즘 보다 압축률이 좋은 BZIP2 알고리즘을 사용한 듯 한데,
BZIP2 압축 알고리즘을 그냥 쓰면 다른 압축 프로그램이 손쉽게 압축을 해제할 것을 걱정(?)하였는지 BZIP2 알고리즘을 수정해서
사용하였다. (보통 수정이라고 하면 "개선"을 의미하지만, ALZ 포맷에서 변형한 방법은 개선과는 거리가 먼... 단순히 리버싱을 막기 위한
변형으로 보인다. 이 때문인지 알집 8.0 초기 버전은 BZIP2 알고리즘을 사용한 ALZ 포맷의 압축을 해제하지 못하는 버그가 있었다.)

  

다음은 [unalz](unalz.md) 소스에서 변형된 bzip2 소스에 대한 부분 중 일부  

    
    
    switch (s->state) {  // [ALZ] - 머리떼기  /*      GET_UCHAR(BZ_X_MAGIC_1, uc);      if (uc != BZ_HDR_B) RETURN(BZ_DATA_ERROR_MAGIC);      GET_UCHAR(BZ_X_MAGIC_2, uc);      if (uc != BZ_HDR_Z) RETURN(BZ_DATA_ERROR_MAGIC);      GET_UCHAR(BZ_X_MAGIC_3, uc)      if (uc != BZ_HDR_h) RETURN(BZ_DATA_ERROR_MAGIC);*/  case BZ_X_MAGIC_1 :// 없어진헤더인식대신  // [ALZ] - blocksize 지정없음      //GET_BITS(BZ_X_MAGIC_4, s->blockSize100k, 8)  s->blockSize100k = 0x39;// static 할당.....  /* [ALZ] - 원래헤더      if (uc == 0x17) goto endhdr_2;      if (uc != 0x31) RETURN(BZ_DATA_ERROR);      GET_UCHAR(BZ_X_BLKHDR_2, uc);      if (uc != 0x41) RETURN(BZ_DATA_ERROR);      GET_UCHAR(BZ_X_BLKHDR_3, uc);      if (uc != 0x59) RETURN(BZ_DATA_ERROR);      GET_UCHAR(BZ_X_BLKHDR_4, uc);      if (uc != 0x26) RETURN(BZ_DATA_ERROR);      GET_UCHAR(BZ_X_BLKHDR_5, uc);      if (uc != 0x53) RETURN(BZ_DATA_ERROR);      GET_UCHAR(BZ_X_BLKHDR_6, uc);      if (uc != 0x59) RETURN(BZ_DATA_ERROR);*/      s->currBlockNo++;      if (s->verbosity >= 2)         VPrintf1 ( "\n    [%d: huff+mtf ", s->currBlockNo );       s->storedBlockCRC = 0;  /* [ALZ] - crc 빼기      GET_UCHAR(BZ_X_BCRC_1, uc);      s->storedBlockCRC = (s->storedBlockCRC << 8) | ((UInt32)uc);      GET_UCHAR(BZ_X_BCRC_2, uc);      s->storedBlockCRC = (s->storedBlockCRC << 8) | ((UInt32)uc);      GET_UCHAR(BZ_X_BCRC_3, uc);      s->storedBlockCRC = (s->storedBlockCRC << 8) | ((UInt32)uc);      GET_UCHAR(BZ_X_BCRC_4, uc);      s->storedBlockCRC = (s->storedBlockCRC << 8) | ((UInt32)uc);  */      // [ALZ] - 1bit 아끼기      //GET_BITS(BZ_X_RANDBIT, s->blockRandomised, 1);...

  

하지만, BZIP2 알고리즘 자체가 Defalte 알고리즘보다 압축률은 아주 조금 더 좋을 뿐이고, 속도는 무척 느렸기 때문인지, 아니면
알집이 "회사에서는 유료" 정책으로 바뀌었기 때문인지는 모르겠지만, 알집 5.0 부터는 ALZ 압축시 Deflate 압축 알고리즘만을
사용하여 압축을 하기 시작 하였다. (중간에 아주 아주 잠깐 [변형
Deflate](https://code.google.com/p/theunarchiver/wiki/AlZipSpecs) 알고리즘도
사용되었지만, 이 포맷으로 압축된 압축 파일은 거의 찾기 힘들다.)

  

이후, 알집 8.0 부터는 4GB 이상의 파일 압축이나, 분할 압축을 할 때, ALZ 대신 [EGG](EGG.md) 포맷을 주력으로
밀기 시작하였다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ALZ?action=edit&section=2)]

## 2. 단점 ¶

ALZ 포맷은 [WinRAR](WinRAR.md)을 비롯한 외국산 압축프로그램에서는 거의 대부분 지원이 안 된다.
[빵집](%EB%B9%B5%EC%A7%91.md), [V3 Zip](V3%20Zip.md),
[반디집](%EB%B0%98%EB%94%94%EC%A7%91.md) 등의 알집 호환을 내세운 몇몇 한국산 압축 프로그램이 특별한 경우.
커뮤니티에 자료를 ALZ 포맷으로 올리면 [포풍](%ED%8F%AC%ED%92%8D.md)같이 까일 수도 있으니 조심하자. 외국
커뮤니티라면 말할 것도 없다. [정체불명의 파일 때문에 ALZ 언패커를
만들었다.](http://www.totalcmd.net/plugring/new_unalz_wcx.html) **[WTF](WTF.md)
is ALZ!?**

  

새로운 압축 포맷을 만드는 것 자체는 문제가 안 된다. 기존에 존재하던 ZIP이나 RAR, 7z도 처음 나올 때는 새로운 압축 포맷이었다.
그러나 다른 압축 포맷이 압축을 푸는 모듈이나 소스를 공개하거나, 압축을 푸는 방법에 대한 문서를 제공해서 꼭 자사의 압축 프로그램을
설치하지 않아도 되도록 했는데, ALZ는 이런 행동을 전혀 취하지 않았다. 즉 정상적인 방법으로 다른 압축 프로그램에서 ALZ를 푸는 길을
막아놓은 것이다. ALZ가 욕먹는 이유가 바로 이것.

  

의도한 바는 아니지만 이런 특성 때문에 ALZ는 스페이스 인터내셔널의 가상CD
[확장자](%ED%99%95%EC%9E%A5%EC%9E%90.md) LCD와 함께 소프트웨어 불법복제 확산 방지에 조금이나마 기여하기도
했다.(사용자 편의성을 위해 존재하는 유틸리티가 오히려 편의성을 저해한 셈이니 절대 자랑이 아니다.)

  

하위 호환성을 안드로메다로 보내버리기 때문에 기업이나 개인이나 고생한다. 압축할 때의 프로그램 버전과 압축 풀때 프로그램이 일치하지 않으면
안풀릴 수도 있다. <del>본격 압축파일 세대차이</del>

  

[알집](%EC%95%8C%EC%A7%91.md) 4.X 까지는 개인이나 공공기관, 회사 등에서 전부 무료로 사용이 가능한
라이선스였는데, [알집](%EC%95%8C%EC%A7%91.md) 5.X 부터는 공공기관, 회사에서 사용시 유료 정책으로 바뀌면서 같이
ALZ 포맷의 내부 압축 알고리즘도 바꾸어 버렸다.`[1]` 이 때문에 기존 무료 알집 4.X 사용자들은 알집 5.0 에서 압축한 ALZ
파일을 풀 수 없다는 이유 때문에 어쩔 수 없이 알집을 구매해서 사용하게 되는 결과를 낳았다. --[ALZ인데 왜 알집으로 풀지를 못해](/
wiki/%EC%84%A4%EB%A0%81%ED%83%95%EC%9D%84%20%EC%82%AC%EC%99%94%EB%8A%94%EB%8D%
B0%20%EC%99%9C%20%EB%A8%B9%EC%A7%80%EB%A5%BC%20%EB%AA%BB%ED%95%B4)  

[이 글(주의. 여기 운영자는 리그베다 위키 항목 작성이 금지된 offree.net의
운영자이다)](http://qaos.com/article.php?sid=1507)과 [이
글](http://www.mediatoday.co.kr/news/articleView.html?idxno=100759)을 읽어보면 ALZ가
까이는 이유를 더 자세히 알 수 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ALZ?action=edit&section=3)]

## 3. ALZ를 풀기위한 노력들 ¶

  

[ALZ](ALZ.md)포맷은 본래 알집의 독자적인 포맷이었으나, 지금은 [빵집](%EB%B9%B5%EC%A7%91.md),
트집, [반디집](%EB%B0%98%EB%94%94%EC%A7%91.md), CocoAL, 다집 같은 ALZ 포맷을 지원하는
프로그램들이 많이 개발되었다.  
ALZ 파일의 압축 해제는 [빵집](%EB%B9%B5%EC%A7%91.md)의 개발자인 양병규가 처음 성공하였고, 이후 이에 자극 받은
키플러가 ALZ 포맷을 독자적으로 분석 후 [unalz](unalz.md)를 [오픈소스](%EC%98%A4%ED%94%88%20%EC%86%8C%EC%8A%A4.md)로 공개하면서 이후 수많은 프로그램에서 ALZ
파일을 지원하게 되었다.

  

UNALZ 소스: <http://www.kippler.com/win/unalz/>

  

unalz 가 오픈 소스로 공개된 이후 알집 이외의 ALZ 포맷을 지원하는 프로그램의 한 축을 이루고 있다. Mac OS X용의
CocoAL이 그 예. 빵집 개발자가 개발한 alz 해제 모듈(dll)은 지펜놀과 밤톨이에 사용되었다.

  
  

UNALZ가 나오기까지는 우여곡절이 좀 있었는데, 2000년대 초반 키플러가 처음 만든 ALZ 압축 해제 프로그램은 알집의 실행파일을
이용해서 ALZ 파일의 압축을 푸는 프로그램이었는데 이건 불법이었기 때문에 이스트소프트가 키플러를 고소. 키플러는 빡쳐서 ALZ를 리버스
엔지니어링 해서 2004년 오픈소스로 내놓은 것이 [트집](%ED%8A%B8%EC%A7%91.md)(tzip)이라는 프로그램이었다.
물론 이건 리버스 엔지니어링을 통해서 나온 것이기 때문에 불법이 아니다. UNALZ는 이 트집의 *nix 판이다.

  

현재 국내에서 공개된 대부분의 압축 프로그램은 ALZ 파일의 압축 해제를 지원하고 있지만, 일부 프로그램은 분할 압축이나 변형 BZIP2
알고리즘을 제대로 지원하지 못하고 있으므로 ALZ 파일을 지원한다는 말만 믿고 깔면 낭패를 볼 수도 있다. (하지만
[반디집](%EB%B0%98%EB%94%94%EC%A7%91.md)은 잘 푼다.)

`\----`

  * `[1]` 알집 4.X 에서 사용한 알고리즘은 변형된 [bzip2](bzip2.md) 이고, 알집 5.x 사용하는 알고리즘은 [ZIP](ZIP.md) 포맷에서 사용하는 [Deflate](Deflate.md) 알고리즘을 사용한다.

