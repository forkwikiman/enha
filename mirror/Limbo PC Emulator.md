## Contents

    

1. 개요 
2. 특징 
3. 사용법 
4. 하드웨어 
    

4.1. CPU

4.2. VGA

4.3. 네트워크 카드

4.4. 사운드 카드

5. 기타 
6. 림보 에뮬레이터가 구동 권장하는 운영체제 
7. 림보 에뮬레이터 지원하는 하드 디스크 이미지 확장자 

[[edit](http://rigvedawiki.net/r1/wiki.php/Limbo%20PC%20Emulator?action=edit&s
ection=1)]

## 1. 개요 ¶

Limbo PC Emulator는 안드로이드에서 x86 가상화를 지원하는 오픈소스 애플리케이션이다.  
2013년 말, 개발이 중단되었으며 최신버전은 0.9.9 ARM v7 버전이다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Limbo%20PC%20Emulator?action=edit&s
ection=2)]

## 2. 특징 ¶

[bochs](bochs.md)와는 다르게 GUI덕분에 사용이 편리하고, Bochs에 비하여 다양한 하드웨어를 가상화시킬 수 있다.
하지만 Bochs에 비하여 자잘한 오류가 많은 편이다. 하지만 QEMU에 기반을 둔 에뮬레이터이기에, Bochs보다 속도는 빠르지만
불안정하다.

  

개발 초창기 시절의 Limbo는 굉장히 불안정하고 느린 에뮬레이터였다. 2013년 초중반기였는데, 이미 그 때는 안드로이드 ICS가 널리
보급되었던 때였으나 Limbo는 2.2, 2.3에는 안정성을 보여주지만 안드로이드 4.0 이상의 버전에서는 극도로 불안정한 모습을
보여주었다.`[1]`

  

개발자도 이를 고려했는지, 개발중단 직전에 ARM v7을 지원하는 0.9.9 버전을 공개하였다. 안드로이드 4.0 이상의 버전에 대해서도
호환성을 가지게 된 것이다. 그래서 많은 사람들이 다시 림보 에뮬레이터에 관심을 가지게 되었다. `[2]`

  

그리고 Limbo는 디스켓, CD를 꺼내는 기능을 지원한다. 예를 들어 DOS 설치시, Bochs에서는 DOS 설치파일을 따로 하드디스크에
미리 전부 복사해서 설치해야 하지만, Limbo에서는 실제 컴퓨터와 같이 디스켓을 순서대로 넣으며 설치를 진행할 수 있다. 또한 화면크기
설정, 마우스, 키보드 설정까지 모두 할 수 있다. 일부 특수키의 입력도 지원한다.

  

Bochs보다 진보된 기능은 여기서 끝이 아니다. 운영체제 디스크이미지도 이 앱과 운영체제 설치파일만 있으면 만들 수 있다. 공
디스크이미지를 만들 수 있다. 용량은 임의로 설정가능하다. 여기서 만들어지는 디스크이미지의 형식은 IMG가 아니라 QCOW2라는 QEMU
디스크이미지 규격으로 만들어진다. 물론 IMG 형식의 디스크이미지도 림보에서 사용할 수 있다.

  

QCOW2는 IMG와 달리, 디스크이미지에서 실제로 사용한 공간만큼만 용량은 차지하기 때문에, 굉장히 효율적이다.  
같은 300MB 짜리 빈 디스크이미지라도 IMG는 300MB를 그대로 먹고 들어가지만 QCOW2는 1MB 미만의 크기를 가진다.

  

가장 주목할 부분은 바로 네트워크의 지원이다. 별 다른 복잡한 과정없이 림보에서 네트워크 카드를 선택하고, 드라이버를 설치하면 인터넷이
사용가능하다. 드라이버가 가장 흔한 네트워크 카드는 NE2000 이나 Realtek 8139 등이다. 인터넷을 하기에 가장 편리하고 빠른
운영체제는 Kolibri OS. Live CD 운영체제인데, 용량이 10MB를 넘지 않으며 각종 드라이버를 내장하고 있어서 사용이 간편하다.
많은 툴도 지원하고 있다.

  

QEMU Manager나 VMware 등의 유명 가상화 프로그램들이 '프로필'을 사용하여 다중의 운영체제 설정을 저장하듯이, 림보에서도
프로필을 이용하여 각각의 설정을 따로 저장할 수 있다.

  

가상머신의 구동방식도 선택할 수 있다. SDL방식과 VNC 방식 둘 중에서 선택가능하다. SDL방식은
[bochs](bochs.md)에서 사용하는 구동방식이다. 후술할 VNC처럼 가상 디스플레이를 사용하는것이 아니라서, 구동상태가 바로
출력되는 형태이다. 게임을 할때에 추천되는 구동방식이다.

  

VNC방식은 에뮬레이터 구동부와 출력부가 분리된 형태이다. VNC라고 해서 IP나 포트 설정을 할 필요없이 바로 구동이 가능하다. 구동화면을
바로 출력하는 형태가 아니기에, 약간의 딜레이가 있다.  
일부 운영체제는 SDL, VNC에 따라 구동이 안될 수 있다.

  

또 하나, 림보에서의 가장 독특한 기능은 바로 ARM 에뮬레이션이다.  
네이티브 ARM RISC CPU를 가상화하는것이 가능한 매우 독창적인 기능이다. 그래서 이론적으로는 안드로이드나 Windows CE 등의
모바일 운영체제를 이식하는것이 가능하다.(실제로 해당 AP를 장착한 기기가 안드로이드와 Windows CE의 펌웨어가 제작되었던 기기이다.)
하지만 가상화를 지원하는 ARM CPU가 구형이라, 해당 AP를 탑재한 기기의 펌웨어나 소스코드를 받기 힘들다. 고로, 아직 ARM
디스크이미지는 4PDA에서도 개발-배포되지 않았다.  
그리고, ARM 에뮬레이션을 이용하려면 커널 이미지와 initd 이미지도 필요하다.

  
  

[[edit](http://rigvedawiki.net/r1/wiki.php/Limbo%20PC%20Emulator?action=edit&s
ection=3)]

## 3. 사용법 ¶

애플리케이션을 실행하고 맨 위의 프로필 메뉴를 터치하여 프로필을 만들면, 본격적인 사용이 가능하다.  
설정창을 보면 좀 복잡하긴 하지만 확실히 [bochs](bochs.md)보다는 쉽고 간편하다. 자신이 원하는대로 선택하면 되니..  
CPU, RAM, VGA, 디스크이미지를 선택하고 부팅설정도 올바르게 했다면 Start를 선택하여 가상머신을 부팅할 수 있다. 부팅시간은
운영체제/기기마다 다르나, DOS는 30초 이내, 윈도우 95는 1분 이내에 부팅이 완료된다.  
메뉴키를 누르면 메뉴가 열리는데, 키보드와 마우스, 화면크기, 설정 창으로 이동, CD/DVD또는 디스켓을 변경할 수 있다.  
메뉴에서 마우스를 선택해야 마우스가 사용가능해지니 꼭 미리 활성화시켜 놓아야 한다. 손가락을 터치하면 클릭, 손가락을 이동하면 마우스 커서
이동, 한 손가락을 터치한 상태에서 다른 손가락으로 아무곳이나 터치하면 우클릭이다. (듀얼 핑거 탭 이라고도 한다. 하지만 이렇게 하면 일반
클릭으로 인식하는 경우가 잦다.)  
드래그는, 한 항목을 2~3초간 커서로 누르고 있다가 커서를 이동하면 된다. <del>윈도우 기본 카드게임을 할때에 좋다</del>

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Limbo%20PC%20Emulator?action=edit&s
ection=4)]

## 4. 하드웨어 ¶

Limbo PC Emulator의 하드웨어에 대하여 설명합니다.

[[edit](http://rigvedawiki.net/r1/wiki.php/Limbo%20PC%20Emulator?action=edit&s
ection=5)]

### 4.1. CPU ¶

-Default x86  

![Screenshot_2014-04-16-22-08-28.png](//rv.wkcdn.net/http://rigvedawiki.net/r1
/pds/Limbo_20PC_20Emulator/Screenshot_2014-04-16-22-08-28.png)

[PNG image (218.81 KB)]

  

-QEMU 32  

![Screenshot_2014-04-16-22-10-08.png](//rv.wkcdn.net/http://rigvedawiki.net/r1
/pds/Limbo_20PC_20Emulator/Screenshot_2014-04-16-22-10-08.png)

[PNG image (218.16 KB)]

  

-CoreDuo  
[인텔 코어 시리즈](%EC%9D%B8%ED%85%94%20%EC%BD%94%EC%96%B4%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md) 1세대.

  

-486

  

-Pentium 1

  

-Pentium 2

  

-Pentium 3

  

-athlon

  

-n270  
[인텔 아톰 시리즈](%EC%9D%B8%ED%85%94%20%EC%95%84%ED%86%B0%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md) N270 넷북용 CPU.

  

-default (64)

  

-qemu64

  

-phenom  
AMD Phenom 64.

  

-core2duo  
인텔 [코어 2 듀오](%EC%BD%94%EC%96%B4%202%20%EB%93%80%EC%98%A4.md).

  

-kvm64

  

-dafault (arm)

  

-arm926

  

-arm946

  

-arm1026

  
  

[[edit](http://rigvedawiki.net/r1/wiki.php/Limbo%20PC%20Emulator?action=edit&s
ection=6)]

### 4.2. VGA ¶

  

-qxl

  

-cirrus  
Cirrus GD-5446

  

-vmware  
VMWare SVGA-II

  

-xenfb

  

-std  
일반 VGA 카드

  
  

[[edit](http://rigvedawiki.net/r1/wiki.php/Limbo%20PC%20Emulator?action=edit&s
ection=7)]

### 4.3. 네트워크 카드 ¶

  

-rtl8139  
Realtek 8139 네트워크 카드

  

-ne2k  
Novell NE2000

  

-e1000

  

-i82551

  

-i82557b

  

-pcnet  
AMD PC-NET 10Mbps.

  

-i82559er

  

-virtio

  
  

[[edit](http://rigvedawiki.net/r1/wiki.php/Limbo%20PC%20Emulator?action=edit&s
ection=8)]

### 4.4. 사운드 카드 ¶

  

-sb16  
Creative 의 SoundBlaster16 이다.

  

-es1370  
ENSONIQ AudioPCI ES-1370

  

-ac97  
Realtek AC97

  

-hda  
PC 스피커. [똥컴](%EB%98%A5%EC%BB%B4.md)에서 나는 그 부저음 맞다.

[[edit](http://rigvedawiki.net/r1/wiki.php/Limbo%20PC%20Emulator?action=edit&s
ection=9)]

## 5. 기타 ¶

DOS 기반의 운영체제 설치프로그램의 동작이 림보에서는 오류가 발생한다. 다음 단계로 넘어가야하는 상황에서 예를 들어 F3을 눌러야 하는데,
분명히 Hacker's Keyboard로 눌렀는데 인식이 안되는 경우이다. 0.9.9  
에서도 해결이 안 돼있다.

  
  
  

[[edit](http://rigvedawiki.net/r1/wiki.php/Limbo%20PC%20Emulator?action=edit&s
ection=10)]

## 6. 림보 에뮬레이터가 구동 권장하는 운영체제 ¶

  
  

[Damn Small Linux](Damn%20Small%20Linux.md), Trinux, ttylinux, Minix,
[FreeBSD](FreeBSD.md), AROS(Icaros Desktop), [KolibriOS](Kolibri%20OS.md), FreeVMS, OpenWRT, Other OSes`[3]`  
<del>xp는 여기도 버림받았구나</del>  
<del>98도 쓸모 있군... 잠깐 2000이 있잖아?</del>

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Limbo%20PC%20Emulator?action=edit&s
ection=11)]

## 7. 림보 에뮬레이터 지원하는 하드 디스크 이미지 확장자 ¶

  

IMG, QCOW, QCOW2, VMDK, VDI, VHD

`\----`

  * `[1]` 잘 튕겼다. 안드로이드 4.0 이상 버전에서 Limbo를 사용하면 대부분 5분을 넘기지 못하고 튕겼다. 때때로 시작하자마자 튕기는 경우도 있었다.
  * `[2]` 0.9.9 업데이트로 인하여 거의 Bochs 급의 안정성이 확보되었다. 다만 아직 자잘한 부분들은 여전히 불안정하다. 예로 특정 윈도우 XP 이미지를 돌릴 때 부팅이 되지 않고 튕긴다던가... 같이 좀 부족하지만, 다양한 설정이 이 단점을 보완하고도 남는다.
  * `[3]` 윈도우 XP이하의 운영체제, 비 리눅스 운영체제

