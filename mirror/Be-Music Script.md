## Contents

    

1. 개요 
2. **[BMS/목록](BMS/%EB%AA%A9%EB%A1%9D.md)(이름순)**
3. BMS 아티스트 
    

3.1. 일본

3.2. 한국

3.3. 이외 국가의 BMS 아티스트

3.4. BMS 활동을 중단한 아티스트

4. BGA 아티스트 
5. BMS 제작팀 / 레이블 
6. BMS 이벤트 
7. 관련 용어 
8. 유통방식 
    

8.1. BMS 이벤트

8.2. 패키지

8.3. 투고 사이트

9. BMS 관련 사이트 
10. 주요 BMS/PMS 구동기 목록 
    

10.1. 구세대 구동기

10.2. 현세대 구동기

10.3. 불법 구동기

[[edit](http://rigvedawiki.net/r1/wiki.php/Be-
Music%20Script?action=edit&section=1)]

### 1. 개요 ¶

![1223773908_lunaticrave.png](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/122
3773908_lunaticrave.png)

[PNG image (192.07 KB)]

![1223773908_ruvit1.png](//rv.wkcdn.net/http://rigvedawiki.net/r1/pds/12237739
08_ruvit1.png)

[PNG image (246.1 KB)]

  

(위의 스크린샷은 각각 Lunatic Rave, ruv-it에서 BMS를 구동한 스크린샷)  

  

[BM98](BM98.md)을 시작으로 프리웨어
[리듬게임](%EB%A6%AC%EB%93%AC%EA%B2%8C%EC%9E%84.md)에서 사용하는 파일 형식.

  

BMS포멧은 일본의 프로그래머인 Yane Urao가 1998년에 제안한 것이다. BMS형식은
[beatmania](beatmania.md)의 연습용으로 만들어진 [BM98](BM98.md)에서 처음 사용되었다. 이 포멧은
그 이후에 만들어진 수많은 bms구동기에서도 차용되었다.

  

이 BMS를 직접 만드는 것이 장난이 아닌 노가다 작업이다. 배경음, [키음](%ED%82%A4%EC%9D%8C.md) 등을 배치할
위치를 일일히 하나하나 잡아야 하기 때문이다. 게임 유저데이터 제작 중에서 노가다가 아닌 것이 없긴 하지만.

  

BMS들의 [확장자](%ED%99%95%EC%9E%A5%EC%9E%90.md)는 아래의 네 가지 형태가 있다.  
(이것은 새로 만들어진 BMS가 예전 프로그램에서 지원하지 않는 기능을 탑재한 경우 인식을 하지 못하기 때문에 확장자를 분리한 것.
Lunatic Rave나 ruv-it`[1]` 등의 버전에서는 모든 확장자가 플레이 가능하다.)  

  * BMS - Be-Music Script (5키만을 지원하는 BM98때의 데이터)
  * BME - Be-Music Extended (키를 7개로 늘린 것 - 5키밖에 없어도 BM98때는 없었던 확장 기능을 사용하는 것은 BME라고 분류하기도 한다.)
  * BML - Be-Music Longnote (BMS나 BME에다 EZ2DJ 형태의 [롱노트](%EB%A1%B1%EB%85%B8%ED%8A%B8.md)를 추가한 데이터)
  * PMS - 약자는 불명(Pop'n Music Script쯤 이라고 추측). [모 게임](%ED%8C%9D%ED%94%88%EB%AE%A4%EC%A7%81.md)처럼 9키를 사용하는 데이터. 그래서 BMS와는 난이도 책정 기준이 다르다`[2]`. 이쪽은 지원하는 플레이어가 극소수이며, feeling pomu라는 전용 플레이어가 과거에 있었고, 현재는 nanasi groove 시리즈와 Lunatic Rave 시리즈에서 지원한다.  

처음에는 [WAV](WAV.md) 형식의 사운드 파일과 [BMP](BMP.md) 형식의 그림 파일밖에 사용을 못 했으나,
BMS플레이어가 발전하면서 그림 파일을 [JPG](JPG.md)나 [PNG](PNG.md)로, 사운드 파일을
[MP3](MP3.md)나 [Ogg Vorbis](Ogg%20Vorbis.md)로(다만 MP3쪽은 사실 거의 안 쓰고 대부분
Ogg Vorbis 쪽으로 쓰는 분위기) 사용할 수 있게 되었으며, 일부 BMS 플레이어에서는 동영상 파일까지 지원한다.

  

BMS포멧에 대한 더 자세한 설명은 다음 링크에 있다.
<http://bit.sparcs.org/~tokigun/article/bmsguide.php>

  

BM98이 히트를 하게 되면서 BMS 데이터에 대한 문제 또한 생겼는데,

  

첫째는 저작권이 있는 음원의 무단 사용이다. [beatmania](beatmania.md)나 그 후신인 [beatmaniaIIDX](beatmania%20IIDX.md), [EZ2DJ](EZ2DJ.md) 등 업소용 리듬게임의 데이터를 그대로
옮긴`[3]` 이른바 벙어리 BMS라는 것도 있는가 하면`[4]` 아예 키음까지 재연한 BMS도 있다. 이 부분은
[beatmania](beatmania.md)와 [beatmania IIDX](beatmania%20IIDX.md)의 판권을
가지고 있는 [코나미](%EC%BD%94%EB%82%98%EB%AF%B8.md)에서 민감하게 반응할 법도 하지만 아직까지 공식적으로
제재를 가한건 확인되지 않았다. 그 외에도 한국가요나 J-POP 등의 저작권이 있는 곡들을 무단사용한 문제가 있었다.

  

둘째는 완성도가 조악한 BMS의 범람. 특히 1999년~2000년 쯤에 그냥 가요를 배경음악으로 흘려놓고 키음은 그냥 드럼만 쿵짝거리며
배치하거나 아니면 키음을 아예 넣지 않는 BMS가 비일비재했으며, 그래서 곡 제목만 믿고 다운로드한 플레이어들의 좌절을 불러일으켰다.

  

그리고 셋째는 국내에서 BM98 프로그램 제작자 및 BMS 제작자의 허락도 받지 않고 'DJ BEAT'라는 이름으로 불법 판매를 한 적이
있다. (게다가 스킨을 개조해서 프로그램 맨 처음에 뜨는 **NOT FOR SALE**이라는 메시지도 뜨지 않게 했다) 더 심한 것은,
[한국](%ED%95%9C%EA%B5%AD.md)에서 BMS 형태의 데이터를 무단으로 사용한 **오락실 게임**인 [비트플레이어2000](%EB%B9%84%ED%8A%B8%ED%94%8C%EB%A0%88%EC%9D%B4%EC%96%B4%202000.md)이라는
것까지 나왔다. 물론 BMS 제작자 및 플레이어들한테 제대로 까였으며, 그 게임의 제작사는 이미 사과문을 쓴 상태.

  

특히 두번째 요소 때문에 라이트 유저들이 'BM98에는 이런 곡들밖에 없나'라는 오해를 하게 해서 BM98에서 이탈하게 한 원인이
되었다(......)

  

그 이후로 club stubborn 등의 BMS 리뷰 사이트가 나와서 BMS 데이터에 대한 옥석이 많이 가려졌다.

  

[한국](%ED%95%9C%EA%B5%AD.md)의 몇몇 사람들은 BMS 제작자의 저작권을 무시하고 인터넷 상의 BMS를
[펌](%ED%8E%8C.md)질한 사이트를 만들고 그것을 그냥 받을 수 있게 함으로서, 그것에 실망한 BMS 제작자가 BMS 제작을
그만두거나 한국쪽 IP를 차단하는 불미스러운 일이 일어나기도 했다. ([MUGEN](MUGEN.md)쪽에서도 마찬가지 상황이 일어나기도
했다)

  

현재는 나오고 있는 BMS들의 대다수가 제작자가 직접 작곡한 오리지날 곡이거나, 게임음악들의 동인계 리믹스인 사례가 많아서 저작권 문제가
있는 데이터들은 많이 사라졌다. (이것은 제작자들과 플레이어의 인식 변화 뿐 아니라 [JASRAC](JASRAC.md)의 단속으로
판권곡 무단사용이 봉쇄된 것도 이유이다) 오리지날 곡들의 경우 몇몇 곡의 경우는 상용 리듬게임 수록곡 뺨치는 엄청난 퀄리티를 보여주기도
했다. 실제로 이 BMS쪽 데이터를 작성하는 사람들을 상용 리듬게임 제작사에서 채용해 간 적이 있다. (ex - EZ2DJ 7th의 메인
프로듀서인 [RYUminus](RYUminus.md)는 본래 BMS쪽의 배경 애니메이션을 만든 제작자이며, 일본쪽에도 tats라는
BMS 제작자가 beatmania IIDX의 배경 애니메이션을 맡았고, sasakure.UK, sta, sun3 등의 제작자가 한국의 상업
리듬게임인 EZ2DJ, Sabin Sound Star에 참여하기도 하였다.)

  

아무래도 아마추어 작곡이라는 측면에서는 [동인음악](%EB%8F%99%EC%9D%B8%EC%9D%8C%EC%95%85.md) 활동과 큰
차이가 없기때문에, 현재 대부분
[동방프로젝트](%EB%8F%99%EB%B0%A9%ED%94%84%EB%A1%9C%EC%A0%9D%ED%8A%B8.md)`[5]`를
비롯한 2차 동인 어레인지 앨범에서 활동하는 아티스트가 상당수 BMS제작자와 겹치기도 한다. 굳이 작곡자뿐만이 아니라 보컬, BGA를
제공하는 디자이너 및 일러스트레이터에 걸쳐서도.

  

가끔 BMS쪽에서 나온 오리지날 곡이 매드무비에 삽입되어서 히트치는 경우도 있지만 그 경우 원출처가 BMS곡이라는 것을 사람들이 모르는
경우가 많다. - [노상의기리진](%EB%85%B8%EC%83%81%EC%9D%98%20%EA%B8%B0%EB%A6%AC%EC%A7%84.md) (이 곡의 경우
원곡이 따로 있지만, 각종 매드무비에 삽입된 버전은 BMS버전)

  

BMS는 제작자가 만드는 패턴 외에도, 유저가 개조하여 더 어렵게 한 패턴이나, 파일 중 숨겨진 패턴이 존재하는데, 이를 **차분(또다른
채보)**이라고 한다. 또한 차분패턴의 등장으로 기존의 12난이도 체계를 뛰어넘은 곡들이 난립하기 시작했기 때문에 등장한 새로운 난이도개념이
바로 [발광 BMS](%EB%B0%9C%EA%B4%91%20BMS.md). 최근 BMS 영상에서도 발광BMS 플레이영상 및 오토플레이로
보면을 소개하는 영상들이 꽤 올라오는편이라 소위 '[본가](beatmania%20IIDX.md)'유저들사이에서 BMS에 대한 인식은
'상식을 뛰어넘는 아득한 병외천 채보들이 가득한 영역'으로 인식되는 경우도 잦다.보통 [본가](beatmania%20IIDX.md)에서
새로운 흉악곡이 등장하면 BMS라고 욕하는 식으로. (이것은 일본쪽 본가 뿐 아니라 한국의 건반 리듬게임 플레이어들 역시 비슷한 인식이다)

  

BMS의 또 다른 용도가 하나 있는데, 바로 [리플렉 비트](%EB%A6%AC%ED%94%8C%EB%A0%89%20%EB%B9%84%ED%8A%B8%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md) 채보 확인용(...)`[6]` 리플렉 비트는 탑오브젝트를 제외한
오브젝트가 떨어지는 속도나 위치가 완전히 랜덤이기 때문에 완벽히 대응하는 채보는 만들 수 없지만 오브젝트가 떨어지는 타이밍은 표기할 필요가
있는데, beatmania IIDX 기반의 BMS는 탑오브젝트와 파란 노트가 3개로 일치하기 때문에 어느 정도 대응이 가능하다.
[예시](http://www.youtube.com/watch?v=ag5UWdBF6YY) 흰건반은 판정선, 검은건반은 3탑`[7]`에
대응시키고 스크래치는 5점 동시치기가 아니면 일반적으로 사용하지 않는다. 체인노트의 구분은 보통 같은 레인에 연속으로 떨어지면 체인노트,
아니면 일반 폭타인 것으로 한다. 다만 이 경우에도 6점 이상 동시치기나 버티컬 오브젝트는 구현할 수 없다는 사소한 단점이 있다.`[8]`

  
  

[[edit](http://rigvedawiki.net/r1/wiki.php/Be-
Music%20Script?action=edit&section=2)]

### 2. **[BMS/목록](BMS/%EB%AA%A9%EB%A1%9D.md)(이름순)** ¶

[BMS/목록](BMS/%EB%AA%A9%EB%A1%9D.md) 참조.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Be-
Music%20Script?action=edit&section=3)]

### 3. BMS 아티스트 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/Be-
Music%20Script?action=edit&section=4)]

#### 3.1. 일본 ¶

  * -45 (= 裏吉川)
  * 8 to 7 (= Amane Kudoh)
  * An (= AcuticNotes)
  * Anubasu-anubasu (= kinohito = π/3)
  * AOiRO_Manbow (= hapi⇒)
  * aozuna (= dj sapphire)
  * [atomic sphere](atomic%20sphere.md)(= ARMYTOM = ATM = 軍人)
  * azu
  * BACO 
  * cinako
  * cittan
  * copyyyy
  * [cranky](cranky.md) (= Queen P.A.L) 
  * cromo
  * cybermiso (= SABERMISSILE)
  * daisan
  * dexhip (= w32, socer, xiang&yuan)
  * DG-P
  * DOT96
  * eicateve 
  * ELE-G
  * eoll `[9]`
  * Est (= TOMA = LuL)
  * ETIA.
  * EXAM.S
  * EXCALIpUR
  * extrose`[10]`
  * FALL (= ele-rabbit외 매우 많음`[11]`)
  * [fether](fether.md)
  * fmy.
  * ginkiha
  * glustar 
  * gmtn. (= witch's slave)
  * H.U.T GiGAR
  * HaL (= Sentire)
  * haleit
  * Hate (= IDEAL, IDEA+RHYTHM)
  * HOUJIROU
  * Ino
  * Junk (= Nostalgraph`[12]` = 定額P)
  * kanone (= NS-Factory)
  * Kaoru (= Brilliance = MONOLITH)
  * kei_iwata 
  * Kei Izumi (= MKT, イズミケイ, ismK, 夕闇P)
  * kireji
  * kju8 (= Takuya Namba = mentalhealz)
  * kotira sample (= morigasigeru)
  * Le DoS-on
  * LeaF
  * Lime
  * LU
  * maki (= guna, ridis)
  * mao sawatari (= maozon)
  * miii (= dust.c = dustcloth)
  * mommy
  * monotone
  * MORRIGAN
  * Mr.ABC
  * Nankumo (= Knot)
  * Nitrix
  * [nixx](%EB%8B%89%EC%8A%A4#s-7.md)
  * nmk
  * O-SE (= seofire = Tosatsu)
  * orangentle (= papyrus, ogrt, Yu_Asahina)
  * otokaz 
  * [P*Light](P%2ALight.md) `[13]`
  * puru
  * q/stol
  * ras
  * riutaso
  * roop
  * [Ryunosuke Kudo](96.md) (= doku, 96)
  * s-don
  * Shaman Cure-All
  * [SHIKI](SHIKI.md)
  * SINK
  * siromaru 
  * spine
  * [sta](sta.md) (= Crolul)`[14]`
  * [sun3](sun3.md)
  * sweez
  * syatten (=ツナマヨ)
  * tarolabo`[15]`
  * taqumi
  * tcheb
  * tetsuo
  * tigerlily
  * Totsumal
  * TrioStaR
  * ume `[16]`
  * [void](void.md) (= Personative, 렌쟈쿠P)
  * wa.
  * wata
  * xarva (= narve, ken)
  * [xi](xi.md)
  * Y.W
  * [Yamajet](Yamajet.md)
  * yassu
  * Ym1024
  * Yozora Mixtape
  * yujurie (= ユズ売り, itsuki shiina, ユジュリィ, sie)
  * zen (= LINDA = Fuckroach)
  * [削除](%E5%89%8A%E9%99%A4.md)(= Magic Mash Man, Is Kingdom`[17]` )
  * 痛男次郎
  * 天音
  * 愛新覚羅溥儀 (= judithz = Process 2.3.1.)
  * 牧野 (= pentate)
  * カラフル･サウンズ･ポート(= C.S.P)
  * ミッチ・ミキハラ
  * ねこみみ魔法使い
  * ねこみりん (= NECO-X)
  * ルゼ (= djHiro)   

[[edit](http://rigvedawiki.net/r1/wiki.php/Be-
Music%20Script?action=edit&section=5)]

#### 3.2. 한국 ¶

  * Applesoda 
  * AQuness
  * Aiel Eltlinde`[18]` (= jueL, Xai☆, selenite, DR.J, Soblian, back-straights, Lijexua) 
  * bbangsami (= 9903)
  * BeatniK (= Teddist, Alex G.)
  * Blue-J (= Vector27)
  * Chelp (= Semi-Digital, あるさん)
  * CORE-D (= MMMP, DJ.273K)
  * CP.ARCHE (= DeathisM)
  * CrYmson
  * dimcynical
  * Dr.ReB
  * easyamateur
  * eFeL
  * Ehne (= N)
  * [E.B (=Electronic Boutique)](Electronic%20Boutique.md)`[19]`
  * Emilio Valentine (= ST.Emilio)
  * [Envy](Envy.md) (= Transin, SpringHead)
  * exci (= MarisaB)
  * F.NET
  * Ferrum (= Fe2plus)
  * Gal
  * genesik (= The Bottom)
  * Gothpheus
  * JongCor
  * Ixia
  * IX
  * Kamisys
  * [Kari](Kari.md)
  * KHTP (= Kago Pengchi)
  * KRX
  * litmus*
  * [LhoU](LhoU.md)
  * Lunaticat
  * [Lunatic Sounds](Lunatic%20Sounds.md)
  * Marky
  * Mellover (= FateMaker, TransoL)
  * Mer
  * MoonHare
  * Mystinia (= Hypercube, Leaf, Gradian)
  * Nerd (= Sub Question)
  * NDEX
  * NEUROSE (= Quarkpop)
  * on_OTL
  * OptiU
  * P4koo (= AHA*, NONE)
  * Phenom (= Helldruggie, Irrlicht)
  * PrimeMIX
  * Rave Cyanide (= 적절, Blacksparrow)
  * Red_Eye `[20]`
  * RedFOX (= DJ.ZEST, CrazieDogg, HOUSENATION)
  * RiraN
  * [RMHN](RMHN.md)
  * [Ruby.G](Ruby.G.md) (= Speed Magician, K137, Shinabro, Sound Piercer)
  * [SANY-ON](SANY-ON.md)`[21]` (= 3034)
  * Saturn. Dreams (= Lentorek)
  * Seibin
  * sing88
  * Symphonian (= Symphoniac, Quillah)
  * TheN
  * V-Ex.Far (= Endle Fronte)
  * Warp-E (= WarpEmperor)
  * w_tre
  * [wigen](wigen.md)
  * Zekk
  * ZerA
  * 옐로고양 (= Yellowcat)
  * <del>[오픈마인드월드](%EC%98%A4%ED%94%88%EB%A7%88%EC%9D%B8%EB%93%9C%EC%9B%94%EB%93%9C.md)</del>`[22]`
  * 잔구스손 (= 7200, Zangoose`[23]`Tidal_Waver)

[[edit](http://rigvedawiki.net/r1/wiki.php/Be-
Music%20Script?action=edit&section=6)]

#### 3.3. 이외 국가의 BMS 아티스트 ¶

  * humdrumbass (대만)
  * lup (이탈리아)
  * [T2o](t2o.md) (중국)
  * [Vospi](Vospi.md) (러시아)
  * ice (대만)
  * 3R2

[[edit](http://rigvedawiki.net/r1/wiki.php/Be-
Music%20Script?action=edit&section=7)]

#### 3.4. BMS 활동을 중단한 아티스트 ¶

  * BMS 아티스트(활동중단 및 BMS 제외한 분야로 전향)  

    * AKITO
    * alex (※2004년 경 폐렴으로 작고)
    * Awryong `[24]`
    * [aym](aym.md)
    * [Beatmario](%EB%B9%84%ED%8A%B8%EB%A7%88%EB%A6%AC%EC%98%A4.md)
    * [Bphex Twin](Bphex%20Twin.md) `[25]`
    * CCNN (= r300k) 
    * <del>Cyclone Area</del> `[26]`
    * dai `[27]`
    * darkvirus (= SIGN, [masayoshi minoshima](alstroemeria%20records.md))
    * DIMU
    * [DJ TECHNORCH](DJ%20TECHNORCH.md)
    * [fen](fen.md) (= Xacla = hendrex)
    * General`[28]`  

      * Syrufit (Poplica와의 합작 명의)`[29]`
    * Glome (= maxXx65535) 
    * Grand Thaw (= careless, 井上⊿)`[30]`
    * Hiro
    * Is-m
    * parakeet 41 (SINK와 합작을 할 때 쓰는 명의)
    * [KIEN](KIEN.md)
    * Kommy `[31]`
    * LiTaNia
    * [Love™](XeoN.md) (= [XeoN](XeoN.md))`[32]`
    * [Lubinn](TAK.md) (= ice_volt, TAK`[33]`)
    * Lv.4
    * [MAX](MAX.md)(= euntaesu)
    * Nacky 
    * [naotyu-](naotyu-.md)
    * onaide
    * [onoken](onoken.md) (= [Ax](Ax.md), Ani`[34]`)
    * Paraoka
    * PASS
    * Pory
    * PUFF `[35]`
    * RANDO (= RED L:TUS, [HALF LIFE](%ED%95%98%ED%94%84%20%EB%9D%BC%EC%9D%B4%ED%94%84%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md) 등)`[36]`
    * Riss `[37]`
    * Ryo ohnuki (※2009년 작고)
    * saikoro (※2011년 3월 3일 작고)
    * [sasakure.UK](sasakure.UK.md) (= TJ.Hangnail, Chocolate Max)
    * [SHK](SHK.md)
    * TAK `[38]`
    * TAROS `[39]`
    * UROS `[40]`
    * XeON `[41]`
    * Xion (= PiZZ)
    * 忠建 `[42]`  

[[edit](http://rigvedawiki.net/r1/wiki.php/Be-
Music%20Script?action=edit&section=8)]

### 4. BGA 아티스트`[43]` ¶

  * 140
  * 1B
  * [anomie](anomie.md)
  * CAPOKI
  * cislv (= キャシー)
  * coda
  * cyclia
  * deadblue238 `[44]`
  * EMSH 
  * etch (= S.in`[45]`)
  * fity `[46]`
  * Highluin
  * Identity 7 (= brinda, pastel_eyes, kawasaki underground, KO-KO, 鑓田) `[47]`
  * jubeated
  * Kreshia
  * K_Hexa
  * [Lepusnette](Lepusnette.md) (= Toxvid, TOGANGE, Granite, 라면스프)
  * Masquerade (= SoundOnly[* BGA가 없을때 쓰는 Sound Only와는 다르다!!)
  * Mentalstock (= MiRA)
  * misokabocha
  * murasin (= むらしん)
  * mzet:-P `[48]`
  * Personality (= LimitFlow)
  * photonskyto
  * reku (= レク)
  * [RYUminus](RYUminus.md) (=RYU-)
  * sta (= Crolul)`[49]`
  * SMIN (= 재스민향기, VJ MecFlow)
  * SuperRacer `[50]`
  * Tofa Kim
  * TORHU MiTSUHASHi (= 壱air, S.P.S.B.`[51]`, Cube3, (불확실) Douglas`[52]`)
  * Yusie
  * ZBRANSTRIM (= SilverMax, Katou Huyuko)
  * [浪漫映像制作倶楽部(낭만영상제작클럽)](HDLV.md)  

[[edit](http://rigvedawiki.net/r1/wiki.php/Be-
Music%20Script?action=edit&section=9)]

### 5. BMS 제작팀 / 레이블 ¶

  * [Be-Music Phase](Be-Music%20Phase.md)
  * Creation Records
  * FakeChordUnion
  * Holic Sound
  * NEXTISION`[53]`
  * Maple brit'S
  * Purple Moon `[54]`
  * STR
  * STZ
  * Team.Labyrincle
  * Team.Livet
  * [Team Progressive](Team%20Progressive.md)
  * Team Varistyle
  * [zest:rave](zest%3Arave.md)  

[[edit](http://rigvedawiki.net/r1/wiki.php/Be-
Music%20Script?action=edit&section=10)]

### 6. BMS 이벤트 ¶

  * A-1 ClimaX
  * Be Happy!
  * BGA BATTLE
  * [BMS OF FIGHTERS](BMS%20OF%20FIGHTERS.md)  

    * <del>BMS OF FOON</del>
  * BJ CUP
  * Chaos stage
  * [GENRE-SHUFFLE](GENRE-SHUFFLE.md)
  * [KBP](KBP.md) \- Korea BMS Party
  * MAXBEAT - EXTREMEBEAT - ULTRAEXTREMEBEAT
  * Wire Puller
  * 東方音弾遊戯(동방음탄유희)
  * 自称無名BMS作家が物申す！(자칭 무명 BMS 작가가 불평한다!)  

[[edit](http://rigvedawiki.net/r1/wiki.php/Be-
Music%20Script?action=edit&section=11)]

### 7. 관련 용어 ¶

  * BMS 패키지  

    * BMS Starters pack
    * Director's cut
    * Plugout 
  * FOON
  * [발광 BMS](%EB%B0%9C%EA%B4%91%20BMS.md) / overjoy
  * 토탈치

[[edit](http://rigvedawiki.net/r1/wiki.php/Be-
Music%20Script?action=edit&section=12)]

### 8. 유통방식 ¶

BMS 초창기에는 BMS 전문 사이트가 드물고 잘 알려져 있지 않아서 개인 홈페이지에 공개하거나 아무 공개 자료실에 올리는 경우가 많았지만,
차차 BMS 전문 사이트 및 이벤트가 늘어나며 그런 쪽으로 BMS를 투고하는 경우가 많아졌다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/Be-
Music%20Script?action=edit&section=13)]

#### 8.1. BMS 이벤트 ¶

온라인에서 1년에 10번 정도의 크고 작은 이벤트를 벌인다. 이벤트가 열리면 BMS제작자들이 곡을 투고(업로드)한다. 투고기간이 끝나면 많은
BMS유저들이 곡들에 대해 평가한다. 이벤트의 형식은 각 이벤트마다 다르지만 크게 다음과 같이 분류해 볼 수 있다.  

  * 통상적인 대회 : 어떠한 BMS라도 투고가 가능한 대회이다. 단 IIDX 등으로 부터 음원을 추출해온 카피곡이나 키음이 없는 무키음 BMS, 이벤트 규정에 어긋나는 BMS는 실격 처리가 될 수 있다.
  * 리믹스 대회 : 기존 오리지날 BMS로부터 리믹스, [동프](%EB%8F%99%ED%94%84.md) 관련 리믹스 등 리믹스 BMS를 투고하는 대회.
  * BGA 대회 : BGA가 없거나 부실한 BMS의 BGA를 제작해 투고하는 대회.  
  
이벤트 투고 형식은 주로 다음과 같이 나뉜다.

  * 팀 형식 : 말 그대로 팀을 짜서 투고하는 형식이다. [BMS OF FIGHTERS](BMS%20OF%20FIGHTERS.md)가 대표적이다.
  * 개인 : 개인이 투고하는 형식이다.  
  

[[edit](http://rigvedawiki.net/r1/wiki.php/Be-
Music%20Script?action=edit&section=14)]

#### 8.2. 패키지 ¶

개인이 아니라 패키지로 한꺼번에 공개한다. 이벤트를 한 후에 이벤트에 등록된 곡을 한꺼번에 패키지로 공개하는 경우도 있다. 보통 패키지에는
곡 수십여개 + 구동기 형태로 공개되는것이 보통이다. BMS 입문자를 위한 스타터팩이 대표적인 예이다. 주로 WinRAR와 같은 압축
프로그램으로 압축해 배포하나, 최근에는 토렌트로 배포하는 경우도 있다.

  

\- BMS Starter Pack 2006 (일본)  
\- BMS Starter Pack 2007 (일본)  
\- BMS Starter Pack 2008 (일본)  
\- BMS Starter Pack 2009 (일본) <http://starterpack.bms.ms/>  
\- Korea BMS Starter Pack 2009 (한국)
<http://kimti20.aquz.biz/kbmsstp/index.php>  
\- Korea BMS Starter Pack "Polaris" (한국) <http://bmpolaris.xo.st/>  
\- Korea BMS Starter Pack "Primrose" (한국) <http://k-bms.com/primrose/>  
\- LUMINOUS PACK (한국/일본) <http://l-bms.com/ko/download.html>  

[[edit](http://rigvedawiki.net/r1/wiki.php/Be-
Music%20Script?action=edit&section=15)]

#### 8.3. 투고 사이트 ¶

투고 기간을 따로 정하지 않아 언제든지 BMS를 투고해 평가받을 수 있는 사이트도 있다. 투고 사이트에 다수의 곡을 투고해 피드백을 받으면서
실력을 올린 아티스트도 적잖게 있는 편이다.

  

\- b.i.n. <http://dot908.s17.xrea.com/bin2/>  
\- pupuly <http://pupuly.net/>  
\- old pupuly <http://nekokan.dyndns.info/~pupuly/>  
\- 微糖
<http://cerebralmuddystream.nekokan.dyndns.info/betoo/index.php?mode=index>  
  
  

[[edit](http://rigvedawiki.net/r1/wiki.php/Be-
Music%20Script?action=edit&section=16)]

### 9. BMS 관련 사이트 ¶

  * 커뮤니티 (BMS를 주로 다루는 사이트만을 기입했습니다)  

    * <del>BMS Academy <http://bmsacademy.net></del> `[55]`
    * TOE BMS포럼 <http://toez2dj.net/zeroboard/zboard.php?id=f_bms>
    * k-bms <http://k-bms.com/> (리뉴얼 종료후 커뮤니티 기능 탑재 예정)  

  * 리뷰 전문 사이트, 블로그  

    * mihoclap (일본) <http://bmsmiho.cocolog-nifty.com/blog/>
    * HaiM (한국) <http://blog.naver.com/jokm90>  
  
  

[[edit](http://rigvedawiki.net/r1/wiki.php/Be-
Music%20Script?action=edit&section=17)]

### 10. 주요 BMS/PMS 구동기 목록 ¶

[[edit](http://rigvedawiki.net/r1/wiki.php/Be-
Music%20Script?action=edit&section=18)]

#### 10.1. 구세대 구동기 ¶

  * Be-Music 98 ([BM98](BM98.md))  
BMS의 시작을 연 레전드 오브 레전드 구동기. 자세한 건 해당 항목 참고.

  * Mixwaver I, II  
최초의 한국산 BMS 구동기. [홈페이지](http://loa1.x-y.net) 리듬잇 이전에 국산 구동기의 한 시대를 풍미했었다. 개발자는
LOA`[56]`. 스캔 모드, 웨이브 모드 등 아케이드 게임에는 없는 다양한 요소를 제공한 것도 특징. 비교적 본가 beatmania에
가까운 시스템이었으며, 기본 판정이 리듬잇에 비해서 비교적 짠 편이었다.  
1의 경우 초기에 EZ2DJ처럼 스크래치-5키-페달 인터페이스를 지원했으나, 이를 이용한 EZ2DJ 불법 BMS가 판을 치는 바람에 패치를
통해 이 인터페이스를 지워버렸다.

  * Rhythm-it! (리듬잇)  
국산 BMS계의 한 획을 그은 토종 구동기. 개발자는 Nvyu.`[57]`

  * Flash Terminal  
최초로 7키BMS를 지원하기 시작한 구동기. 당시 [beatmania IIDX 1ststyle](beatmania%20IIDX%201st%20style.md)이 나올 때쯤이라 UI는 이 게임을 의식한것 같다. 그 외에,
BMS 플레이어 중에서는 최초로 코스플레이 기능을 지원했다.

  * nazoBMplayer  
통칭 나조BM. [홈페이지](http://manbow.nothing.sh/nazobmplay/) 인터넷 랭킹 지원. 루나틱레이브보다는 사양을
덜 탄다. LR 나오기전에 나왔던 7건반 구동 시뮬레이터중 하나. 구 리듬잇처럼 기본판정이 좋다.

  * Whistle (휘슬)  
[EZ2DJ](EZ2DJ.md)의 입력 체계를 본딴 구동기. 베타버전에서 개발이 중단되었다. 초창기 버전이었던 0.73의 경우 디폴트
스킨을 EZ2DJ 1st~4th 스킨을 그대로 카피해서 사용했기 때문에 불법 구동기로 낙인찍혔으나, 0.82 버전부터 독자적인 스킨을
사용하면서 이런 오명을 벗게 된다. 이후 0.9X 버전이 나왔으나 앞의 두 버전에 비해 상대적으로 덜 알려졌을 뿐더러 파일을 가진 사람도
극소수이다.  
개발자는 ShininG. 후에 펜타비전에 들어가서 [DJMAX시리즈](DJMAX%20%EC%8B%9C%EB%A6%AC%EC%A6%88.md)의 패턴 개발자로 근무했다.

  * BMDX
  * SSRMAX  
휘슬과 마찬가지로 디폴트 스킨이 [beatmania IIDX](beatmania%20IIDX.md) 9th를 그대로 배낀 것이기 때문에
불법 구동기로 낙인찍혔다.  

[[edit](http://rigvedawiki.net/r1/wiki.php/Be-
Music%20Script?action=edit&section=19)]

#### 10.2. 현세대 구동기 ¶

  * Lunatic Rave 2 (루나틱 레이브)  
일본에서 개발된 BMS/PMS 구동기. [홈페이지](http://www.lr2.sakura.ne.jp/index2.html) 인터넷 랭킹
지원. 현재 BMS계에서 [발광 BMS](%EB%B0%9C%EA%B4%91%20BMS.md) IR 집계등을 할때 가장 표준적으로 쓰이는
구동기이다. 인터페이스나 점수체계가 [본가](beatmania%20IIDX.md)와 상당히 흡사한 편.[그런데 메모리 관리가 잘
안된다고 한다.](http://gall.dcinside.com/list.php?id=rhythmgame&no=2713763) 그래서인지,
쿼드코어에 8GB의 램 등을 갖춘 고성능 컴퓨터에서조차 프랩스 등을 돌릴 경우 렉을 유발하는 등 **심각하게
[개적화](%EA%B0%9C%EC%A0%81%ED%99%94.md)다.**`[58]`  
다만, 개발자가 베타버전 개발중 소스분실로 인해 디버깅이 불가능 한 상태이기에 현재 그런 상태였다고 한다. 애초에 일반적인 프로그램 개발
과정 자체가 구현해야 할 기능과 프로그램 완성이 최우선이고, 구현이 끝나고나서 디버깅 및 최적화를 거쳐서 완성하게 된다.  
개발 도중 소스 분실로, 기능도 덜 구현해버렸고, 디버깅은 할 수도 없는 상황에서 Lnatic Rave 2의 프로그램 '자체'의 문제를
운운하기엔 너무 성급한 판단이다. 소스 분실을 한 개발자도 어느정도 문제가 있지만, 돈을 받고 일하는 것이 아닌 거의 봉사나 다름없다는 것을
고려하면(...) 오히려 이런 구동기가 있다는 것이 감사해야하지 않을까.  

    * LR2HD  
LR2의 소스가 유실된 상태에서 **실행파일을
<del>[마개조](%EB%A7%88%EA%B0%9C%EC%A1%B0.md)</del>뜯어고쳐서** HD 사이즈를 구현한 물건.
안그래도 발적화인 물건에 HD까지 얹었으니 [메모리 사용량은 안드로메다로](%EA%B0%9C%EB%85%90%EC%9D%80%20%EC%95%88%EB%93%9C%EB%A1%9C%EB%A9%94%EB%8B%A4%EB%A1%9C.md)(....)  
참고로 기본 스킨이 [트리코로](%ED%8A%B8%EB%A6%AC%EC%BD%94%EB%A1%9C.md)의 그것인데 굳이 신경쓰는
사람은 별로 없다.

  * [Ruv-it!](Ruv-it%21.md)  
리듬잇의 개발자 Nvyu가 만든 리듬잇의 후속 프로그램. 국내에서 많이 쓰인다.

  * Nanasigroove (나나시 그루브)  
일본에서 개발된 BMS/PMS 구동기. [홈페이지](http://asdf.bms.ms/) 이 프로그램에서 지원되는 새로운 BMS 확장
명령어를 많이 만들면서 BMS 제작에 큰 영향을 끼쳤다. 여타 다른 구동기와는 다른 노선을 지향하는 요소를 많이 볼 수 있어 마이너하긴 해도
인지도는 있는 구동기. 일본의 PMS 패키지 Toy Musical은 이 구동기를 기반으로 제작되며, 2012년 초에 Toy Musical 3
체험판에서 Nanasigroove 2 베타 버전이 최초로 공개되는 등, Toy Musical과 Nanasigroove의 관계가 밀접함을 알
수 있다.

  * <del>[osu!](osu%21.md) \- osu!mania 모드</del>  
osu!mania 전용 제작툴이 업데이트되면서 BMS처럼 제작할 수 있게 되었으나, 비트맵(BeatMap, *.osu) 파일을 쓰므로 BMS
구동기는 아니다. 하지만 전용 비트맵 제작시 BMS/BME파일로부터 채보를 그대로 가져오는 기능이 있다. 100만 만점제를 사용하며, 판정은
MISS, 50, 100, 200, 300(노랑), **MAX(무지개색 300)**`[59]`로 다른모드보다 더 세분화되어 있다. 4키 ~
8키 모드`[60]`가 있고 EZ2DJ와 같은 서바이벌 게이지를 쓴다. 최근, BMS계에서 이미 유명한 Imperishable Night
2006의 ★23 패턴을 그대로 컨버트 한 것에 1:03 ~ 1:13 부분의 롱노트 패턴 추가와 다소 몇가지 부분의 수정을 거쳐서 만들어져서
랭크맵으로 등록 되었다. 랭크맵 이란 것은 OSU! 운영자와 그 외 몇 관계자들이 공식적인 비트맵으로써 받아들인다는 의미를 가지고 있는데,
(스코어 랭킹 등록 가능 맵) 예컨대 Imperishable Night 2006가 beatmania IIDX에 이식된다면 어떨 것이라
생각하나? 별 차이 없는 이치라고 생각한다. 하지만 4K 차분 포함 5개 난이도를 따로 제작하는 둥 나름대로 신경은 쓴 걸로 보이고 어찌됬건
현존 랭크맵중 단연 보스곡으로 뽑히는 곡으로 입지는 상당한 편. [비트맵 정보](https://osu.ppy.sh/s/92190)

[[edit](http://rigvedawiki.net/r1/wiki.php/Be-
Music%20Script?action=edit&section=20)]

#### 10.3. 불법 구동기 ¶

일단 프로그램 자체가 상용 온라인 리듬게임의 인터페이스를 무단으로 복사한데다가, 상용 리듬게임의 데이터를 에뮬레이트 할 수 있는 기능까지
있는 구동기로, 착한 게이머들이라면 가까이 해서는 안될 불법 프로그램들이다.  

  * o2mania (오투매니아)  
중국산 [BMS](BMS.md) 구동기, 아니 BMS 구동은 덤에 가까운
[오투잼](%EC%98%A4%ED%88%AC%EC%9E%BC.md) 및 [DJMAX온라인](DJMAX%20%EC%98%A8%EB%9D%BC%EC%9D%B8.md)의 음악파일
[에뮬레이터](%EC%97%90%EB%AE%AC%EB%A0%88%EC%9D%B4%ED%84%B0.md). 최신 버전에서는 VOS 구동도
지원하는듯. 판정선이 어긋나 있어 판정이 비정상적으로 후하므로 이걸로 리듬게임을 연습하다간 다른 게임에서 판정이 망한다고 한다.

그 외 오투잼 관련 에뮬레이터로 오투에뮤, 오투솔로가 있으며 오투잼 온라인 서비스 종료 이후 오투잼을 즐기고 있다면 이 에뮬레이터들을
사용하는 것이다.  
오투매니아의 등장 이후 오투미디어 측에서 내부 파일 형식을 살짝 바꿔서 오투매니아에서 지원이 안 되도록 했었다.  

  * Synth'N  
O2Mania가 오투잼 에뮬레이터라면 이쪽은 DJMAX 온라인의 에뮬레이터. 구세대 구동기라서 확장 Bms들은 제대로 인식을 못한다.
특이사항으로 구동기를 다운받으면 생뚱맞게도 처음에 EZ2DJ의 [Lovely Days](Lovely%20Days.md)가 기본으로
딸려온다. 확장자는 Bms가 아니라 독자적인 확장자를 쓰므로 BMSE 등으로 활용해볼 생각은 하지 말자.

`\----`

  * `[1]` PMS 제외
  * `[2]` BMS의 경우 beatmania 시리즈나 EZ2DJ 시리즈의 난이도 기준을 따라가는 반면 PMS의 경우 팝픈뮤직 시리즈의 난이도 기준을 따라가기 때문
  * `[3]` 다소 유감스럽게도 이 문제는 여전하다. 하드데이터 카피로 인해 업소용 곡의 BMS가 대량으로 양산되고 있으며 과거 벙어리 BMS가 유포되던 것에 비하여 지금은 키음에 BGA까지 떡하니 갖춘 BMS가 유포되고 있다. LR2측에서는 이에 대한 제제조치로 투덱BMS의 누적플레이가 기록되면 인랭등록이 불가능하도록 조치했다는 **[카더라](%EC%B9%B4%EB%8D%94%EB%9D%BC.md)**가 있는데 정확히 아시는 분이 [수정바람](%EC%88%98%EC%A0%95%EB%B0%94%EB%9E%8C.md). 또한 LR2의 공식 입장은 'BMS는 IIDX의 에뮬레이터가 아니다'라고 못박은 상태이다.
  * `[4]` 벙어리 BMS는 배경음 하나만 있고 [키음](%ED%82%A4%EC%9D%8C.md)이 없는 BMS의 통칭 - 업소용 곡을 딴 BMS 중에서는 가정용에서 키음데이터를 뺀 버전도 있음. 이런 것은 벙어리 BMS라고 하지 않는다
  * `[5]` 동방프로젝트 이전에는 Key와 Leaf로 대표되는 에로게 및 라그나로크 온라인같이 동인계에서의 인기 소재를 어레인지. 대표적인 예로는 SLK-8888.sys(a.k.a. 스페랑카)가 오너인 Silly walker 레이블이나 이에 참여하는 아티스트들이 있다.
  * `[6]` PMS의 경우 [스쿠페스](%EC%8A%A4%EC%BF%A0%ED%8E%98%EC%8A%A4.md) 채보 확인용으로 간혹 쓰인다.(...)
  * `[7]` 2-4-6번키가 각각 좌-중-우로 대응된다.
  * `[8]` [리플렉 비트 그루빈 어퍼](%EB%A6%AC%ED%94%8C%EB%A0%89%20%EB%B9%84%ED%8A%B8%20%EA%B7%B8%EB%A3%A8%EB%B9%88%20%EC%96%B4%ED%8D%BC.md)의 추가요소들. 이것을 표현하기 위해 BMS 대신 [스텝매니아](%EC%8A%A4%ED%85%9D%EB%A7%A4%EB%8B%88%EC%95%84.md)를 수정해서 쓰는 경우가 늘고 있다.
  * `[9]` 본명은 에구치 타카히로(江口孝宏)로 BMS 활동후 후일 [호소에 신지](%ED%98%B8%EC%86%8C%EC%97%90%20%EC%8B%A0%EC%A7%80.md)가 주도하는 레이블 supersweep와 인연을 맺음. 2014년 국산 리듬게임인 [BEATCRAFT CYCLON](BEATCRAFT%20CYCLON.md)에서도 본명 명의로 [The Lemon Squash](The%20Lemon%20Squash.md)를 투고.
  * `[10]` 테크니카 채보 프로그램인 technika viur의 개발자.
  * `[11]` 심지어 어떤 분기에는 BMS마다 명의를 다르게 하기도 했다 (...)
  * `[12]` 아직까지는 음반활동용 명의인듯.
  * `[13]` [J-CORE](%ED%95%98%EB%93%9C%EC%BD%94%EC%96%B4%20%ED%85%8C%ED%81%AC%EB%85%B8.md) DJ/프로듀서로도 알려져있기도 하다. BMS 제작자로서의 주력장르도 이쪽이긴 하지만...
  * `[14]` BGA 작업도 직접 한다. 최근엔 다른 사람들에게도 BGA를 달아주는듯
  * `[15]` 2012년 여름 이후 활동 중지 상태
  * `[16]` 이 분의 BMS에 나오는 여성보컬은 자신의 목소리에 피치업을 한 것이다. <del>류수정?</del> 남성보컬의 경우는 본인이다.
  * `[17]` 음반활동용 명의. A[D](Diverse%20System.md):100에서 Now is a dull party라는 곡을 제공한 적이 있는데 개인앨범인 selentia에서 같은 곡이 실림으로써 削除 본인 인증.
  * `[18]` 이 인물에 대한 문서는 본인의 요청에 의해 [작성이 금지되어 있다](%EC%9E%91%EC%84%B1%EA%B8%88%EC%A7%80.md).
  * `[19]` 현재 [쏜애플](%EC%8F%9C%EC%95%A0%ED%94%8C.md)의 베이시스트로 활동중
  * `[20]` 주로 피아노 BMS로 유명하다. ez2dj의 Red Eye와는 **다른 인물**이다.
  * `[21]` 3034의 뒷 두자리를 일본식으로 읽으면 SAN-YON이 되는데, 하이픈 위치를 바꿔서 만든 닉네임으로 보인다.
  * `[22]` 발매하는 CD게임 안에 유난히 그 게임 OST를 Bms로 만들어 우겨넣은게 몇몇 있다. 대표적으로 [리플레이](%EB%A6%AC%ED%94%8C%EB%A0%88%EC%9D%B4.md)
  * `[23]` 곡명 등 국내 커뮤니티를 제외한 대외적으로는 이 닉네임을 쓰는듯 하다.
  * `[24]` 한국 1.5세대 제작자. [애국가](%EC%95%A0%EA%B5%AD%EA%B0%80.md)를 드럼앤 베이스 리듬(...)으로 어레인지한 BMS가 유명.
  * `[25]` 현재 보컬로이드P로 활동중.
  * `[26]` **1세대**시절 대만 출신의 제작자이긴한데... BMS 퀄리티가 너무나도 저질이라 세간의 지탄을 받고 잊혀졌다. Binary numbers는 이미 전설.(이후 일본인 제작자가 리믹스까지 했다.)5건반 beatmania 관련 리믹스 곡도 있었지만 리믹스 수준 역시 끔찍했다. 니코동에 가면 해당 제작자의 BMS를 [모아둔 영상](http://www.nicovideo.jp/watch/sm5751952)이 있다. <del>손발리 오그라든다</del>.
  * `[27]` 1998년 8월, 최초로 자신이 작곡한 곡으로 자작 BMS를 만든 인물. 이 사람으로부터 BMS의 역사가 시작됐다고 해도 과언이 아니다. 현재는 M.Graveyard 소속으로 [용기사07](%EC%9A%A9%EA%B8%B0%EC%82%AC07.md) 제작의 [울 적에](%EC%93%B0%EB%A5%B4%EB%9D%BC%EB%AF%B8%20%EC%9A%B8%20%EC%A0%81%EC%97%90.md)[시리즈](%EA%B4%AD%EC%9D%B4%EA%B0%88%EB%A7%A4%EA%B8%B0%20%EC%9A%B8%20%EC%A0%81%EC%97%90.md)의 BGM을 주로 담당하는 중.
  * `[28]` 현재 명의는 hiro.na
  * `[29]` 지금의 Syrufit는 hiro.na의 단독명의에 가깝다.
  * `[30]` 2013년 5월 해체
  * `[31]` 한국 BMS 1세대 아티스트. 현재 관련 계통에서의 활동 소식은 없지만 IT분야에서 활동하고 있다.
  * `[32]` 아래의 XeON과는 다른 인물이다.
  * `[33]` 현재 사용하는 명의의다. 아래의 TAK과는 관련없다.
  * `[34]` [Cytus](Cytus.md)에서 쓰는 명의
  * `[35]` 대충 onoken이 초창기 BMS현역시절일때쯤 활동했던, spider(이 역시 활동중단)와 더불어 **네타/개그BMS 전문**작자. 대표작은 성룡 영화를 샘플링한 [개버](%EA%B0%9C%EB%B2%84.md)곡인 RIOT IN JACKIE 등. 당시 한 익명투고BMS 이벤트의 우승곡이었던 8 o'clock trippin(**이것 역시 네타 BMS다**.)의 작곡자인 take-o가 이 사람의 부명의라는 설이 있었었지만 불명. <del>지금은 몰라도 좋은일</del>. [스타오션](%EC%8A%A4%ED%83%80%EC%98%A4%EC%85%98.md) 시리즈의 팬이라 그런지 관련 네타를 간혹 쓰기도 했다.
  * `[36]` 하프라이프 명의는 작곡자 본인이 밸브 FPS게임 팬이라서 만든 명의인듯 하다. 그리고 BMS 활동시절에는 Rask라는 명의의 아티스트와 합작한 적도 있다.
  * `[37]` KBP2010에 출전한다는 의사를 밝혔으나 소식은 없기에 여기에 분류.
  * `[38]` BMS 활동당시 명의는 TAK-sk를 줄여서 TAK으로 썼다. 위의 Lubinn과는 관련없는 사람이며, 현재는 Poplica*라는 명의를 사용한다.
  * `[39]` 1세대시절 [애니송](%EC%95%A0%EB%8B%88%EC%86%A1.md) 카피곡 위주로 제작해서 유명해졌다. 오리지널곡을 제작한 적이 없는건 아닌데, **거의 한개**(Love's Rebirth, 후에 Naotyu- 등의 작곡가들에게 리믹스된다.)밖에 없을정도로 희귀하다. 그럼에도 꽤나 호평이었다.
  * `[40]` 한국 1.5세대 제작자
  * `[41]` 역시 위의 Love™와는 관련없는 사람이다.
  * `[42]` 한국 1~1.5세대 제작자
  * `[43]` 본인 곡에만 BGA를 다는 사람들은 적지 않았다.
  * `[44]` 2013년 5월 이후 아무런 소식이 없다. 블로그도 폭파되었고, 트위터와 [니코니코동화](%EB%8B%88%EC%BD%94%EB%8B%88%EC%BD%94%EB%8F%99%ED%99%94.md) 계정의 활동도 각각 5월 10일과 3월 이후의 활동이 없는 상태다. 일본쪽에서도 아무런 소식통이 없어 당황하는중..
  * `[45]` etch는 BGA 명의, S.in은 작곡 명의. 현재는 BGA 제작이 메이저이다.
  * `[46]` 일러스트 위주로 제공하던 사람. 현재 활동을 중단했다.
  * `[47]` 작곡 활동도 제법 했지만 역시 BGA 작업이 압도적으로 많다. 휴지기를 거쳤다가 鑓田(야리타)라는 명의로 부활
  * `[48]` 최근엔 작곡 활동을 시작했다. [HYPERMESS Recordings](HYPERMESS%20Recordings.md)를 통해 릴리즈 하고 있다.
  * `[49]` BMS 작업도 한다.
  * `[50]` 플래시로 BGA와 아이캐치를 만든다고 한다. 흠좀무.
  * `[51]` 이 명의로는 주로 Hate의 곡에 BGA를 제작해 줌
  * `[52]` BOF2009를 끝으로 은퇴선언을 했지만 이후 이 명의로 몇몇 BMS에 BGA를 제작해 주었다. 공식 언급이 없었기에 확신할 순 없지만 시기 상으로나 스타일 면에서나 상당히 비슷함.
  * `[53]` 현재는 BMS 제작을 중단한 상태. 게임 리뷰팀으로 활동 중이다.
  * `[54]` 현재는 동명의 [트랜스](%ED%8A%B8%EB%9E%9C%EC%8A%A4.md) 레이블로 활약 중 <http://purplemoon-records.com>
  * `[55]` 폐쇄됐는데 다른 사이트를 만들어서 옮겼는지 아니면 그냥 없어졌는지 알 수 없다.
  * `[56]` BEMANI 올드팬으로, 과거 자신의 홈페이지에 아케이드용 beatmania 시리즈에 대한 정보와 수록곡을 소개하는 페이지를 운영한 적도 있다.
  * `[57]` [마비노기](%EB%A7%88%EB%B9%84%EB%85%B8%EA%B8%B0.md)용 트윅 유틸리티도 몇몇 개발한바가 있다. [I've](I%27ve.md)의 오래된 팬이기도 하다. 그것도 **국내 인지도가 전무하던 시절**부터 밀어줬다.
  * `[58]` 그래도 프랩스같은거 안돌리고 옵션을 조금 건들면 펜티엄 3 컴퓨터에서도 무리없이 돌아갈 수 있다. 심지어 싱글플레이 한정으로 동영상BGA도 어느정도 가능. 단 역시 메모리 관리가 잘 안되기 때문에 로딩이 끔직하다.
  * `[59]` 이 판정의 존재 때문에 정확도 100%는 찍을 수 있어도, **분명 확실한 만점이 존재함에도 불구하고 [만점 내기는 매우 힘들며](%EC%97%91%EC%84%A4%EB%9F%B0%ED%8A%B8.md)**, 판정 하나로 랭크가 오르락내리락 한다. <del>무엇보다 **오토플레이를 이길 수가 없다.**</del>
  * `[60]` O2JAM처럼 4 ~ 8K로 지정할 수 있고 IIDX처럼 S + 3 ~ 7K로 설정 할 수 있다.

