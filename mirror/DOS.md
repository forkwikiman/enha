## Contents

    

1. 운영체제 
    

1.1. 도스의 종류

1.2. 도스의 내장 명령어

    

1.2.1. CLS

1.2.2. CD

1.2.3. COPY

1.2.4. DIR

1.2.5. DEL

1.2.6. MD

1.2.7. RD

1.2.8. REN

1.2.9. VER

1.2.10. TYPE

1.3. 외장 명령어

    

1.3.1. FORMAT

1.3.2. DISKCOPY

1.3.3. EDIT

1.3.4. DEBUG

1.4. 기타

    

1.4.1. *

1.4.2. ?

1.4.3. >>

1.4.4. /?

1.5. 관련항목

2. 해킹방법 
3. Density of state 
4. [워크래프트3](%EC%9B%8C%ED%81%AC%EB%9E%98%ED%94%84%ED%8A%B83.md)의 [AOS](AOS.md) [유즈맵](%EC%9C%A0%EC%A6%88%EB%A7%B5.md) [Dream of Scheherazade](Dream%20of%20Scheherazade.md)의 약칭 
5. [코즈믹 브레이크](%EC%BD%94%EC%A6%88%EB%AF%B9%20%EB%B8%8C%EB%A0%88%EC%9D%B4%ED%81%AC.md)의 【힘】의 [아크](%EC%95%84%ED%81%AC.md) "[도스트렉스](%EB%8F%84%EC%8A%A4%ED%8A%B8%EB%A0%89%EC%8A%A4.md)"밑으로 모인 연합. 

[[edit](http://rigvedawiki.net/r1/wiki.php/DOS?action=edit&section=1)]

## 1. 운영체제 ¶

Disk Operating System. 디스크 운영 체제. 운영체제 중 하나로 [UNIX](UNIX.md)와 더불어 텍스트 기반의
대표적인 운영체제이다.

  

검은 화면 위의 프롬프트라고 불리는 곳에 키보드로 명령어를 입력하는 흔히 원시적인 형태의 [문자입력인터페이스](CUI.md)의 쉘을
가진 운영체제를 말한다. 예전에 만들어진 OS(운영체제)다 보니 윈도우즈와는 달리 파일 이름이 영문자 기준으로 최대 8자, 확장자는
3자까지만 입력할 수 있다.`[1]` 일명 8.3 파일 체제.  

흔히 [마이크로소프트](%EB%A7%88%EC%9D%B4%ED%81%AC%EB%A1%9C%EC%86%8C%ED%94%84%ED%8A%B8.md)사에서 개발한 [MS-DOS](MS-DOS.md)를 많이 썼기 때문에 일반적으로 DOS라 하면 고유명사 비슷하게 되어 MS-
DOS, 혹은 그와 호환성을 지닌 텍스트 기반의 운영체제(DR-DOS, Free DOS 등)를 가리키는 경우가 많으나 원래 DOS라는 단어는
일반명사로 디스크 운영 체제를 가리키기 때문에 [애플 II](%EC%95%A0%ED%94%8C%20II.md)의 DOS 3.3이나
Pro DOS, [MSX](MSX.md)의 MSX-DOS처럼 MS-DOS랑 그다지 상관이 없는 별개의 운영체제인 경우도 있다.`[2]`

  

DOS의 모습을 보고 싶으면 윈도우의 시작 아이콘을 누르고, 실행 창에 cmd 라고 치면 쉘이 뜬다. 창을 닫을 때는 exit를 치거나 닫기
버튼을 누른다. 물론 도스 프롬프트는 도스를 그럴듯하게 흉내낸 프로그램이지 도스는 아니다.

  

[Microsoft Windows](Microsoft%20Windows.md)도 3.1버전까지는 도스 상에서 실행하는 일종의
프로그램이었다. 95, 98, ME의 경우에도 도스 셸을 포함하면서 도스의 영향 아래 있었으나, NT커널은 도스 커널이 포함되지 않았기에
점점 영역이 축소되었고 2001년 윈도우 XP가 본격적으로 보급되면서 역사의 뒤안길로 사라졌다.

  

윈도 ME시절까지는 윈도우에서 바로 지원하지 못하는 기능이나 숨어 있는 기능을 쓸 수 있어 도스를 아는 사람은 종종 도스 창을 사용했었다.
`[3]`

  

[[edit](http://rigvedawiki.net/r1/wiki.php/DOS?action=edit&section=2)]

### 1.1. 도스의 종류 ¶

  * [QDOS](QDOS.md)
  * [MS-DOS](MS-DOS.md)
  * [DR-DOS](DR-DOS.md)
  * [FreeDOS](FreeDOS.md)
  * [K-DOS](K-DOS.md)
  * PC-DOS
  * MSX-DOS
  * <del>[DOS/V](DOS/V.md)</del>
  * <del>[GLaDOS](GLaDOS.md)</del>

[[edit](http://rigvedawiki.net/r1/wiki.php/DOS?action=edit&section=3)]

### 1.2. 도스의 내장 명령어 ¶

이 내장 명령어는 부팅 시 기본적으로 실행되는 command.com 파일에 내장된 것들로, 별도의 실행파일을 실행시키지 않고도 사용가능한
것들이다.

  

여기에서는 공통적으로 들어가 있는 것만 기술한다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/DOS?action=edit&section=4)]

#### 1.2.1. CLS ¶

CLear Screen  
지저분한(...) 화면을 청소할 때 사용하는 명령어.

[[edit](http://rigvedawiki.net/r1/wiki.php/DOS?action=edit&section=5)]

#### 1.2.2. CD ¶

Change Directory  
하위 디렉토리로 갈 때 사용하는 명령어.  
CD .. 라고 치면 상위 디렉토리로 갈 수 있다. CD\로 쓰면 가장 상위 디렉토리로 이동한다.  
예) CD _이동하고 싶은 하위 디렉토리_

[[edit](http://rigvedawiki.net/r1/wiki.php/DOS?action=edit&section=6)]

#### 1.2.3. COPY ¶

파일을 복사할 때 쓰는 명령어다. Unix에서는 cp  
예) COPY _복사하고 싶은 파일_ _복사할 디렉토리_  
파일에서 파일만이 아니라, 파일에서 프린터로, 화면(console)에서 파일, 명령어의 출력 결과를 파일이나 프린터로 복사할 수도 있다.

[[edit](http://rigvedawiki.net/r1/wiki.php/DOS?action=edit&section=7)]

#### 1.2.4. DIR ¶

DIRectory  
해당 디렉토리에 어떤 파일이 있는지 볼때 사용한다.  

DIR/w - 간단하게 파일명만 볼 때 사용하는 문구 (wide)  
DIR/p - 파일 리스트를 한 화면씩 넘기고 싶을 때 사용하는 문구 (pause)  
DIR/s - 서브 디렉토리까지 출력한다. 한 화면을 넘기므로 대개 /p와 함께 사용한다.

[[edit](http://rigvedawiki.net/r1/wiki.php/DOS?action=edit&section=8)]

#### 1.2.5. DEL ¶

DELete  
해당 파일을 지울 때 쓰는 명령어다.  
예) DEL _지우고 싶은 파일_

[[edit](http://rigvedawiki.net/r1/wiki.php/DOS?action=edit&section=9)]

#### 1.2.6. MD ¶

Make Directory  
해당 디렉토리를 생성할 때 사용하는 명령어다.  
예) MD _생성하고 싶은 디렉토리 이름_

[[edit](http://rigvedawiki.net/r1/wiki.php/DOS?action=edit&section=10)]

#### 1.2.7. RD ¶

Remove Directory  
해당 디렉토리를 삭제할 때 사용하는 명령어이며, 해당 디렉토리 안에 파일이 있으면 삭제할 수 없다.  
예) RD _삭제하고 싶은 디렉토리 이름_

[[edit](http://rigvedawiki.net/r1/wiki.php/DOS?action=edit&section=11)]

#### 1.2.8. REN ¶

REName  
해당 파일의 이름을 바꿀 때 사용한다.  
예) REN _이름을 바꾸고 싶은 파일_ _그 파일의 새 이름_

[[edit](http://rigvedawiki.net/r1/wiki.php/DOS?action=edit&section=12)]

#### 1.2.9. VER ¶

VERsion  
해당 DOS의 버전을 표시해준다.

[[edit](http://rigvedawiki.net/r1/wiki.php/DOS?action=edit&section=13)]

#### 1.2.10. TYPE ¶

텍스트로 된 파일을 화면에 출력한다.

[[edit](http://rigvedawiki.net/r1/wiki.php/DOS?action=edit&section=14)]

### 1.3. 외장 명령어 ¶

도스의 시스템 디렉토리 내에 .exe나 .com 실행파일의 형태로 들어가 있는 명령.

[[edit](http://rigvedawiki.net/r1/wiki.php/DOS?action=edit&section=15)]

#### 1.3.1. FORMAT ¶

디스크를 포맷한다.

[[edit](http://rigvedawiki.net/r1/wiki.php/DOS?action=edit&section=16)]

#### 1.3.2. DISKCOPY ¶

디스크의 내용을 다른 디스크로 그대로 복사한다.

[[edit](http://rigvedawiki.net/r1/wiki.php/DOS?action=edit&section=17)]

#### 1.3.3. EDIT ¶

텍스트 파일의 내용을 편집한다. 단 전체 화면 에디터.

[[edit](http://rigvedawiki.net/r1/wiki.php/DOS?action=edit&section=18)]

#### 1.3.4. DEBUG ¶

메모리나 레지스터, 파일의 어셈블리를 보거나 편집한다.

[[edit](http://rigvedawiki.net/r1/wiki.php/DOS?action=edit&section=19)]

### 1.4. 기타 ¶

명령어가 아니나 명령어와 함께 사용되어 기능하는 키워드들.

[[edit](http://rigvedawiki.net/r1/wiki.php/DOS?action=edit&section=20)]

#### 1.4.1. * ¶

애스터리스크(Asterisk)  
모든 파일을 지정할 때 사용하는 와일드카드.  
예) *.EXE라 하면 EXE [확장자](%ED%99%95%EC%9E%A5%EC%9E%90.md)를 가진 모든 파일을 지정해 준다.

[[edit](http://rigvedawiki.net/r1/wiki.php/DOS?action=edit&section=21)]

#### 1.4.2. ? ¶

* 와 비슷하게 사용되나 * 가 길이가 어떠하든지 모두 지칭하는데 반해 `?`는 정확히 사용된 개수만큼의 문자수와 1대 1로 대응된다.

[[edit](http://rigvedawiki.net/r1/wiki.php/DOS?action=edit&section=22)]

#### 1.4.3. >> ¶

리다이렉션(redirection). 리다이렉션이란 프로그램의 출력 결과를 파일이나 프린터로 보내는 것을 말한다. 예를 들어 DIR 명령은
디렉터리와 파일 목록을 화면에 출력하는 명령이지만, DIR >> dir.txt 라고 치면 화면에 나와야 할 목록이 _dir.txt라는 파일로
만들어진다._ 같은 식으로, dir >> prn 이라고 하면 파일 목록이 프린터로 출력이 된다. (윈도우의 도스 에뮬레이션 창에서는 프린터
사용은 불가능)  
리다이렉션에는 한 개짜리 부등호와 두 개짜리 부등호가 있는데, 한 개짜리는 파일을 **덮어쓰는 것**이고, 두 개짜리는 파일 뒤에
**추가**하는 것이다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/DOS?action=edit&section=23)]

#### 1.4.4. /? ¶

대부분의 명령어에는 /? 옵션을 붙이면 도움말 화면이 나온다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/DOS?action=edit&section=24)]

### 1.5. 관련항목 ¶

  * [윈도우즈](%EC%9C%88%EB%8F%84%EC%9A%B0%EC%A6%88.md)
  * [셸](%EC%85%B8.md)  

[[edit](http://rigvedawiki.net/r1/wiki.php/DOS?action=edit&section=25)]

## 2. 해킹방법 ¶

Denial of Service의 약자로 서버에 쉴새 없이 말(명령어)을 걸어대 서버를 마비시키는
[해킹](%ED%95%B4%ED%82%B9.md)방법 중 하나이다. 이의 한 종류로
[DDoS](DDoS.md)(Distributed DOS: 특히 여러 곳에서 DOS 공격하는 것)가 있다.

  

[인터넷 익스플로러](%EC%9D%B8%ED%84%B0%EB%84%B7%20%EC%9D%B5%EC%8A%A4%ED%94%8C%EB%A1%9C%EB%9F%AC.md)의 F5 연타도 DOS 공격의 일종이다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/DOS?action=edit&section=26)]

## 3. Density of state ¶

  

[[edit](http://rigvedawiki.net/r1/wiki.php/DOS?action=edit&section=27)]

## 4. [워크래프트3](%EC%9B%8C%ED%81%AC%EB%9E%98%ED%94%84%ED%8A%B83.md)의
[AOS](AOS.md) [유즈맵](%EC%9C%A0%EC%A6%88%EB%A7%B5.md) [Dream ofScheherazade](Dream%20of%20Scheherazade.md)의 약칭 ¶

  

[[edit](http://rigvedawiki.net/r1/wiki.php/DOS?action=edit&section=28)]

## 5. [코즈믹 브레이크](%EC%BD%94%EC%A6%88%EB%AF%B9%20%EB%B8%8C%EB%A0%88%EC%9D%B4%ED%81%AC.md)의 【힘】의 [아크](%EC%95%84%ED%81%AC.md)
"[도스트렉스](%EB%8F%84%EC%8A%A4%ED%8A%B8%EB%A0%89%EC%8A%A4.md)"밑으로 모인 연합. ¶

`\----`

  * `[1]` 파일 이름 길이 제한은 당시 DOS가 사용했던 FAT파일시스템의 한계일 뿐 당시 하드웨어의 한계가 아니다. 단적인 예로 [UNIX](UNIX.md)운영체제는 DOS보다도 옛날에 만들어졌지만 이 운영체제는 파일 이름 길이 제한이 없거나 있더라도 상당히 긴 파일 이름을 허용했다.
  * `[2]` MSX-DOS의 경우에는 외형이나 커맨드는 MS-DOS 1.0에 준하여 만들어지기는 했으나 MS-DOS와 호환성은 전혀 없고 엉뚱하게 CP/M과 호환성을 가지고 있었다. 이미 8비트 업계에 쫙 깔려있었던 CP/M 애플리케이션의 인프라를 이용하기 위한 방책이었다.
  * `[3]` 일반 사용자용 운영체제가 [Windows NT](Windows%20NT.md)계열로 넘어온 현재에도 각종 고급 기능의 사용을 위해 명령 프롬프트(CMD.EXE)를 사용하는 경우가 많다.

