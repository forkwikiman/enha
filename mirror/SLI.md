SLI(스케일러블 링크 인터페이스 / Scalable Link Interface)

![http://i47.tinypic.com/1sih3r.jpg](http://i47.tinypic.com/1sih3r.jpg)

[[JPG external image]](http://i47.tinypic.com/1sih3r.jpg)

![Example.jpg](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/SLI/Example.jpg)

[JPG image (129.7 KB)]

  
사진은 GTX Titan 4way SLI이다... <del>가격이 중고차급</del>

![http://www.eurocom.com/ec/data/images/m233_2.jpg](http://www.eurocom.com/ec/
data/images/m233_2.jpg)

[[JPG external image]](http://www.eurocom.com/ec/data/images/m233_2.jpg)

  
사진은 최상급 그래픽카드 2개를 박아넣은 유로컴 사의 워크스테이션. <del>이거 살 돈이면 그냥 고급 워크스테이션을 맞출 수
있다</del>

[GPU](GPU.md)제조사인 [nVIDIA](nVIDIA.md)가 내놓은 자사의 칩셋을 사용한 동일한 그래픽카드를 연결하여
비약적인 성능 향상`[1]`을 얻도록 하는 기술이다. 원래 [3dfx](3dfx.md)가 1998년에
[Voodoo2](Voodoo.md) 그래픽카드를 통해 공개한 기술이나 이후 [nVIDIA](nVIDIA.md)가
[3dfx](3dfx.md)를 인수한 후 취득하여, 2004년에 지포스 6000시리즈(NV40 GPU)를 출시하며 선보인
기술이다.(이때 3dfx의 SLI는 Scan-Line Interleave의 약자다.) 우선 이 기술은 3가지 방식으로 작동된다.  
첫번째 방식인 화면분할 방식(SFR)은 렌더링할 화면을 작업량이 동일하게 상하로 분할하여 각각 다른 그래픽카드가 렌더링 작업을 분담하게
한다.  
두번째 방식인 AFR 방식은 1개의 프레임을 번갈아가며 각각 그래픽 카드가 렌더링하는 방식이다.  
마지막으로는 각자의 그래픽카드가 [안티에일리어싱](%EC%95%88%ED%8B%B0%EC%97%90%EC%9D%BC%EB%A6%AC%EC%96%B4%EC%8B%B1.md) 작업량을 분담하는 방식이 있다.

[메인보드](%EB%A9%94%EC%9D%B8%EB%B3%B4%EB%93%9C.md)에 따라 최소 2개에서 최대 4개까지 그래픽 카드를
연결할 수 있다. 단, 한 카드에 GPU가 두개 장착된 듀얼 GPU카드는 두개까지만 장착이 허용된다.(어디까지나 GPU를 최대 4개까지만
사용하는 거니까...)`[2]`  
단 무엇보다 [메인보드](%EB%A9%94%EC%9D%B8%EB%B3%B4%EB%93%9C.md)에서 SLI기술을 지원해야만 사용할 수
있으며 동급사양의 그래픽카드끼리만 연결이 가능하여 다른 사양의 카드와도 연결이 가능한 [AMD](AMD.md)의
[크로스파이어](%ED%81%AC%EB%A1%9C%EC%8A%A4%ED%8C%8C%EC%9D%B4%EC%96%B4.md)에 비해 한수
뒤쳐진다는 평이다.`[3]`실제로 크로스파이어는 메인스트림급 보드에서도 2way는 무난하게 할 수 있는 반면에 Sli는 대체로 오버클럭이
가능한 보드부터 2way 사용이 가능하다.(라이센스를 지불해야 하는 Sli칩셋을 장착해야하니...)

이래저래 인지도가 이래저래 크로스파이어에 밀리는 편. 그래선지 카드 두개를 묶어 쓰는 걸 크파라고 싸잡아 말하는 사람이 의외로 많은 편.
다만 엔비디아에서 SLI를 처음 출시했을 때에는 크파가 없었기 때문에 SLI의 인지도가 더 높던 시절이 있었다.

`\----`

  * `[1]` 물론 전력 소모량도 비약적...까지는 아니더라도 늘어난다. 2way Sli는 보통 최소 7~800w의 파워를 요구한다.
  * `[2]` MARS 760과 같은 예외의 경우도 있다.
  * `[3]` 크로스 파이어는 상급+하급은 하급 X2로 사용되기는 하나 세대차이가 크게 나지 않으면 하급 X2가 낫고 APU와 하이브리드 크로스파이어도 된다. 거기다 R 200 세대의 하와이 칩부터는 그냥 PCI-E에 꽂기만 해도 크파가 된다.

