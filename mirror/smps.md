switched(혹은 switching) mode power supply  

현대 파워서플라이의 모든 근간을 이루는 전원시스템 구성 방법이다.  
들어오는 전원을 게이트 소자를 사용해 modulation 한 다음에 전자기 결합을 통해 전압을 변경한다.  
리니어 방식과 달리, 전원을 전자기 결합을 통해 변환하므로 에너지 손실이 적다.

스위칭 주파수가 대부분 khz 대역으로 높지만, 일부 smps 는 60hz 등의 저주파수로 스위칭하기도 한다.  
그리고, 스위칭 주파수가 높을수록 크기는 작아지는게 포인트.

토플로지(topology)는 다음과 같다. 유명한 것만 일단.....  

  * 비 절연식   

    * buck switching   

    * boost switching   

    * buck-boost switching   

    * boost-buck switching   

    * charge-pump  

맨 아래에 charge-pump 빼고는 전부 인덕터를 통해 back-emf로 전압이 변환된다.

  * 절연식   

    * flyback  

    * half-forward   

    * forward   

    * push-poll  

    * half-bridge  

    * full-bridge   

    * ZVC  

중간에 반드시 transformer 가 들어간다. 흔이 뜯었을 때 노란 코일덩어리가 저것.

각 토플로지는 어플리케이션마다 다른 특성을 가진다.  

흔히 사용되는 [파워서플라이](%ED%8C%8C%EC%9B%8C%20%EC%84%9C%ED%94%8C%EB%9D%BC%EC%9D%B4.md) 의 경우,
half-bridge 이거나 full-bridge 형식으로 만들어진다.

### 비 절연식 토플로지의 구성들 ¶

  

buck switching  

  

step down 계열의 비절연형 초크포함 고정 케리어 전원 변환 방법  

  

전원과 초크코일이 일직선상에 있는데 스위칭 소자와 초크코일 사이에 역방향으로 전원과 병렬로 된 역방향 다이오드가 하나 끼여있다.  

  

전압은 스위칭 소자의 duty 비에 전적으로 결정되는데, pwm 과 비슷한 원리로, back-emf 에 의한다.  

