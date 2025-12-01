|제목1|제목2|제목3|
|---:|:---|:---:|
|데이터1|데이터2|데이터3|
|데이터11111|데이터22222|데이터33333|
|데이터44444|데이터555555|데이터66666|
# 1. 오픈소스 소프트웨어
* 오픈소스 라이선스의 종류 : GPL,Apache License  
+ 오픈소스 형태의 운영체제 : 리눅스  
- 개발 시 활용되는 관리 시스템 : Git/Github


# 2. 리눅스
> 아래 내용은 **Ubuntu**기준으로 작성되었음  
> ~~_여러줄_~~    
>  
> <ins><b><i>여러줄</i></b></ins>
- /있으면 닫기 없으면 열기
## 2.1 명령어 종류
1. 파일관리 : : `ls`, `cd`, `mkdir`, `rmdir`, `touch`, `vi`, `cat`, `mv`, `rm`, `find`
2. 쉘 : `chsh`, `echo`, `export`, `alias`, `unalias`, `history`
3. 파일 엑세스 관리 : `chmod`, `umask`, `chown`
4. 패키지 관리 :  
| 기능               | apt 형식        | apt-get / apt-cache 형식 |
|:---:|:---:|:---:|
| 패키지 검색        | apt search     | apt-cache search         |
| 패키지 정보 검색   | apt show       | apt-cache show           |
| 패키지 정보 업데이트 | apt update     | apt-get update           |
| 패키지 업그레이드   | apt upgrade    | apt-get upgrade          |
| 패키지 설치        | apt install    | apt-get install          |
| 패키지 삭제        | apt autoremove | apt-get autoremove       |
| 패키지 파일 다운로드 | apt download   | apt-get download         |


6. 아카이빙/압축 : `tar`, `gzip`, `gunzip`, `bzip2`, `bunzip2`
7. 프로세스 : `ps`, `pgrep`, `kill`, `sleep`, `jobs`, `fg`, `bg`
8. 시스템 사용자 관리
   - 사용자 : `useradd`, `usermod`, `userdel`, `passwd`, `su`
   - 그룹 : `groupadd`, `groupmod`, `groupdel`, `gpasswd`, `newgrp`
9. 파일 시스템 관리 : `fdisk`, `mkfs`, `dd`, `df`, `du`, `mount`, `umount`
10. 네트워크 관리 : `nmcli`, `ip`, `route`, `ping`, `traceroute`, `netstat`, `nmap`, `ufw`

# 3. Github
## 3.1. Github 활용법
### 3.1.1. 로컬 레포지토리에서 작업

``` shell 
git clone <remote -repo>
git add .|<files>
git commit -m "<msg>"
git push <remote> <branch>
```
### 3.1.2. 원격 레포지토리의 변경사항 가져오기

```shell
git fetch <remote>
```
```shell
git merge <remote> <branch>
```
### 3.1.3. 브랜치 및 로그 확인
``` shell
 opensw@tux:~/gitlab/openswproject$ git branch
 develop
 * main
 opensw@tux:~/gitlab/openswproject$ git log --oneline --dec
 orate --graph --all
 * c3dc21d (HEAD -> release) Resolve conflict
 |\
 | * 4cfe584 (develop) New line about log
 | * 332c95b New feature's code
 * | b88648d Create introduction file about new version
 |/
 * b2f6043 (main) Need to a new function
```
