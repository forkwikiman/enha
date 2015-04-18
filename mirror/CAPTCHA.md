**C**ompletely **A**utomated **P**ublic **T**uring test to tell **C**omputers and **H**umans **A**part  
(<del>영어권 사용자와 비영어권 사용자를 구분짓기 위한</del>컴퓨터와 사람을 구분짓기 위한 완전 자동 [튜링테스트](%ED%8A%9C%EB%A7%81%20%ED%85%8C%EC%8A%A4%ED%8A%B8.md))`[1]`

[공식 사이트](http://www.captcha.net/)

![http://www.captcha.net/images/recaptcha-
example.gif](http://www.captcha.net/images/recaptcha-example.gif)

[[GIF external image]](http://www.captcha.net/images/recaptcha-example.gif)

  
(사진은 reCAPTCHA)

<del>스팸 그만하고 책을 읽으란 문구가 정말 인상적이다.</del>`[2]`

## Contents

    

1. 개요 
2. 유래 
3. 상세 
4. reCAPTCHA 
5. no CAPTCHA 
6. 한국에서는? 
    

6.1. [리그베다위키](%EB%A6%AC%EA%B7%B8%EB%B2%A0%EB%8B%A4%20%EC%9C%84%ED%82%A4.md)에서는?

[[edit](http://rigvedawiki.net/r1/wiki.php/CAPTCHA?action=edit&section=1)]

## 1. 개요 ¶

사용자가 사람인지 자동화된 [봇](%EB%B4%87.md) 혹은 자동화
[프로그램](%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%A8.md)인지 판단하기 위해 사용되는 일종의 행동 전
[테스트](%ED%85%8C%EC%8A%A4%ED%8A%B8.md).

  

[[edit](http://rigvedawiki.net/r1/wiki.php/CAPTCHA?action=edit&section=2)]

## 2. 유래 ¶

1999년에 최고의 컴퓨터 과학 프로그램을 가진 대학을 뽑는 투표가 인터넷 상에서 이루어졌다. 이때 [카네기 멜론 대학교](%EC%B9%B4%EB%84%A4%EA%B8%B0%20%EB%A9%9C%EB%A1%A0%20%EB%8C%80%ED%95%99%EA%B5%90.md)와
[매사추세츠 공과대학교](%EB%A7%A4%EC%82%AC%EC%B6%94%EC%84%B8%EC%B8%A0%20%EA%B3%B5%EA%B3%BC%EB%8C%80%ED%95%99%EA%B5%90.md)의 학생들이 자동으로 투표를 하는 프로그램을 만들어 매우 많은
투표(...)를 얻었는데, 이후 이런 것들을 방지하기 위해 만들어졌다고 한다.`[3]`

  

[[edit](http://rigvedawiki.net/r1/wiki.php/CAPTCHA?action=edit&section=3)]

## 3. 상세 ¶

테스트 방식은 매우 단순하다. 출력된 숫자나 글자를 있는 그대로 입력란에 입력하고 확인을 받으면 끝. 이런 작업은 프로그램으로서는 진행할 수
없고 오직 유동적으로 사고할 수 있는 사람만이 할 수 있기 때문에 이게 사람인지 봇인지를 판별하는데 유용하게 사용된다. 물론 화면상의
텍스트가 폰트를 있는 그대로 사용하는 거라면 프로그램도 당연히(...) 맞힐수 있으므로 변형을 준다. 글자를 휘거나 글자의 가로획을 이어
버린다거나 등등. 아니면 호실/번호판등을 흐린 이미지로 보여주기도 한다.

  

특히 [스팸](%EC%8A%A4%ED%8C%B8.md) 방지를 위해 많이 쓰인다. 스팸 소프트웨어의 자동 계정 등록을 막기 위해 계정
등록할 때 거치는 테스트로 이미지 단어를 보여준 뒤 그 단어를 쓰는 것으로 사용자의 명령을 수행하는 프로세스로 진행.

  

물론 소프트웨어가 진화하다보면 그냥 숫자나 글자는 인식해버리기도 하는지라, 가끔 단어를 시각적으로 변형시킨 복잡한 패턴을 사용하기 때문에
심하면 사람이 봐도 이게 글자인지 뭔지 모를 단어를 보여주고 입력하라고 하는 경우가 있다.(…) 이런 경우을 대비해서 친절하게 해결책이
마련되어 있는데, 단어를 새로고침하거나 단어를 직접 음성으로 들려주어 입력하게끔 하는 옵션을 이용하면 된다`[4]`.

  

일반적인 CAPTCHA 패턴은 사람은 쉽게 알아볼 수 있지만 스팸 소프트웨어나 봇은 자동으로 인식할 수 없다. 결과적으로는 자동 계정
생성이나 메일 자동발송등을 어렵게 하여 스팸을 차단하는 효과를 보게 되는 것. 사실 이런 게 가능한 이유는 CAPTCHA에 들어가는 연산의
대부분이 일단 실행된 뒤에는 되돌릴 수 없는, **비가역적 연산**이기 때문이다. 그럴만도 한 게, 대부분이 글자를 비틀거나 회전시키는 등,
역연산이 존재하지 않는 방법으로 글자를 왜곡하고 있는데,
[양자컴퓨터](%EC%96%91%EC%9E%90%EC%BB%B4%ED%93%A8%ED%84%B0.md)라도 상용화되지 않는 한
현재로서는 이걸 소프트웨어만으로는 완벽하게 깰 방법이 없다.`[5]` 같은 이유로 [JPEG](JPEG.md)으로 저장된 이미지를
완벽하게 복원하는 것도 불가능하다.

  

하지만, 이미 문자 기반의 CAPTCHA중 일부는 연구자들에 의해
[뚫린](http://www.phrack.org/issues.html?issue=68&id=4#article) 상태.`[6]` 이를 보완하기
위해 문자 대신 이미지를 변형시키는 형태도 연구되고 있다. 특히 이미지 기반의 CAPTCHA는 이미지 특성상 특정 문화에 익숙해져 있지
않으면 맞추기 어렵게 하는 경우(예 : [세종](%EC%84%B8%EC%A2%85.md),
[태극기](%ED%83%9C%EA%B7%B9%EA%B8%B0.md),
[무궁화](%EB%AC%B4%EA%B6%81%ED%99%94.md) 등)도 있어 해외 스패머들을 막을 수 있지만, 이미지를 이용하기
때문에 데이터베이스의 크기가 커질 수 있다는 단점을 지니고 있다.

  

CAPTCHA의 단점은 기본적으로 웹 접근성에 위배된다는 점이다. 특성상 이미지를 보고 텍스트화를 해야 되기 때문에, 이미지를 볼 수 없는
시각장애인은 CAPTCHA를 통과할 수 없다는 문제점이 있다. 시각장애인을 위한 텍스트 리더 프로그램은 이미지로 된 CAPTCHA를 읽지
못하기 때문. 이 때문에 요즘 CAPTCHA에는 음성으로 읽어주는 오디오 기능이 들어가 있다. 이 오디오 기능을 이용해서 프로그램으로
CAPTCHA를 뚫는 경우도 있다. 음성의 경우 정도의 차이는 있지만 명확하게 나오기 때문이다.

  

설정에 따라서는 대소문자나 띄어쓰기 혹은 점 하나만 틀려도 까칠하게 오답처리할 수도 있고, 한두글자 정도는 틀려도 그냥 넘어가도록 설정할
수도 있다.

  

CAPTCHA를 설치했는데도 우르르 스팸 게시물이 등록되는 경우가 종종 있는데, 이건 CAPTCHA의 결함이라기보다는 게시판이나 서버에 보안
구멍이 있는 경우가 많다. 보안 구멍을 이용해서 CAPTCHA를 우회하는 것. 만약 CAPTCHA가 설치되어 있는데도 스팸 게시물이 많이
등록된다면 CAPTCHA만 맹신하지 말고 게시판이나 서버에 다른 경로로 게시물이 등록되는 것이 가능한지도 점검해 봐야 한다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/CAPTCHA?action=edit&section=4)]

## 4. reCAPTCHA ¶

[설명 1](http://www.ted.com/talks/view/lang/ko//id/1295) [설명
2](http://tvcast.naver.com/v/214835)

  

CAPTCHA의 종류 중 많이 쓰이는 reCAPTCHA라는 것은 사실 [구글](Google.md)에서 고서의 내용을 처리하는데(!)
사용되고 있다. 이것의 정체는 구글이 보유하고 있는 고서 스캔 데이터에서 자동 처리에 실패한 단어들의 이미지를 따온 뒤, 그것을 사람이 보고
입력하도록 함으로서 이미지를 텍스트로 바꾸는 프로그램이다. 즉, 한마디로 말하자면 **인간 [OCR](OCR.md) 프로그램**.
<del>[네놈은 그냥 하루하루 구글신에게 텍스트를 갖다 바치는 OCR일 뿐이지!](%EB%84%A4%EB%86%88%EC%9D%80%20%EA%B7%B8%EB%83%A5%20%ED%95%98%EB%A3%A8%ED%95%98%EB%A3%A8%20%EB%98%A5%20%EB%A7%8C%EB%93%9C%EB%8A%94%20%EA%B8%B0%EA%B3%84%EC%9D%BC%20%EB%BF%90%EC%9D%B4%EC%A7%80.md)</del>`[7]` 이 때문에 reCAPTCHA에 나오는 단어 중에는 옛날에나 사용되던 좀 생소한 단어들이 섞여 있다.

  

reCAPTCHA에서 나오는 문제를 보면 꼭 단어가 두 개씩 짝을 이뤄서 나온다. 둘 중 하나는 이미 연산을 통해 데이터로 처리가 된
단어고, 나머지 하나는 아직 처리가 안 된 단어이다. 전자는 답이 밝혀져 있지만 후자는 답이 밝혀져있지 않다. 하지만 전자를 맞히면 (사람이
입력한 이상) 후자도 정답일 확률이 높다고 처리하는 식으로 연산하는 것.

  

reCAPTCHA는 [무료로 쓸 수 있다.](http://www.google.com/recaptcha)

  

2014년 4월 10일에 중국 연구팀이 [reCAPTCHA의 해킹을
성공했다.](http://www.dailysecu.com/news_view.php?article_id=6679)

  

[[edit](http://rigvedawiki.net/r1/wiki.php/CAPTCHA?action=edit&section=5)]

## 5. no CAPTCHA ¶

  

[no CAPTCHA 개발자 블로그 글](http://googleonlinesecurity.blogspot.kr/2014/12/are-
you-robot-introducing-no-captcha.html) [공식
홈페이지](https://www.google.com/recaptcha) [관련
기사](http://techneedle.com/archives/19453)

  

기존의 캡차는 사람조차 알아보기 힘들어서 가끔 사람도 오타를 낸다. 이러한 문제를 해결하기 위해 구글에서는 노 캡차를 개발했다.  

![http://4.bp.blogspot.com/-wt7yljKcU_8/VH5MJTUCBOI/AAAAAAAAACw/WKqE3ixUUdw/s1
600/Recaptcha_anchor%402x.gif](http://4.bp.blogspot.com/-wt7yljKcU_8/VH5MJTUCB
OI/AAAAAAAAACw/WKqE3ixUUdw/s1600/Recaptcha_anchor%402x.gif)

[[GIF external image]](http://4.bp.blogspot.com/-wt7yljKcU_8/VH5MJTUCBOI/AAAAA
AAAACw/WKqE3ixUUdw/s1600/Recaptcha_anchor%402x.gif)

  
PC 버전의 경우 클릭시 사람 특유의 마우스 포인팅이나 쿠키 값 기타 알려지지 않은 구분방법을 통해 구별해 낸다.  

![http://2.bp.blogspot.com/-3ylGBdjKA08/VH5MJ0jAuYI/AAAAAAAAAC4/m8QhettQP1Y/s1
600/cat_captcha.png](http://2.bp.blogspot.com/-3ylGBdjKA08/VH5MJ0jAuYI/AAAAAAA
AAC4/m8QhettQP1Y/s1600/cat_captcha.png)

[[PNG external image]](http://2.bp.blogspot.com/-3ylGBdjKA08/VH5MJ0jAuYI/AAAAA
AAAAC4/m8QhettQP1Y/s1600/cat_captcha.png)

  
모바일 버전의 경우 맞는 그림 찾기가 실행된다.  

![http://4.bp.blogspot.com/-sLrMDmf4gOc/VH5MJRg7VnI/AAAAAAAAACU/svXWqwOpyds/s1
600/CAPTCHA.png](http://4.bp.blogspot.com/-sLrMDmf4gOc/VH5MJRg7VnI/AAAAAAAAACU
/svXWqwOpyds/s1600/CAPTCHA.png)

[[PNG external image]](http://4.bp.blogspot.com/-sLrMDmf4gOc/VH5MJRg7VnI/AAAAA
AAAACU/svXWqwOpyds/s1600/CAPTCHA.png)

  
그때 마저도 사람과 구분이 안된다면 전통적인 캡차를 실행한다.  

[[edit](http://rigvedawiki.net/r1/wiki.php/CAPTCHA?action=edit&section=6)]

## 6. 한국에서는? ¶

한국에서는 좀처럼 보기 힘든 인증 시스템이기도 하다. 한국은 기본적으로 대부분의 사이트에 가입시
[주민등록번호](%EC%A3%BC%EB%AF%BC%EB%93%B1%EB%A1%9D%EB%B2%88%ED%98%B8.md)나 핸드폰
번호, [공인인증서](%EA%B3%B5%EC%9D%B8%EC%9D%B8%EC%A6%9D%EC%84%9C.md) 같은 인증 가능한 제한적
수단을 요구하기 때문에 굳이 CAPTCHA가 필요하지 않은 상황이다. 정 스패머가 이런 과정을 거쳐 정상 등록을 한다손 쳐도 그냥 그 계정을
차단해버리면 그만이다. 인증용으로 사용되는 특정 주민번호나 전화번호 등에 아이디 생성 개수 제한이 걸려있기 때문에 돌려쓰기도 불가능한고로
오래 버티기도 힘들다.

  

따라서 매우 편하고 좋다고 생각할 수 있겠지만...대신 반대로 사이트 자체의 보안이 취약해진다는 문제가 지적되고 있다. 이런 식으로
인증처리를 할 경우 대부분 <del>저주받은</del> **[ActiveX](ActiveX.md)**를 사용하기 때문에 악성프로그램이
유포될 가능성이 높아지는데다가, 주민번호나 전화번호가 사이트에 저장이 되니 해킹당하면 개인의 신상정보가 속절없이 털리기 때문이다.

  

대신 CAPTCHA를 사용하면 일단 가입할 때 인증 자체는 확실히 되고, 또 사이트가 털려봐야 그 계정만 못쓰게 될 뿐 개인정보는 애초에
사이트에 저장이 되어있지 않으니 털릴 염려가 완전히 없어진다. ActiveX 같은 낡은 유통경로를 사용하는 것도 아니니 CAPTCHA를 통해
악성 코드가 유입될 가능성도 전혀 없다.`[8]`

  

한국에서는 이 CAPTCHA 대신에 그냥 아에 회원가입을 유도하는 방법을 사용해서 잘 사용되지 않는 때도 있었다. 주민번호 같은 고급 개인
정보를 너무 쉽게 수집하는 관습에 젖어서 귀찮게 CAPTCHA 같은 걸 쓰느니, 주민번호 수집을 바탕으로 회원 가입을 하면 이는 곧 사람인
것이다라는 식으로 처리한 것. 이후에 개인정보 유출 문제가 심각해져 사용이 크게 제한되면서 주민번호 같은 고급 개인 정보는 그냥 수집할 수
없고 인증 업체 등을 통하는 것으로 변경 되었다. 문제는 이런 인증 업체들을 이용하는 것은 공짜가 아니라는 것. 이에 따라 중소규모 사이트의
경우는 굳이 별도의 개인 인증을 요구하기 보다는 CAPTCHA를 이용해 인증 과정을 사용하는 경우가 늘어났다. [리그베다위키](%EB%A6%AC%EA%B7%B8%EB%B2%A0%EB%8B%A4%20%EC%9C%84%ED%82%A4.md) 역시 좋은 예시
중 하나이다.

  

![i4385157094.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/CAPTCHA/i43851
57094.jpg)

[JPG image (52.61 KB)]

  

[졷](%EC%A2%86.md)[븃신](%EB%B3%91%EC%8B%A0.md)`[9]`

  

![5521_485_0.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/CAPTCHA/5521_48
5_0.jpg)

[JPG image (20.11 KB)]

  

[붷큐](Fuck.md)[죶](%EC%A2%86.md)

  

게임 사이트에서 CAPTCHA를 이용해 인증을 하게 하는데, [한 게임사이트](%EC%97%94%EC%94%A8%EC%86%8C%ED%94%84%ED%8A%B8.md)에서는 CAPTCHA가 유저에게 욕을
썼다.(...) <del>비밀번호 잊어버린 것도 서러운데!</del>

  

![5522_363_5.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/CAPTCHA/5522_36
3_5.jpg)

[JPG image (34.61 KB)]

  

년게씌쁨렬

  

![http://thimg.todayhumor.co.kr/upfile/201412/1417773113179.jpg?width=500](htt
p://thimg.todayhumor.co.kr/upfile/201412/1417773113179.jpg)

[[JPG external
image]](http://thimg.todayhumor.co.kr/upfile/201412/1417773113179.jpg)

  
[처제](%EC%B2%98%EC%A0%9C.md)덜따먹<del>...뭐?</del>

  

[던전 앤파이터](%EB%8D%98%EC%A0%84%20%EC%95%A4%20%ED%8C%8C%EC%9D%B4%ED%84%B0.md)에서는 게임
내에서 클린패드를 입력할 수 있는데, 여기서 부적절한 단어가 나왔다.`[10]`

  

![http://i1.ruliweb.daumcdn.net/uf/image/U01/ruliweb/54E16BC43942FD000A?.jpg](
http://i1.ruliweb.daumcdn.net/uf/image/U01/ruliweb/54E16BC43942FD000A)

[[JPG external
image]](http://i1.ruliweb.daumcdn.net/uf/image/U01/ruliweb/54E16BC43942FD000A)

  
[처녀](%EC%B2%98%EB%85%80.md)굿바이

  

![http://i1.ruliweb.daumcdn.net/uf/image/U01/ruliweb/54E16BCD39462E0007?.jpg](
http://i1.ruliweb.daumcdn.net/uf/image/U01/ruliweb/54E16BCD39462E0007)

[[JPG external
image]](http://i1.ruliweb.daumcdn.net/uf/image/U01/ruliweb/54E16BCD39462E0007)

  
[어머니](%EC%96%B4%EB%A8%B8%EB%8B%88.md)[벌레](%EB%B2%8C%EB%A0%88.md)
<del>[패드립](%ED%8C%A8%EB%93%9C%EB%A6%BD.md)</del>

  

[마비노기 영웅전](%EB%A7%88%EB%B9%84%EB%85%B8%EA%B8%B0%20%EC%98%81%EC%9B%85%EC%A0%84.md)에서도 나왔다.

[[edit](http://rigvedawiki.net/r1/wiki.php/CAPTCHA?action=edit&section=7)]

### 6.1. [리그베다위키](%EB%A6%AC%EA%B7%B8%EB%B2%A0%EB%8B%A4%20%EC%9C%84%ED%82%A4.md)에서는? ¶

![제목_없음_6.JPG](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/%EC%A0%9C%EB%AA%A9
_%EC%97%86%EC%9D%8C_6.JPG)

[JPG image (13.98 KB)]

  

다섯번째 알파벳은 m인가 n인가 h인가? 이건 **매우 양호한 이미지이다.**

  

2015년경 [위키 게시판](%EC%9C%84%ED%82%A4%20%EA%B2%8C%EC%8B%9C%ED%8C%90.md)에서 사용하는
캡챠가 문제가 되기 시작했다. 글자들이 사람도 알아보기 힘들 정도로 어려워서(...) 명백한 글자가 나올 때까지 몇번이나 새로고침해야 했으며
명백히 어떤 알파벳으로 보여서 쳤는데도 틀렸다든지 하는 문제가 있어서
[유동닉](%EC%9C%A0%EB%8F%99%EB%8B%89.md)들의 불만을 증폭시켰다. 캡챠를 변경해달라는 문의가 몇번 들어왔지만
2015년 3월 초까지도 다소 늦어지고 있었..지만 3월 5일 구글이라든지에서 볼 수 있는 다른 방식으로 변경되었다.

`\----`

  * `[1]` 다른 약어, 특히 상표에서 흔히 보이는 것이지만 [직관적인 의미전달도 의도](%EC%97%AD%20%EB%91%90%EB%AC%B8%EC%9E%90%EC%96%B4.md)한 듯하다. **CAPT**ure(d) + **CHA**racter
  * `[2]` 굉장히 흠좀무한 문구인데, 이건 사실 아래 항목에서 후술하듯이, reCAPTHA가 사실 자동 처리에 실패한 고서의 단어의 인식을 누리꾼들에게 떠넘기는(...) 용도로 쓰이기 때문이다. 즉 이 리캡차를 하는 동안 사용자들은 강제로 고서를 읽게되는 셈 (...)
  * `[3]` 출처는 리더스뱅크 Level3 교재.
  * `[4]` 음성 기능은 원래 시각[장애인](%EC%9E%A5%EC%95%A0%EC%9D%B8.md)에 대한 배려 차원에서 들어간 것이다.
  * `[5]` 의심된다면 포토샵에서 아무 필터나 이용해보자. 대부분은 한번 이미지가 일그러지면 실행을 취소하지 않는 한 절대로 완벽히 되돌릴 수 없다.
  * `[6]` 그나마 어느정도 가역이 가능한, 단순한 형태뿐이기 때문에 [리그베다 위키 게시판](%EB%A6%AC%EA%B7%B8%EB%B2%A0%EB%8B%A4%20%EC%9C%84%ED%82%A4%20%EA%B2%8C%EC%8B%9C%ED%8C%90.md)의 것은 아직 뚫리지 않고 있다.
  * `[7]` 이런 식으로 자기도 모르는 새에 인간 고유의 지적 능력을 아주 조금이나마 갖다 바치도록 하는 기법을 ‘인간 기반 연산’이라고 한다. 이 분야의 선도주자는 미국 카네기 멜론 대학교의 루이스 본 안 교수. 이 교수는 reCAPTCHA 기술을 2009년에 구글에 팔았다.
  * `[8]` 물론 악의적으로 심으려고만 한다면 할 수야 있겠지만. 그렇게 따지면 못할 건 없는 거니까, 제외.
  * `[9]` [출처](http://www.pumzil.com/index.php?mid=pumzil&document_srl=12678530)는 [아이온](%EC%95%84%EC%9D%B4%EC%98%A8%20%3A%20%EC%98%81%EC%9B%90%EC%9D%98%20%ED%83%91.md) 서버별 텔레마커스 게시판에 누군가가 비번 틀렸다고 엔씨가 욕했다는 식으로 제목을 쓴 글에 나온 이미지.
  * `[10]` 전체 이용가 게임인 메이플스토리의 아이템인 [거짓말탐지기](%EA%B1%B0%EC%A7%93%EB%A7%90%ED%83%90%EC%A7%80%EA%B8%B0#s-2.md)에도 많이 나온다.(...)

