# 미션 - 로또

---

## 프로젝트 소개

해당 프로젝트는 사용자가 구입 금액과 당첨 로또 번호를 입력하면  
로또 번호를 금액만큼 컴퓨터가 자동으로 생성하고  
로또 당첨 여부와 수익률을 확인할 수 있도록 개발된 로또 시뮬레이션 게임입니다.  
  
게임 진행 흐름은 다음과 같습니다.  

```
사용자는 구입 금액을 입력합니다  
3000

자신이 구입한 로또의 번호 확인합니다  
[2, 15, 16, 26, 27, 39]
[3, 11, 31, 33, 38, 45]
[1, 5, 7, 11, 12, 28]

이어서 당첨 번호와 보너스 번호를 입력합니다  
2,15,16,3,11,5
7

당첨 결과 및 구입 금액 대비 당첨금이 얼마나 되는지 수익률로 확인합니다  
3개 일치 (5,000원) - 1개
4개 일치 (50,000원) - 0개
5개 일치 (1,500,000원) - 0개
5개 일치, 보너스 볼 일치 (30,000,000원) - 0개
6개 일치 (2,000,000,000원) - 0개
총 수익률은 166.7%입니다.
```

---

## 구현할 기능 목록

### 입력

- [X] 로또 구입 금액을 입력 받는다.
- [X] 당첨 번호를 입력 받는다.
- [X] 보너스 번호를 입력 받는다.

---

### 입력 후 처리

- [X] 당첨 번호를 ',' 단위로 파싱한다.

---

### 입력 검증 (구입 금액)

- [X] 숫자인지 검증한다
- [X] 값이 1000원 이상인지 검증한다.
- [X] 값이 int 자료형의 최대 값을 벗어나지 않는지 검증한다.
- [X] 값이 1000원 단위인지 검증한다.

---

### 입력 검증 (당첨 번호)

- [X] 숫자인지 검증한다.
- [X] 1~45 사이의 숫자인지 검증한다.
- [X] 6개인지 검증한다.
- [X] 중복된 당첨 번호가 있는지 검증한다.

---

### 입력 검증 (보너스 번호)

- [X] 숫자인지 검증한다.
- [X] 1~45 사이의 숫자인지 검증한다.
- [X] 보너스 번호가 당첨 번호와 중복인지 검증한다.

---

### 로또 추첨

- [X] 로또 구입 금액을 1000으로 나누어 구입한 로또의 개수를 계산한다.
- [X] 구입한 로또의 개수만큼 1~45 사이 6개의 난수를 생성한다.
- [X] 생성한 난수와 당첨 번호, 보너스 번호를 비교한다.
- [X] 비교 후 일치하는 번호 개수를 통해 당첨 순위를 계산한다.

---

### 당첨 통계 계산

- [X] 당첨 순위의 횟수를 계산한다.
- [X] 총 당첨금을 계산한다.
- [X] 구입 금액과 총 당첨금을 비교하여 수익률을 계산한다.

--- 

### 출력

- [X] 로또 구입 금액을 입력 받는 메시지를 출력한다.
- [X] 발행한 로또 수량을 출력한다.
- [X] 수량만큼 로또 번호를 출력한다.
- [X] 당첨 번호를 입력 받는 메시지를 출력한다.
- [X] 보너스 번호를 입력받는 메시지를 출력한다.
- [X] 당첨 내역을 출력한다.
- [X] 수익률을 출력한다.