# 첫 번째 깃 실행

## 터미널
**터미널 환경이란 예전의 MS-DOS 또는 셸처럼 텍스트 명령어 입력하고 실행하는 환경을 의미한다.**

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
