[Deflate](Deflate.md) 압축 알고리즘을 [C](C%28%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D%20%EC%96%B8%EC%96%B4%29.md) 언어로 구현한 라이브러리이다.

홈페이지는 <http://www.zlib.net/>

zlib 와 deflate 를 구분하지 못하는 경우가 종종 있는데, deflate 는 압축 알고리즘이고, zlib 는 이걸 실제 프로그래밍
언어로 구현한 구현체 이다. 이 둘을 혼동하는 것은 설계도와 이를 토대로 만든 기계 실물을 헷갈리는 격.
<del>[한글](%ED%95%9C%EA%B8%80.md)과 [한국어](%ED%95%9C%EA%B5%AD%EC%96%B4.md)를
헷갈리는 사람도 있는 판이니</del>

원래 [Deflate](Deflate.md) 는 [ZIP](ZIP.md)포맷에 사용하기 위해서 만들어진 [비손실 압축 알고리즘](
/wiki/%EB%AC%B4%EC%86%90%EC%8B%A4%20%EC%95%95%EC%B6%95%20%ED%8F%AC%EB%A7%B7)
인데, 이 알고리즘이 구현되자 이를 Jean-Loup Gailly 와 Mark Adler 가 [오픈소스](%EC%98%A4%ED%94%88%20%EC%86%8C%EC%8A%A4.md)로 구현후 공개한것이 zlib 이다.

zlib 의 특징은 완전 무료로 거의 제한 없이 사용 가능한 라이선스([zlib license](zlib%20license.md)) 와
매우 deflate 압축 알고리즘을 매우 빠르게 구현하였고, 이식성이 높은 c 언어를 사용하였다는 것이다.

이때문에 압축 알고리즘계의 산업 표준이며 수 많은 프로그램에 이식되어 사용되고 있다.

