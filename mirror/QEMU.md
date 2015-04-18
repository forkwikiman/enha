![qemu.png](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/qemu.png)

[PNG image (203.54 KB)]

Quick EMUlator [홈페이지](http://www.qemu.org)

하드웨어 가상화의 기능을 갖춘 무료이자 오픈 소스 소프트웨어이다.

## Contents

    

1. 개요 
2. 안드로이드 
3. 기타 
4. 같이보기 

[[edit](http://rigvedawiki.net/r1/wiki.php/QEMU?action=edit&section=1)]

## 1. 개요 ¶

QEMU는 하이퍼바이저`[1]`라는 기술을 채용했다. 이를 이용해 여러개의 가상 머신을 한 플랫폼 안에서 돌릴 수 있다. 이와 비슷한
소프트웨어로는 [VMware](VMware.md)와 [VirtualBox](VirtualBox.md) 등이 있다

  

[[edit](http://rigvedawiki.net/r1/wiki.php/QEMU?action=edit&section=2)]

## 2. 안드로이드 ¶

[안드로이드](%EC%95%88%EB%93%9C%EB%A1%9C%EC%9D%B4%EB%93%9C%28OS%29.md) 에서도 사용이
가능해서 놀랍게도 **안드로이드에서 [Windows XP](Windows%20XP.md) 같은 운영체제와 그 프로그램들을 돌릴 수
있다!** <del>단점이 있다면 느리다</del>  
돌려도 [Windows 95](Windows%2095.md), [Windows NT4.0](Windows%20NT%204.0.md)로 추천한다. <del>그냥 [bochs](bochs.md)로 돌린는게 정신건강이
이롭다.</del>

  

다음 링크는 안드로이드 운영체제에 윈도우XP를 돌리는 방법을 소개한다. 심심하거나 시간나면 직접 한번 해보자.
[#](http://neoray.tistory.com/370) 가능하면 성능이 좋은 스마트폰으로 하는게 정신건강에 이롭다.  
자세한건 [bochs](bochs.md)나 [Limbo PC Emulator](Limbo%20PC%20Emulator.md) 참조
(QEMU 기반이다)

  

[[edit](http://rigvedawiki.net/r1/wiki.php/QEMU?action=edit&section=3)]

## 3. 기타 ¶

VMware에 비해 성능이 절망적이다. (...) 오죽하면 같은 운영체제, 같은 프로그램을 돌려도 VMware은 CPU 사용량이 20%대,
QEMU는 CPU 사용량이 50%대겠는가 (...)

  

사실 이 부분은 QEMU의 성격 상 어쩔 수가 없는 부분이다. VMware나 VirtualBox가 동종 아키텍처(x86, x86-64)의
에뮬레이션을 목적으로 하는데 비해서, QEMU는 이종 아키텍처간의 에뮬레이션을 목적으로 한다. VMWare류는 동종 아키텍처의
에뮬레이션이므로 CPU에 내리는 명령은 별도의 번역과정 없이 바로 CPU로 바이패스되며 근래의 CPU라면 VT-x와 같은 하드웨어적인
지원까지 받아 더욱 오버헤드가 줄어들며 호환성 역시 나쁠 수가 없다. 그러나 QEMU나 Bochs와 같은 이종 아키텍처 에뮬레이터의 경우,
CPU 레벨부터 소프트웨어로 구축하여 가상 CPU를 구동한다. 말하자면 [MAME](MAME.md)와 마찬가지의 원리로 돌아간다는
것이다. 그 덕분에 안드로이드(ARM)과 같은 환경에서도 구동이 되는 것이지만 그 대가는 호환성과 속도이다. 속도는 당연히 느릴 수 밖에
없으며 호환성은 CPU 에뮬레이션 코드의 완성도에 좌우된다. x86위에서 돌린다 하더라도 x86 위에서 소프트웨어로 x86을 에뮬레이션 하는
<del>옥상옥</del> 결과가 되므로 당연히 속도는 느리다.

  

게다가 QEMU의 x86 에뮬레이션을 제작한 개발자가 바로 VirtualBox의 개발자로, VirtualBox를 개발하면서 QEMU의
개발에서는 손을 뗐다. 반면, 이러한점을 활용해서 실제 사용자 환경을 바탕으로 한 CPU나 아키텍처 시뮬레이터 용도로 많이 활용되고 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/QEMU?action=edit&section=4)]

## 4. 같이보기 ¶

  * [에뮬레이터](%EC%97%90%EB%AE%AC%EB%A0%88%EC%9D%B4%ED%84%B0.md)
  * [bochs](bochs.md)
  * [Limbo PC Emulator](Limbo%20PC%20Emulator.md)  

`\----`

  * `[1]` 호스트 컴퓨터에서 다수의 [운영체제](%EC%9A%B4%EC%98%81%EC%B2%B4%EC%A0%9C.md)를 동시에 실행하기 위한 논리적 플랫폼

