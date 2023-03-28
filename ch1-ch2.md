# What is OS
---
- 정보량 : $I(x)={log_2}P(x)$
    - 만약 주사위의 예시를 든다면, $P(x) = \frac{1}{6}$ 이 되고 정보량은 $log_2{6}$ 이 된다.

- 정보의 단위 : bit, bianry digit ($P(x) = \frac{1}{2}$ 인 경우
- 튜링 머신의 구조로 부터 나왔음

    |앨런 튜링|현대 컴퓨터
    |------|---|
    |튜링 머신|응용 프로그램|
    |유니버설 튜링 머신|**운영 체제**|
    |테이프|메모리|

- A stored-program computer (폰노이만 아키텍쳐)
- 보통 kernel 이라고 부른다.
- bootstrap program : 컴퓨터가 켜질때 처음으로 동작해야하는 프로그램
- Interrupts : I/O device로 부터 신호를 전달 받는 과정
- CPU가 명령어를 memory로 부터 fetch 하여 실행하는 구조 - 폰노이만 구조
    - instruction register
