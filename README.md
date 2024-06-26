# opensw

### 1. `top`

`top` 명령어는 리눅스 시스템의 현재 상태를 실시간으로 모니터링하는 도구입니다. 
시스템의 여러 리소스 사용량을 실시간으로 확인할 수 있으며, 주로 CPU 및 메모리 사용량을 확인하는 데 사용됩니다. 
`top` 명령어를 실행하면 프로세스 목록과 리소스 사용량이 업데이트되는 화면이 표시됩니다. 
이를 통해 시스템 부하나 특정 프로세스의 리소스 사용량 등을 모니터링할 수 있습니다.

주요 옵션:
- `-d` : 갱신 주기를 지정합니다. 예를 들어, `top -d 5`는 5초마다 화면을 갱신합니다.
- `-n` : `top` 명령어의 실행 횟수를 지정합니다. 예를 들어, `top -n 10`는 10번 실행 후 종료합니다.

사용 예시:
```
top
```

### 2. `ps`

`ps` 명령어는 현재 실행 중인 프로세스 목록을 보여주는 유닉스 및 리눅스 명령어입니다. 
`ps` 명령어를 사용하면 특정 사용자나 프로세스의 정보를 확인할 수 있습니다. 
예를 들어, 현재 시스템에서 실행 중인 모든 프로세스의 PID(프로세스 ID), CPU 및 메모리 사용량 등을 출력할 수 있습니다.

주요 옵션:
- `-e` : 모든 프로세스를 보여줍니다.
- `-f` : 프로세스의 전체 포맷으로 출력합니다.
- `-aux` : 모든 사용자의 모든 프로세스를 상세하게 보여줍니다.

사용 예시:
```
ps -aux
```

### 3. `jobs`

`jobs` 명령어는 현재 셸에서 실행 중인 백그라운드(background) 작업을 보여줍니다. 
셸 스크립트나 명령어를 백그라운드에서 실행했을 때 해당 작업의 상태를 확인할 때 사용됩니다. 
백그라운드 작업이란 사용자가 현재 셸에서 다른 작업을 수행하면서도 특정 작업이 실행되는 것을 의미합니다.

주요 옵션:
- `-l` : 작업 번호와 프로세스 ID(PID)를 함께 보여줍니다.

사용 예시:
```
jobs
```

### 4. `kill`

`kill` 명령어는 특정 프로세스를 중단시키는 명령어입니다. 
이를 통해 프로세스를 종료하거나, 신호를 보내어 프로세스의 동작을 변경할 수 있습니다. 
`kill` 명령어는 보통 프로세스의 PID(프로세스 ID)를 사용하여 동작합니다.

주요 옵션:
- `-<signal>` : 특정 시그널을 보냅니다. 예를 들어, `-9`는 SIGKILL을 의미합니다.

사용 예시:
```
kill -9 <PID>
```

위와 같이 `top`, `ps`, `jobs`, `kill` 명령어를 사용하여 리눅스 시스템에서 프로세스 관리와 시스템 모니터링을 할 수 있습니다. 
이러한 명령어들은 시스템 관리자나 개발자에게 매우 유용한 도구입니다.
