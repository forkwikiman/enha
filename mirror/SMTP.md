간이 우편 전송 프로토콜(Simple Mail Transfer Protocol)의 약자. 이메일 전송에 사용되는 네트워크 프로토콜이다.

인터넷에서 메일 전송에 사용되는 표준이다. 1982년 RFC821에서 표준화되어 현재는 RFC5321에서 정의된 ESMTP(Extended
SMTP; 확장 SMTP)로 2008년 갱신되었다. SMTP는 보안과 호환성의 문제로 그대로는 사용하지 않는 경우가 많다. 일반적으로 쓰이는
확장 프로그램은 SMTP-AUTH(송신자 인증 서비스), [ESMTP](ESMTP.md)([SASL](SASL.md)을 이용한
보안 연결), [MIME](MIME.md)(non-ascii 데이터 전송 포맷)가 있다.

SMTP는 25/tcp와 587/tcp 포트를 사용하며 SMPTS는 465/tcp 포트를 사용한다.

SMTP는 연결지향적이고 텍스트 기반으로 작동하는 프로토콜이다. SMTP 클라이언트와 SMTP 서버 사이에 **SMTP 세션**이 생성되며,
명령행을 이용해 메일을 송수신한다. **SMTP 교환**은 다음의 세 명령어를 통해 이루어진다.  

  1. MAIL 명령어: 수신자 지정
  2. RCPT 명령어: 송신자 지정
  3. DATA 명령어: 메시지 내용의 시작이 되는 부분이다. 메시지 헤더와 바디로 구성된다.  
  

SMTP 세션의 예:  

> S: 220 smtp.example.com ESMTP Postfix  
C: HELO relay.example.org  
S: 250 Hello relay.example.org, I am glad to meet you  
C: MAIL [FROM:＜[email
protected]＞](/wiki/FROM%3A%EF%BC%9Cbob%40example.org%EF%BC%9E)  
S: 250 Ok  
C: RCPT [TO:＜[email
protected]＞](/wiki/TO%3A%EF%BC%9Calice%40example.com%EF%BC%9E)  
S: 250 Ok  
C: RCPT [TO:＜[email
protected]＞](/wiki/TO%3A%EF%BC%9Ctheboss%40example.com%EF%BC%9E)  
S: 250 Ok  
C: DATA  
S: 354 End data with ＜CR＞＜LF＞.＜CR＞＜LF＞  
C: From: "Bob Example" ＜[[email protected]](http://rigvedawiki.net/cdn-cgi/l
/email-protection)＞  
C: To: "Alice Example" ＜[[email protected]](http://rigvedawiki.net/cdn-cgi/l
/email-protection)＞  
C: Cc: [[email protected]](http://rigvedawiki.net/cdn-cgi/l/email-protection)  
C: Date: Tue, 15 January 2008 16:02:43 -0500  
C: Subject: Test message  
C:  
C: Hello Alice.  
C: This is a test message with 5 header fields and 4 lines in the message
body.  
C: Your friend,  
C: Bob  
C: .  
S: 250 Ok: queued as 12345  
C: QUIT  
S: 221 Bye  
{The server closes the connection}

