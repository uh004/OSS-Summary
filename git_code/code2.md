# clone
```
원격 저장소를 지역 저장소에 복제가 가능하다.
-공개된 저장소는 소유와 관계 없이 가능하다.
$ git clone [복사된 주소] [새로운 폴더명]
```
![images](https://user-images.githubusercontent.com/105197524/196172105-975da763-6e5e-4366-86e8-b1df0d6e3b17.png)

# push && pull
```
push && pull 사용하려면 원격 저장소와 지역 저장소가 연동되어 있는지 확인해야한다.
$ git remote --> 원격 저장소 이름 목록
안되어 있을 경우 $ git remote add [원격저장소주소]
지역저장소의 수정 내용을 다시 원격저장소로 올릴때 사용한다. --> push
$ git pull
원격저장소의 수정 내용을 다시 지역저장소로 끌어온다. --> pull
$ git pull
```
![download](https://user-images.githubusercontent.com/105197524/196176570-24cd7cf9-bdea-4af2-bb00-79ee0d644284.jpg)

# fetch/merge
```
fetch: 원격 저장소에서 커밋된 코드를 임시 브랜치로 내려받습니다.내려받은 후 현재 브랜치와 자동 병합하지 않습니다.
$ git fetch [원격저장소URL]
merge: 페치는 데이터를 내려받기만 할 뿐 자동 병합이 되지않는다.
내려받은 커밋을 로컬 저장소에 적용하려면 병합 명령을 실행해야 하는데 이때 merge 명령어를 사용한다.
$ git merge [원격저장소별칭/브랜치이름]
```
![1622436019-103268](https://user-images.githubusercontent.com/105197524/196176331-a0d5a8d5-f8cd-4483-a4bb-e1cdbf1c4bce.png)
