  * 상위 항목 : [동음이의어·다의어/알파벳](%EB%8F%99%EC%9D%8C%EC%9D%B4%EC%9D%98%EC%96%B4%C2%B7%EB%8B%A4%EC%9D%98%EC%96%B4/%EC%95%8C%ED%8C%8C%EB%B2%B3.md)  

## Contents

    

1. Multimedia Messaging System 
2. Microsoft Media Server 
3. Multi Mode Service 
    

3.1. 사례

    

3.1.1. 해외

    

3.1.1.1. ATSC

3.1.1.2. DVB-T

3.1.1.3. ISDB-T

3.1.2. 대한민국

[[edit](http://rigvedawiki.net/r1/wiki.php/MMS?action=edit&section=1)]

## 1. Multimedia Messaging System ¶

**이동통신 메시지 전송 방식**

**네트워크 종속**
1세대

2세대

3세대

[문자메시지](%EB%AC%B8%EC%9E%90%EB%A9%94%EC%8B%9C%EC%A7%80.md)

**MMS**
[joyn](joyn.md)

**플랫폼 종속**
[통합메시지함](%ED%86%B5%ED%95%A9%EB%A9%94%EC%8B%9C%EC%A7%80%ED%95%A8.md)

[아이메시지](%EC%95%84%EC%9D%B4%EB%A9%94%EC%8B%9C%EC%A7%80.md)

  
기존의 [문자메시지](%EB%AC%B8%EC%9E%90%EB%A9%94%EC%8B%9C%EC%A7%80.md)가 이름 그대로 문자만
보낼 수 있는 반면, MMS는 문자 외에 [그림](%EA%B7%B8%EB%A6%BC.md)과
[동영상](%EB%8F%99%EC%98%81%EC%83%81.md)을 함께 보낼 수 있다. 요금은 문자메시지보다 비싼 편이다.
SK텔레콤에서는 **컬러메일**`[1]`, kt에서는 **멀티메일**, LG유플러스에서는 **샷메일**이란 이름으로 서비스하고 있다.
<del>통화연결음은 컬러링/링투유/필링, 발신자통보서비스는 콜키퍼/캐치콜/매너콜</del>

  

유럽에서는 자주 쓰이지만 한국에서는 자리를 잡지 못한 서비스. 특히 MMS를 대체할 수 있는
[카카오톡](%EC%B9%B4%EC%B9%B4%EC%98%A4%ED%86%A1.md)의 등장 이후 가격이 비싼 MMS는 거의 쓰지 않게
되었다. 국제 표준 SMS규격은 140Byte, 국내에선 80Byte(즉, 완성형한글 40자)로 제한 되는 까닭에, 커뮤니케이션의 스타일과
언어 습관 또한 많이 바뀌었다. '밥 먹었어?' '뭐해?' 등. [트위터](%ED%8A%B8%EC%9C%84%ED%84%B0.md)
같은 요소가 이미 자리잡고 있었던 것이다.  
국제표준 SMS의 경우, 7bit를 1글자로 치환하는 꼼수를 써서 알파벳,숫자 등 [아스키코드](%EC%95%84%EC%8A%A4%ED%82%A4%20%EC%BD%94%EB%93%9C.md) 문자**만**으로는 140자가
아닌 160자까지 써진다. 하지만 한글 등 아스키 코드 이외 문자가 **한 자라도** 있으면 해당 메시지 전체가
[유니코드](%EC%9C%A0%EB%8B%88%EC%BD%94%EB%93%9C.md)로 전환되기 때문에 70자까지만 써진다. 즉, 한글
1자+알파벳 138자(2+138=140)가 아니라, 한글 1자+영어 69자(1+69=70)라는 뜻이다.  
국내에선 국제표준은 생까고 80Byte였는데, 문자메시지 수요가 현저이 줄어들고 나서야 KT는 2011년<del>역시 선구자 아이폰 덕을
톡톡히 본다</del> 11월부터, SKT는 2013년 8월부터, LG U+는 2013년 10월 17일 부터 70자(140byte)까지 쓸
수 있게 하였다. 기존 단말기도 똑같이 적용되어 40자가 넘어 MMS로 변환되어도 140byte까지는 MMS요금(보통 30원)이 아닌
SMS요금(보통 20원)이 부과된다.

  

한편 이 MMS를 구현하기 위해 만들어졌던 것이 있으니... <del>[공공의적](%EA%B3%B5%EA%B3%B5%EC%9D%98%20%EC%A0%81.md)</del>
[통합메시지함](%ED%86%B5%ED%95%A9%EB%A9%94%EC%8B%9C%EC%A7%80%ED%95%A8.md) 참조.  
하지만 지금은 [망했어요](%EB%A7%9D%ED%96%88%EC%96%B4%EC%9A%94.md). 2012년 5월부터 <del>말
뿐인</del>[단말기자급제](%EB%8B%A8%EB%A7%90%EA%B8%B0%20%EC%9E%90%EA%B8%89%EC%A0%9C.md)가 실시된 이후,
각 통신사 고유 MMS가 사라지고, 이후 출시되는 휴대폰에선 모두 국제표준인 OMA-MMS가 탑재된다. 물론 해외 출시 폰들은 옛날옛적부터
OMA-MMS였다.  
그런 고로 2012년 5월 이후에 출시되는 국산 폰들은 타사 유심 기변을 해도 MMS가 정상적으로 되며, 만약 안 되더라도 그건 [버그일
뿐](http://www.ppomppu.co.kr/zboard/view.php?id=phone&no=1687439)이니 APN 설정을
[적절히](%EA%B9%80%EB%8C%80%EA%B8%B0.md) 한다면 MMS를 문제없이 쓸 수 있다. 이전에도 OMA-MMS가
탑재된 국산 폰이 있는데, [참고하라](http://likesoft.info/163).

  

참고로, [카카오톡](%EC%B9%B4%EC%B9%B4%EC%98%A4%ED%86%A1.md)·[텔레그램](%ED%85%94%EB%A0%88%EA%B7%B8%EB%9E%A8.md)같은 인스턴트메신저나 [joyn](joyn.md)(RCS) 뿐만 아니라 MMS도
**무료**로 '상대방 수신확인·읽음확인'이 가능하다. [KT](KT.md)의 경우 한술 더 떠서, '등기문자'라고 해서 SMS까지도
수신확인을 지원하는데, 문제는 이게 SMS일 땐 20원이 추가되는 **유료**서비스라는 점. 즉 SMS로 등기문자를 보내면
20원+20원=**40**원이 청구된다. 문자 기본제공량에서 100개를 제공하든 200개를 제공하든 등기료 20원은 별도다(...)  
하지만 위에 서술한 대로 3사 모두 MMS로 보내더라도 140byte까지는 SMS요금이 나오기 때문에(즉, MMS로 140Byte까지는
수신·읽음확인을 요청하든 안하든 30원이 아니라 **20**원만 나온다는 뜻이다. 당연히 기본제공량이 있으면 그냥 거기서 차감) 이를 적절히
이용하면 수신확인·읽음확인을 활용할 수 있다. 그럼 어떻게 70자 이하일 때 MMS로 보내냐고? **제목**을 추가하면 70자 이내라도
SMS가 아닌 MMS로 발송되며, 혹은 글자색을 한 자라도 바꾸면 MMS로 발송된다. 그러니 써먹자.

  

`\----`

  * `[1]` 초창기에는 메시지 발신은 물론 수신 시에도 [WAP](WAP.md)(모바일 인터넷)에 접속하여 요금을 내야 하는 흠좀무한 서비스였다.

[[edit](http://rigvedawiki.net/r1/wiki.php/MMS?action=edit&section=2)]

## 2. Microsoft Media Server ¶

[마이크로소프트](%EB%A7%88%EC%9D%B4%ED%81%AC%EB%A1%9C%EC%86%8C%ED%94%84%ED%8A%B8.md)가 만든 멀티미디어 스트리밍 프로토콜이다. 이를 통해 전송하는 멀티미디어의 주소는 MMS:// 로 시작한다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/MMS?action=edit&section=3)]

## 3. Multi Mode Service ¶

![Koreaview_2_2_1.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Koreaview_
2_2_1.jpg)

[JPG image (454.82 KB)]

  

기존 [디지털 TV](%EB%94%94%EC%A7%80%ED%84%B8%20%EB%B0%A9%EC%86%A1.md)의 대역을 여러 개로
나누어 2개 이상의 채널을 동시에 송출하는 방식이다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/MMS?action=edit&section=4)]

### 3.1. 사례 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/MMS?action=edit&section=5)]

#### 3.1.1. 해외 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/MMS?action=edit&section=6)]

##### 3.1.1.1. ATSC ¶

[미국](%EB%AF%B8%EA%B5%AD.md)의 경우 [2000년대](2000%EB%85%84%EB%8C%80.md)부터 일부
방송사들이 MMS를 시행하고 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/MMS?action=edit&section=7)]

##### 3.1.1.2. DVB-T ¶

DVB-T를 디지털 공중파 방송 방식으로 채택한 나라에서는 ATSC처럼 한 채널에 여러 방송을 우겨넣는(?) 일이 없는 대신에
[멀티플렉스](%EB%A9%80%ED%8B%B0%ED%94%8C%EB%A0%89%EC%8A%A4.md)라는 개념이 있다. 이들
나라에서는 [유료](%EC%BC%80%EC%9D%B4%EB%B8%94%EB%B0%A9%EC%86%A1.md)[방송](%EC%9C%84%EC%84%B1%EB%B0%A9%EC%86%A1.md)의 대체재로 작용하면서 지상파 직접 수신 가구수가 유료 방송 가입 가구수보다 많은
기현상이 나타났다[#](http://s1.postimg.org/j2k7l118t/Koreaview_4.jpg).  

  * [영국](%EC%98%81%EA%B5%AD.md) : 프리뷰`[(Freeview)]`
  * [오스트레일리아](%EC%98%A4%EC%8A%A4%ED%8A%B8%EB%A0%88%EC%9D%BC%EB%A6%AC%EC%95%84.md) : 프리뷰`[(Freeview)]`
  * [뉴질랜드](%EB%89%B4%EC%A7%88%EB%9E%9C%EB%93%9C.md) : 프리뷰`[(Freeview)]`
  * [프랑스](%ED%94%84%EB%9E%91%EC%8A%A4.md) : TNT (Television Numerique Terrestre)
  * [말레이시아](%EB%A7%90%EB%A0%88%EC%9D%B4%EC%8B%9C%EC%95%84.md) : 마이뷰(Myview)  

[[edit](http://rigvedawiki.net/r1/wiki.php/MMS?action=edit&section=8)]

##### 3.1.1.3. ISDB-T ¶

일본의 경우 [NHK](NHK.md)의 교육채널인 E텔레(Eテレ)에서 2004년 9월부터 부분적인 다채널 서비스를 제공하고 있다. 한
채널에 정규편성을 하고 다른 채널에 다른 편성을 하는 형식. [원세그](%EC%9B%90%EC%84%B8%EA%B7%B8.md) 채널도
마찬가지여서 NHK의 원세그 2채널은 원세그의 특징을 살린 프로그램을 일부 시간대에 편성한다.

  

민영방송의 경우 도쿄MX가 2008년 6월에 원세그 멀티채널, 2014년 4월에 지상파 멀티채널(091ch, 092ch)을 시작했다. 하지만
화질 열화가 발생하면서 주변에서 욕을 먹고 있다.[관련 포스팅](http://knousang.egloos.com/3461159)

[[edit](http://rigvedawiki.net/r1/wiki.php/MMS?action=edit&section=9)]

#### 3.1.2. 대한민국 ¶

[대한민국](%EB%8C%80%ED%95%9C%EB%AF%BC%EA%B5%AD.md)의 경우
[2006년](2006%EB%85%84.md)에 지상파 MMS 시험방송을 실시한 적이 있었으나, 화질 저하 등으로 인한 시청자들의
항의가 빗발치면서 20여 일 만에 중단해야만 했던 [흑역사](%ED%9D%91%EC%97%AD%EC%82%AC.md)가 있었다[#](h
ttp://news.inews24.com/php/news_view.php?g_serial=209554&g_menu=020300). 당시에
지상파 MMS 채널에서는 [독일 월드컵 관련프로그램](2006%20FIFA%20%EC%9B%94%EB%93%9C%EC%BB%B5%20%EB%8F%85%EC%9D%BC.md)들과
몇몇 교양 프로그램들을 방영하였다고 한다. 당시의 지상파 디지털 TV 화질이 어땠는지는
[여기](http://1967jk.blog.me/20024772082)를 참조하자.

  

![Koreaview_3_1.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Koreaview_3_
1.jpg)

[JPG image (704.65 KB)]

  
이후 [2010년](2010%EB%85%84.md)에
[KBS](%ED%95%9C%EA%B5%AD%EB%B0%A9%EC%86%A1%EA%B3%B5%EC%82%AC.md)가
코리아뷰(Koreaview, 약칭 K-View) 사업을 계획하게 된다. 그런데, 지난 번의 MMS 시험방송에서 화질 저하로 인하여 문제가
되었는지 이번에는 [HD](HD.md) 채널만 기존 TV 수상기와의 호환성 유지를 위해 MPEG 2 코덱으로 압축하고, SD 채널은
종전과 달리 화질저하 문제를 줄이기 위해 H.264 코덱으로 압축하여 송출하는 것으로 결정하였다. 결국 기존 TV로는 SD 채널을 시청할 수
없기 때문에 별개의 수신기가 필요하게 된 것이다`[3]`.

  

![Koreaview_3_3.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Koreaview_3_
3.jpg)

[JPG image (169.64 KB)]

  
KBS는 [2010년](2010%EB%85%84.md) [9월 3일](9%EC%9B%94%203%EC%9D%BC.md)부터 2주
동안 수도권 내 500가구를 대상으로 코리아뷰 시험방송을 실시할 예정이었으나, 방송통신위원회로부터 허가를 받지 못해 실시하지
못했다[#](http://www.mediaus.co.kr/news/articleView.html?idxno=13328). 시험방송 대상이었던
가구들 [지못미](%EC%A7%80%EB%AA%BB%EB%AF%B8.md). 이는 나중에 국회의 국정감사에서도 지적되었다[#](http
://www.zdnet.co.kr/news/news_view.asp?artice_id=20111004111516&type=det). 이후
[국회의사당](%EA%B5%AD%ED%9A%8C%EC%9D%98%EC%82%AC%EB%8B%B9.md) 등에서 시연회를 실시하다
[2011년](2011%EB%85%84.md) [12월 27일](12%EC%9B%94%2027%EC%9D%BC.md)에 [제주특별자치도](%EC%A0%9C%EC%A3%BC%ED%8A%B9%EB%B3%84%EC%9E%90%EC%B9%98%EB%8F%84.md) 북부
지역에서 기상재난 시험방송을 송출하는 것으로 코리아뷰 시험방송을
시작하였다[#](http://news.kbs.co.kr/tvnews/news9/2011/12/27/2410656.html).

  

![Koreaview_3_2.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Koreaview_3_
2.jpg)

[JPG image (119.32 KB)]

  
코리아뷰의 주 목적은 유료방송 미가입자들의 정보격차 해소를
위해서라고[#](http://news.kbs.co.kr/tvnews/news9/2011/12/31/2412757.html). 실제로 설문조사
결과 코리아뷰 도입에 찬성한 사람의 비율이 90%를 넘는 것으로 밝혀졌다[#](http://news.naver.com/main/read.nh
n?mode=LSD&mid=sec&sid1=106&oid=003&aid=0003910731). <del>하지만 화질이 개판이 된다는 것을
알고도 찬성할 사람은 얼마나 될까?</del>

  

![Koreaview_1_1.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/Koreaview_1_
1.jpg)

[JPG image (173.39 KB)]

`[4]`  
[2014년](2014%EB%85%84.md) [1월 2일](1%EC%9B%94%202%EC%9D%BC.md)부터 [3월31일](3%EC%9B%94%2031%EC%9D%BC.md)까지 수도권 일부 지역에서 지상파 다채널 실험방송을 실시하였다. 이를 위해
관악산에 송신 시설을 설치하였으며, 4대 방송사가 3주씩 번갈아가며 방송을 운영하였다([관련
기사](http://news.kbs.co.kr/news/NewsView.do?SEARCH_NEWS_CODE=2782094&ref=A)).  
실험방송 이후 정식으로 개국하게 되면 지상파 방송 4사가 자사 계열
[유료방송](%EC%BC%80%EC%9D%B4%EB%B8%94%EB%B0%A9%EC%86%A1.md)
[채널](%EC%BC%80%EC%9D%B4%EB%B8%94%EB%B0%A9%EC%86%A1/%EC%B1%84%EB%84%90.md)을
지상파로 송출하게 되어 채널 수가 20개`[5]`로 늘어날 것이다.

  

[방송통신위원회](%EB%B0%A9%EC%86%A1%ED%86%B5%EC%8B%A0%EC%9C%84%EC%9B%90%ED%9A%8C.md)는 [2014년](2014%EB%85%84.md) [8월 4일](8%EC%9B%94%204%EC%9D%BC.md)에 발표한
간담회에서 7대 정책 과제를 발표하면서 2015년부터 [EBS](%ED%95%9C%EA%B5%AD%EA%B5%90%EC%9C%A1%EB%B0%A9%EC%86%A1%EA%B3%B5%EC%82%AC.md)를 시작으로 다채널 서비스를 시작하겠다고 밝혔다. 최성준 방송통신위원장은
“유료방송에 있는 교육방송을 MMS로 내보내면 사교육비 절감 등의 효과를 기대할 수 있다”며 “나머지 지상파 방송에 대해서는 기술적으로 큰
문제가 없다고 판단하지만 다양한 요소를 고려해 시행 계획을 세워갈 것”이라고
했다.[#](http://www.hankyung.com/news/app/newsview.php?aid=2014080466591)  
김유열 EBS 정책기획부장은 12월 10일 한국방송협회가 주최한 ‘지상파 다채널 방송(MMS) 정책 토론회’에서 “사교육 경감을 위해 EBS
플러스 1, EBS 플러스 2, EBS 잉글리쉬 등 3개의 PP 채널을 운영하고 있지만 SO에서 EBS 학습채널 론칭을 기피해 시청자
도달률이 매우 낮고 영어채널의 경우 10%도 론칭되지 않고 있다”면서 “MMS가 허용돼 PP 채널에서 만든 콘텐츠를 재송신하면 시청자복지와
정보격차 해소에 도움될 것”이라고
말했다.[#](http://www.mediatoday.co.kr/news/articleView.html?idxno=120578)

  

[2015년](2015%EB%85%84.md) [2월 11일](2%EC%9B%94%2011%EC%9D%BC.md)에 최초의 다채널
방송인 [EBS 2TV](EBS%202TV.md)가 개국하였다.[#](http://www.ebs.co.kr/customer/servic
e/notice/10001510861?p=Yy5wYWdlPTEmYy5wYWdlU2l6ZT0yMCZzZWFyY2hLZXl3b3JkPSZzZWF
yY2hDb25kaXRpb249) <del>정적인 화면이 많아 깍두기 안 생겨서 화질 하면 EBS였는데...</del> <del>EBS 화질
떨어지는 소리가 벌써부터 들린다</del>

`\----`

  * `[(Freeview)]` 이름만 같을 뿐 전혀 다른 서비스다.
  * `[3]` 그 이유는 기존의 디지털TV가 MPEG 2 코덱만 지원하기 때문이다.
  * `[4]` 참고로, MBC ESPN은 현재의 [MBC 스포츠플러스](MBC%20%EC%8A%A4%ED%8F%AC%EC%B8%A0%ED%94%8C%EB%9F%AC%EC%8A%A4.md)이다. 또한, [KTV](KTV.md)는 [2014년](2014%EB%85%84.md)에 한국정책방송이 [국민방송](%EA%B5%AD%EB%AF%BC%EB%B0%A9%EC%86%A1.md)으로 바뀌면서 로고도 함께 바뀐 상태이다. 단, 한국정책방송원이라는 단체명은 바뀌지 않았다. [KBS N 스포츠](KBS%20N%20%EC%8A%A4%ED%8F%AC%EC%B8%A0.md)도 같은 해에 로고가 바뀐 상태.
  * `[5]` 서울과 비수도권 지역 한정이며, [인천](%EC%9D%B8%EC%B2%9C%EA%B4%91%EC%97%AD%EC%8B%9C.md)과 [경기 지역](%EA%B2%BD%EA%B8%B0%EB%8F%84.md)은 [OBS](OBS#s-1.md)도 송출하므로 21개까지 수신 가능. 만일, OBS까지 다채널 방송을 실시한다면 해당 지역에서는 최대 24개 채널을 수신할 수 있다.

