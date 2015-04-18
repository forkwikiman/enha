* 상위 항목 : [마인크래프트/명령어](%EB%A7%88%EC%9D%B8%ED%81%AC%EB%9E%98%ED%94%84%ED%8A%B8/%EB%AA%85%EB%A0%B9%EC%96%B4.md)  

## Contents

    

1. 개요 
2. 목표 
3. 화면 슬롯 
4. 팀 
5. 명령어 문법 
    

5.1. 목표 관련

5.2. 플레이어 관련

5.3. 팀 관련

[[edit](http://rigvedawiki.net/r1/wiki.php/scoreboard?action=edit&section=1)]

# 1. 개요 ¶

  

scoreboard, 즉 점수판 명령어는 맵 제작자들을 위한 복잡한 시스템이다. 커맨드나 커맨드 블럭을 이용하여 사용할 수 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/scoreboard?action=edit&section=2)]

# 2. 목표 ¶

  

목표는 이름, 보이는 이름, 기준으로 되어 있다. 점수는 32비트 `[1]`값이며, 10진수를 지원하지 않는다.

  

  * 목표의 **이름(name)**은 여러 커맨드나, 타겟 지정, 또는 파일 포맷에 사용되는 이름이다. 한 어절이어야 한다.
  * 목표의 **보이는 이름(display name)**은 실제 화면상에 보이는 이름으로, 여러 어절이어도 상관 없다.
  * 목표의 **기준(criteria)**은 점수의 기준.  

기준

내용

임의설정

dummy

명령어에 의해서만 변할 수 있고, 게임 내 상황에 따라서 변하지 않는다. 사용자가 임의로 만드는 기준이므로, 게임 자체와 전혀 상관 없는
점수에 편리하다. 예를 들어 마인크래프트에 없는 금전 개념`[2]` 등에 사용하거나,

가능

trigger

명령어에 의해서만 변할 수 있고, 게임 내 상황에 따라서 변하지 않는다. trigger 명령어에 의해서 조절될 수 있는데`[3]`,
trigger 명령어는 op가 아니어도 사용할 수 있기에 tellraw 명령어를 사용할 때 편리하다.

가능

deathCount

플레이어가 죽을 때마다 자동으로 증가한다.

가능

playerKillCount

플레이어가 다른 플레이어를 죽일 때마다 자동으로 증가한다.

가능

totalKillCount

플레이어가 다른 플레이어나 몹을 죽일 때마다 자동으로 증가한다.

가능

health

일반적인 플레이어의 하트는 10개 `[4]` 체력 부스터나 흡수 효과로 체력이 증가하면 그것도 반영된다.

불가능

  
위에 있는 간단한 기준과 달리, 복합적인 기준들도 있다.

  

기준

내용

임의설정

achivement

하위 기준은 "acquireIron", "bakeCake", "blazeRod", "bookcase", "breedCow",
"buildBetterPickaxe", "buildFurnace", "buildHoe", "buildPickaxe",
"buildSword", "buildWorkBench", "cookFish", "diamonds", "diamondsToYou",
"enchantments", "exploreAllBiomes", "flyPig", "fullBeacon", "ghast",
"killCow", "killEnemy", "killWither", "makeBread", "mineWood", "onARail",
"openInventory", "overkill", "overpowered", "portal", "potion",
"snipeSkeleton", "spawnWither", "theEnd", "theEnd2"의 34 가지가 있다. `[5]` 값들은 이
업적을 몇 번 달성했는가에 따라 달라진다. 예를 들어 플레이어가 소를 5마리 죽였다면, achivement.killCow 기준의 값은 5가
된다.

가능

stat

하위 기준은 "animalsBred", "boatOneCm", "climbOneCm", "crouchOneCm", "damageDealt",
"damageTaken", "deaths", "diveOneCm", "drop", "fallOneCm", "fishCaught",
"flyOneCm", "horseOneCm", "jump", "junkFished", "leaveGame", "minecartOneCm",
"mobKills", "pigOneCm", "playerKills", "playOneMinute", "sprintOneCm",
"swimOneCm", "talkedToVillager", "timeSinceDeath", "tradedWithVillager",
"treasureFished", "walkOneCm"의 28가지이다. stat은 statistics의 약자로, 플레이어의 통계값들이다. 이
값들은 플레이어의 행동에 따라 자동으로 증가한다.

가능

stat.craftItem

하위 기준은 조합 가능한 아이템, 제련 가능 아이템들이다. 조합한 횟수에 따라 자동으로 증가한다. `[6]` 총 199 가지가 있다.
`[7]`

가능

stat.useItem

하위 기준은 아이템의 사용 횟수. 사용한 횟수에 따라 자동으로 증가한다. `[8]` 총 318 종류가 있다.

가능

stat.breakItem

하위 기준은 내구도가 있는, 부술 수 있는 아이템들이다. `[9]` 총 50 종류가 있다.

가능

stat.mineBlock

하위 기준은 부술 수 있는 블럭들로, 총 135가지가 있다. 크리에이티브에서는 값이 증가하지 않는다.

가능

stat.killEntity

하위 기준은 "Bat", "Blaze", "CaveSpider", "Chicken", "Cow", "Creeper", "Enderman",
"Endermite", "EntityHorse", "Ghast", "Guardian", "LavaSlime", "MushroomCow",
"Ozelot", "Pig", "PigZombie", "Rabbit", "Sheep", "Silverfish", "Skeleton",
"Slime", "Spider", "Squid", "Villager", "Witch", "Wolf", and "Zombie"의 24
가지이며, 이 엔티티들을 죽일 때마다 값이 증가한다.

가능

stat.entityKilledby

하위 기준은 "Bat", "Blaze", "CaveSpider", "Chicken", "Cow", "Creeper", "Enderman",
"Endermite", "EntityHorse", "Ghast", "Guardian", "LavaSlime", "MushroomCow",
"Ozelot", "Pig", "PigZombie", "Rabbit", "Sheep", "Silverfish", "Skeleton",
"Slime", "Spider", "Squid", "Villager", "Witch", "Wolf", and "Zombie"의 24가지로,
이 몹에 의해서 사망하면 값이 증가한다.

가능

teamkill

하위 기준은 팀의 색깔이다. 가능한 색은 "black", "dark_blue", "dark_green", "dark_aqua",
"dark_red", "dark_purple", "gold", "gray", "dark_gray", "blue", "green",
"aqua", "red", "light_purple", "yellow", and "white"의 16 가지로, 각각의 색을 가진 팀원이 다른
팀원을 죽이면 값이 증가한다.

가능

killedByTeam

하위 기준은 팀의 색깔이다. 가능한 색은 "black", "dark_blue", "dark_green", "dark_aqua",
"dark_red", "dark_purple", "gold", "gray", "dark_gray", "blue", "green",
"aqua", "red", "light_purple", "yellow", and "white"의 16 가지로, 각각의 색을 가진 팀원이 다른
팀원에게 사망하면 값이 증가한다.

가능

  
health를 제외한 기준은 모두 명령어로 수정할 수 있다. `[10]` 또한 명령어를 이용해서 다른 플레이어의 점수를 확인할 수 있다.
score_name 또는 score_name_min 등의 명령어를 사용하여 확인 가능하다. 예를 들어  
deaths의 기준이 deathCount라면, testfor`[11]`
@p`[score_deaths=5,score_deaths_min=1]`을 통해 죽은 횟수가 1~5인 플레이어의 수를 셀 수 있다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/scoreboard?action=edit&section=3)]

# 3. 화면 슬롯 ¶

  

마인크래프트 화면상에 점수판을 표시할만한 곳은 3곳이 있다.

  

슬롯

설명

list

Tab을 누르면 나오는 리스트, 플레이어 이름 오른쪽에 노란 글씨로 숫자가 표시 된다.

sidebar

화면 오른쪽에 표시된다. 플레이어가 오프라인이라도 표시된다.

sidebar.team <color>

위 sidebar에 색깔 별로 정해진 팀을 표시한다. 예를 들어 sidebar.team.red 라 쓰면 red 팀에 소속된 플레이어들의
점수가 표시된다.

belowName

플레이어 위에 있는 이름 밑에 점수가 표시된다. 플레이어가 10칸 너머에 있거나, 은신 `[12]` 시 보이지 않는다.

[[edit](http://rigvedawiki.net/r1/wiki.php/scoreboard?action=edit&section=4)]

# 4. 팀 ¶

  

팀을 정의할 때는 이름, 보이는 이름, 접두사, 접미사`[13]`, 아군 공격 설정을 정해주어야한다. 목표 때와 마찬가지로 이름은 한 어절,
보이는 이름은 여러 어절이어도 상관 없다. 접두사는 포맷팅 코드`[14]`를 이용하여 여러 색을 지정해 줄 수 있고, 접미사는 리셋 코드만
가능하다.

  

아군 공격 설정을 거짓(false)으로 할 경우, 팀끼리는 근접 공격, 활, 피해 포션 등의 무기로 데미지를 입힐 수 없다. `[15]`
참고로 이 설정을 참으로 했을 경우, 자신에게도 데미지를 입힐 수 수 없다. `[16]`자신도 팀의 일원이므로. 설정을 참(true)로 할
경우에는 일반 PvP 처럼 적용된다.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/scoreboard?action=edit&section=5)]

# 5. 명령어 문법 ¶

<> 안의 문법은 필수 입력 사항, `[]` 안의 문법은 선택 입력 사항이다. 또한 명령어는 대소문자를 구분하니 주의.

  

[[edit](http://rigvedawiki.net/r1/wiki.php/scoreboard?action=edit&section=6)]

## 5.1. 목표 관련 ¶

명령어 문법

설명

작동 조건

scoreboard objective list

: 모든 목표의 이름과 보이는 이름, 기준을 화면에 표시한다.

하나 이상의 목표가 있어야 작동한다.

scoreboard objective add <이름> <기준> `[보이는 이름]`

새 목표를 만든다. 보이는 이름은 생략 시 이름과 같게 된다.

이름은 이미 있는 것과 달라야 하며, 16자 이하이어야 한다. 기준은 가능한 종류이어야하며, 보이는 이름은 32자 이하이어야 한다.

scoreboard objective remove <이름>

특정 목표를 삭제한다.

삭제하려는 목표가 존재해야한다.

scoreboard objective setdisplay <슬롯> `[목표]``[17]`

목표를 특정 슬롯에 보이게 한다. 화면 슬롯 문단 참고. 목표 칸을 생략할 경우 그 슬롯을 비운다. `[18]`

목표가 존재해야하며, 슬롯도 3가지 중 하나로 존재해야한다.

[[edit](http://rigvedawiki.net/r1/wiki.php/scoreboard?action=edit&section=7)]

## 5.2. 플레이어 관련 ¶

명령어 문법

설명

작동 조건

scoreboard player list `[플레이어]`

점수판 시스템에 의해 영향을 받는 플레이어를 모두 표시한다. 뒤에 플레이어 이름을 쓰면 특정 플레이어의 점수를 확인할 수 있다.

플레이어는 적어도 하나 이상의 저장된 점수가 있어야 한다.

scoreboard player set <플레이어> <목표> <점수> `[데이터 태그]`

플레이어의 점수를 임의로 설정한다.

-2147483648~2147483647까지의 수만 가능하고, 기준이 health인 목표는 변경할 수 없다. 데이터 태그는 플레이어의 특성을 NBT 태그 형식으로 표현한 것이다. 

scorebaord player add <플레이어> <목표> <수> `[데이터 태그]`

'수'만큼 그 목표의 점수를 증가시킨다.

1~2147483647 까지의 수만 가능하고, 기준이 health인 목표는 변경할 수 없다. 데이터 태그는 플레이어의 특성을 NBT 태그
형식으로 표현한 것이다.

scorebaord player remove <플레이어> <목표> <수> `[데이터 태그]`

'수'만큼 그 목표의 점수를 감소시킨다.

1~2147483647 까지의 수만 가능하고, 기준이 health인 목표는 변경할 수 없다. 데이터 태그는 플레이어의 특성을 NBT 태그
형식으로 표현한 것이다.

scoreboard players reset <플레이어> `[목표]`

플레이어의 모든 점수를 초기화한다. `[목표]`를 쓰면 그 목표의 점수만 초기화한다. `[19]`

언제나 작동.

scoreboard player enable <플레이어> <트리거>

플레이어가 trigger 명령어를 통해 점수를 수정할 수 있도록 허락한다.`[20]`

목표의 기준이 trigger 이어야한다.

scoreboard player test <플레이어> <기준> <최솟값> <최댓값>

플레이어의 점수가 최솟값~최대값 사이에 있는지 판별한다. `[21]`

플레이어의 점수가 범위 내에 있어야한다.

scoreboard player operation <대상이름> <대상목표> <연산> <선택자> <목표>

선택자의 특정 목표의 점수를 이용해서 대상의 특정 목표의 점수에 대해 연산을 실행시킨다.

기준이 health인 목표는 변경할 수 없다. 두 목표의 점수가 있어야한다.

  
마지막 scoreboard players opertion 에서 가능한 연산은 아래와 같다.

  

  * "+=" : 선택자의 점수를 대상에게 더한다.
  * "-=" : 뺀다.
  * "*=" : 곱한다.
  * "/=" : 나눈다.
  * "%=" : 대상과 선택자 사이의 나눗셈 결과의 나머지를 대상의 점수로 한다.
  * "=" : 같게한다.
  * "<" : 만약 선택자의 점수가 대상보다 작으면, 대상의 점수를 선택자 점수로 만든다.
  * ">" : 만약 선택자의 점수가 대상보다 크면, 대상의 점수를 선택자 점수로 만든다.
  * "><" : 대상과 선택자의 점수를 바꾼다.  

[[edit](http://rigvedawiki.net/r1/wiki.php/scoreboard?action=edit&section=8)]

## 5.3. 팀 관련 ¶

명령어 문법

설명

작동 조건

scoreboard teams list {`팀이름]`

팀의 목록을 표시하거나, 팀이름을 추가 할 시 그 팀의 소속 플레이어를 표시한다.

적어도 1개 이상의 팀이 있어야한다.

scoreboard teams add <이름> `[보이는 이름]`

팀을 만든다. 보이는 이름은 생략시 이름과 같다.

이름은 16자, 보이는 이름은 32자 이하이어야한다.

scoreboard teams remove <이름>

팀을 없앤다.

팀이 있어야한다.

scoreboard teams empty <이름>

팀의 플레이어를 모두 없앤다.

팀이 있어야하고, 그 팀에 한 명 이상의 플레이어가 있어야한다.

scorebaord temas join <팀이름> `[플레이어]`

팀에 가입한다. 플레이를 생략 시 명령어를 입력하는 플레이어가 가입된다.

팀이 존재해야한다.

scoreboard teams leave `[팀이름]` `[플레이어]`

팀에서 나간다.

팀이 있어야한다.

scoreboard teams option <팀이름> color <값>

팀의 색을 정한다. 색은 채팅, Tab메뉴, 사이드바 메뉴에 모두 적용된다. 가능한 색은 "black", "dark_blue",
"dark_green", "dark_aqua", "dark_red", "dark_purple", "gold", "gray",
"dark_gray", "blue", "green", "aqua", "red", "light_purple", "yellow", and
"white"의 16가지이며, "reset"을 할 경우 기본 색으로초기화된다.

두 값이 모두 유효한 것이어야한다.

scoreboard teams option <팀이름> friendlyfire <true / false >

아군 공격 설정을 켜거나 끈다.`[22]`

true 또는 false이어야한다.

scoreboard teams option <팀이름> seeFriendlyInvisible <true / false >

자신을 포함한 팀원이 반투명하게 보인다.

true 또는 false이어야한다.

scoreboard teams option <팀이름> nametagVisibillity <설정>

플레이어 캐릭터 위의 이름표가 어떻게 나올지 설정한다. always`[23]`, never, hideForOtherTeams`[24]`,
hideForOwnTeam`[25]` 중 하나로 택해야한다.

넷중 택일.

scoreboard teams option <팀이름> deathMessageVisibillity <설정>

위 이름표 설정과 동일한다.

넷중 택일

`\----`

  * `[1]` -2147483648 ~ 2147483647
  * `[2]` 물론 에메랄드가 있긴 하지만 플레이어간 사용이 불편하므로
  * `[3]` 단, 그 목표가 활성화되어 있어야 사용가능하다.
  * `[4]` 하트 하나가 체력 2이므로, 보통 플레이어는 체력이 20이다.
  * `[5]` 모두 업적들이다.
  * `[6]` 통계 - 블록에서 확인 가능.
  * `[7]` minecraft:sotne, 1 같이 이름과 ID 모두 가능하므로 398가지라고 할 수도 있다.
  * `[8]` 통계 - 아이템 에서 확인 가능.
  * `[9]` 곡괭이, 도끼, 칼, 낚시대, 갑옷류
  * `[10]` 즉, 플레이어의 체력을 명령어로 변경할 수는 없다.
  * `[11]` [마인크래프트/명령어](%EB%A7%88%EC%9D%B8%ED%81%AC%EB%9E%98%ED%94%84%ED%8A%B8/%EB%AA%85%EB%A0%B9%EC%96%B4.md) 참조
  * `[12]` shift 키를 누르면 된다.
  * `[13]` 접두사와 접미사는 생략해도 된다. 색을 넣는 등의 효과이기 때문.
  * `[14]` <http://minecraft.gamepedia.com/Formatting_codes> 참조.
  * `[15]` 포션에 의한 나쁜 효과는 여전히 받는다.
  * `[16]` 활을 하늘을 향해 쏴서 자신이 맞게 하거나, 피해 포션을 자신에게 던진다던가. 물론 낙하 데미지는 받는다.
  * `[17]` 위에서 추가한 목표의 이름이다.
  * `[18]` 원래 상태로 되돌린다.
  * `[19]` 초기화 한다는 것은 0을 만드는 게 아니라 플레이어를 그 점수 시스템으로부터 삭제한다는 것이다.
  * `[20]` 이 명령어는 op 이하의 일반 유저도 사용 가능한 명령어이다. 즉, 기준이 trigger인 목표는 사용자들이 임의로 모두 수정할 수 있다. 이 명령어로 허락한 이후부터.
  * `[21]` -2147483648~2147483647 범위. 만약 <기준> * * 이라 쓰면 모든 값이 포함된다. 
  * `[22]` 기본은 참.
  * `[23]` 기본설정
  * `[24]` 팀끼리는 보이나 다른 팀은 않보임.
  * `[25]` 자신이 팀끼리만 안 보임

