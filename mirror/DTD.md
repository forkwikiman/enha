  * [동음이의어·다의어/알파벳](%EB%8F%99%EC%9D%8C%EC%9D%B4%EC%9D%98%EC%96%B4%C2%B7%EB%8B%A4%EC%9D%98%EC%96%B4/%EC%95%8C%ED%8C%8C%EB%B2%B3.md)  

## Contents

    

1. Day to Day 
2. Document Type Definition 
3. Down Team is Down 
4. [소드걸스](%EC%86%8C%EB%93%9C%EA%B1%B8%EC%8A%A4.md)의 세계의 파괴자 DTD 
5. [프로레슬링](%ED%94%84%EB%A1%9C%EB%A0%88%EC%8A%AC%EB%A7%81.md) [PPV](PPV.md) December To Dismember 
6. [무한의 프론티어](%EB%AC%B4%ED%95%9C%EC%9D%98%20%ED%94%84%EB%A1%A0%ED%8B%B0%EC%96%B4.md)에 나오는 코드 DTD 
7. 그 외 

[[edit](http://rigvedawiki.net/r1/wiki.php/DTD?action=edit&section=1)]

## 1. Day to Day ¶

하루하루.

  

주로 스포츠에서 부상 당한 선수의 상황에 쓰는 말로 부상정도를 하루 하루 지켜보면서 복귀냐 치료냐를 결정하는 단계를 말한다.`[1]`
[판타지리그](%ED%8C%90%ED%83%80%EC%A7%80%EB%A6%AC%EA%B7%B8.md)를 하는 사람들에게 제일 짜증나는
상태. 나올지 안나올지 판단하기 매우 어렵기 때문이다. 때문에 이 상태가 되면 FL에선
[계륵](%EA%B3%84%EB%A5%B5.md)이다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/DTD?action=edit&section=2)]

## 2. Document Type Definition ¶

[XML](XML.md) 파일은 프로그램이 자체적으로 파서를 내장하고 있지 않은 한 생전 처음 보는 태그들이 마구 떠주는데, 이럴 때
처음 부분에서 어떤 DTD를 가리키고 있는지 찾아서 실제로 어떤 녀석인지를 파악하는 데 쓴다.  
무슨 말인지 모르겠는가? **지금 당장 소스 보기로 리그베다 위키를 뜯어봐라.** 첫줄에 떡하니 다음과 같은 문구가 자리하고 있을 것이다.  

    
    
    <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">

저기서 <http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd> 부분이 DTD 파일이다.
메모장으로 열면 아-주 복잡한 게 난잡하게 써 있을 거다.

  

단 실제로 XHTML을 제외하고 개발자들이 접하게 되는 대다수의 XML 파일은 대개 프로그램 내적으로 처리하기 때문에 소스 뜯어봐도 DTD
파일이 안 써있는 경우가 많을 것이다.

  

이것과는 별도로 보고자 하는 XML이 원래 브라우저용이 아닌데 브라우저에 제대로 보이게 하려면 XSL(eXtensible Stylesheet
Language)이라는 것을 또 따로 써줘야 한다. `[2]`

  

여담으로 HTML 4.01이든 XHTML 1.0이든 뭐든 간에 어쨌든 파일
[확장자](%ED%99%95%EC%9E%A5%EC%9E%90.md)는 .html이기 때문에 브라우저가 파일 확장자만 가지고는 이게 어떤
규격으로 쓰여진 파일인지 알 수가 없기 때문에 **이걸 꼭 써줘야 [웹브라우저](%EC%9B%B9%20%EB%B8%8C%EB%9D%BC%EC%9A%B0%EC%A0%80.md)마다 레이아웃이 달라지는 것을
1차적으로 막을 수 있다.** <del>[물론 그 와중에도](%EC%9D%B8%ED%84%B0%EB%84%B7%20%EC%9D%B5%EC%8A%A4%ED%94%8C%EB%A1%9C%EB%9F%AC.md) [깨질 놈들은 깨진다](%EB%82%B4%EB%A0%A4%EA%B0%88%20%ED%8C%80%EC%9D%80%20%EB%82%B4%EB%A0%A4%EA%B0%84%EB%8B%A4.md)</del>.
하지만 웹 표준 바람이 불기 전까지는 [귀차니즘](%EA%B7%80%EC%B0%A8%EB%8B%88%EC%A6%98.md) 등의 이유로
거의 쓰는 일이 없었고, **그 결과는 [와장창](%EC%99%80%EC%9E%A5%EC%B0%BD.md)**(...)

  

[HTML5](HTML5.md)는 XHTML에서 형식상 많은 부분을 가져오기는 했지만 어쨌든 XML은 아니기 때문에 DTD 파일 경로를
쓰지 않고  

    
    
    <!DOCTYPE html>

그냥 이렇게 쓰면 독타입 선언이 끝난다. 그리고 이걸 어떻게 파싱할까는 그냥 브라우저 내부에서 결정한다. 나중에 HTML5의 표준안이
확정되면 어떻게 바뀔지는 모르지만 아무튼 현재는 그런 상태.

[[edit](http://rigvedawiki.net/r1/wiki.php/DTD?action=edit&section=3)]

## 3. Down Team is Down ¶

**주의. 비하적 내용이 포함된 문서입니다.**  
  
본 문서와 하위 문서는 불쾌감을 느낄 수 있는 [욕설](%EC%9A%95%EC%84%A4.md) 등의 비하적 내용에 대한 직접·간접적인
언급 혹은 설명을 포함하고 있습니다. 또한 이 문서에는 욕설과 모욕적인 표현이 있으므로 열람시 주의를 요하며, 열람을 원하지 않을 경우 이
문서를 닫아 주세요.

  

  

![http://rigvedawiki.net/r1/pds/_eb_82_b4_eb_a0_a4_ea_b0_88_20_ed_8c_80_ec_9d_
80_20_eb_82_b4_eb_a0_a4_ea_b0_84_eb_8b_a4/ㅇㅅㅇ_1.gif](//rv.wkcdn.net/http://rig
vedawiki.net/r1/pds/_eb_82_b4_eb_a0_a4_ea_b0_88_20_ed_8c_80_ec_9d_80_20_eb_82_
b4_eb_a0_a4_ea_b0_84_eb_8b_a4/%E3%85%87%E3%85%85%E3%85%87_1.gif)

[[GIF external image]](http://rigvedawiki.net/r1/pds/_eb_82_b4_eb_a0_a4_ea_b0_
88_20_ed_8c_80_ec_9d_80_20_eb_82_b4_eb_a0_a4_ea_b0_84_eb_8b_a4/%E3%85%87%E3%85
%85%E3%85%87_1.gif)

  
**[내려갈 팀은 내려간다](%EB%82%B4%EB%A0%A4%EA%B0%88%20%ED%8C%80%EC%9D%80%20%EB%82%B4%EB%A0%A4%EA%B0%84%EB%8B%A4.md)**

  

전 [현대 유니콘스](%ED%98%84%EB%8C%80%20%EC%9C%A0%EB%8B%88%EC%BD%98%EC%8A%A4.md),
[LG 트윈스](LG%20%ED%8A%B8%EC%9C%88%EC%8A%A4.md) 감독<del>이자 세계적 권위의 이론
물리학자</del>이었던 [김재박](%EA%B9%80%EC%9E%AC%EB%B0%95.md)이 남긴 명언. 자세한 건
[김재박](%EA%B9%80%EC%9E%AC%EB%B0%95.md)이나
[명언/야구](%EB%AA%85%EC%96%B8/%EC%95%BC%EA%B5%AC.md)항목 참조.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/DTD?action=edit&section=4)]

## 4. [소드걸스](%EC%86%8C%EB%93%9C%EA%B1%B8%EC%8A%A4.md)의 세계의 파괴자 DTD ¶

![http://www.sword-girls.co.kr/Img/Card/300301L.jpg](http://www.sword-
girls.co.kr/Img/Card/300301L.jpg)

[[JPG external image]](http://www.sword-girls.co.kr/Img/Card/300301L.jpg)

  

무소속 더블 레어 카드. 특수능력은 없지만 기본 스테이터스가 좋다. 공12, 방3, 체15.  
깡스텟으로 승부하는 카드인지라 어떤상황이든 대충 던져놔도 대충 기대만큼의 성능은 해준다. 다만 사이즈가 큰편이라 올리기가 꽤 껄끄러우며,
디버프를 당하면 그대로 애물단지가 돼버리는 단점이 있다.<del>아무래도 **Down Team is Down**과 관련이 있는
것같다..</del><del>내려갈 카드는 내려간다...</del>

  

[[edit](http://rigvedawiki.net/r1/wiki.php/DTD?action=edit&section=5)]

## 5. [프로레슬링](%ED%94%84%EB%A1%9C%EB%A0%88%EC%8A%AC%EB%A7%81.md)
[PPV](PPV.md) December To Dismember ¶

2006년 [WWE](WWE.md)가 개최한 <del>WWE 역사에 기억될만한</del> [PPV](PPV.md) [디셈버 투 디스멤버](%EB%94%94%EC%85%88%EB%B2%84%20%ED%88%AC%20%EB%94%94%EC%8A%A4%EB%A9%A4%EB%B2%84.md)의 약자.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/DTD?action=edit&section=6)]

## 6. [무한의 프론티어](%EB%AC%B4%ED%95%9C%EC%9D%98%20%ED%94%84%EB%A1%A0%ED%8B%B0%EC%96%B4.md)에 나오는 코드 DTD ¶

[아센 브레이델](%EC%95%84%EC%84%BC%20%EB%B8%8C%EB%A0%88%EC%9D%B4%EB%8D%B8.md)이
<del>벗어제끼면서</del>발동하는 특수코드.

  

가동시 성능이 오르지만 열폭주를 이용하기에 방열을 위해 <del>벗어제끼며</del>피부노출도가 오르고, 왠지모르지만 성격도 좀 이상해진다.
이름은 기독교쪽 진혼시에 나오는 soil to soil, ash to ash, dust to dust(흙은 흙으로, 재는재로, 먼지는
먼지로)구절의 마지막에서 따온듯. 여담이지만 이 구절은 판타지계열에서 주문으로 의외로 자주 나온다.

  

물론 무한의 프론티어가 아닌 정식 슈퍼로봇대전 OG [라미아 라브레스](%EB%9D%BC%EB%AF%B8%EC%95%84%20%EB%9D%BC%EB%B8%8C%EB%A0%88%EC%8A%A4.md)도 사용할수 있다

  

[[edit](http://rigvedawiki.net/r1/wiki.php/DTD?action=edit&section=7)]

## 7. 그 외 ¶

[ㅇㅅㅇ](%E3%85%87%E3%85%85%E3%85%87.md)을 영타로 치면 나오는 단어. ㅇㅅㅇ이 손에 익은 사람은 잡다한
파일들의 이름을 ㅇㅅㅇ로 짓다가 꽉 차버리면 dtdt 따위로 만들기도 한다.  

`\----`

  * `[1]` 부상자 명단 등록이나 2군 이동등의 조치를 하게되면 최소 7~10일동안은 선수 기용이 불가능하다.
  * `[2]` IIS 로그에 익숙한 사람들이나 Windows Live Messenger의 대화록을 열어본 경우 얘네가 왜 브라우저로 보이는지 의문을 가졌을 수 있을텐데, 그 배후에는 DTD가 아니라 XSL이 있는 것이다.

