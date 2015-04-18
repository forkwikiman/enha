![http://nodejs.org/images/logos/nodejs.png](http://nodejs.org/images/logos/no
dejs.png)

[[PNG external image]](http://nodejs.org/images/logos/nodejs.png)

[로고 다운로드](http://nodejs.org/logos/)  

## Contents

    

1. 개요 
2. 예제 소스 
3. 비동기 
4. npm 
5. 기타 
6. 참조 

[[edit](http://rigvedawiki.net/r1/wiki.php/node.js?action=edit&section=1)]

## 1. 개요 ¶

node.js는 [JavaScript](JavaScript.md) 구현체인 구글 V8에 크로스플랫폼 event 처리 라이브러리인
libuv를 결합한 플랫폼이다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/node.js?action=edit&section=2)]

## 2. 예제 소스 ¶

좋아하는 에디터를 띄우고 다음과 같이 코드를 <del>복사&붙여넣기</del> 작성해보자.  

> var http = require('http');  
http.createServer(function (req, res) {  

>

> res.writeHead(200, {'Content-Type': 'text/plain'});  
res.end('Hello World\n');

>

> }).listen(1337, '127.0.0.1');  
console.log('Server running at <http://127.0.0.1:1337/>');

저장하고 터미널 등에서 'node filename' 라고 입력해주고 나서, 역시 좋아하는 브라우저를 키고 localhost:1337로
들어가면 아마 'Hello World!'라고 뜰 것 이다. `[1]` `[2]`

  

[[edit](http://rigvedawiki.net/r1/wiki.php/node.js?action=edit&section=3)]

## 3. 비동기 ¶

node.js는 고성능의 비동기 애플리케이션 작성 플랫폼으로 구상되었다. 최초 작성자인 Ryan Dahl은 웹 프로그램 분야에서 브라우저의
자바스크립트 엔진이 UI 스레드를 공유할 수 밖에 없는 환경`[3]`에서 락을 피하고자 시분할과 이벤트로 비동기 프로그램을 작성하는 모습을
보고 괜찮은 방법론이라 생각해 만들었다고 한다.

  

이때 프로그램은 리엑터 패턴에 의한 CPS로 작성되는데, 이것이 node.js에 고성능을 선사하는 기법인 동시에 비 숙련자에게 디버깅 지옥을
만드는 애증의 관계를 지니고 있다. 궁금하면 위의 간단한 http서버에서 createServer가 인자로 전달받은 함수를 http 요청에
이어지는 실행지정으로 사용한다는 점을 보도록 하자. node.js가 자랑하는 고성능 비동기 프로그램을 작성하기 위해서는 파일시스템을 포함한
프로그램 전체가 비동기화 지점마다 저렇게 CPS로 연결되어야 한다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/node.js?action=edit&section=4)]

## 4. npm ¶

[npm 사이트](https://www.npmjs.com)

  

node.js Package Manager. 자바의 Maven, Python의 PyPi 와 같은 node.js용 패키지 관리 및 배포
시스템이다. 본격적으로 node.js를 사용하려면 당연히 필수요소.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/node.js?action=edit&section=5)]

## 5. 기타 ¶

우리나라에서는 프레임웍으로 표현되기도 하는데, node.js는 자바스크립트 엔진에 API를 제공하는 기반 플랫폼(libuv)을 연결한 응용
플랫폼이라고 보는 것이 더 적당하다. node.js 홈페이지의 설명에도 플랫폼이라 표기되어 있다.

  

비동기 처리로 인하여 I/O 처리시 대단한 성능을 내는 것이 사실이고 기반이 되는 구글 V8도 꽤 빠른 성능을 내는 JIT 구현이지만 개별
프로세스 내부에서 작동하는 자바스크립트 코드는 무조건 싱글 스레드로 실행 한다는 제약이 걸려있어 병렬연산에는 취약하다. 단 node.js에서
싱글 스레드는 성능상의 제약이 아니라 프로그래밍 모델에 포함된 사양이다. 복잡한 비동기 I/O 응용 프로그램을 싱글 스레드 자바스크립트로
짜는 것이 결과물의 실행 속도와 개발 편의성 측면에서 좋다는 것이 node.js의 근간을 이루는 개념이며, 작성자인 Ryan Dahl은
순수하게 연산력이 중요한 요소는 C로 짜서 붙이라는 상식적인 사실을 이야기 했다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/node.js?action=edit&section=6)]

## 6. 참조 ¶

[Node.js 공식 문서](http://nodejs.org/api/)  
[Node.js 기본 사용법](http://pyrasis.com/nodejs/nodejs-HOWTO/)  
[생활코딩](http://opentutorials.org/course/86)  
[Socket.IO](http://socket.io)

`\----`

  * `[1]` 사실 [Node.js 홈페이지](http://nodejs.org)에 나와있다
  * `[2]` node.js가 설치되어 있어야 한다.
  * `[3]` 브라우저가 DOM API와 자바스크립트 엔진을 동기화 하기 위해서는 어쩔 수 없다.

