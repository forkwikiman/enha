  * 상위 항목 : [iOS](iOS.md)  

## Contents

    

1. 개요 
2. 해결 방법 
3. 참고 

[[edit](http://rigvedawiki.net/r1/wiki.php/iOS%20%EA%B4%B4%EB%AC%B8%EC%9E%90%2
0%EB%B2%84%EA%B7%B8?action=edit&section=1)]

## 1. 개요 ¶

<del>말 그대로 **[보면 죽는 문자](3%EB%B2%88%20%EB%B3%B4%EB%A9%B4%20%EC%A3%BD%EB%8A%94%20%EA%B7%B8%EB%A6%BC.md)** iOS의 [BLIT](BLIT.md) 본격 현실화된
[도시전설](%EB%8F%84%EC%8B%9C%EC%A0%84%EC%84%A4.md)</del>

  

[Bug In Apple’s CoreText Allows Specific String Of Characters To Crash iOS 6,
OS X 10.8 Apps](http://techcrunch.com/2013/08/29/bug-in-apples-coretext-
allows-specific-string-of-characters-to-crash-ios-6-os-x-10-8-apps/) 기사에서 언급된
괴문자와 관련된 버그를 이르는 말.

  

![iOS괴문자.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/iOS%EA%B4%B4%EB%AC%
B8%EC%9E%90.jpg)

[JPG image (6.64 KB)]

  
※ 여기에 표시된 문자열은 이미지로 되어 있다. [iOS](iOS.md) 유저라도 안심해도 된다.

  

일단 해당 문자열 자체에는 아무런 뜻이 담겨 있지 않지만, 이게 기술적인 문제를 불러일으키는 것으로 유명하다.

  

이 아랍 문자를 [iOS](iOS.md) 6과 [OS X](OS%20X.md) 10.8에서 띄우면 프로그램이 뻗거나, 최악의 경우
OS가 탑재된 제품 자체에 치명적인 타격을 준다. iOS 7과 OS X 10.9(Marvericks)에서는 피해 보고가 아직 없다. 이는
iOS와 OS X에 탑재된 Cocoa 프레임워크의 일부분인 CoreText API의
[유니코드](%EC%9C%A0%EB%8B%88%EC%BD%94%EB%93%9C.md) 텍스트 렌더링 부분에
[버그](%EB%B2%84%EA%B7%B8.md)가 있어서 그렇다고. iOS 7과 OS X 10.8.5 업데이트에서 버그가 수정되었다.

  

이 문자열을 [블로그](%EB%B8%94%EB%A1%9C%EA%B7%B8.md) 포스트에 쓰거나
[트위터](%ED%8A%B8%EC%9C%84%ED%84%B0.md) 등에서 이 문자열이 들어간 트윗을 RT할 경우, iOS 6이나 OS
X 10.8을 쓰는 사람을 상당히 빡치게 만들 수 있다. 하지만 일부
[무개념](%EB%AC%B4%EA%B0%9C%EB%85%90.md)들이 아무 게시판 글이나 댓글에 문자열를 달고 있다. 그럴 때에는
신고해주자.

  

[이 글](http://blog.miyu.kr/150)에 따르면, 구체적으로는 다음과 같은 문제가 발생한다고 한다.  

  * 해당 문자열이 포함된 웹 페이지에 들어갈 경우: 웹 브라우저가 죽는다.
  * 해당 문자열이 포함된 푸시 메시지를 수신할 경우: 단말기가 리붓된다. 리붓된 상태에서 푸시 로그를 확인하면 또다시 리붓된다.
  * 메신저로 해당 문자열을 수신할 경우: 메신저 푸시가 뜨면서 단말기가 리붓된다. 메신저로 들어가면서 수신한 메시지를 보려고 하면 메신저가 죽는다.
  * 누군가가 [Wi-Fi](Wi-Fi.md)의 SSID로 해당 문자열을 쓸 경우: 설정 앱에서 Wi-Fi SSID를 검색하는 순간 바로 설정 앱이 다운된다.
사실 엄밀히 말해서 텍스트 렌더링 오류를 내는 부분은 해당 문자열 전체가 아니라, 저 글에서 지적된 것과 같이 해당 문자열의 일부이다.
실제로 저 글에서 지적한 부분만 띄워도 위와 같은 증상이 확인된다.

  

[페이스북](%ED%8E%98%EC%9D%B4%EC%8A%A4%EB%B6%81.md)은 이 문자열을 담벼락이나 타임라인에 올릴 수
없도록 차단했다. [트위터](%ED%8A%B8%EC%9C%84%ED%84%B0.md) 또한 이 문자열을 트윗하지 못하도록 차단했지만,
이 문자열이 포함된 기존 트윗을 RT할 수는 있기 때문에 주의해야 한다.그리고 [네이버웹툰](%EB%84%A4%EC%9D%B4%EB%B2%84%20%EC%9B%B9%ED%88%B0.md)에서도 차단되었다. 그 외
차단된사이트는 [추가바람](%EC%B6%94%EA%B0%80%EB%B0%94%EB%9E%8C.md).

  

[[edit](http://rigvedawiki.net/r1/wiki.php/iOS%20%EA%B4%B4%EB%AC%B8%EC%9E%90%2
0%EB%B2%84%EA%B7%B8?action=edit&section=2)]

## 2. 해결 방법 ¶

OS X 사용자는 10.9(Marvericks) 버전 또는 10.8.5 버전으로 업데이트하면 해결된다.

  

iOS가 탑재된 기기를 사용하는 유저들은 기기를 iOS 7 버전으로 업데이트하거나, iOS 6 이전 버전의 기기를
[탈옥](%ED%83%88%EC%98%A5#s-2.2.md)한 유저는
[Cydia](%EC%8B%9C%EB%94%94%EC%95%84.md)의 기본 소스인 Cydia/Telesphoreo에서
GlyphPatch 패키지를 찾아서 설치하거나 [보안 수정
코드](https://github.com/FilippoBiga/GlyphPatch)를 참조해서 직접 수정하면된다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/iOS%20%EA%B4%B4%EB%AC%B8%EC%9E%90%2
0%EB%B2%84%EA%B7%B8?action=edit&section=3)]

## 3. 참고 ¶

  * [iOS6 및 Mac OS X 10.8에 심각한 버그 특정 텍스트](http://bbs2.ruliweb.daum.net/gaia/do/ruliweb/default/56/read?bbsId=G003&articleId=1184988&itemId=8)
  * [텍스트 한줄로 iOS와 OS X 앱을 강제로 충돌시킬 수 있는 심각한 취약점 발견! 보안 업데이트 시급](http://macnews.tistory.com/1507)
  * [해당 문자열이 포함된 트윗](https://twitter.com/codeblue87/status/372954308397920256)`[1]`

`\----`

  * `[1]` 현재는 트위터측에서 트윗 내용을 바꿔 둔 상태라 iOS 구버전 사용자도 들어가도 괜찮다.

