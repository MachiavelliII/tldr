# unshare

> 사용자 정의 네임스페이스에서 명령을 실행합니다.
> 더 많은 정보: <https://manned.org/unshare>.

- 연결된 네트워크에 대한 액세스를 공유하지 않고 명령 실행:

`unshare {{[-n|--net]}} {{명령어}} {{명령어_인자들}}`

- 마운트, 프로세스, 네트워크를 공유하지 않고 자식 프로세스로 명령 실행:

`unshare {{[-m|--mount]}} {{[-i|--pid]}} {{[-n|--net]}} {{[-f|--fork]}} {{명령어}} {{명령어_인자들}}`
