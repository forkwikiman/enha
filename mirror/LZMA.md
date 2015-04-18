Lempel–Ziv–Markov chain algorithm

[7zip](7zip.md)의 제작자인 Igor Pavlov에 의해 개발된 데이터 압축 알고리즘. [7z](7z.md) 포맷에
사용되고 있으며, [퍼블릭도메인](%ED%8D%BC%EB%B8%94%EB%A6%AD%20%EB%8F%84%EB%A9%94%EC%9D%B8.md)으로
[SDK](SDK.md)를 공개하였다.

[LZMA SDK 홈페이지](http://www.7-zip.org/sdk.html)

이 압축 알고리즘은 1차적으로 LZ77 알고리즘을 이용해서 데이터를 압축하고, 2차적으로 Adaptive Binary Range Coder를
이용해서 압축을 수행한다.

일반적으로 [RAR](RAR.md)포맷에서 사용하는 압축 알고리즘보다 압축률이 좋은 것으로 알려져 있으며, 효율이 좋은 이유는 매우 큰
LZ77 윈도우(4GiB 까지)를 사용하고, 압축 효율을 높이기 위한 최적화가 잘 되었기 때문.

SDK는 공개되어 있지만, 속도 향상을 위해서 코드가 복잡하고, 주석도 한 줄 안 달려 있기 때문에 공개된 소스를 가지고 변형해서 뭔가
다른걸 만들어 보는 것은 거의 불가능한 수준.

[이스트소프트](%EC%9D%B4%EC%8A%A4%ED%8A%B8%EC%86%8C%ED%94%84%ED%8A%B8.md)에서 공개한
[EGG](EGG.md) 포맷은 공개된 압축 알고리즘인 [Deflate](Deflate.md),
[bzip2](bzip2.md), LZMA 이외에도 자체적으로 개발한 [AZO](AZO.md) 알고리즘을 사용하는데, 이
알고리즘은 LZMA와 거의 똑같은 방식을 사용하는 것으로 보인다.

[LZMA2](LZMA2.md)는 LZMA가 멀티 코어 지원에 취약(최대 2개의 쓰레드만 지원)한 점을 개선하기 위해서 만들어진
알고리즘이며, 사용 가능한 수 만큼 쓰레드를 사용하여 병렬로 압축을 하기 때문에 속도가 무척 빠르지만, 메모리도 그만큼 정수 배로 사용하기
때문에 메모리 사용량도 엄청나다. `[1]`

압축 효율이 좋으며, 퍼블릭 도메인으로 공개된 압축 알고리즘이기 때문에 [ZIP](ZIP.md)이나
[EGG](EGG.md)포맷에서도 이 압축 알고리즘을 사용한다.

[[edit](http://rigvedawiki.net/r1/wiki.php/LZMA?action=edit&section=1)]

## 관련 항목 ¶

  

  * [7z](7z.md)
  * [ZIP](ZIP.md)
  * [NSIS](NSIS.md)
  * [EGG(알집)](EGG%28%EC%95%8C%EC%A7%91%29.md)
  * [LZMA2](LZMA2.md)  
  
  

`\----`

  * `[1]` 예를 들어 압축률 최대를 사용하여 8쓰레드로 압축할 경우 최대 4*8GiB 메모리를 필요로 한다.

