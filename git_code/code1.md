# 📌add, commit, log, show 

<img src="https://user-images.githubusercontent.com/105197524/196039835-5fbce362-a775-4ebb-b315-01a3c7d5cf6e.jpg" height = 70% width = 60%>

```
1. 워킹 디렉터리는 작업을 하는 공간을 의미한다.실제로 파일을 생성 및 수정 가능 공간입니다.
2. 스테이지 영역은 임시로 저장하는 공간을 의미한다. 파일들의 스테이지 상태는 status 명령어로 확인 가능하다.
3. 로컬 저장소는 내 PC에 파일이 저장되는 개인 전용 저장소입니다.
4. 원격 저장소는 파일이 원격 저장소 전용 서버에서 관리되며 여러 사람이 함께 공유하기 위한 저장소입니다.
```

## add 명령어
깃의 add 명령어는 워킹 디렉터리의 파일을 스테이지 영역으로 등록한다.
```
$ git add main.py
$ git add . --전체 파일과 폴더를 모두 등록할 수 있다.
```

## commit 명령어
깃의 commit 명령어는 git add를 통해 스테이지 영역에서 지역 저장소로 등록 후 커밋메세지 를 저장한다.
```
$ git commit -m '커밋메세지'
```

## add commit 한번에 하기
git commit -am을 사용해서 add와 commit을 한번에 할 수 있다.
```
$ git commit -am '커밋메시지'
```


## log 명령어
마지막 커밋인 head부터 이전 모든 이력 로그 표시한다.
```
$ git log
```
![제목 없음](https://user-images.githubusercontent.com/105197524/196040065-4f32120d-5261-4910-a44b-a7e3ea8a7d74.png)

## show 명령어
commit의 자세한 정보 확인가능
```
$ git show
```
![제목 없음](https://user-images.githubusercontent.com/105197524/196040317-8bb56aee-7116-4bc0-b7d1-28402fbde653.png)
