# 타워 디펜스 게임

협업하는 것을 목표로 간단한 디펜스 게임을 제작했습니다.  
아직 미구현입니다.

## 툴

- Unity

## 언어

- C#

## 배운 것

- Git, Github을 이용한 협업(Commit, Pull Request)
- Unity Collaboration을 이용한 협업
- 유니티에 코드가 많아질 때 정리하는 센스

## 게임 규칙 및 플레이 방법

- 한 라운드당 몬스터는 20마리이다.
	- 라이프는 40으로 설정한다. 
	- 필드의 몬스터의 개수만큼 라이프는 감소해서 보여진다.
	- 열 라운드마다 몬스터와 함께 필드보스가 등장한다. (몬스터 20마리 + 필드보스 1마리)
- 한 라운드당 시간제한은 30초이다. 단, 필드의 몬스터가 없으면 바로 다음 라운드로 진행된다.
	- 라운드가 끝나기 전까지 필드보스를 잡지 않아도 패배하지 않는다.
	- 일반 몬스터는 한 바퀴를 돌 때마다 방어력이 1씩 오른다.
	- 초기 골드는 0골드이고 스킬을 구매하는 비용은 1500골드이다.
	- 스킬을 판매시, 1000골드를 획득할 수 있다.
- 라운드 시작전, 스킬의 구매와 환불은 골드가 소모되지 않는다. 단, 최대 2번까지 가능하다.
- 일반 몬스터를 잡으면 1골드를, 필드 보스를 잡으면 1000골드를 획득할 수 있다.
- 스킬의 최대 개수는 4개이다.
- 스킬의 등급은 F~S등급까지 존재한다.
- 스킬을 구매할 때 등급은 랜덤으로 정해진다.

[회의록 살펴보기](https://docs.google.com/document/d/1ZOHq64Pf8SKA58J8JNbPd9CHj39g2_qNgI-CO800ncE/edit?usp=sharing)


## 스크린샷

![](https://eliotjang.github.io/assets/images/defense-game/TD-demo.png) 

## 현재 구현한 기능

- 제한시간 이내에 해당 스테이지를 모두 클리어하면 다음 스테이지로 넘어가는 기능
- 해당 스테이지가 끝나면 돈을 얻는 기능
- 일정 스테이지마다 보스 몹이 나오는 기능
- 스테이지마다 몬스터가 일정한 간격마다 나오고, 정해진 길을 따라 타워를 도는 기능
- 몬스터가 사정거리에 들어오면 타워가 포탄을 발사하는 기능
- 몬스터마다 체력이 표시되는데, 포탄이 몬스터에 닿으면 체력이 낮아지고 다 닳으면 사라지는 기능
- 스킬을 구매하게되면, 포탄이 몬스터에 닿을 때, 확률적으로 스킬 이펙트가 나오고 스킬 데미지가 들어가는 기능
- 시각적으로 간단한 UI/UX
  - 좌측 하단 물음표 버튼을 누르면 랜덤으로 스킬 생성
  - 좌측 상단 일시정지 버튼을 누르면 게임이 일시정지됨

## 참고한 게임

- 랜덤능력타워디펜스
