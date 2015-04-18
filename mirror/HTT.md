## Contents

    

1 Hyper Threading Technology

2 Hyper Transport Technology

3 Houkago Tea Time

### 1 Hyper Threading Technology ¶

[인텔](%EC%9D%B8%ED%85%94.md)에서 개발한 [CPU](CPU.md) 기술. 자세한 것은
[하이퍼스레딩](%ED%95%98%EC%9D%B4%ED%8D%BC%EC%8A%A4%EB%A0%88%EB%94%A9.md) 항목 참조.

### 2 Hyper Transport Technology ¶

[AMD](AMD.md)를 중심으로 설립된 '하이퍼 트랜스포트 컨소시엄'이 개발한 컴퓨터 버스 기술.  
기존의 [FSB](FSB.md)를 대체하기 위해서 개발되었으며, AMD는 이 기술을 [AMD 애슬론64시리즈](AMD%20%EC%95%A0%EC%8A%AC%EB%A1%A064%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md)
CPU부터 적용하기 시작헀다.

  

인텔에서는 이에 대항하기 위해 QPI(Quick Pass Interconnect)라는 기술을 개발했다. X58 칩셋부터 적용된 이 버스는
기존의 노스브릿지를 통한 프로세서 간 통식이나 프로세서와 메모리 간 통신 대신 다이렉트 연결을 지원한다. 또한 기존의 FSB보다 훨씬 우월한
대역폭을 통해 필연적으로 야기될 수밖에 없는 병목 현상을 방지한다. 이 때문에 AMD는 그나마 앞서던 대역폭에서까지 인텔에 밀리는 현상이
벌어졌다.  

  

다만 X58 칩셋 이후부터는 아예 노스브릿지를 CPU/사우스브릿지에 각각 통합하여 QPI 자체가 필요 없어졌으며, 옛날부터 노스브릿지-
사우스브릿지를 연결시킬때 써왔던 DMI(Direct Media Interface) 인터페이스를 CPU-사우스브릿지간의 연결에 써먹고 있다.
이러는 이유는 애초에 사우스브릿지는 I/O만을 관장하므로 QPI나 하이퍼트랜스포트 같은 초고속 인터커넥트가 전혀 필요 없기 때문이다. 지금
P55/Z68 같은 칩셋들이 노스 브릿지같은 이름을 가지고 있지만 실제론 옛날 노스브릿지가 하던 일 중 별로 안 중요한거 쪼금 +
사우스브릿지의 일만이 남아 있을 뿐이다. AMD도 APU에서 쓰는 FM 소켓에서 원칩 구조를 도입, 하이퍼트랜스포트는 버리고 DMI와 유사한
UMI(United Media Interface)를 채용하여 CPU-사우스브릿지를 연결하고 있다.  

  

50번대 칩셋에서는 DMI의 대역폭이 10Gbps로 좁아서 I/O 병목 이슈가 있었으나 60번대 칩셋에서 두배인 20Gbps로 늘어나면서
상당히 완화된 상태다.  

  

인텔의 경우 장기적으로 사우스브릿지까지 CPU에 통합한다는 계획을 가지고 있어 DMI 조차 안쓰게 될 날이 올 지도 모른다.  

  

물론 QPI는 아직도 DP 이상의 서버 플랫폼에서 프로세서 간의 연결을 위해 잘 쓰고 있다!  

### 3 Houkago Tea Time ¶

<del>아마도 이 항목에서는 가장 유명할 듯한</del> [케이온!](%EC%BC%80%EC%9D%B4%EC%98%A8%21.md)에
등장하는 [가상의 밴드](%EA%B0%80%EC%83%81%EC%9D%98%20%EB%B0%B4%EB%93%9C.md). 자세한 것은
[방과후 티타임](%EB%B0%A9%EA%B3%BC%ED%9B%84%20%ED%8B%B0%ED%83%80%EC%9E%84.md) 항목
참조.

