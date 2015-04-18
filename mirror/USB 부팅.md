  * [컴퓨터 관련 정보](%EC%BB%B4%ED%93%A8%ED%84%B0%20%EA%B4%80%EB%A0%A8%20%EC%A0%95%EB%B3%B4.md)
  * 상위 항목 : [USB 메모리](USB%20%EB%A9%94%EB%AA%A8%EB%A6%AC.md)  

## Contents

    

1. 개요 
2. 과정 
    

2.1. 준비물

3. 분류 및 방법 
    

3.1. [Windows](Windows.md) OS USB 부팅

3.2. [Mac OS](Mac%20OS.md) USB 부팅

3.3. [리눅스](%EB%A6%AC%EB%88%85%EC%8A%A4.md)계열 OS와 그 외 여러 OS USB 부팅

4. 오류 해결방법 
    

4.1. USB에 [Windows XP](Windows%20XP.md) 설치 ISO파일을 기록했을 때의 문제

5. 장점과 단점 
    

5.1. 장점

5.2. 단점

6. 기타 

[[edit](http://rigvedawiki.net/r1/wiki.php/USB%20%EB%B6%80%ED%8C%85?action=edi
t&section=1)]

## 1. 개요 ¶

먼저 [부팅](%EB%B6%80%ED%8C%85.md)(Booting)이란, 사용자가 컴퓨터를 켰을 때
[운영체제](%EC%9A%B4%EC%98%81%EC%B2%B4%EC%A0%9C.md)를 구동하기 위해 일어나는 초기 구동의 과정을
말한다. 컴퓨터의 전원이 들어왔을 때 비로소 부팅의 과정이 일어난다. 운영체제는
[하드디스크](%ED%95%98%EB%93%9C%EB%94%94%EC%8A%A4%ED%81%AC.md), [CD](CD.md),
[DVD](DVD.md), 플래시메모리 카드, [USB](USB.md),
[플로피디스크](%ED%94%8C%EB%A1%9C%ED%94%BC%EB%94%94%EC%8A%A4%ED%81%AC.md) 등에 설치가
가능하며 본 항목에서는 USB 메모리를 이용한 부팅만을 서술한다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/USB%20%EB%B6%80%ED%8C%85?action=edi
t&section=2)]

## 2. 과정 ¶

**부팅용 USB 메모리를 만들기에 앞서 일단 지금 사용하는 운영체제와 하드디스크를 [백업](%EB%B0%B1%EC%97%85.md) 해놓자.** BIOS를 건드리기 때문에 한순간에 모든 데이터를 날려버릴 가능성이 상주한다. 이는 CD 설치도 마찬가지이다. 

[[edit](http://rigvedawiki.net/r1/wiki.php/USB%20%EB%B6%80%ED%8C%85?action=edi
t&section=3)]

### 2.1. 준비물 ¶

  * USB 메모리 (8GB, 트랜센드나 삼성같은 메이저 제조사를 이용하길 권장)`[1]`  
최소 4GB 용량의 USB를 준비하는 것이 좋다. 보통
[토렌트](%ED%86%A0%EB%A0%8C%ED%8A%B8.md)<del>어둠의 경로</del>및 웹하드를 통해 ISO 파일을 얻는데
이 경우 퍼스널라이징이 되거나 Windows 7이후의 운영체제는 32bit와 64bit가 묶여 있는 경우(마이크로소프트 OS 한정)가 있기
때문에 최소 4GB도 조금 빠듯한 게 사실이다. 거기다가 **[표기보다 작은 하드디스크](%ED%91%9C%EA%B8%B0%EB%B3%B4%EB%8B%A4%20%EC%9E%91%EC%9D%80%20%ED%95%98%EB%93%9C%EB%94%94%EC%8A%A4%ED%81%AC.md)의 특성을 USB 메모리도 그대로 따라가기 때문에** 실제 들어가는 용량은 4GB보다 작다. 4GB면 3.75GB정도로, 윈도우를
넣고 보조프로그램<del>과 야동</del>을 넣으려 했더니 용량이 꽉 차 못 들어가는 눈물나는 사태가 발생할 수 있다. 16GB USB가
매우 저렴해졌으니 16GB를 애용하자.

  * Ultra ISO  
포탈에서 다운받는 Ultra ISO는 기간제 체험판인 경우가 다수이다. 정품을 애용하자. 부팅 USB만 만드는게 목적이라면 대체제로
Rufus라는 툴을 이용할 수 있다. 참고로 이건 **무료**인데다가
**[오픈소스](%EC%98%A4%ED%94%88%EC%86%8C%EC%8A%A4.md)**. 리눅스라면 UUI란 프로그램을 이용할 수
있다. 모든 리눅스를 지원한다고 해도 과언이 아니다. **울트라ISO는 리눅스 USB부팅을 지원하지 않는다.**

  * 각 운영체제의 ISO 파일  
없어선 안 될 가장 중요한 준비물. 만약 못 구했다면? 못 한다. <del>망했어요</del>

  * 자신 컴퓨터에 설치된 [BIOS](BIOS.md)/[UEFI](UEFI.md)에 대한 사전 지식  
일반적으로 Award, Phoenix, Insyde, AMI등이 설치돼있다. 다른 건 몰라도 부팅 순서 변경하는 방법은 알아 놓도록 하자.
일반적으로 F11, F12, Del키중 하나를 누르면 부팅메뉴로 들어간다.

[[edit](http://rigvedawiki.net/r1/wiki.php/USB%20%EB%B6%80%ED%8C%85?action=edi
t&section=4)]

## 3. 분류 및 방법 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/USB%20%EB%B6%80%ED%8C%85?action=edi
t&section=5)]

### 3.1. [Windows](Windows.md) OS USB 부팅 ¶

[Windows 8.1](Windows%208.1.md)인 경우, 별다른 설정 없이 UEFI 모드로 설치가 가능하다.`[2]` 사용중인
메인보드의 UEFI 내장 드라이버에 따라 특정 파일시스템이 지원 되지 않는 경우가 있다.

  

[Windows 7](Windows%207.md) 이상의 운영체제의 경우 Windows 7 USB/DVD 다운로드 도구를 이용할 수
있다.

[[edit](http://rigvedawiki.net/r1/wiki.php/USB%20%EB%B6%80%ED%8C%85?action=edi
t&section=6)]

### 3.2. [Mac OS](Mac%20OS.md) USB 부팅 ¶

  * PC상 설치는 [OS X](OS%20X.md) 항목 5번 해킨토시 참조 

[[edit](http://rigvedawiki.net/r1/wiki.php/USB%20%EB%B6%80%ED%8C%85?action=edi
t&section=7)]

### 3.3. [리눅스](%EB%A6%AC%EB%88%85%EC%8A%A4.md)계열 OS와 그 외 여러 OS USB 부팅 ¶

  * 리눅스나 BSD 계열이라면 UUI를 쓰면 된다. 그러나 이 프로그램은 윈도우에서만 돌아간다.(...) 자신의 컴퓨터의 OS가 [우분투](%EC%9A%B0%EB%B6%84%ED%88%AC.md)라면 '시동 디스크 만들기'를 쓰면 된다. 그러나 이것으로는 윈도우 부팅 USB는 만들 수 없다.   

[[edit](http://rigvedawiki.net/r1/wiki.php/USB%20%EB%B6%80%ED%8C%85?action=edi
t&section=8)]

## 4. 오류 해결방법 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/USB%20%EB%B6%80%ED%8C%85?action=edi
t&section=9)]

### 4.1. USB에 [Windows XP](Windows%20XP.md) 설치 ISO파일을 기록했을 때의 문제 ¶

> INF file txtsetup.sif is corrupt or missing, status 18.  
Setup cannot continue. Press any key to exit.

  

일반적으로 Ultra ISO를 이용해 Windows 7 부팅 USB를 만드는 대로 Windows 부팅 Usb를 만들었을때 발생하는 오류이다.  
위키니트들은 당황하지 말고 Windows 7 ISO도 추가로 준비해주자 <del>그럴꺼면 뭐하러 Windows XP를 까냐</del>  
현재는 윈도우 XP의 보안 지원이 중단되었으므로 쓰지 말자.

[[edit](http://rigvedawiki.net/r1/wiki.php/USB%20%EB%B6%80%ED%8C%85?action=edi
t&section=10)]

## 5. 장점과 단점 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/USB%20%EB%B6%80%ED%8C%85?action=edi
t&section=11)]

### 5.1. 장점 ¶

  * 적절하게 빠르다
  * 소음이 없다
  * USB 안에 드라이버 등을 넣을수 도 있다.`[3]`<del>공구 아니다.</del>  

[[edit](http://rigvedawiki.net/r1/wiki.php/USB%20%EB%B6%80%ED%8C%85?action=edi
t&section=12)]

### 5.2. 단점 ¶

  * USB가 안 좋은 경우 아주 미치고 팔짝 뛰게 만든다
  * 아무 프로그램으로 구울 수 있는 CD, DVD와는 달리 OS마다 다른 프로그램이 필요하다

[[edit](http://rigvedawiki.net/r1/wiki.php/USB%20%EB%B6%80%ED%8C%85?action=edi
t&section=13)]

## 6. 기타 ¶

  * 외장하드도 가능하다. 그러나 외장하드가 있고 윈도우 8 이상을 설치할 것이라면 Windows to go를 쓰는게 낫다. 

`\----`

  * `[1]` 샌디스크나 도시바는 이상하게 잘 안 되는 경향이 있다. 특히 리눅스. 노트북에 ODD가 없어 USB로 설치해야 하는데 6개의 리눅스가 하나도 먹히지 않는 막장 사태가 발생하면 노트북을 작살낼 수 있다. 트랜센드를 권장한다.
  * `[2]` [Windows Vista](Windows%20Vista.md)나 [Windows 7](Windows%207.md)은 별도의 삽질을 해야 한다.
  * `[3]` 단 이것은 특정 폴더(예: mydriver) 안에 모아 넣어야 한다. 가끔 드라이버 등을 넣었는데 설치 자체가 안 된다는 경우가 있다.

