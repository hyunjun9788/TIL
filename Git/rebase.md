## rebase

- merge commit을 남기는 것을 피하는 방법

- 공통된 base에서 파생된 두 branch에서 한 branch의 base를 다른 branch의 최신 커밋으로 옮김 

- 서버에 업로드 된 경우 해당 히스토리는 rebase 하면 안됨.

- 혼자 작업할 때 유용

master 브랜치로 이동하여 최신 master를 가져옴

```
git checkout main
git pull origin main
```

feature 브랜치로 이동한 후 rebase 실행

```
git checkout feature
git rebase main
```

- 전 커밋 히스토리 내용 수정 및 삭제

```
git rebase -i HEAD~2
```

