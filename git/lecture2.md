# 첫 번째 깃 실행

## 터미널
**터미널 환경이란 예전의 MS-DOS 또는 셸처럼 텍스트 명령어 입력하고 실행하는 환경을 의미한다.**

## 깃 명령어로 실행
**git 명령어 사용법 및 간단히 요약된 내용을 확인할 수 있다.**
```
$ git
usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           [--super-prefix=<path>] [--config-env=<name>=<envvar>]
           <command> [<args>]

These are common Git commands used in various situations:

start a working area (see also: git help tutorial)
   clone     Clone a repository into a new directory
   init      Create an empty Git repository or reinitialize an existing one

work on the current change (see also: git help everyday)
   add       Add file contents to the index
   mv        Move or rename a file, a directory, or a symlink
   restore   Restore working tree files
   rm        Remove files from the working tree and from the index

examine the history and state (see also: git help revisions)
   bisect    Use binary search to find the commit that introduced a bug
   diff      Show changes between commits, commit and working tree, etc
   grep      Print lines matching a pattern
   log       Show commit logs
   show      Show various types of objects
   status    Show the working tree status

grow, mark and tweak your common history
   branch    List, create, or delete branches
   commit    Record changes to the repository
   merge     Join two or more development histories together
   rebase    Reapply commits on top of another base tip
   reset     Reset current HEAD to the specified state
   switch    Switch branches
   tag       Create, list, delete or verify a tag object signed with GPG

collaborate (see also: git help workflows)
   fetch     Download objects and refs from another repository
   pull      Fetch from and integrate with another repository or a local branch
   push      Update remote refs along with associated objects

'git help -a' and 'git help -g' list available subcommands and some
concept guides. See 'git help <command>' or 'git help <concept>'
to read about a specific subcommand or concept.
See 'git help git' for an overview of the system.

```


## 간단한 명령어
**깃은 환경 설정을 위해 별도로 config 명령어를 제공합니다.** <br>
- $ git config -help 명령어로 확인 가능하다.

### 로컬 사용자
**로컬 저장소에서 사용자 등록은 별도의 웹 사이트에서 회원 가입하는 것이 아니라 소스 코드의 변경 내역을 기록할 때 <br>구분할 수 있는 사용자 설정 값만
등록하면 된다.**

```
$ cd 저장소 폴더 --> 깃 저장소 폴더
$ git config user.name --> 사용자이름
$ git config user.email --> 이메일 주소
```

### 글로벌 사용자(추천)
**저장소를 생성할 때마다 사용자 등록을 하는 것은 불편하다. 글로벌 사용자 등록을 할 때는 다음과 같이 --global 옵션을 함께 사용한다.**
```
$ git config --global user.name "사용자이름" --> 자신의 영문 이름
$ git config --global user.email "이메일주소" --> 자기의 이메일 주소
```

### 환경 설정 파일 확인 및 직접 수정
**먼저 로컬 저장소를 생성하고, 해당 저장소로 이동하여 사용자 등록을 한 후 설정 파일을 찾는다.**
```
$ mkdir gitstudy02 --> gitstudy02 폴더 생성
$ cd gitstudy02 --> 만든 gitstudy02 폴더로 이동
$ git init --> 깃 초기화
$ git config user.name "사용자이름" --> 로컬 사용자 이름 입력
$ git config user.email "이메일주소" --> 로컬 이메일 주소 입력
$ ls .git --> 깃 목록 보기
$ ls ~/.gitconfig --> .gitconfig 폴더의 경로 보기
cat .git/config --> 내용 확인하기
```

### 별칭
**복잡한 깃 명령어를 단순하게 닉네임 형태로 등록해 두는 기능이다.**
```
$ git config --global alias.lgg 'log --graph --oneline' --> 깃 명령어 log --graph --oneline을 lgg로 등록
```

## 정리
**지금까지 깃의 기본 환경설정을 알아보았습니다.**
