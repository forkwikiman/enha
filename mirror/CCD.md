  * [동음이의어](%EB%8F%99%EC%9D%8C%EC%9D%B4%EC%9D%98%EC%96%B4.md)  

## Contents

    

1. 이미지 센서 
2. 군집붕괴현상 

[[edit](http://rigvedawiki.net/r1/wiki.php/CCD?action=edit&section=1)]

## 1. 이미지 센서 ¶

  

  * 상위항목 : [반도체](%EB%B0%98%EB%8F%84%EC%B2%B4.md)  

Charge-Couple Device  
전하결합소자  
電荷結合素子

  

CCD는 빛을 전하로 변환시켜 이미지를 얻어내는 센서이다. 한 구역에 저장된 전하를 다른 구역으로 이동(결합)시키는 성질을 가졌기 때문에
이런 이름을 붙였다. 여러 개의 MOS(Metal-Oxide-
Silicon)[축전기](%EC%B6%95%EC%A0%84%EA%B8%B0.md)`[1]`들로 부터 전하를 받아들여 한개 또는 여러개의
노드로 신호를 내보낸다. 전하의 총량 은 전압 신호로 바뀌어 버퍼(저장)되고 아날로그 전압 형태로 전달된 신호는 나중에 디지털로 변환시킨다.

  

![http://www.olympusmicro.com/primer/techniques/confocal/images/detectorsfigur
e5.jpg](http://www.olympusmicro.com/primer/techniques/confocal/images/detector
sfigure5.jpg)

[[JPG external image]](http://www.olympusmicro.com/primer/techniques/confocal/
images/detectorsfigure5.jpg)

  
크게 FT(Frame Transfer)방식과 IT(Interline Transfer)방식으로 나눌 수 있다. FT-CCD는 광소자들이 전하를
서로 건네주는 레지스터인 것에 비하여 IT-CCD는 광소자들이 준 전하를 레지스터에 넘겨주고 레지스터가 전하를 전달한다는 차이점이 있다.
따라서 전체 면적 중에서 일부분만 빛을 받아들이게 된다.

  

[디지털 카메라](%EB%94%94%EC%A7%80%ED%84%B8%20%EC%B9%B4%EB%A9%94%EB%9D%BC.md),
[스캐너](%EC%8A%A4%EC%BA%90%EB%84%88.md),
[캠코더](%EC%BA%A0%EC%BD%94%EB%8D%94.md)와 같은 장치의 주요 부품으로 사용된다.

  

CCD는 여러 개의 MOS(Metal-Oxide-Silicon)[축전기](%EC%B6%95%EC%A0%84%EA%B8%B0.md)가
쌍으로 상호 연결되어 있는 회로로 이루어져 있으며, 신호를 읽어낼 때에는 각 축전지들이 이웃한 축전지로 전하를 옮기는 방식(마치 시리얼
통신과 비슷)으로 이미지에서 읽어낸 전하를 전달한다.

  

[천문학](%EC%B2%9C%EB%AC%B8%ED%95%99.md) 분야에선 천문관측 도구 중 대표적으로 꼽히는 물건.

  

MOS축전기를 만들 때, 최근에는 일반적인 방식(CZ 등)으로 생산한 실리콘 결정을 이용하기 보다는 에퍼텍셜 기법(epitaxy)을 통해
저항이 더 높은 실리콘 결정을 제작하여 사용한다. 저 주파수(붉은 빛 및 그 아래 영역)에서는 빛이 더 깊이 투과할 수 있으므로
MOS축전기의 공핍층(Depletion Region)보다 더 깊은 곳에서 전하 캐리어(carrier)로써 전자 정공 쌍(Electron-
Hole Pair)을 생성하게 되어 효과적으로 전하를 모을 수 없는 일이 발생한다. 전자 정공 쌍이 생성되면 전기장에 의해 전하를 띤
입자로써 외력(로렌츠힘)을받아 이동하거나(Drift), 자연적으로 브라운 운동을 하며 확산(Diffusion)을 하게 되는데`[2]`,
공핍층 내부엔 전기장이 있기 때문에 캐리어의 확산이 큰 역할을 수행하지 못 하나 그 이외 지역에서는 확산만 일어나서 결국 애써 생성한 전자
정공 쌍이 재결합(Recombination) 등으로 사라져 버리거나, 타 픽셀로 옮겨가는 안습한 현상이 일어나게 된다. 에퍼텍셜 기법을 통해
만들어진 매우 얇고 저항이 큰 실리콘은 얇은 두께로 인해 거의 대부분에 공핍층 이 형성되게 되고, 이 곳에 생성되는 전자 정공 쌍은 전기장의
영향을 더 많이 받으므로 자연히 MOS 축전기로 쌓이게 되는 것이다. 물론 저항이 큰 것은 확산길이(Diffusion Length)를
줄이기도 한다. 이를 Deep Depletion CCD라 한다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/CCD?action=edit&section=2)]

## 2. 군집붕괴현상 ¶

[군집붕괴현상](%EA%B5%B0%EC%A7%91%EB%B6%95%EA%B4%B4%ED%98%84%EC%83%81.md)(Colony
Collapse Disorder). 항목 참조.

`\----`

  * `[1]` 실리콘을 기반으로 Oxidization 공정을 통해 축전지를 형성하여 빛으로 인하여 생성된 전하를 Depletion Region 을 통해 모은다.
  * `[2]` 사실, 두 가지 동시에 일어난다.

