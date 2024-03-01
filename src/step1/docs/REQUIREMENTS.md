#### LottoGenerator

- 발행 번호 6개를 랜덤으로 생성한다.

- 발행 번호는 오름차순으로 정렬한다.

#### LottoCalculator

- 당첨 번호(로또 번호 + 보너스 번호)와 발행 번호 비교

- 5개가 일치하면 보너스 번호가 로또 번호에 있는지 비교

- 당첨 통계 객체 반환

- 수익률 계산

* 당첨 금액

1등: 6개 번호 일치 / 2,000,000,000원

2등: 5개 번호 + 보너스 번호 일치 / 30,000,000원

3등: 5개 번호 일치 / 1,500,000원

4등: 4개 번호 일치 / 50,000원

5등: 3개 번호 일치 / 5,000원

#### 기타

- 로또는 구입 금액에 해당하는 만큼 로또를 발행해야 한다.

- 로또 1장의 가격은 1,000원이다. -> 로또 몇개를 샀는지 저장?

- 당첨 통계 출력 후 재시작/종료 여부 입력받기

- 잘못 입력받을 시 예외 발생, 그 부분부터 다시 입력받기

- 구입 금액

  - 자연수를 입력하지 않은 경우 에러 발생

- 발행 번호

  - 전체 발행 번호 리스트
    - 6개의 숫자를 콤마(,) 로 구분하여 입력
    - 각 숫자의 공백 제거 후 리스트 반환

- 발행 번호 하나

  - 1~45 사이의 숫자가 아닌 경우 에러 발생

- 보너스 번호
  - 1~45 사이의 숫자가 아닌 경우 에러 발생

---

### 요구사항 명세서

로또 구입 금액을 입력하면 구입 금액에 해당하는 만큼 로또를 발행해야 한다.

로또 번호는 오름차순으로 정렬하여 보여준다.

로또 1장의 가격은 1,000원이다.

당첨 번호와 보너스 번호를 입력받는다.

사용자가 구매한 로또 번호와 당첨 번호를 비교하여 당첨 내역 및 수익률을 출력한다.

당첨은 1등부터 5등까지 있다. 당첨 기준과 금액은 아래와 같다.

1등: 6개 번호 일치 / 2,000,000,000원

2등: 5개 번호 + 보너스 번호 일치 / 30,000,000원

3등: 5개 번호 일치 / 1,500,000원

4등: 4개 번호 일치 / 50,000원

5등: 3개 번호 일치 / 5,000원

당첨 통계를 출력한 뒤에는 재시작/종료 여부를 입력받는다.

재시작할 경우 구입 금액 입력부터 게임을 다시 시작하고, 종료하는 경우 그대로 프로그램을 종료시킨다.

사용자가 잘못된 값을 입력한 경우 throw문을 사용해 예외를 발생시키고, 에러 메시지를 출력 후 그 부분부터 입력을 다시 받는다.