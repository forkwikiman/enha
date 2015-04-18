U+00A0, NO-BREAK SPACE. 줄여서 NBSP.  
HTML 엔티티는 &nbsp;이다.

일반적으로 사용되는 U+0020 SPACE( )와는 기능이 다르다. 영어 등의 서양 언어에서는 워드 랩을 적용할 때 space를 기준으로
하며, 따라서 space가 삽입된 위치에서 줄을 바꾼다.  
the quick brown fox를 예로 들자면 각 단어는 space로 구분돼 있으며, 워드 랩을 적용했을 때 the와 quick 사이,
quick과 brown 사이, brown과 fox 사이에서 줄이 나뉠 수 있다.

반면 no-break space는 외관상으로는 space와 똑같이 보이지만, 이 위치에서는 줄이 나뉠 수 없음을 의미한다. quick과
brown 사이에 no-break space가 쓰인 the quick brown fox를 예로 들자면, 워드 랩 적용 시 the와 quick
사이, brown과 fox 사이에서는 줄이 나뉠 수 있지만 quick과 brown 사이에서는 줄이 나뉠 수 없다.  

그리고 이 문자는 에서도 유용하게 쓰인다. HTML은 소스에 space 문자를 연속으로 여러 번 써도 출력 결과는 그냥 space를 하나 쓴
것과 차이가 없다. 공백 문자를 연속으로 여러 개 삽입하고 싶을 경우 no-break space를 써 주면 정상적으로 출력된다.  

이 항목은 NBSP로도 들어올 수 있다.  

