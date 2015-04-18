International Mobile Subscriber Identity

[휴대폰](%ED%9C%B4%EB%8C%80%ED%8F%B0.md)의 [SIM](SIM.md)에 저장된 가입자 고유 번호. SIM
외부에 기록된 8982로 시작하는 열 아홉자리 숫자와는 다르다. 그건 ICCID.

크게 세 부분으로 구성되어 있다. MCC, MNC, 그리고 MSIN. MCC와 MNC는 [APN](APN.md) 설정을 할 때 꼭
필요하다.  

  * MCC : Mobile Country Code, 즉 핸드폰(SIM)이 개통된 국가의 세자리 숫자 코드이다. 한국은 450, [일본](%EC%9D%BC%EB%B3%B8.md)은 440~441, [미국](%EB%AF%B8%EA%B5%AD.md)은 310, [북한](%EB%B6%81%ED%95%9C.md)은 467이다.
  * MNC : Mobile Network Code, 통신사의 고유한 숫자 코드이다. 세자리를 쓰는 곳도 있고 두자리를 쓰는 곳도 있긴 있다. 아직까지 한국에서는 두자리만 쓴다. [SK텔레콤](SK%ED%85%94%EB%A0%88%EC%BD%A4.md)은 05, [KTF](KTF.md)는 02와 04, [KT](KT.md)([olleh](olleh.md))는 08, [LG U+](LG%20U+.md)는 06, SK텔레콤의 [MVNO](MVNO.md)인 티플러스는 11을 쓴다.
  * MSIN : Mobile Subscription Identification Number. 가입자 고유번호다. LG U+는 특이하게 가입자 전화번호와 동일하다. 전화번호가 010-1234-5678이면 MSIN도 1012345678이다.  

자신의 IMSI가 궁금하면 IC 카드 리더기를 구입하고 SIM의 정보를 읽어주는 프로그램을 인터넷으로 다운받은 후 핸드폰에 꽂혀있는
USIM을 뽑아서 리더기에 꽂으면 된다. <del>[참쉽죠?](%EC%B0%B8%20%EC%89%BD%EC%A3%A0.md)</del> [안드로이드](%EC%95%88%EB%93%9C%EB%A1%9C%EC%9D%B4%EB%93%9C%28%EC%9A%B4%EC%98%81%EC%B2%B4%EC%A0%9C%29.md)
[스마트폰](%EC%8A%A4%EB%A7%88%ED%8A%B8%ED%8F%B0.md)에서는 앱으로 확인하면 된다. 대표적으로
[Network signal
info](https://play.google.com/store/apps/details?id=de.android.telnet)나 [Check
my android](https://play.google.com/store/apps/details?id=com.checkmyandroid.a
pp).

이걸 복제할 수 있으면 [3G](3G.md)와 [4G](4G.md)에서도 브릿지폰을 만들 수 있다. 하지만 [현실은시궁창](%ED%98%84%EC%8B%A4%EC%9D%80%20%EC%8B%9C%EA%B6%81%EC%B0%BD.md). **이론상**
가능하다는 것이지, 실제로는 불가능하다. 지금까지 기존 SIM에서 이걸 뽑아서 빈 SIM에 복제하는 데 성공한 사람이 없다.

여담으로 [구글 플레이](%EA%B5%AC%EA%B8%80%20%ED%94%8C%EB%A0%88%EC%9D%B4.md)에서는 이
IMSI의 앞부분을 읽어서 어느 나라의 어느 통신사인지를 구분한다. 따라서 한때 외국 통신사의 SIM을 구해다 꽂고 [Wi-Fi](/wiki
/Wi-Fi)로 플레이 마켓에 접속하면 해당 국가에서 받을 수 있는 앱을 다운로드할 수 있...었으나, **막혔다.** 해당 계정의 최근
접속 국가까지 로그로 남겨서 체크하는 걸로 정책이 바뀌었기 때문에 타국가에 오래 있으면 한국에 귀국해서도 그 오래 있던 국가의 구글 플레이를
볼 수 있는 [아햏햏](%EC%95%84%ED%96%8F%ED%96%8F.md)한 현상을 볼 수 있다.

