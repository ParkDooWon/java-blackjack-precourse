# 3. 블랙잭 게임
## 게임 규칙
- 21을 넘지 않으면서 21에 가장 가까운 수를 합계로 가진 사람이 승리한다.
	- 게임에서 승리하면 베팅한 금액을 받는다.
	- 처음 받은 카드 2장의 합계가 21인 경우, 베팅 금액의 1.5배를 딜러에게 받는다.
- 가지고 있는 카드의 합계가 21을 넘으면, 그 즉시 패배한다.
  
## 프로그래밍 요구사항
- Card, Player, Dealer 객체를 활용하여 구현하는데, 주어진 필드의 접근 제어자를 변경하지 않는다.
- Class에 필드(인스턴스 변수)를 추가할 수 없다.
- 3항 연산자를 사용하지 않는다.
- else 예약어를 사용하지 않는다.
- 함수(메소드)의 길이가 10라인을 넘어가지 않도록 한다.
- indent depth를 2가 넘지 않도록 구현한다. (1까지만 허용한다.)
- 함수(메소드)의 인자 수를 3개까지만 허용한다.
  
## 기능 요구사항
1. 플레이어들의 이름을 쉼표로 분리하여 입력받는다.
	- 플레이어의 이름에 중복이 없도록 한다.
	- 플레이어가 1명 이상이 되도록 한다.
	- 게임의 원활한 진행을 위해 플레이어 수는 8명으로 제한한다.  
2. 각 플레이어의 베팅 금액을 입력받는다.
	- 베팅 금액이 양의 정수가 되도록 한다.
	- 베팅 금액은 10의 배수가 되도록 한다.  
3. 딜러와 플레이어들에게 2장의 카드를 나누어준다.
	- 나눠주는 카드에는 중복이 없도록 한다.  
4. 딜러와 플레이어에게 나눠준 카드를 출력한다.
	- 딜러의 경우 두 장의 카드 중 첫 번째 한장의 카드만 공개한다.  
5. 딜러와 플레이어 모두 처음 두 장의 카드 합이 21인 경우(블랙잭)를 확인한다.
	4-1) 플레이어만 블랙잭인 경우 딜러에게 베팅 금액의 1.5배를 받는다. 
	4-2) 플레이어와 딜러 모두 블랙잭인 경우 플레이어는 베팅한 금액을 돌려받는다.  
6. 블랙잭이 없으면 각 플레이어에게 추가로 카드를 드로우할지 질문한다.  
7. 모든 추가 드로우가 끝나면 딜러는 처음에 받은 2장의 합계를 확인하고,  
16이하이면 반드시 1장의 카드를 추가하고 17이상이면 추가로 받지않는다.  
8. 딜러와 모든 플레이어의 결과를 구하여 출력한다.  
9. 최종 수익을 계산하여 출력한다.  
  
## 예외사항
- 플레이어
	- 참여할 플레이어 수가 1명 이상이 되도록 한다.
	- 참여할 플레이어 수가 8명 이하가 되도록 한다.
	- 참여할 플레이어의 이름에 중복이 없도록 한다.  
- 베팅 금액
	- 베팅 금액이 양의 정수가 되도록 한다.
	- 베팅 금액이 10의 배수가 되도록 한다.  
- 카드 분배
	- 분배한 카드에 중복이 없도록 한다. 
