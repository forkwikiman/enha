![http://upload.wikimedia.org/wikipedia/commons/thumb/9/9a/Vmware.svg/200px-Vm
ware.svg.png](http://upload.wikimedia.org/wikipedia/commons/thumb/9/9a/Vmware.
svg/200px-Vmware.svg.png)

[[PNG external
image]](http://upload.wikimedia.org/wikipedia/commons/thumb/9/9a/Vmware.svg
/200px-Vmware.svg.png)

<http://www.vmware.com/>

가상화 프로그램 및 해당 제품을 생산하는 회사.

## Contents

    

1. 특징 
    

1.1. VMware Tools

1.2. Unity 모드

2. 제품 
    

2.1. 데스크탑 계열

2.2. 서버 계열

2.3. 기타

3. 관련 항목 

[[edit](http://rigvedawiki.net/r1/wiki.php/VMware?action=edit&section=1)]

## 1. 특징 ¶

x86 가상머신의 [끝판왕](%EB%81%9D%ED%8C%90%EC%99%95.md). IBM 계열 PC 가상화에 있어 오랜 역사를
자랑한다. 99년도에 첫 VMware Workstation이 나왔으니 Locus의 Merge나 Connectix의 Virtual PC보다는
늦은 편. 다만 Merge는 오래전에 망했고 Virtual PC는 MS에 먹혔으니
[지못미](%EC%A7%80%EB%AA%BB%EB%AF%B8.md)... 그만큼 많은 제품 라인업을 가졌다.

  

많이 알려진 주력 제품들은 대개 하드웨어 레벨 가상화 위주이다. 즉 [sandboxie](sandboxie.md)처럼 OS 상단에서
작동하는 가상화 제품은 없다고 알려져 있는데, 사실 있긴 있다. 아래 ThinApp를 보자. 다만 잘 안 알려진 것을 보아 딱히 경쟁자에
비해 뛰어난 편은 아닐지도.

  

역사가 오래된 만큼 성능과 호환성이 좋다. 가상머신을 돌리고 있는 진짜 하드웨어를 호스트, 가상머신 안에서 돌아가는 시스템을 게스트라
하는데, 기본적으로 호스트 CPU의 모든 기능을 가져다 쓸 수 있고, 심지어는 32비트 호스트에서도 64비트 게스트 운영체제를 돌릴 수
있다! 단 CPU가 64비트 명령어 세트를 지원해야 하며, CPU와 메인보드의 BIOS가 가상화 기능(Virtualization
Technology)을 지원해야 한다. 멀티코어 CPU는 게스트의 코어 총 수가 호스트의 개수만 안 넘으면 자유롭게 갖다 쓰는게 가능하다.
성능이 호스트급이라는 말은 과대포장이지만, 그래도 거의 모든 벤치마크에서 다른 가상화 프로그램들을 **가볍게 씹어드시는** 수준의 퍼포먼스를
자랑한다. 제품에 관계없이 CPU 멀티코어 SMP 성능은 넘사벽급. 서버 제품군은 해당 안되지만 3D 가속 지원도 대단히 뛰어나다.
<del>물론 그만큼 가격도 하늘나라로.</del> VirtualBox나 Virtual PC 등 x86 가상머신 제품 중, 거의 유일하게
유료 제품 라인업을 고수하고 있다. 다만 VMware Player가 나온 후 개인사용자 대상으로는 <del>사실상</del> 무료 개방을
했다.`[1]` <del>개인사용자가 아닌 업체에 가상화 제품 팔아대는 회사가 애초에 거의 없다</del>

  

[[edit](http://rigvedawiki.net/r1/wiki.php/VMware?action=edit&section=2)]

### 1.1. VMware Tools ¶

최적화를 위해 게스트에서 커스텀 하드웨어를 제공한다. 해당 게스트에 전용 드라이버 모음인 VMware Tools를 설치하면, 호스트에서
"커스텀 하드웨어"에 직접 접근해 속도가 비약적으로 상승한다. 부가기능인 파일을 드래그한다든지 클립보드 공유나 시간 동기화, Unity
모드와 디버깅 등을 하기 위해서도 반드시 설치해야한다. 다만 지원하지 않는 게스트는 [그런거없다](%EA%B7%B8%EB%9F%B0%EA%B1%B0%20%EC%97%86%EB%8B%A4.md).

  

[[edit](http://rigvedawiki.net/r1/wiki.php/VMware?action=edit&section=3)]

### 1.2. Unity 모드 ¶

데스크탑 제품에서 Unity 모드를 사용하면 Windows 7에서 [VirtualPC](Windows%20Virtual%20PC.md)로 XP 모드를 쓰던 것과 똑같이 게스트의 프로그램을 호스트 프로그램인 것처럼 쓸
수 있다. 단 XP 모드와 달리 VM이 자동 실행되거나 시작메뉴 프로그램이 자동으로 통합되지 않는 것은 단점. 아예 시작메뉴 위에 마우스를
갖다대면 가상머신의 시작메뉴가 따로 뜬다. 리눅스 계열도 마찬가지.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/VMware?action=edit&section=4)]

## 2. 제품 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/VMware?action=edit&section=5)]

### 2.1. 데스크탑 계열 ¶

  * VMware Workstation - 주력 개인용 제품. 데스크탑 성능 및 디버깅 특화.
  * VMware Player - **공짜다.**`[2]` Workstation에 비해 스냅샷 기능 및 디버깅 기능이 부족하다. 원래는 말 그대로 [플레이어](%ED%94%8C%EB%A0%88%EC%9D%B4%EC%96%B4.md)가 목적이라 3.0 이전엔 이미 만들어진 가상머신만 취급할수 있었으나 3.0에선 신규 가상머신 생성도 가능하다.
  * VMware Player Pro`[3]` \- Player 의 상업용 버전 
  * VMware View - 서버 계열 제품에 원격 연결하는 프로그램.
  * VMware Fusion - [인텔 맥](%EB%A7%A4%ED%82%A8%ED%86%A0%EC%8B%9C.md)용.

[[edit](http://rigvedawiki.net/r1/wiki.php/VMware?action=edit&section=6)]

### 2.2. 서버 계열 ¶

  * VMware ESX - 주력 서버 제품. 하지만 단종. 그 자체가 리눅스 커널을 얹은 OS로, 가상화만을 위해 작동한다.
  * VMware ESXi - ESX를 단종시키고 새로 출시한 Hypervisor. ESX와 비교하여 용량이 대폭 감소하였고, 성능은 올라갔다. 
  * VMware Server - 단종. 비슷한 공짜 프로그램인 VMware Player에 비해 IO 성능이 좋은 대신 반응성이 떨어졌다.
  * VMware vSphere - ESX(ESXi) 에 vCenter를 더한 통합 가상화 플랫폼.
  * VMWare vCenter - ESX(ESXi) Hypervisor 기반 인프라를 관리하기 위한 통합 관리 센터, 이거 없으면 vMotion 도 HA도 FT도 못쓴다.  

[[edit](http://rigvedawiki.net/r1/wiki.php/VMware?action=edit&section=7)]

### 2.3. 기타 ¶

요즘엔 vCloud라는 이름으로 눈을 클라우드 시장으로 돌리고 있다. 데이터센터의 넘쳐나는 잉여자원을 모조리 가상화해서 성능을
<del>쥐어짠다는</del>높인다는 것.

  

참고로 2012년에 SDN(Software-defined Networking) 스타트업의 선두 주자인 Nicira Network를 무려
12억 6천만 달러에 인수하였다. 이 금액은 2014년 현재까지도 스타트업 인수 금액 10위권에 드는 규모.. 니시라를 통해 네트워크
가상화와 데이터센서 네트워크 솔루션 시장에서도 잘 나가는 듯하다.

  

그리고 희한한 플랫폼을 여럿 흡수하거나 인수하고 있는데, 웹개발을 위한 SpringSource라든지, 프레젠테이션 솔루션인
SlideRocket, 일정관리 (오픈소스) 용 Zimbra, 웹/애플리케이션 플랫폼인 vFabric 등을 잔뜩 벌리는 것을 보아
애플리케이션 플랫폼 시장을 노리고 있다.

  

그리고 [sandboxie](sandboxie.md)와 비슷한 VMware ThinApp라는 게 있는데, 어떤 프로그램의 **포터블
버전**을 자동으로 만들어준다. 이동식 샌드박스인 셈. [흠좀무](%ED%9D%A0%EC%A2%80%EB%AC%B4.md)

  

[온라인 게임](%EC%98%A8%EB%9D%BC%EC%9D%B8%20%EA%B2%8C%EC%9E%84.md)
[스톤에이지](%EC%8A%A4%ED%86%A4%EC%97%90%EC%9D%B4%EC%A7%80.md) 유저들이 자주 사용하는
프로그램이기도 하다. 스톤에이지를 실행할 때 게임가드에서 VMware의 실행을 막지 않기 때문에, 스톤에이지에서 공식적으로 다중 클라이언트를
허용하기 전에는 VMware를 써서 유저들이 사실상의 다중 클라이언트 플레이를 했다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/VMware?action=edit&section=8)]

## 3. 관련 항목 ¶

  * [가상화 프로그램](%EC%86%8C%ED%94%84%ED%8A%B8%EC%9B%A8%EC%96%B4/%EB%AA%A9%EB%A1%9D#s-13.md)
  * [Windows Virtual PC](Windows%20Virtual%20PC.md)
  * [VirtualBox](VirtualBox.md)
  * [sandboxie](sandboxie.md)
  * [Parallels Desktop](Parallels%20Desktop.md)

`\----`

  * `[1]` 4.0.3까지는 영업용도 무료, 현재는 개인용만 무료이며, 영업용은 유료이다.
  * `[2]` 비 상업적 목적에 한정. 4.0.3버젼등은 상업용 목적에도 무료로 사용할수 있다? <del>진짜?</del>
  * `[3]` Player 6까지는 Plus, 7부터 Pro

