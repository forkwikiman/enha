  * 상위 항목 : [컴퓨터 관련 정보](%EC%BB%B4%ED%93%A8%ED%84%B0%20%EA%B4%80%EB%A0%A8%20%EC%A0%95%EB%B3%B4.md), [단자/데이터 입출력](%EB%8B%A8%EC%9E%90/%EB%8D%B0%EC%9D%B4%ED%84%B0%20%EC%9E%85%EC%B6%9C%EB%A0%A5.md)  

## Contents

    

1. 개요 
2. 종류 
    

2.1. pre-ATA (IDE)

2.2. ATA-1 (IDE)

2.3. ATA-2 (E-IDE)

2.4. ATA-3 (E-IDE)

2.5. ATA/ATAPI-4 (Ultra ATA/33)

2.6. ATA/ATAPI-5 (Ultra ATA/66)

2.7. ATA/ATAPI-6 (Ultra ATA/100)

2.8. ATA/ATAPI-7 (Ultra ATA/133, SATA 1)

2.9. SATA 3Gb/s (SATA/300, gen 2)

2.10. SATA 6Gb/s (SATA/600, gen 3)

3. 관련항목 

[[edit](http://rigvedawiki.net/r1/wiki.php/ATA?action=edit&section=1)]

# 1. 개요 ¶

![http://upload.wikimedia.org/wikipedia/commons/thumb/6/66/PATA-cable.jpg
/333px-PATA-
cable.jpg](http://upload.wikimedia.org/wikipedia/commons/thumb/6/66/PATA-
cable.jpg/333px-PATA-cable.jpg)

[[JPG external
image]](http://upload.wikimedia.org/wikipedia/commons/thumb/6/66/PATA-
cable.jpg/333px-PATA-cable.jpg)

![http://www.sierra-cables.com/Cables/Images/SATA-Signal-
Cable-1.jpg?width=270](http://www.sierra-cables.com/Cables/Images/SATA-Signal-
Cable-1.jpg)

[[JPG external image]](http://www.sierra-cables.com/Cables/Images/SATA-Signal-
Cable-1.jpg)

IDE

SATA

  
Advanced Technology Attachment(고급 기술 결합)으로, IDE(Integrated Drive Electronics)
규격으로 시작된 [표준](%ED%91%9C%EC%A4%80.md)화 명칭이다. IBM-PC와 그 호환기종에서
[하드디스크](%ED%95%98%EB%93%9C%EB%94%94%EC%8A%A4%ED%81%AC.md)와
[ODD](ODD.md), [SSD](SSD.md)등과 같은 보조기억장치를 연결하기 위한 인터페이스 규격이다. PATA나 SATA
같은 인터페이스가 모두 이 [표준](%ED%91%9C%EC%A4%80.md) 규격 안에 들어가 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ATA?action=edit&section=2)]

# 2. 종류 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/ATA?action=edit&section=3)]

## 2.1. pre-ATA (IDE) ¶

표준화되기 전의 규격으로, 22비트 LBA를 사용, 하드디스크 크기는 2.1GB까지 지원하였다. 전송 방식은 PIO 0만 사용, 속도는
3.3MB/s 정도였다.

  

표준화되면서 ATA-1로 넘어갔다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ATA?action=edit&section=4)]

## 2.2. ATA-1 (IDE) ¶

이 표준은 1994년에 지정되었고, 보통 IDE라고 하면 이 규격을 가장 많이 이야기한다. 486 초창기까지 긴 세월동안 쓰인 규격으로,
28비트 LBA를 사용하면서 하드디스크 크기를 137GB까지 지원했다. 이 때의 규격은 40핀 단자와 40선 병렬 케이블을 사용했으며, 해당
케이블은 리본 케이블이라는 명칭으로 많이 불렸다.

  

하드디스크 이외의 장치는 연결할 수 없었다. 그 이유는 이 당시만 해도 CD-ROM이 일반화되기 이전의 상황이었고, 이 때 CD-ROM은
[SCSI](SCSI.md) 또는 [사운드카드](%EC%82%AC%EC%9A%B4%EB%93%9C%20%EC%B9%B4%EB%93%9C.md)에 연결하는 형태가 일반적이었다.

  

전송 방식도 다양화하여 PIO 0,1,2와 Single-word DMA 0,1,2 / Multiword DMA 0를 지원했다. 최고 속도는
8.3MB/s.

  

원래 처음에는 슬롯은 기본으로 1개만 지원했고, 별도의 인터페이스 카드를 꽂으면 확장이 가능했다. 1개의 슬롯에는 마스터와 슬레이브로 2개의
하드디스크를 연결할 수 있었다. 이후 슬롯을 한 개 더 지원해 최대 4개까지의 하드디스크가 장착 가능해졌다. (이때 슬롯 명칭이
프라이머리(Primary)와 세컨더리(Secondary)로 나눠졌다.)

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ATA?action=edit&section=5)]

## 2.3. ATA-2 (E-IDE) ¶

이 표준은 1996년에 지정되었다. E-IDE(Enhanced IDE)라고 명명된 방식으로, 향상된 IDE라는 뜻이다. 고속 IDE라든가
고속 ATA라는 명칭으로도 많이 불렸다.

  

이 때의 전송 방식은 PIO 3,4와 Multiword DMA 1,2를 지원했다. 최고 속도는 8.3MB/s. 펜티엄으로 넘어오면서 대세가
된 방식이다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ATA?action=edit&section=6)]

## 2.4. ATA-3 (E-IDE) ¶

이 표준은 1997년에 정식으로 지정되었다. 이 때부터 S.M.A.R.T가 들어갔다. 속도에는 변함이 없었고, 보안성이 향상된 버전.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ATA?action=edit&section=7)]

## 2.5. ATA/ATAPI-4 (Ultra ATA/33) ¶

이 표준은 1998년에 정식으로 지정되었다. 드디어 IDE 슬롯에 하드디스크 이외의 보조기억장치를 연결할 수 있게 되었다. (이 때부터
ATAPI라는 글자가 붙는데, 이것이 하드디스크 이외의 보조기억장치 인터페이스 표준을 정의한다.) 이 표준부터 CD-ROM을 비롯한 ODD
장비를 연결할 수 있다. (이전에도 비표준 등으로 지원하기는 했다)

  

전송 방식도 달라져, Ultra DMA 0,1,2를 지원했다. 최대 속도가 33MB/s로 올라갔기 때문에 이 표준을 Ultra ATA/33
이라고도 부른다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ATA?action=edit&section=8)]

## 2.6. ATA/ATAPI-5 (Ultra ATA/66) ¶

이 표준은 2000년에 정식으로 지정되었다. 이 때부터 케이블이 80선으로 바뀐다. 40선 케이블에서 발생하는 신호 간섭을 줄이기 위해 선
사이사이에 접지(Ground) 역할을 하는 선을 추가한 것이다. 이 때문에 빠른 속도가 가능했지만, 선이 너무 많고 가늘어지는 바람에 고장이
잘 나는 부품이 되었다. 따라서 넓적한 리본 케이블이 아닌 둥근 라운드 케이블이 등장한 것도 이 때부터이다. 물론 이 라운드 케이블은
비규격이었기 때문에 신호 간섭에는 취약한 편이었다.

  

전송 방식은 Ultra DMA 3,4까지 지원. 최대 속도가 66MB/s로 올라갔기 때문에 Ultra ATA/66이라고도 부른다.

  

ATA66형 하드가 나왔지만 당시에는 ATA33까지 속도를 낼 수 있는 BX칩셋 메인보드를 거의 많이 사용하는 바람에 66의 진정한 속도를
느끼려면 [SCSI](SCSI.md)같이 컨트롤러를 따로 끼워야 했다. 이유인즉슨
[인텔](%EC%9D%B8%ED%85%94.md)이 RD[RAM](RAM.md)과 함께 주구장창 밀었던 i820의 대참패
때문이었다. 당시 PC133 SDRAM+4X AGP+ATA66이 가능한 메인보드는 [VIA](VIA.md) 694X밖에 없었고, 인텔은
ATA66은 커녕 PC133 SDRAM을 꽂을 수 있는 메인보드가 AGP가 없는 i810E밖에 없었다. 이로 인해 1999년부터 2000년대
초반까지는 [인텔](%EC%9D%B8%ED%85%94.md)이 [VIA](VIA.md)에게 강공을 당한 시기이기도 하다. 결국
[인텔](%EC%9D%B8%ED%85%94.md)은 두손 들고 크게 에러난 i820 SDRAM MTH 버전을 전량 회수했고,
i810E를 좀 고쳐서 i815를 부랴부랴 만들었다.

[[edit](http://rigvedawiki.net/r1/wiki.php/ATA?action=edit&section=9)]

## 2.7. ATA/ATAPI-6 (Ultra ATA/100) ¶

이 표준은 2002년에 지정되었다. 이 때부터 48비트 LBA를 사용하여 최대 용량 137GB의 벽이 깨진다. 2000년대 초반에
137GB를 넘는 하드디스크가 등장하면서 용량 인식이 전부 되지 않는 문제는 이 표준이 아직 적용되지 않은 PC와 OS 때문이었다. 이후 이
규격을 지원하는 메인보드가 속속 나왔고, OS는 업데이트를 통해 해결되었다. 대표적으로 윈도우즈의 경우 XP 서비스팩 1에서 지원되었다.

  

전송 방식도 Ultra DMA 5를 지원, 최대 속도는 100MB/s에 도달했으며, 실제 속도는 동급 최고속 제품이 80MB/s에 달했다.
이 때문에 Ultra ATA/100으로도 불린다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ATA?action=edit&section=10)]

## 2.8. ATA/ATAPI-7 (Ultra ATA/133, SATA 1) ¶

이 때에 이르러서 드디어 넓적한 리본 케이블과 함께 얇고 빨간 케이블이 등장한다. SATA라고 부르는 직렬 전송 케이블이 등장한 것이 이
표준. 이것은 80선짜리 리본 케이블이 고장나기 쉬운 데다가 병렬 방식의 단점인 신호 간섭 때문에 더 이상의 속도 향상이 어렵기 때문에
등장하게 되었다. SATA가 등장하면서 기존의 병렬 케이블을 사용하는 방식을 PATA(Parallel ATA)라고 통칭하게 되었다.`[1]`

  

전송 방식은 Ultra DMA 6을 지원한다. 이에 따라 PATA는 133MB/s까지, SATA는 150MB/s까지 지원하게 되었다.
ODD만 사용한다면 이 이상의 규격은 그다지 의미가 없다. 다만 하드디스크는 표준 ATAPI-7의 실제 대역폭이 사우스브릿지의
ATA컨트롤러에 따라 다소 차이는 있지만 90~100MB/s 정도이므로 대략 2007년 이후 출시된 SATA2 하드디스크는 ATAPI-7에서
성능강하를 보일 수 있다. 참고로 2010년에 출시된 모 국산 하드디스크의 초기 시퀀셜이 이미 150MB/s를 돌파했다.

  

참고로 커넥터부분에 금속잠금기능이 없는 SATA케이블을 사용할 경우 자꾸 케이블이 빠지는 경험을 할 수가 있다. 잠금기능이 있는
SATA케이블은 천원정도에 살 수 있다. 그리고 케이블이 안 꼽힐 때는 무조건 힘으로 넣으려 하지 말고, 꼽는 방향이 맞는지 살펴보자.
방향이 맞으면 쉽게 들어간다. 끼우는 방향이 틀릴 때 너무 힘을 주면 플라스틱으로 된 커넥터가 의외로 약하기 때문에, 쉽게 금이 가거나
심하면 부서지기도 한다.

  

보기 좋게 선정리한다고 케이블을 돼지꼬리처럼 돌돌 말아놓기도 하는데, 내부 단선으로 인해 오류나 합선 등이 일어날 가능성이 있기에 추천하지
않는 방법이다. 있는대로 꽉꽉 접어 케이블타이 따위로 동여매는 짓도 절대 하지 말도록 하자. 미관을 위해서라면 기존의 납작한 SATA
케이블이 아닌 라운드 케이블 구매를 고려해보도록.

[[edit](http://rigvedawiki.net/r1/wiki.php/ATA?action=edit&section=11)]

## 2.9. SATA 3Gb/s (SATA/300, gen 2) ¶

보통 **SATA 2**라는 이명으로 불린다. SATA 1의 2배인 300MB/s를 지원하는 규격으로, 현재 표준에 들어가있다(다만
SATA2라는 이름이 표준이 아니다). 상당수의 하드디스크와 메인보드가 지원하고 있으며, 기계식 보조기억장치의 속도향상 한계로 인해 향후
몇년간은 더 사용될 것으로 보인다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ATA?action=edit&section=12)]

## 2.10. SATA 6Gb/s (SATA/600, gen 3) ¶

보통 **SATA 3**라는 이명으로 불린다. SATA 2의 2배인 600MB/s를 지원하는 규격으로,
[SAS](SAS/%EB%8F%99%EC%9D%8C%EC%9D%B4%EC%9D%98%EC%96%B4#s-7.md)와 호환성이 있다.
일부 하드디스크가 이걸 지원하지만 역시 자체 속도가 발목을 잡는 바람에 큰 의미가 없다. 참고로 2013년 초 일반 하드디스크의 최대
시퀀셜은 200MB/s을 약간 넘는 정도로, 캐시를 통하지 않는 경우에는 SATA/300으로도 충분하다.

  

단 [SSD](SSD.md)의 경우 삼성이나 플렉스터의 신 제품군, 비압축 패턴에 한해서 샌드포스 컨트롤러 등의 이 규격의 대역폭을
충분히 활용하는 제품들이 많이 나오고 있으므로 메인보드 구입 시 지원 여부를 확인해야 한다.

  

현재 위의 [SSD](SSD.md)들이 이 규격의 대역폭의 속도 한계에 부딪쳐서 SATA-express 등의 새로운 규격을 도입하려
하고 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/ATA?action=edit&section=13)]

# 3. 관련항목 ¶

  * [하드디스크](%ED%95%98%EB%93%9C%EB%94%94%EC%8A%A4%ED%81%AC.md)
  * [SSD](SSD.md)
  * [메인보드](%EB%A9%94%EC%9D%B8%EB%B3%B4%EB%93%9C.md)
  * [SCSI](SCSI.md)
  * [SAS](SAS/%EB%8F%99%EC%9D%8C%EC%9D%B4%EC%9D%98%EC%96%B4#s-7.md)  

`\----`

  * `[1]` 정식 명칭까지는 아니다.

