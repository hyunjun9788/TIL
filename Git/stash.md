### stash

---

- 작업이 아직 끝나지 않은 작업을 커밋하기는 애매하고, 안 하기에는 checkout 할 수가 없을 때 사용하는 명령어
- 작업했던 내용을 숨길 수 있다.
- working directory와 staging area의 작업물을 임시 저장공간에 저장하는 명령어
- stash 하지 않으면 새로운 브랜치로 딸려감

```
git stash
```

: 최소한 버전관리 되고 있는 파일에 대해서만 stash (untracked X)

```
git stash list
```

: stash 목록 확인 

```
git stash apply
```

: 기존 작업을 불러옴.

```
git stash drop
```

: 최근의 stash 제거

```
git stash pop
```

:  git stash로 저장했던 부분들을 해당 코드로 꺼냄, 임의 공간에 저장됐던 파일들은 삭제됨. 삭제하지 않는 방법이 git stash apply (임의공간은 둔 채로 변경사항만 꺼내줌)