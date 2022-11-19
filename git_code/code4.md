# fast forward merge, 3-way merge, rebase

## fast-forward 병합
```
$ git merge 브랜치 이름
```
- Merge할 대상이 현재 커밋의 직접적인 뿌리가 되는 경우 fast-forward 병합이 실행
- 병합할 브랜치의 조상이 기준 브래친인 경우 병합의 기본은 fast-forward 병합

## 3-way 병합
```
$ git merge 브랜치 이름 --3 way 병합은 브랜치 경로가 다른 갈래로 뻗어 나가 있을 때 적용
$ git merge --no-ff 브랜치 이름 -- --no-ff 옵션을 사용하면 3-way 병합으로 적용
```
- 두 브랜치의 조상이 같은 경우 새로운 커밋을 사용하여 두 기록을 합침

## 병합 시 주의점
- Merge 명령을 실행하기 전에 작업과 Stage 영역에 작업중인 파일이 없는지 꼭 확인

## rebase
