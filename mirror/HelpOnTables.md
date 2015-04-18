**[위키 관련 정보](%EC%9C%84%ED%82%A4%20%EA%B4%80%EB%A0%A8%20%EC%A0%95%EB%B3%B4.md)**

**주요 도움**
[위키를 작성하기 전에](%EC%9C%84%ED%82%A4%EB%A5%BC%20%EC%9E%91%EC%84%B1%ED%95%98%EA%B8%B0%20%EC%A0%84%EC%97%90.md)

[리그베다 위키 기본방침](%EB%A6%AC%EA%B7%B8%EB%B2%A0%EB%8B%A4%20%EC%9C%84%ED%82%A4%20%EA%B8%B0%EB%B3%B8%EB%B0%A9%EC%B9%A8.md)

[인터페이스 설명](HelpForBeginners.md)

[항목 생성하기](HelpOnPageCreation.md)

[편집 도움말](HelpOnEditing.md)

**보조 도움**
[위키 연습장 1](WikiSandbox.md)

[위키 연습장 2](Wiki%20Sandbox.md)

[단축키](%EB%8B%A8%EC%B6%95%ED%82%A4.md)

[추가기능](%EC%B6%94%EA%B0%80%EA%B8%B0%EB%8A%A5.md)

[FAQ](FAQ.md)

* * *

[리그베다 위키](%EB%A6%AC%EA%B7%B8%EB%B2%A0%EB%8B%A4%20%EC%9C%84%ED%82%A4.md)의 표
작성에 사용되는 각종 확장문법에 대한 설명입니다.

## Contents

    

1. 병합 
    

1.1. 가로줄 병합

1.2. 세로줄 병합

2. 정렬 
    

2.1. 가로 정렬

2.2. 세로 정렬

2.3. 표 위치 정렬

3. 배경 색 
    

3.1. 각 셀의 배경색 지정

3.2. 표 전체 배경색 지정

3.3. 한 줄 배경색 지정

4. 테두리 
    

4.1. 테두리 색상 지정

5. 표 크기 
    

5.1. 표 전체의 가로크기 지정

    

5.1.1. 상대크기 지정

5.1.2. 절대크기 지정

5.2. 각 셀의 가로크기 지정

6. 캡션 

[[edit](http://rigvedawiki.net/r1/wiki.php/HelpOnTables?action=edit&section=1)
]

## 1. 병합 ¶

편집 도움말 페이지에 설명된 간단한 가로병합 기능 외에, 문법을 이용한 병합기능이 있습니다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/HelpOnTables?action=edit&section=2)
]

### 1.1. 가로줄 병합 ¶

가로줄 병합은 <-#> 형태로, 가로선을 태그로 사용합니다.

  

#에 적당히 큰 숫자를 집어넣으면, 셀의 개수를 일일이 세지 않아도 통째로 합칠 수 있습니다.

  

    
    
    ||1열||2열||3열||4열||5열||||한칸||||<-2>두칸||||<-3>세칸||||<-4>네칸||||<-100>한줄 통째로||

1열

2열

3열

4열

5열

한칸

두칸

세칸

네칸

다섯칸

한줄 통째로

[[edit](http://rigvedawiki.net/r1/wiki.php/HelpOnTables?action=edit&section=3)
]

### 1.2. 세로줄 병합 ¶

세로줄 병합은 <|#> 형태로, 세로선을 태그로 사용합니다. 참고로 뒷부분에 뭐든 내용이 있어야만 작동하니 주의 공백으로 하고싶다면 (
)`[1]`을 입력하도록하자

  

#에 적당히 큰 숫자를 집어넣으면, 셀의 개수를 일일이 세지 않아도 통째로 합칠 수 있습니다.

  

    
    
    ||1행||<|1>1줄||<|2>2줄||<|3>3줄||<|4>||<|100>세로 통째로||||2행||||3행||||4행||||5행||

1행

1줄

2줄

3줄

4줄

세로 통째로

2행

3행

4행

5행

`[2]`

[[edit](http://rigvedawiki.net/r1/wiki.php/HelpOnTables?action=edit&section=4)
]

## 2. 정렬 ¶

편집 도움말에 간단히 기술된 정렬방식 외에, 태그를 사용한 정렬이 가능합니다.

  

특히, 위의 병합 태그를 사용하여 표를 병합한 경우엔, 정렬 태그를 사용해야 정렬이 됩니다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/HelpOnTables?action=edit&section=5)
]

### 2.1. 가로 정렬 ¶

기본은 왼쪽 정렬입니다.

  

  * 왼쪽 정렬: <(> 태그를 사용합니다.
  * 가운데 정렬: <:> 태그를 사용합니다.
  * 오른쪽 정렬: <)> 태그를 사용합니다.  

  

    
    
    ||　첫번째 열　||　두번째 열　||　세번째 열　||||<(>왼쪽 정렬||<:>가운데 정렬||<)>오른쪽 정렬||||<-3><(>병합 후 왼쪽 정렬||||<-3><:>병합 후 가운데 정렬||||<-3><)>병합 후 오른쪽 정렬||

　첫번째 열

　두번째 열

　세번째 열

왼쪽 정렬

가운데 정렬

오른쪽 정렬

병합 후 왼쪽 정렬

병합 후 가운데 정렬

병합 후 오른쪽 정렬

[[edit](http://rigvedawiki.net/r1/wiki.php/HelpOnTables?action=edit&section=6)
]

### 2.2. 세로 정렬 ¶

기본은 가운데 정렬입니다.

  

세로정렬은 가로정렬과 달리 단독으로 사용되지 않고, 세로병합을 할 때 붙여줘야 합니다.

  

  * 위쪽 정렬: <^|#> 형태로, 병합하는 태그 앞에 ^ 를 붙입니다.
  * 가운데 정렬: 기본이며, 아무 기호도 붙이지 않습니다.
  * 아래쪽 정렬: <v|#> 형태로, 병합하는 태그 앞에 v 를 붙입니다.  

  

    
    
    ||1행||<^|4>위쪽 정렬||<|4>가운데 정렬||<v|4>아래쪽 정렬||||2행||||3행||||4행||

1행

위쪽 정렬

가운데 정렬

아래쪽 정렬

2행

3행

4행

[[edit](http://rigvedawiki.net/r1/wiki.php/HelpOnTables?action=edit&section=7)
]

### 2.3. 표 위치 정렬 ¶

  

<tablealign=위치> 태그를 사용하면 표 자체의 위치를 변경할 수 있습니다.

  

  * 왼쪽 정렬: 기본이며, 아무 기호도 붙이지 않습니다.
  * 가운데 정렬: <tablealign=center> 태그를 사용합니다.
  * 오른쪽 정렬: <tablealign=right> 태그를 사용합니다.  

  

    
    
    ||<-2>왼쪽 정렬||||<:>A||<:>B||

왼쪽 정렬

A

B

  

    
    
    ||<-2><tablealign=center>가운데 정렬||||<:>A||<:>B||

가운데 정렬

A

B

  

    
    
    ||<-2><tablealign=right>오른쪽 정렬||||<:>A||<:>B||

오른쪽 정렬

A

B

[[edit](http://rigvedawiki.net/r1/wiki.php/HelpOnTables?action=edit&section=8)
]

## 3. 배경 색 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/HelpOnTables?action=edit&section=9)
]

### 3.1. 각 셀의 배경색 지정 ¶

<bgcolor=#000000> 형태의 태그를 넣어주면 해당 칸의 배경색을 지정해줄 수 있으며, 리그베다 위키에서는 단순히 <#000000>
으로 간략하게 지정해도 가능합니다. 참고로 뒷부분에 뭐든 내용이 있어야만 작동하니 주의 공백으로 하고싶다면 (　)`[3]`을
입력하도록하자.`[4]`

  

# 태그 뒤의 여섯자리 숫자는 RGB 코드입니다.

  

    
    
    ||<-10><:>무지개 색깔 || ||<bgcolor=#FF0000> 빨 ||<#FFA500> 주 ||<#FFFF00> 노 ||<#009900> 초 ||<#0000FF> 파 ||<#082567> 남 ||<#8000FF> 보 ||

무지개 색깔

빨

주

노

초

파

남

보

[[edit](http://rigvedawiki.net/r1/wiki.php/HelpOnTables?action=edit&section=10
)]

### 3.2. 표 전체 배경색 지정 ¶

표의 배경색은 표의 가장 첫 칸에 tablebgcolor 태그를 사용하여 지정해줍니다.

  

    
    
    ||<tablebgcolor=#00FF00> 우리강산 푸르게 푸르게 |||| 나무를 심어줄게 |||| 산아 산아 이겨라 ||

우리강산 푸르게 푸르게

나무를 심어줄게

산아 산아 이겨라

[[edit](http://rigvedawiki.net/r1/wiki.php/HelpOnTables?action=edit&section=11
)]

### 3.3. 한 줄 배경색 지정 ¶

해당하는 줄의 가장 첫 칸에 rowbgcolor 태그를 사용합니다.

  

    
    
    ||<rowbgcolor=#000000>안 보이지?||이것도 안 보이지?||||<rowbgcolor=#FFFFFF>산은 산이요||물은 물이로다.||||<rowbgcolor=#FF0000>이 색깔을 입히면||3배 빨라지지.||

안 보이지?

이것도 안 보이지?

산은 산이요

물은 물이로다.

이 색깔을 입히면

3배 빨라지지.

[[edit](http://rigvedawiki.net/r1/wiki.php/HelpOnTables?action=edit&section=12
)]

## 4. 테두리 ¶

  

[[edit](http://rigvedawiki.net/r1/wiki.php/HelpOnTables?action=edit&section=13
)]

### 4.1. 테두리 색상 지정 ¶

  

해당하는 표의 가장 첫 칸에 table bordercolor 태그를 사용합니다.

  

  * 가장 바깥쪽 테두리의 색상만 변경하실 수 있습니다.
  * 표의 굵기는 자동으로 하단의 예시와 같게 설정됩니다.
  

    
    
    ||<table bordercolor="red">테두리 색상 변경||테두리 색상 변경||

테두리 색상 변경

테두리 색상 변경

  

    
    
    ||<table bordercolor=#00FF00>테두리 색상 변경||테두리 색상 변경||

테두리 색상 변경

테두리 색상 변경

[[edit](http://rigvedawiki.net/r1/wiki.php/HelpOnTables?action=edit&section=14
)]

## 5. 표 크기 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/HelpOnTables?action=edit&section=15
)]

### 5.1. 표 전체의 가로크기 지정 ¶

표의 가로크기를 지정하고 싶은 경우, 가장 첫 칸에 tablewidth 태그를 사용합니다.

  

표의 크기는 상대크기 지정, 절대크기 지정의 두 가지 방식이 있습니다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/HelpOnTables?action=edit&section=16
)]

#### 5.1.1. 상대크기 지정 ¶

%를 사용하면, 창의 크기에 따라 표의 크기도 달라집니다.

  

다만, 리그베다 위키는 가로크기가 600 픽셀로 고정되어 있으므로, 100%를 사용하면 그냥 600 픽셀입니다.

  

    
    
    ||<tablewidth=100%> 한줄 가득 차게 ||

한줄 가득 차게

[[edit](http://rigvedawiki.net/r1/wiki.php/HelpOnTables?action=edit&section=17
)]

#### 5.1.2. 절대크기 지정 ¶

px 혹은 cm 등을 사용하여 표의 구체적인 크기를 지정할 수 있습니다.

  

    
    
    ||<tablewidth=400px> 400px ||

400px

  

    
    
    ||<tablewidth=4cm> 4cm ||

4cm

[[edit](http://rigvedawiki.net/r1/wiki.php/HelpOnTables?action=edit&section=18
)]

### 5.2. 각 셀의 가로크기 지정 ¶

셀 각각의 가로크기는 width 태그를 사용합니다.

  

    
    
    ||<tablewidth=100%><-10><:> 가로크기 100%중에 ||||<width=10%><#FF0000> 빨강은 10% ||<width=20%><#00FF00> 초록은 20% ||<width=30%><#0000FF> 파랑은 30% ||<width=40%> 나머지는 잉여 ||

가로크기 100%중에

빨강은 10%

초록은 20%

파랑은 30%

나머지는 잉여

  

    
    
    ||<tablewidth=100%><width=10%><#FF0000> 빨강은 10% ||<width=20%><#00FF00> 초록은 20% ||<width=30%><#0000FF> 파랑은 30% ||<width=40%> 나머지는 잉여 ||

빨강은 10%

초록은 20%

파랑은 30%

나머지는 잉여

[[edit](http://rigvedawiki.net/r1/wiki.php/HelpOnTables?action=edit&section=19
)]

## 6. 캡션 ¶

`|`를 사용하여 캡션을 달 수 있습니다.

  

    
    
    |'''캡션'''|<tablebgcolor=#CCCCCC>|||| '''캡션 있는 테이블'''||||<|2> 1호 || 2호 |||| 3호 ||

**캡션**

**캡션 있는 테이블**

1호

2호

3호

`\----`

  * `[1]` ㄱ 한자변환 1
  * `[2]` 알아보기 쉽게 색을 첨가했습니다. 실제로 위에 나온대로 입력한 것과 표색에 차이가 있으니 주의
  * `[3]` ㄱ 한자변환 1
  * `[4]` 표를 만드는 부분에서 가장 간과하는 부분이 바로 여기입니다.

