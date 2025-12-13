# 1. 오픈소스 소프트웨어
# 2. 리눅스
> 아래 내용은 Ubuntu 기준으로 작성되었음
## 2.1. 명령어 종류
1. 파일 관리 : `ls`, `cd`,  `mkdir`, `rmdir`, `touch`, `vi`, `cat`, `mv`, `rm`, `find`
2. 쉘 :  `chsh`, `echo`, `export`, `alias`, `unalias`, `history`
3. 파일 액세스 관리 :  `chmod`, `umask`, `chown`
4. 패키지 관리 :
5. 아카이빙/압축 : `tar`, `gzip`, `gunzip`, `bzip2`, `bunzip2`
6. 프로세스 : `ps`, `pgrep`,  `kill`, `sleep`, `jobs`, `fg`, `bg`
7. 시스템 사용자 관리
     - 사용자 :  `useradd`, `usermod`, `userdel`, `passwd`, `su`
     - 그룹 :  `groupadd`, `groupmod`, `groupdel`, `gpasswd`, `newgrp`
8. 파일 시스템 관리 : `fdisk`, `mkfs`, `dd`, `df`, `du`, `mount`, `umount`
9. 네트워크 관리 : `nmcli`, `ip`, `route`, `ping`, `traceroute`, `netstat`, `nmap`, `ufw`
# 3. GitHub
## 3.1. GitHub 활용법
### 3.1.1. 로컬 레포지토리에서 작업
### 3.1.2. 원격 레포지토리의 변경사항 가져오기
### 3.1.3. 브랜치 및 로그 확인
### 3.2.1. 로컬 레포지토리에서 작업
> 원격 레포지토리가 GitHub에 생성되어 있음을 가정
```
git clone <remote-repo>
```
```
git add .|<files>
```
```
git commit -m "<msg>"
```
```
git push <remote> <branch>
```
### 3.2.2. 원격 레포지토리의 변경사항 가져오기
```
git fetch <remote>
```
```
git merge <remote> <branch>
```
### 3.2.3. 브랜치 및 로그 확인
```
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
