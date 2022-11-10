# 과제 설명

## 로또 게임의 규칙

- 로또 번호 숫자 범위 : 1 ~ 45
- 한 개의 로또는 6개의 숫자로 구성
- 당첨 번호 뽑기 : 중복되지 않는 숫자 6개 + 보너스 숫자 1개
- 당첨 기준과 금액
    - 1등: 6개 번호 일치 / 2,000,000,000원
    - 2등: 5개 번호 + 보너스 번호 일치 / 30,000,000원
    - 3등: 5개 번호 일치 / 1,500,000원
    - 4등: 4개 번호 일치 / 50,000원
    - 5등: 3개 번호 일치 / 5,000원

## 로또 게임 진행 순서

1. 구매 금액을 입력한다.
2. 구매 급액에 맞게 알맞은 횟수의 로또 번호 6자리를 난수로 생성한다.
3. 당첨 번호 6자리를 입력한다.
4. 보너스 번호를 입력한다.
5. 당첨 통계를 나타내면서 사용자의 수익률을 계산해 출력한다.

## 로또 게임 예시

```markdown
구입금액을 입력해 주세요.
8000

8개를 구매했습니다.
[8, 21, 23, 41, 42, 43] 
[3, 5, 11, 16, 32, 38] 
[7, 11, 16, 35, 36, 44] 
[1, 8, 11, 31, 41, 42] 
[13, 14, 16, 38, 42, 45] 
[7, 11, 30, 40, 42, 43] 
[2, 13, 22, 32, 38, 45] 
[1, 3, 5, 14, 22, 45]

당첨 번호를 입력해 주세요.
1,2,3,4,5,6

보너스 번호를 입력해 주세요.
7

당첨 통계
---
3개 일치 (5,000원) - 1개
4개 일치 (50,000원) - 0개
5개 일치 (1,500,000원) - 0개
5개 일치, 보너스 볼 일치 (30,000,000원) - 0개
6개 일치 (2,000,000,000원) - 0개
총 수익률은 62.5%입니다.
```

# 기능

## 생각해 볼 예외 사항

1. 구매 금액을 입력한다.
    - 구매 금액 입력을 0을 포함한 음수를 입력할 수 있다.
    - 구매 금액의 상한이 없다.
    - 1000으로 떨어지지 않을 경우
2. 구매 급액에 맞게 알맞은 횟수의 로또 번호 6자리를 난수로 생성한다.
3. 당첨 번호 6자리를 입력한다.
    - 당첨 번호가 6자리가 아닐 경우
    - 당첨 번호가 1 ~ 45 범위가 아닐 경우
    - 구분자가 `,`가 아닐 경우
    - 구분자가 5개가 아닐 경우
    - 번호가 중복될 경우
4. 보너스 번호를 입력한다.
    - 보너스 번호가 1 ~ 45 범위가 아닐 경우
    - 보너스 번호가 당첨 번호와 중복될 경우
5. 당첨 통계를 나타내면서 사용자의 수익률을 계산해 출력한다.

## 기능 목록

- [ ] 로또 난수 생성 기능
- [ ] 생성된 로또 저장 기능
- [ ] 구매 금액 입력 기능
- [ ] 로또 당첨 번호 입력 기능
- [ ] 로또 보너스 번호 입력 기능
- [ ] 로또 번호 비교 기능
- [ ] 당첨 통계 출력 기능

## 예외 목록

### 구매금액

- [ ] 구매 금액이 숫자가 아닌 경우
- [ ] 구매 금액이 음수인 경우
- [ ] 구매 금액이 1000으로 나누어 떨어지지 않을 경우

### 당첨 번호

- [ ] 당첨 번호가 1 ~ 45의 범위가 아닐 경우
- [ ] 당첨 번호가 6개가 아닐 경우
- [ ] 당첨 번호가 중복될 경우
- [ ] 구분자가 `,`가 아닐 경우
- [ ] 구분자가 5개가 아닐 경우

### 보너스 번호

- [ ] 보너스 번호가 당첨 번호와 중복될 경우
- [ ] 보너스 번호가 1 ~ 45이 범위가 아닐 경우