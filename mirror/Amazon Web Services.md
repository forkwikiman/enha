## Contents

    

1. 개요 
2. 제공하는 서비스 목록 
3. 배경 
4. 참조 

![http://d36cz9buwru1tt.cloudfront.net/logo_aws.gif](http://d36cz9buwru1tt.clo
udfront.net/logo_aws.gif)

[[GIF external image]](http://d36cz9buwru1tt.cloudfront.net/logo_aws.gif)

<http://aws.amazon.com/>

Amazon Web Services. AWS라는 약어로도 불린다.  
2012년 5월 11일부터 [ 한국어 서비스를 시작했다.](http://aws.amazon.com/ko)

[[edit](http://rigvedawiki.net/r1/wiki.php/Amazon%20Web%20Services?action=edit
&section=1)]

## 1. 개요 ¶

[2006년](2006%EB%85%84.md) 경부터
[아마존닷컴](%EC%95%84%EB%A7%88%EC%A1%B4%EB%8B%B7%EC%BB%B4.md)에서 서비스 중인 [클라우드컴퓨팅](%ED%81%B4%EB%9D%BC%EC%9A%B0%EB%93%9C%20%EC%BB%B4%ED%93%A8%ED%8C%85.md)
플랫폼으로, [아마존닷컴](%EC%95%84%EB%A7%88%EC%A1%B4%EB%8B%B7%EC%BB%B4.md) 쇼핑몰에서
[추수감사절](%EC%B6%94%EC%88%98%EA%B0%90%EC%82%AC%EC%A0%88.md)이나
[크리스마스](%ED%81%AC%EB%A6%AC%EC%8A%A4%EB%A7%88%EC%8A%A4.md) 같은 시즌마다 몰리는
[트래픽](%ED%8A%B8%EB%9E%98%ED%94%BD.md)을 감당하기 위해 왕창 증설해둔 서버들이 평소엔 남아도니, 이걸
밖에서 쓸 수 있는 서비스를 만들어 팔아보자는 의도로 시작했는데, 지금은 **세계 1위**의 클라우드 플랫폼이 되어버렸다.(...)

  

이름대로 웹 서비스를 할 때 필요할 만한 온갖 서비스들을 제공하며, **서비스의 모든 기능을 [API](API.md)로 제어할 수
있다.** 다시 말해 아마존의 모든 기능을 당신이 필요한 대로 자동화할 수 있다는 것으로, 가능한 얼마든지 사용량, 곧 **비용**을 줄이는
방식으로 최적화를 할 수 있다. 심지어 아마존에서도 이렇게 해서 비용 절감하는 걸 적극 권장한다! 물론 간편하게 AWS의 기능을 제어할 수
있는 웹 콘솔도 제공하는데, 이것조차 AWS에서 제공하는 API로**만** 되어 있다. 그래서 오히려 웹 콘솔에서 못하는데 API로 할 수
있는 것도 <del>굉장히</del>많다. API 호출은 기본적으로 [HTTP](HTTP.md)나 [SOAP](SOAP.md)로
이루어지며, [Java](%EC%9E%90%EB%B0%94.md)나
[Python](%ED%8C%8C%EC%9D%B4%EC%8D%AC#s-2.md), [PHP](PHP.md),
[Ruby](%EB%A3%A8%EB%B9%84.md), [.NET](.NET%20Framework.md) 등에서 쓸 수 있는
라이브러리 및 샘플 코드도 제공한다.[#](http://aws.amazon.com/code) 일단
[문서](http://aws.amazon.com/documentation/)를 보자. 그리고 느끼자.(...)

  

힘들게 비싼 돈주고 서버 사고 [IDC](IDC.md)에 넣고 골치썩일 없이 쓴 만큼만 아마존에 내면 땡이기 때문에, 가진 게
아이디어하고 두뇌밖에 없는 [실리콘밸리](%EC%8B%A4%EB%A6%AC%EC%BD%98%20%EB%B0%B8%EB%A6%AC.md) 워너비
[벤쳐기업](%EB%B2%A4%EC%B3%90%EA%B8%B0%EC%97%85.md)들이 사업 시작할 때 가장 많이 쓰는 서비스가
되었다. 심지어 AWS 위에다가 클라우드 서비스를 재구성해서 [다른 개발자나 기업한테 팔아먹는 식의서비스](%EC%A4%91%EA%B0%9C%EC%97%85%EC%9E%90.md)까지 생겨날 정도가 되었으며, 개중에는 심지어 API는
있는데 AWS 웹 콘솔이 지원 안 하는 기능을 자기들이 콘솔로 만들어서 서비스하는 데까지 있다.(...)`[1]` 작은 기업들만 쓰는 것도
아닌 게, 심지어 [애플](%EC%95%A0%ED%94%8C.md)의 [iCloud](iCloud.md)도 [MicrosoftAzure](Microsoft%20Azure.md)와 AWS 위에서 동작하는 것으로 유명하다.
[?!](http://venturebeat.com/2011/09/03/icloud-azure-amazon/)

  

국내에서는 스타트업 문화 자체가 약해서인지 인지도가 엄청 떨어지는 편이다. 심지어 AWS 얘기를 하면 "왜 서점회사가 그런 걸 하나요?"
하고 되묻는 경우도 있다고(...) 그래도 알게 모르게 쓰는 곳이 있다는 듯. 국내에선 수도권에 있는 [IDC](IDC.md) 하나면
대충 내수용 서비스에는 무리가 없다는 게 이유일지도 모른다. 국내에 아마존닷컴 데이터 센터가 없기도 하고.`[2]`

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Amazon%20Web%20Services?action=edit
&section=2)]

## 2. 제공하는 서비스 목록 ¶

  * [Amazon Elastic Compute Cloud (EC2)](http://aws.amazon.com/ec2/) : 일종의 가상 서버. CPU 사용량 그런 거 없이 기본적으로 켜놓은 시간을 기준으로 과금하는 구조다. 다만 새 서버 인스턴스를 생성하고 프로그램 올리고 구동하는 게 전부 제공되는 API로 다 되기 때문에 Auto Scaling 서비스와 연계해서 **트래픽이 몰리면 인스턴스를 자동으로 늘려서 대응하고 트래픽이 줄어들면 만들었던 인스턴스를 없애는** 일을 할 수 있다. 성능별로 micro/small/large/xlarge 등으로 세분화되는데, 주의할 것은 성능 좋은 인스턴스를 쓸수록 **그만큼 과금액이 기하급수적으로 늘어난다.** 때문에 작은 서버 여러 대로 분산처리를 하는 것이 필수고, 고성능이 필요한 연산이 있으면 필요할 때만 잠깐씩 서버를 생성했다가 필요한 계산 끝내고 다시 없애버리는 식으로 사용시간을 아껴야 한다. 시간당 요금을 결재하는 방법부터 다양한 방식의 사용/[과금](http://aws.amazon.com/ko/ec2/pricing/)법이 존재한다.  

    * On Demand  
사용한 만큼 과금된다. 단, 과금의 단위가 1시간 이기 때문에 1초를 사용해도 1시간 어치가 과금된다.

    * [Spot Instance](http://aws.amazon.com/ko/ec2/spot-instances/)  
현재 사용되고 있지 않은 EC2자원을 경매로 싸게 낙찰받아 이용할 수 있는 방법. 위의 링크를 참고하자.

    * [Reserved Instance](http://aws.amazon.com/ko/ec2/reserved-instances/)  
사용할 기간(1년 혹은 3년)과 사용량(Light, Medium, Heavy)을 예약하면서 초기 선납비용을 내면, 시간당 사용료를 할인받는
방식. 주의할 점으로는 Reserved Instance 초기 비용을 납부하더라도, 시간당 사용료 자체가 0원이 되는건 아니다. 다만 할인폭은
매우 큰편. 최대 69%까지 저렴하다.

  * [Amazon Simple Storage Service (S3)](http://aws.amazon.com/s3/) : 웹에서 보여줄 이미지 등을 저장하는 데에 특화된 스토리지 서비스. 매우 약간의 데이터 저장 비용과 약간의 리퀘스트 비용을 지불하면 되는데, 아래의 CloudFront를 쓰면 더 줄일 수도 있다.
  * [Amazon CloudFront](http://aws.amazon.com/cloudfront/) : 세계 어디서나 빠른 속도로 파일을 제공하도록 최적화하는 content delivery network(CDN) 서비스.`[3]` 위의 S3와 연계하면 이미지 서비스의 극을 달릴 수 있다.
  * [Glacier](http://aws.amazon.com/glacier/) : 본격 **[백업](%EB%B0%B1%EC%97%85.md) 전용** 스토리지. 얼핏 S3와 비슷해 보이지만 S3가 개별 스토리지를 "Bucket"이라고 부르는 데 비해 이쪽은 그걸 "**[Vault](%EB%B3%BC%ED%8A%B8%28%ED%8F%B4%EC%95%84%EC%9B%83%20%EC%8B%9C%EB%A6%AC%EC%A6%88%29.md)**"라고 부른다. 고리짝 옛날옛적 [테이프](%ED%85%8C%EC%9D%B4%ED%94%84.md) 백업 시스템 느낌으로 일단 데이터가 들어갈 때는 마음대로인데 [나올때는 그렇지가 못하다](%EC%97%89%EB%8D%A9%EA%B5%AD.md). 데이터 반출신청을 하면 24~48시간 후에 꺼내주는 방식이므로 한번 쳐박아두면 정말 폴아웃스러운 상황이 닥치지 않는 이상 꺼내지 않을 것들을 저장해 둘 때 유용하다. 대신 가격 하나는 끝내주게 저렴해서 **1기가당 월 1센트**.  
단 여기에는 [함정](%ED%95%A8%EC%A0%95.md)이 있는데, Glacier가 저 가격에 저런 용량을 제공할 수 있는 이유는
유저가 데이터를 저장하고 나면 그 다음엔 해당 파일이 들어 있던 서버에는 [최소한의 전원만공급하다가](%EB%8F%84%EB%9E%80%EC%8A%A4%20%EB%82%B4%EB%A0%A4.md) 사용자가 데이터 반출요청을
하려고 하면 그 때 다시 서버 전원을 켜서 파일 리스트를 보여주고 요청한 데이터를 다른 서버에 옮겨서 다운받을 수 있게 해 주는 식이라
그만큼 서버 유지비용이 싸서 그런 것. 대신 그 반대 급부로 일단 파일 리스트를 보려면 서버 전원을 켜고 전기를 넣어야만 하기 때문에
**파일 리스트 보는 데만도 돈을 받는다**. 일단 백업해 놨다면 진짜 핵이라도 떨어지지 않은 이상 존재를 잊도록 하자.

  * [Auto Scaling](http://aws.amazon.com/autoscaling/)
  * [Amazon Route 53](http://aws.amazon.com/route53/) : [DNS](DNS.md) 서비스. 다만 API는 제공하는데 콘솔에는 메뉴가 없어서 좀 귀찮다. 대신 이걸 제어해주는 서드파티 웹 서비스가 있다.  

이외에도 수많은 서비스들을 제공하며, 지원하는 서비스의 종류는 지금도 계속 늘어나고 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Amazon%20Web%20Services?action=edit
&section=3)]

## 3. 배경 ¶

사족일지 모르지만 AWS가 왜 이런 무지막지한 규모의 API를 제공하게 되었냐면... **이미 아마존 자체가 이렇게 되어 있어서이다.**
그러니까, 아마존닷컴 쇼핑서비스 자체가 AWS 위에서 돌아가고 있다는 소리다. 아마존을 설립하고 지금도 아마존의 CEO인 [제프베저스](%EC%A0%9C%ED%94%84%20%EB%B2%A0%EC%A0%80%EC%8A%A4.md)가
[2002년](2002%EB%85%84.md) 어느 날에 [이런 메일을 사내에 돌렸다고
한다](http://eggy.egloos.com/3763434).

  

  1. 모든 팀들은 데이터와 기능들을 서비스 인터페이스로 연결시켜라.
  2. 팀들은 이 인터페이스를 통해서 연락해야 한다.
  3. 다른 어떤 커뮤니케이션 방법도 허용되지 않는다. 직접 링크를 보내거나 다른 팀의 스토리지에 직접 억세스 해서도 안 되며, 공유 메모리나 백도어 같은 것도 안 된다. 모든 커뮤니케이션은 네트워크를 통한 서비스 인터페이스로 이루어져야 한다.
  4. 어떤 기술을 쓰든 상관없다. HTTP, Cobra, Pubsub, 독자 프로토콜...그건 상관없다. 베저스는 그런데 관심 없다.
  5. 모든 서비스 인터페이스는 예외 없이 외부에서 이용 가능하게 만들어져야 한다. 그 말은 팀들은 외부 개발자들이 인터페이스를 이용할 수 있게 해야한다는 것이다. 예외는 없다.
  6. **이를 실천하지 않는 사람은 누구든 해고될 것이다.**
  7. <del>읽어줘서 고맙다. 좋은 하루가 되길.</del>`[4]`  

※ 출처: [스티브의 구글 플랫폼
폭언(http://eggy.egloos.com/3763434)](http://eggy.egloos.com/3763434)

  

그래서 아마존 직원들은 열심히 [아마존닷컴](%EC%95%84%EB%A7%88%EC%A1%B4%EB%8B%B7%EC%BB%B4.md)의
인프라를 [서비스 지향 아키텍쳐](SOA.md)로 갈아치웠다. **[2006년](2006%EB%85%84.md)까지**.
<del>[어쩌겠어 짤리기 싫으면 해야지](%EA%B3%B5%EB%B0%80%EB%A0%88.md)</del> 자세한 내용은 출처
참조. 원 작성자인 [스티비 예이그(Stevey
Yegge)](https://plus.google.com/110981030061712822816/)가
[키워](%ED%82%A4%EB%B3%B4%EB%93%9C%20%EC%9B%8C%EB%A6%AC%EC%96%B4.md) 기질이
다분하다는 걸 감안하고 읽자. 읽다보면
[아마존](%EC%95%84%EB%A7%88%EC%A1%B4%EB%8B%B7%EC%BB%B4.md)도 까고
[구글](%EA%B5%AC%EA%B8%80.md)도 까고 [MS](MS.md)도 까고 다 깐다는 걸 알 수 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Amazon%20Web%20Services?action=edit
&section=4)]

## 4. 참조 ¶

[아마존 웹 서비스를 다루는 기술](http://www.pyrasis.com/private/2014/09/30/publish-the-art-
of-amazon-web-services-book)`[5]`

  

`\----`

  * `[1]` Route 53이 이렇다.
  * `[2]` 아시아에는 [일본](%EC%9D%BC%EB%B3%B8.md)과 [싱가폴](%EC%8B%B1%EA%B0%80%ED%8F%B4.md)에 데이터센터가 있다.
  * `[3]` [아마존닷컴](%EC%95%84%EB%A7%88%EC%A1%B4%EB%8B%B7%EC%BB%B4.md)이 얼마나 많은 상품 사진을 서비스해야 하는지 생각해보자. 
  * `[4]` **"하하! 150명의 전 아마존 직원들(현 구글 직원)들은 7번이 내가 끼워넣은 농담이란 걸 알테지. 왜냐면 베저스는 자기가 삘 받은 날에 저런 좋은 말은 절대 하지 않으니까."** \- [Stevey Yegge](https://plus.google.com/110981030061712822816/)
  * `[5]` 책 내용이 모두 웹에 공개되어 있다.

