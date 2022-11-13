# branch checkout switch 명령어
## 브랜치 개념
- 여러 개발자들이 동시에 다양한 작업을 할 수 있게 만들어 주는 기능
- 각자 독립적인 작업 영역안에서 마음대로 소스코드를 변경 가능
 
![1_PiduCtSA7kMwdPiMZo1nHw](https://user-images.githubusercontent.com/105197524/201524623-5006b04a-5d26-4100-b597-b36cb0e76441.jpg)

## 브랜치 명령어
- git branch는 브랜치 목록을 확인한다.
```
$ git branch -- 브랜치 확인
```
![제목 없음](https://user-images.githubusercontent.com/105197524/201523476-66a2a5ee-c3ab-4d2c-8bc5-63cdfd2024fd.png)
- 브랜치 생성
```
$ git branch '브랜치이름' -- 브랜치 생성
```
![화면 캡처 2022-11-13 224156](https://user-images.githubusercontent.com/105197524/201524835-5f6675e3-e13c-4c9d-989f-96a35de2930b.png)
- 브랜치 생성 확인
![제목 없음](https://user-images.githubusercontent.com/105197524/201523584-61f1f58f-e7b0-45ad-880d-2d8f1a8b2b91.png)
- git checkout, switch를 사용하면 다른 브랜치로 이동이 가능하다.
```
$ git checkout '브랜치이름' -- 브랜치 이동
$ git switch '브랜치이름' -- 브랜치 이동
```
![화면 캡처 2022-11-13 221806](https://user-images.githubusercontent.com/105197524/201523744-5894456a-2509-4852-ba8e-e4aa8b667290.png)
- checkout은 -b switch는 -c 옵션을 사용하면 생성 및 이동이 가능하다.
```
$ git checkout -b '브랜치이름' -- 브랜치 생성 및 이동
$ git switch -c '브랜치이름' -- 브랜치 생성 및 이동
```
![화면 캡처 2022-11-13 222002](https://user-images.githubusercontent.com/105197524/201523796-507e4bb4-9e5a-4fa3-b9da-22a5293aa8af.png)
- -d 옵션은 브랜치를 삭제한다.
```
$ git branch -d '브랜치이름' -- 브랜치 삭제
```
![화면 캡처 2022-11-13 222155](https://user-images.githubusercontent.com/105197524/201523878-21cf4921-ba8f-4509-8b13-4be55fb4cd88.png)
