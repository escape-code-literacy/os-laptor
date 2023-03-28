- process life cycle
1. New
2. Running
3. Waiting
4. Ready
5. Terminated

IO도 하나의 행위 인데 왜 waiting을 하는 걸까

PCB : Process control block
- Process state
- Program counter : Instruction registry에서 참고 할 프로그램의 메모리 주소
- CPU registers
- CPU scheduling information
- Memory-management information
- Accounting information
- I/O status information
Thread : lightweight process

The objective of multiprogramming
- to have some process running at all times
- so as to maximize CPU utilization

The objective of time sharing
- to switch a CPU core among processes so frequently
- users can interact with each program while it is running

Scheduling Queues
실제 구현에서는 linked list로 구현
- ready queue : CPU에서 실행 될 때 까지 순서를 기다리는 큐
- wait queue : 어떤 이벤트 (i/O 와 같은)의 동작을 기다리고 있는 상태의 프로세스 큐

Context switch
1. switches the CPU core to another process
2. performs a state save of current process
3. a state restore of a different prcoess 

- Context : 프로세스 컨트롤 블럭을 의미
- Interrupt 발생시 실행중인 프로세스의 context를 저장하고, 추후에 다시 복구시켜서 사용