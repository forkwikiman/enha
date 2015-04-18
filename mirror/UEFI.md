  * 상위항목 : [컴퓨터 관련 정보](%EC%BB%B4%ED%93%A8%ED%84%B0%20%EA%B4%80%EB%A0%A8%20%EC%A0%95%EB%B3%B4.md)  

이 항목은 [EFI](EFI.md)로도 들어올 수 있습니다.

  
<del>[UEFA](%EC%9C%A0%EB%9F%BD%20%EC%B6%95%EA%B5%AC%20%EC%97%B0%EB%A7%B9.md)[와는 다르다! UEFA와는!](%EC%9E%90%EC%BF%A0%EC%99%80%EB%8A%94%20%EB%8B%A4%EB%A5%B4%EB%8B%A4%20%EC%9E%90%EC%BF%A0%EC%99%80%EB%8A%94.md)</del>

![http://upload.wikimedia.org/wikipedia/commons/thumb/d/df/Uefi_logo.svg
/368px-Uefi_logo.svg.png](http://upload.wikimedia.org/wikipedia/commons/thumb/
d/df/Uefi_logo.svg/368px-Uefi_logo.svg.png)

[[PNG external
image]](http://upload.wikimedia.org/wikipedia/commons/thumb/d/df/Uefi_logo.svg
/368px-Uefi_logo.svg.png)

  

![http://www.tonymacx86.com/attachments/mountain-lion-desktop-
guides/26881d1344251404-guide-ga-z68ma-d2h-b3-uefi-bios-all-working-dsdt-not-
required-sata-hotswap.jpg](http://www.tonymacx86.com/attachments/mountain-
lion-desktop-guides/26881d1344251404-guide-ga-z68ma-d2h-b3-uefi-bios-all-
working-dsdt-not-required-sata-hotswap.jpg)

[[JPG external image]](http://www.tonymacx86.com/attachments/mountain-lion-
desktop-guides/26881d1344251404-guide-ga-z68ma-d2h-b3-uefi-bios-all-working-
dsdt-not-required-sata-hotswap.jpg)

  
**최근에 나온 UEFI 지원 메인보드의 CMOS 셋업 화면**

## Contents

    

1. 개요 
2. Secure Boot 
3. CSM 

[[edit](http://rigvedawiki.net/r1/wiki.php/UEFI?action=edit&section=1)]

## 1. 개요 ¶

  

**U**nified **E**xtensible **F**irmware **I**nterface`[1]`  
통일 확장 펌웨어 인터페이스

  

[BIOS](BIOS.md)를 대체하는 [펌웨어](%ED%8E%8C%EC%9B%A8%EC%96%B4.md) 규격으로,
[샌디브릿지](%EC%83%8C%EB%94%94%EB%B8%8C%EB%A6%BF%EC%A7%80.md) 이후에 출시된
[메인보드](%EB%A9%94%EC%9D%B8%EB%B3%B4%EB%93%9C.md)는 대부분 이것을 쓴다고 보면 된다.  
[CUI](CUI.md)인 경우도 있지만, 요 근래는 대부분 [GUI](GUI.md)를 지원하는 추세이다. 심지어 터치도
되는(...) UEFI 펌웨어도 있다`[2]`. 기존 CUI 인터페이스와는 달리 마우스를 통한 클릭도 지원한다.

  

또한 GPT(GUID Partition Table) 디스크`[3]`에서의 부팅 지원, SecureBoot 등의 많은 기능이 있는데, 여기에
대해서는 [더 이상의 자세한 설명은 생략한다](%EB%8D%94%20%EC%9D%B4%EC%83%81%EC%9D%98%20%EC%9E%90%EC%84%B8%ED%95%9C%20%EC%84%A4%EB%AA%85%EC%9D%80%20%EC%83%9D%EB%9E%B5%ED%95%9C%EB%8B%A4.md). 단 이 펌웨어 인터페이스를 제대로 사용하려면 [Windows 8](Windows%208.md)이나
[Windows 8.1](Windows%208.1.md)을 사용해야 한다. [WindowsVista](Windows%20Vista.md)/[Windows 7](Windows%207.md)의 경우 UEFI 부팅을
지원하지만 삽질을 해야 하며 완벽한 UEFI 부팅도 아니다. [OS X](OS%20X.md)의 경우는 이전부터 UEFI를 지원해 왔으며
이를 잘 이용하여 UEFI를 달고 나온 메인보드의 경우 해킨토시 삽질이 수월해진 편.

  

의외로 [1990년](1990%EB%85%84.md)부터 논의되어 왔던 규격으로,
[인텔](%EC%9D%B8%ED%85%94.md)이 개발한 EFI`[4]`가 그 모토. 이것을
[2005년](2005%EB%85%84.md)에 규격을 공개했고, 오늘날에는 BIOS를 완전히 대체했다. [오오 인텔 오오](/wiki
/%EC%98%A4%EC%98%A4%20%ED%8A%B8%EB%A1%A4%EB%82%A8%EC%BA%90%20%EC%98%A4%EC%98%A
4).

  

진입 방법은 BIOS와 똑같다.`[5]`

  

빠른 부팅을 지원하며, UEFI+[SSD](SSD.md)+[Windows 8.1](Windows%208.1.md)의 조합으로
**[우사인 볼트](%EC%9A%B0%EC%82%AC%EC%9D%B8%20%EB%B3%BC%ED%8A%B8.md)급**의 부팅 속도를
체험할 수 있다. <del>이제 세계신기록 찍는 일만 남았다</del>

  

[[edit](http://rigvedawiki.net/r1/wiki.php/UEFI?action=edit&section=2)]

## 2. Secure Boot ¶

UEFI Specification 2.2부터 지원하는 기능. OS 부트로더가 검증된 인증서에 의해 디지털 서명되었는지를 검증하여 부팅
과정에서의 보안성을 높였다. 디지털 서명되지 않은 경우, 또는 검증된 인증서에 의해 서명되지 않은 경우에는 부팅이 중단된다. 이 기능을
정상적으로 사용하려면 [Microsoft Windows](Microsoft%20Windows.md) 계열에서는 Windows 8,
Windows 8.1이 설치되어야 한다. 반드시 UEFI 모드로 설치할 것.

  

[Linux](Linux.md) 배포판 중에서는 [페도라](%ED%8E%98%EB%8F%84%EB%9D%BC#s-2.md),
[우분투](%EC%9A%B0%EB%B6%84%ED%88%AC.md), OpenSuse가 해당되는데, 페도라 항목을 보면 알겠지만 리눅스
진영에서는 M$에 돈을 바쳤다고 일단 까고 시작한다.(...) 이념적인 감정도 있는지라 Secure Boot를 끄기도 하는 상황.

  

여담으로 [노트북](%EB%85%B8%ED%8A%B8%EB%B6%81.md)사용자중
[스팀(플랫폼)](%EC%8A%A4%ED%8C%80%28%ED%94%8C%EB%9E%AB%ED%8F%BC%29.md)을 통해 [소스엔진](%EC%86%8C%EC%8A%A4%20%EC%97%94%EC%A7%84.md)게임을 구동할 경우 그림자 옵션이 보통이나 낮음으로
밖에 선택 할 수 없는 경우가 있다. 이를 해결하기 위해선 바이오스 설정에 들어가서 Secure Boot 옵션을 꺼두면 해결이 된다 카더라.
<del>엔비디아와 밸브측에서는 왜 아직도 해결해 주지 않는지 모르겠다</del>

[[edit](http://rigvedawiki.net/r1/wiki.php/UEFI?action=edit&section=3)]

## 3. CSM ¶

**C**ompatibility **S**upport **M**odule.  
레거시 호환성을 위해 제공되는 모드이다. [Windows Vista](Windows%20Vista.md)/[Windows7](Windows%207.md)의 경우 CSM을 활성화 한 뒤 설치해야 한다. 대부분 메인보드가 CSM을 활성화 하는 방식으로 되어
있지만 MSI 노트북이나 일부 제품의 경우 UEFI 모드 설정에 UEFI with CSM 이런식으로 기재되어 있는 경우도 있으니 참고하자.
제대로된 UEFI 부팅이 UEFI + GPT + SecureBoot이라면, 이건 BIOS 모드에서 GPT 디스크로 부팅하는 정도밖에 안 되는
모드다.`[6]`

`\----`

  * `[1]` 읽을 때는 유-이-에프-아이 식으로 알파벳을 읽기도 하지만, 유이파이라고 읽기도 한다. [위키백과 참조](http://en.wikipedia.org/wiki/Unified_Extensible_Firmware_Interface)
  * `[2]` 삼성 아티브 계열에 들어가는 UEFI가 마우스 조작과 터치 조작을 지원한다. <del>터치감은 똥망이다.</del>
  * `[3]` 기존 MBR 디스크의 크기 한계를 넘어서 파티션을 잡을 수 있는 디스크 형식. 2TB 이상. 레거시 BIOS 모드에서도 사용할 수는 있지만 부팅용으로 사용할 수 없다.
  * `[4]` Extensible Firmware Interface. 규격 공개 이후 Unified가 붙어서 UEFI가 되었다.
  * `[5]` 주로 Delete나 F2
  * `[6]` 물론 이 설명은 [Windows Vista](Windows%20Vista.md)/[Windows 7](Windows%207.md)의 반쪽짜리 UEFI 설치 모드에 대한 설명이다. [Windows 8](Windows%208.md) 이후 버전에서는 CSM을 켜놔도 UEFI 설치가 되어 있다면 제대로 된 UEFI 부팅이 가능하겠지만, 기종에 따라 CSM이 켜진 경우 SecureBoot는 꺼지는 경우도 있고, CSM이 켜져야 UEFI 부팅이 가능한 경우도 있고 [케바케](%EC%BC%80%EB%B0%94%EC%BC%80.md)이므로 OS를 UEFI로 설치하는 경우 메인보드나 노트북의 바이오스 설명서를 꼭 잘 읽어 보자.

