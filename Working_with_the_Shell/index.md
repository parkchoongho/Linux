# Working with the shell

## /폴더1/폴더2 구조로 만들때(폴더1이 없는 경우)
```bash
~ >>> mkdir -p /폴더1/폴더2
```
## Shell의 종류

1. Bourne Shell
2. C Shell(csh or tcsh)
3. Korn Shell(ksh)
4. Z Shell(zsh)
5. Bourne again Shell(bash)

## 내가 어떤 shell을 쓰는지 알 수 있는 명령어
```bash
~/D/P/Linux ❯❯❯ echo $SHELL
/bin/zsh
```
## Default shell을 바꾸는 명령어
```bash
~/D/P/Linux ❯❯❯ chsh
```
## Alias
`alias`를 활용하여 명령어를 더 간단하게 입력 가능
```bash
~/D/P/Linux ❯❯❯ alias dt=date
```
## History
`history` 명령어는 그 전에 내가 동작한 명령어들을 보여줌
```bash
~/D/P/Linux ❯❯❯ history
 1438  vi rand.c
 1444  gcc rand.c
```
## Bash Environment Variables
```bash
~ ❯❯❯ echo $SHELL
/bin/zsh
```
$을 붙이면 해당 환경 변수를 불러올 수 있음
```bash
~ ❯❯❯ env
HOME=/Users/choonghopark
LOGNAME=choonghopark
```
env를 입력하면 환경변수들을 가져울 수 있음
```bash
~ ❯❯❯ export OFFICE=parkchoongho
```
환경변수에 새로운 값을 할당하려면 `export` 명령어를 사용 그런데 이렇게 변수를 사용하는 것은 해당 쉘에서만 사용하기 때문에 계속해서 사용하기 위해서는 `~/.profile`이나 `/.pam_environment`에 추가해야함. 추가하는 방식은 아래와 같이 함
```bash
~ >>> echo 'export OFFICE=parkchoongho' >> ~/.profile
```