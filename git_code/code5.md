# 📌reset revert

# reset

reset 명령어를 사용하면 지정된 커밋 코드로 되돌아간다. 즉 특정 커밋의 해시 값 상태로 모든 코드를 복구한다.
```
$ git reset 옵션 커밋ID
```

## 옵션1 soft 
- 커밋 내용만 수정되고 작업공간과 stage는 이전과 같음
- 바로 다시 커밋할 수 있는 상태로 남아있는 것 다시 마지막 이전 head로 돌아가려면 Commit만 필요
```
$ git reset --soft 커밋ID
```

## 옵션2 mixed
- 커밋 내용과 stage가 같음
- 이력은 되돌려지고 stage도 되돌아가는 커밋의 내용으로 초기화 다시 마지막 이전 head로 돌아가려면 Add, Commit 필요
```
$ git reset --mixed 커밋ID
```

## 옵션3 hard
- 커밋 내용으로 작업공간과 stage 모두 동일하다.
- 돌아가려는 이력 이후의 모든 내용을 삭제 다시 마지막 이전 head로 돌아가려면 파일 수정 add, commit 필요
```
$ git reset --hard 커밋ID
```

Reset 이후에 다시 이전 상태로 돌아가려면 다음을 특별히 제공한다.
```
$ git reset --hard ORIG_HEAD
```

# revert
- 지정한 커밋을 취소해 바로 이전 상태로 되돌리는 방법이다.
- 이전의 커밋 히스토리는 그대로 유지되며 이것을 되돌리는 새로운 커밋이 그 이후에 추가된다.
```
$ git revert 커밋ID
```

기본 편지기에서 커밋메세지 편집 화면 실행
```
$ git revert HEAD
```

편집 화면 실행없이 자동 커밋 메세지로 커밋 Revert '이전메세지'
```
$ git revert HEAD --mo-edit
```

- 리버트로 병합을 취소할 때는 --mainline 옵션을 사용할 수 있다.
```
$ git revert --mainline 숫자 병합커밋ID
```
