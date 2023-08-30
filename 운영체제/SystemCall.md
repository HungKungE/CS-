## System Call

1. 설명
Process 생성과 제어를 위한 System call

2. 종류
- fork() : 자식 프로세스 생성. 부모와 동일한 작업
- exec() : 자식 프로세스 생성. 부모와 다른 작업
- wait() : parent가 child 끝날 때까지 대기.