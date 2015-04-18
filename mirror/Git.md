## Contents

    

1. Git 
2. Git 사용법 배우기 
3. 기타 

[[edit](http://rigvedawiki.net/r1/wiki.php/Git?action=edit&section=1)]

## 1. Git ¶

[리누스 토르발스](%EB%A6%AC%EB%88%84%EC%8A%A4%20%ED%86%A0%EB%A5%B4%EB%B0%9C%EC%8A%A4.md)가 개발한 분산 버전 관리 [프로그램](%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%A8.md). 혹자는
리누스 토르발스가 리눅스를 개발하지 않았더라도 이놈으로 인해서 존경을 받았을 것이라고 주장하기도 한다. 오픈소스는 공산주의라고 까던
[MS](MS.md)가 Git을 잘 써먹고 있으며, 페이스북, 트위터, 모질라 등등에서도 Git를 잘 써먹고 있다. Git은 리누스
토르발즈가 [리눅스](%EB%A6%AC%EB%88%85%EC%8A%A4.md) 커널 관리를 위해서 개발한 놈인데, 매우 빠른
속도`[1]`와 분산형 저장소 지원이 특징이다. 오픈소스 개발의 특성상 여럿이 달려들어 자기 맘에 드는걸 하기도 하며, 또한 잘못 붙었다
이상한걸 건드려 망하기 쉬운 환경으로 인해 Git는 다음과 같은 체제를 갖고 있다. 일단 Git의 작업 폴더는 전체 기록과 각 기록을 추적할
수 있는 정보를 포함하고 있는 저장소이다. 즉 자기 컴퓨터에 모든 파일을 다 받아서 하는 셈. 위키로 치자면 위키 전체를 다 받아서 수정하는
것과 같다.`[2]`

  

작업이 끝나면 Git 원격 저장소로 다시 발행하는데, 여기에도 원 저장소를 보호하기 위한 가지치기가 있어 가지의 개발이 완료될 시 원
저장소와 합칠 수 있으며, 또한 개발 중간중간 꼬리표를 매겨 개발을 더 수월하게 할 수 있다.

  

이런 강력한 Git를 호스팅 해주는 [Github](https://github.com/)란 곳이 자유 소프트웨어의 성지로 부각되고 있다.
여기엔 오픈소스 프로젝트라면 뭐든지 올라올 수 있기 때문에 가끔 뭔가 괴한 것들이 올라오기도 하는데 몇몇 예를 들어보자면,  

  * <https://github.com/jmechner/Prince-of-Persia-Apple-II> [페르시아의 왕자](%ED%8E%98%EB%A5%B4%EC%8B%9C%EC%95%84%EC%9D%98%20%EC%99%95%EC%9E%90.md) 오리지널 버전 소스: 공개자는 조던 메크너 본인. 근데 워낙 예전 소스라 자기도 기억 안 나니까 궁금한 거 있어도 묻지 말라고 써 놨다. 더군다나 사용언어는 [애플 II](%EC%95%A0%ED%94%8C%20II.md) [어셈블리어](%EC%96%B4%EC%85%88%EB%B8%94%EB%A6%AC%EC%96%B4.md)(...).
  * [남자친구 구인광고](https://github.com/norinori2222/boyfriend_require): 체크하여 점수도 내어주는 스크립트도 있다! <del>스스로 조건에 맞는다고 생각하는 [위키니트](%EC%9C%84%ED%82%A4%EB%8B%88%ED%8A%B8.md)라면 메일 보내보자</del> \- 엄청난 인기를 얻었으며(이공계에 여자가 없다보니) 남자친구를 구했는지 삭제 되었다.
  * [아예 이슈트래커만 사용해서 집안일 관리](https://github.com/frabcus/house/issues): README파일이 가관이다. "My house has no source code, so I only use the issue tracker."(...). 더군다나 이 레포지토리는 2012년 12월말 현재 github에서 트렌드 1위를 먹고 있다!!
  * 모 Git 강좌 책은 책을 쓸때 Git을 사용해서 집필했다고 한다. 그리고 그걸 예제로 Git의 장점을 설명한다(...)(그런데 GitBook라는 서비스는 GitHub랑 연결해서 실제 책을 집필하게 해준다! <del>[몰라 뭐야 이거 무서워](%EB%AA%B0%EB%9D%BC%20%EB%AD%90%EC%95%BC%20%EC%9D%B4%EA%B1%B0%20%EB%AC%B4%EC%84%9C%EC%9B%8C.md)</del>)
  * GitHub은 Gollum 이라는 MarkDown 을 사용하는 위키와 Jekyll 이라는 정적 CMS 프로그램을 내장하고 있다. 이를 적극 활용하면 GitHub만 가지고도 혼자나 소수의 사람이 쓰는 데에는 지장이 없을 정도의 위키나 블로그를 GitHub 상에서 운용할 수 있다. 이 GitHub의 Jekyll에 얹을 수 있는 WordPress의 클론인 OctoPress 라는 블로그 프로그램도 존재한다. OctoPress의 댓글은 정적 컨텐츠의 한계로 인해 DisQus 로 처리한다고 한다.   

(...)

  

그 외에 돈 내면 비공개 프로젝트도 생성 가능하며, 실제 현장에서 서버 돌리기는 뭣할때 여기를 사용해서 프로젝트를 호스팅하는 경우도 있다.
"비공개 프로젝트가 필요한데 유료라 쓰기 애매하다 + 팀원이 몇 명 안된다"같은 상황이라면
[BitBucket](https://bitbucket.org/)도 괜찮은 대안이 될 수 있다. 이쪽은 5명`[3]` 이하가 참여하는
프로젝트라면 비공개 프로젝트도 무료로 생성 가능.

  

이러한 외부에서 제공되는 서비스 형태가 아닌, 설치형 Git 서버는 [리눅스](%EB%A6%AC%EB%88%85%EC%8A%A4.md)
서버라면 별다른 추가 프로그램 없이 리눅스의 기본 프로그램(SSH 등)과 배포본에 들어있는 패키지 만으로도 서버를 구동할 수 있다. 그 밖에
유닉스 계열 서버에서도 손쉽게 설정할 수 있다. 그런데 윈도우라면 쉽게 답이 나오지 않았는데,
[gitbucket](https://github.com/takezoe/gitbucket) 이라는 JVM 기반에 Scala 로 GitHub 을
흉내내어 작성된 오픈소스 프로그램이 등장했다. JVM 구동으로 메모리를 많이 먹는 단점을 제외하면 HTTP는 물론, <del>윈도우에서
운용하려면 매우 번거롭고 짜증나는</del> SSH와 메일 알림 같은 여러 서버 기능을 자체적으로 지원하며, GitHub 의 상당히 많은
기능을 매우 비슷하게 구현해 놓았기 때문에 GitHub을 쓰던 사람이라면 거의 그대로 사용할 수 있고, 그렇지 않더라도 GitHub 처럼
매우 쉽게 쓸 수 있다는 장점이 있다.

[[edit](http://rigvedawiki.net/r1/wiki.php/Git?action=edit&section=2)]

## 2. Git 사용법 배우기 ¶

인터넷에 공개된 자료가 매우 많다.

  

  * [간단히 보는 git 사용법](http://rogerdudler.github.io/git-guide/index.ko.html)
  * [Git 브랜치 배우기 튜토리얼](http://learnbranch.urigit.com/?demo)
  * [progit](http://dogfeet.github.io/articles/2012/progit.html) github의 CIO가 직접 쓴 책을 번역한 자료. 
  * [책](http://www.insightbook.co.kr/post/5633)으로도 나와 있다.  

[[edit](http://rigvedawiki.net/r1/wiki.php/Git?action=edit&section=3)]

## 3. 기타 ¶

리누스 토르발스는 [Subversion](Subversion.md)을 아주 싫어하며 대놓고 깐다. [구글에서 GIT
강연](http://www.youtube.com/watch?v=4XpnKHJAok8)

  

> 오픈소스계의 영원한 아이돌 리누스 토르발스는 리눅스 커널을 관리하는 기존 툴이 엉망인 것에 너무 빡친 바람에 git이라는 소스관리 툴을
만든다. 그게 리누스에게 얼마나 깊은 빡침이었는지, **단 2주만**에 완성하는 기염을 토했다 (그러고는 후에 **“git 만드는게 제일
쉬웠어요”** 라는 인터뷰를 했다.).

  

\- [오픈소스의 승리](http://sangminpark.wordpress.com/2013/04/22/%ec%98%a4%ed%94%88%e
c%86%8c%ec%8a%a4%ec%9d%98-%ec%8a%b9%eb%a6%ac/)에서 발췌  

엔하위키의 위키엔진인 [모니위키](%EB%AA%A8%EB%8B%88%EC%9C%84%ED%82%A4.md)도 Git으로 관리되고 있다.
중앙 서버는 예상되듯이 Github. <https://github.com/wkpark/moniwiki>

`\----`

  * `[1]` 방대한 리눅스 커널 소스코드를 생각해보라. 속도 문제가 매우 중요해질 수 밖에 없다. <del>개발자가 커널 코어 개발자니 안 빠를 수가 없다</del>
  * `[2]` git이 아니더라도 DVCS(분산 버전관리 시스템)에 해당하는 Mercurial이나 Bazaar도 해당하는 사항이다.
  * `[3]` 메일로 회원을 <del>[다단계](%EB%8B%A4%EB%8B%A8%EA%B3%84.md)</del>초대하면 8명까지 가능.

