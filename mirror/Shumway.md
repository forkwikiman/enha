2012년부터 [모질라](%EB%AA%A8%EC%A7%88%EB%9D%BC.md) 재단에서 개발하고 있는 플래시 플러그인의 대체품.
순수한 HTML5 만으로 플래시 런타임의 기능을 구현하고자 한다.

공식홈: <http://mozilla.github.io/shumway/>  
Github: <https://github.com/mozilla/shumway>

## Contents

    

1. 개요 
2. 성능 

[[edit](http://rigvedawiki.net/r1/wiki.php/Shumway?action=edit&section=1)]

## 1. 개요 ¶

  

2012년 11월, [모질라](%EB%AA%A8%EC%A7%88%EB%9D%BC.md)에서 순수한 웹 기반의 기술로 플래시를 대체하기
위한 프로젝트, Shumway를 개발 중이라고 발표했다. [발표
내용](https://blog.mozilla.org/research/2012/11/12/introducing-the-shumway-open-
swf-runtime-project/) 순수한 HTML5 기술으로 브라우저 내에서 .SWF 파일을 실행할 수 있도록 하는 것이 목표라고
한다. 모질라는 이를 통해 오픈 웹과 웹 표준을 한 걸음 진보시킬 수 있을 것으로 기대하고 있다.

  

2012년 초부터 개발되었으며, 현재 파이어폭스용 부가 기능으로 제공되고 있다. 파이어폭스 Nightly를 쓰고 있다면
about:config에서 shumway를 활성화할 수 있다. 오픈 소스와 오픈 웹을 지지하는 사람이고, 파이어폭스를 사용 중이라면 한 번
쯤 써볼만 하다. 부가 기능은
[여기를](http://mozilla.github.io/shumway/extension/firefox/shumway.xpi) 클릭하면 설치할
수 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Shumway?action=edit&section=2)]

## 2. 성능 ¶

  

아직... 매우... 느리다.  
어도비의 플래시 런타임과 비교과 안될 정도로 느리다. 그리고 파이어폭스에 설치한 경우, 플래시 플러그인을 대체하지 않기 때문에
Shumway를 설치하고 플래시 플러그인을 비활성화해버리면 유투브 등 비디오 사이트들에서는 플래시가 설치되어 있지 않다고 경고가 뜨거나,
그냥 HTML5 플레이어를 보여준다. 그렇다고 플래시를 활성화하면 Shumway 대신 플래시를 사용한다.(...) 단순하게 swf 파일을
임베드해놓은 웹페이지들에서는 이런 문제는 없다.  
아직 여러 비디오 사이트들에 대한 지원이 완전하지는 않지만, 활발하게 개발이 진행되고 있으므로 조만간 유투브, 데일리모션, 비메오 등에 대한
지원이 추가될 것이 기대된다.  
몇몇 플래시 게임은 구동할 수 있다. 다만 좀 버벅대는 것과 느린 초기 구동 속도를 견뎌야 한다.  
아직 개발 초기 단계이니 안되는 게 더 많아도 이해하자.

