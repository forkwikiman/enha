  * [워크래프트](%EC%9B%8C%ED%81%AC%EB%9E%98%ED%94%84%ED%8A%B8.md) 시리즈에 등장하는 [샤](%EC%83%A4%28%EC%9B%8C%ED%81%AC%EB%9E%98%ED%94%84%ED%8A%B8%29.md)를 찾으십니까?
  * [놈](%EB%86%88.md)의 [오타체](%EC%98%A4%ED%83%80%EC%B2%B4.md)이기도 하다.
Secure Hash Algorithm

> 52532fe14769afa2c1f35d35e5072b89bdc39493  
\- "[http://www.rigvedawiki.net/r1/wiki.php/SHA](SHA.md)"(따옴표 제외)의 SHA-1값

  

> b6b16fa2109fb5865798d6aee4ed370ab60da957c757376eeccd4055a4212850  
\- "[http://www.rigvedawiki.net/r1/wiki.php/SHA](SHA.md)"(따옴표 제외)의 SHA-2중
SHA-256값

  

> 0c58a896cb964559a0f4a9ec60cafc22f1924f0245a47d3f8804785488931909  
968f639b61b6ad7001a26cba2db957e1e021234a32b211bf3c9f060d07850821  
\- "[http://www.rigvedawiki.net/r1/wiki.php/SHA](SHA.md)"(따옴표 제외)의 SHA-3값
<del>길다</del> `[1]`

  
1993년부터 미국 [NSA](NSA.md)가 제작하고 미국 국립표준기술연구소(NIST)에서 표준으로 제작한
[해쉬](%ED%95%B4%EC%89%AC.md) [암호](%EC%95%94%ED%98%B8.md) 알고리즘이다. 1993년
SHA-0을 시작으로, 현재 최신 버전은 2001년 방식이 나온 SHA-2을 사용중이고, 2012년 10월에 SHA-3이 정식 발표되었다.
[#](http://en.wikipedia.org/wiki/SHA-3)

현재 사용중인 SHA-2는 SHA-1을 대체하는 해쉬암호로, SHA-224, SHA-256, SHA-384, SHA-512등의 종류가 있다.
2005년도엔 SHA-1에 보안 구멍이 생겼으며, 2008년 결국 해쉬 충돌이 발생해`[2]` 현재 많이 쓰이는 해쉬암호 기술이다. 그러나,
일단 기본은 SHA-1과 큰 차이가 없다(...) 현재는 SHA-1과 2와 생판다른 알고리즘인 SHA-3을 개발중이며`[3]`, 2012년
10월 2일자로 [Keccak](http://keccak.noekeon.org)이 SHA-3로 확정되었다.
[#](http://www.nist.gov/itl/csd/sha-100212.cfm)

[대한민국](%EB%8C%80%ED%95%9C%EB%AF%BC%EA%B5%AD.md)
[인터넷뱅킹](%EC%9D%B8%ED%84%B0%EB%84%B7%EB%B1%85%ED%82%B9.md)은 SHA-256을 사용하고
있으며`[4]`, [비트토런트](%EB%B9%84%ED%8A%B8%ED%86%A0%EB%9F%B0%ED%8A%B8.md)는 파일을
BASE32로 바꾼 SHA-1을 해쉬로 사용한다.
[비트코인](%EB%B9%84%ED%8A%B8%EC%BD%94%EC%9D%B8.md)은 작업 증명에 SHA-256을 사용한다.

SHA는 파일 값이 약간만 바뀌어도 값이 천차 만별로 바뀔수 있다. 보통 이를 가리켜 [눈사태효과](%EB%88%88%EC%82%AC%ED%83%9C%20%ED%9A%A8%EA%B3%BC.md)라 부른다.

`\----`

  * `[1]` 이것은 엄밀히 말해서 Keccak(r=576, c=1024)의 512-bit 해시값이다. Keccak 알고리즘은 이전의 SHA 알고리즘과는 달리 출력 길이가 제한되어 있지 않고, 알고리즘 자체에도 변경 가능한 파라미터가 있기에 어떤 파라미터를 쓰느냐에 따라 얼마든지 결과값이 달라질 수 있다.
  * `[2]` 아 물론 이건 알려진 것이다. **모든 암호화 알고리즘이 다 그렇지만 암호학의 지하에선 더 빨리 뚫렸을지 모른다**(...)
  * `[3]` 개발이라기보단, 여러 보안 전문가들과 [컴덕후](%EC%BB%B4%EB%8D%95%ED%9B%84.md)들이 만들어낸 해시 알고리즘 중 몇 개를 추려서 가장 견고한 것에 SHA-3 딱지를 붙이는 **공모전**에 가깝다. [고려대학교](%EA%B3%A0%EB%A0%A4%EB%8C%80%ED%95%99%EA%B5%90.md)에서도 [아리랑](%EC%95%84%EB%A6%AC%EB%9E%91.md)이라는 이름으로 출품했지만... **[광탈](%EA%B4%91%ED%83%88.md)해버렸다**(...) 3차 후보까지 남은 건 [BLAKE](http://131002.net/blake), [Grøstl](http://www.groestl.info), [JH](http://www3.ntu.edu.sg/home/wuhj/research/jh/index.html), [Keccak](http://keccak.noekeon.org), [Skein](http://www.skein-hash.info)의 5개 알고리즘이다.
  * `[4]` 2011년 전까진 2008년에 이미 뚫린(...) SHA-1을 사용중이었다(...)

