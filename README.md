# top
### 시스템 상태를 모니터링하고 현재 실행 중인 프로세스 목록을 실시간으로 표시하는 명령어
### CPU, 메모리, 스왑, 프로세스 등의 정보를 볼 수 있으며, 프로세스의 CPU 및 메모리 사용량, 실행 시간 등을 확인할 수 있으며 시스템 리소스 사용을 추적하거나 프로세스 관리에 유용
![이미지](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Fblog.kakaocdn.net%2Fdn%2Frxlg4%2FbtqYfV2LE3L%2FSW5SbyO65ZUa5PggM3KI8K%2Fimg.png)

# ps
### 현재 실행 중인 프로세스의 정보를 표시하는 명령어
### 프로세스 ID(PID), 부모 프로세스 ID(PPID), CPU 및 메모리 사용량, 실행 시간 등의 정보를 확인
![이미지](https://mblogthumb-phinf.pstatic.net/MjAxODA0MDFfODUg/MDAxNTIyNTgzOTQxMDU3.VqSCrZyRucmK86WgoUCC-zrOPlZi6cKwHfy1LN-6uKEg.JBONDewYx7xBM1PdRlPp6SP8IO6BF2tLjAXEnOrslhEg.PNG.jjune095/image.png?type=w800)
### 옵션 https://m.blog.naver.com/PostView.naver?isHttpsRedirect=true&blogId=kkh0879&logNo=70176245345
##### -A : 모든 프로세스를 보여준다.
##### -N : -A 옵션과 비슷하나, ps 명령을 위해 실행한 ps 프로세스만 제외하여 보여준다. (실행을 취소한다)
##### -a : 세션 리더 및 터미널과 관련되지 않은 프로세스를 제외한 모든 프로세스를 보여준다.
##### -d : 세션 리더를 제외한 모든 프로세스를 보여준다.
##### -e : 커널 프로세스를 제외한 모든 프로세스를 보여준다.
##### T : 현 터미널에서의 모든 프로세스를 보여준다.
##### a : 한 터미널의 사용자 고유 프로세스를 보여준다.
##### r : 현재 실행중인 프로세스를 보여준다.
##### x : 터미널 없는 프로세스를 보여준다.
##### --deselect : -N 옵션과 같다. 등등 

# jobs
### 현재 쉘 세션에서 실행 중인 작업(백그라운드 또는 중지된 작업)의 상태를 표시
### 작업은 일반적으로 백그라운드에서 실행되는 프로세스이며 작업의 번호와 상태를 표시하며, fg나 bg와 함께 사용하여 작업을 전경으로 가져오거나 백그라운드로 보낼 수 있음
### bg : 백그라운드 실행 fg : 포그라운드 실행
![이미지](https://mblogthumb-phinf.pstatic.net/MjAxODA0MDFfMjkz/MDAxNTIyNTg0NzQzMjUx.-lhdey-gJC6zoXoKkP4FUhwd3aWtHYTWFFlWijuidDsg.-HtK32Ei5nPnUZGL9u_skGlz3ZqM4WuhIgXOzcbIjWgg.PNG.jjune095/image.png?type=w800)
### 옵션
##### -l : 프로세스 그룹 ID를 state 필드 앞에 출력
##### -n : 프로세스 그룹 중에 대표 프로세스 ID를 출력
##### -p : 각 프로세스 ID에 대해 한 행씩 출력
##### command : 지정한 명령어를 실행

# kill
### 실행 중인 프로세스를 종료하는 데 사용 
### 프로세스에 시그널(signal)을 보내어 프로세스를 제어 기본적으로 kill 명령어는 TERM 시그널을 사용하여 프로세스를 종료
![이미지](https://img1.daumcdn.net/thumb/R1280x0/?scode=mtistory2&fname=https%3A%2F%2Ft1.daumcdn.net%2Fcfile%2Ftistory%2F993696485C6377E90C)
### 옵션
##### -9 : 프로세스아이디(PID)를 직접 지정하여 종료시 사용 
##### -l : 신호(Signal)로 사용할 수 있는 신호(Signal) 이름들을 보여줌
