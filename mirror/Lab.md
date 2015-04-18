  * [연구소](%EC%97%B0%EA%B5%AC%EC%86%8C.md)를 찾으십니까?  

![http://archive.xaraxone.com/guest/guest58/LAB-Color-
Model.png](http://archive.xaraxone.com/guest/guest58/LAB-Color-Model.png)

[[PNG external image]](http://archive.xaraxone.com/guest/guest58/LAB-Color-
Model.png)

## Contents

    

1. 개요 
2. 관련 항목 

[[edit](http://rigvedawiki.net/r1/wiki.php/Lab?action=edit&section=1)]

## 1. 개요 ¶

색을 구성하는 방법의 하나로, **실제 안구가 색을 인식하는 방식**에 비추어서 간상 세포가 느끼는 밝기(**L**ightness), 원추
세포가 느끼는 적록과 황청(**a** Channel, **b** Channel)의 조합으로 구성된다.

  

여기서 밝기를 제외한 두 요소는 적록, 황청의 **서로 대립되는 색을 묶은 개념**으로,
[회색](%ED%9A%8C%EC%83%89.md)을 기준점으로 잡고 서로 반대 방향으로 뻗어가는 구조.
[포토샵](%ED%8F%AC%ED%86%A0%EC%83%B5.md) 등에서는 이 둘을 -127 ~ 128의 정수 형태로 구현하고
있다(0이 회색).`[1]`

  

잘 쓰이지 않는 색상 구성법이지만 굳이 활용법을 찾아보자면 **[색맹](%EC%83%89%EB%A7%B9.md)의 입장에서 이미지를
검증할 때.** 이미지를 Lab 모드로 바꾼 다음 a 채널이나 b 채널을 켜고 끄면 대충 황청 색맹, 적록 색맹이 보는 거랑 비슷해진다. 둘
다 끌 경우는? **전색맹**.

  

다른 [동물](%EB%8F%99%EB%AC%BC.md)의 색각을 시뮬레이션할 때에도 Lab의 성질을 이용한다. 물론 세부적인 부분에서는
차이가 나지만.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Lab?action=edit&section=2)]

## 2. 관련 항목 ¶

  * [색](%EC%83%89.md)
  * [색맹](%EC%83%89%EB%A7%B9.md)
  * [RGB](RGB.md)
  * [CMYK](CMYK.md)
  * [HSB](HSB.md)

`\----`

  * `[1]` 신기하게도 모든 수치가 최대여도 흰색이 아니며([주황색](%EC%A3%BC%ED%99%A9%EC%83%89.md)에 가까움), 마찬가지로 모든 수치가 최저여도 [검은색](%EA%B2%80%EC%9D%80%EC%83%89.md)이 아니다([남색](%EB%82%A8%EC%83%89.md)에 가까움). 사실 신기할 건 없고 위 그림만 봐도 알겠듯이 a, b채널은 당연히 최소, 최대값은 채도를 가지게 되므로 흰색과 검은색은 아닐 수 밖에 없다. 앞서 설명되어 있듯이 a, b값의 기준점이 **회색**이다. 여기서 흰색, 검은색을 보려면 당연히 L값을 변화시켜야 한다.

