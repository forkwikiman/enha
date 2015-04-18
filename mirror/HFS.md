  * [동음이의어](%EB%8F%99%EC%9D%8C%EC%9D%B4%EC%9D%98%EC%96%B4.md), [컴퓨터 관련 정보](%EC%BB%B4%ED%93%A8%ED%84%B0%20%EA%B4%80%EB%A0%A8%20%EC%A0%95%EB%B3%B4.md)  

## Contents

    

1 파일 전송 서버

2 파일 시스템

[[편집](http://rigvedawiki.net/r1/wiki.php/HFS?action=edit&section=1)]

## 1 파일 전송 서버 ¶

![hfs.png](http://z2.enha.kr/http://rigvedawiki.net/r1/pds/HFS/hfs.png)

  
<http://www.rejetto.com/hfs>  
HFS - http file server  
http를 기반으로 하는 파일 전송 서버이다. [베리즈](%EB%B2%A0%EB%A6%AC%EC%A6%88.md)와 유사하게 단 하나의
실행파일로 동작한다.  
easy 모드를 쓸 경우 베리즈 처럼 간단히 쓸수 있고 전문가 모드를 사용하면 MIME 타입도 설정할수 있는 고급 프로그램이다.

  

다만 사용을 주의해야 한다. 일부 백신에서는 riskware`[1]` trojan으로 분류하기 때문이다. 단순히 서버를 생성하기에
경고하는것이 아니다. 소켓에 직접 접속, 키보드 입력을 직접 접근하는 등 악성코드가 주로 하는 행위를 한다. 웹서버 프로그램은 이러한 기능
없이도 구현이 가능하다. 퍼포먼스에 민감한 게임마저도 운영체제가 제공하는 일반적인 기능을 사용하지 이렇게 직접 접근은 안한다. 예외가 있다면
보안프로그램이 보호를 위해 직접적으로 접근하는정도? [관련글](http://www.rejetto.com/forum/f-a-q-s/virus-
alert-about-hfs) 에서 제작자는 백신이 문제라고 변명을 하고 있지만 상식적으로 웹서버 프로그램이 키보드에 직접 접근할 이유가
없다.

[[편집](http://rigvedawiki.net/r1/wiki.php/HFS?action=edit&section=2)]

## 2 파일 시스템 ¶

Hierarchical File System

  

[애플](%EC%95%A0%ED%94%8C%28%EA%B8%B0%EC%97%85%29.md)이 개발해서 [맥OS](%EB%A7%A5%20OS.md)이 사용하는 파일 시스템. 한국어로 굳이 옮기자면 계층적 파일 시스템 정도가 되겠다.

  

맥OS에서부터 감이 팍팍 오지만, 이 파일 시스템은 개발된 지 25년이 넘은 구닥다리 파일 시스템이다. 파일 하나당 최대 용량도
2기가바이트, 파티션당 파일 개수는 65536개, 파일명이 최대 31자밖에 안 되는 갑갑한 물건이다.`[2]` 만약
[부트캠프](%EB%B6%80%ED%8A%B8%EC%BA%A0%ED%94%84.md)를 쓰고 있다면
[윈도](Microsoft%20Windows.md)에서 제한적으로 읽기가 가능하다.

  

워낙에 케케묵은 파일 시스템인지라 OS X이 등장한 이후에는 잘 쓰이지 않고`[3]`, 상위 버전인 HFS+(Mac OS Extended)가
쓰인다.

`\----`

  * `[1]` 정상 작동은 하나 잠재적 위험이 있는 프로그램
  * `[2]` 물론 이것이 널리 사용되던 당시 DOS의 8.3 형식의 제한보다는 훨씬 나았으나...
  * `[3]` 아예 제대로 지원하지 않는다.

