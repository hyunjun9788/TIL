## reset

- 커밋을 했지만 이전 커밋으로 돌아가고 싶을 때 사용

  </br>

```
git reset HEAD~3
```

:HEAD로 부터 세 번째 전 커밋으로 되돌아감

</br>

```
git reset --hard 커밋hash
```

: 커밋hash 이후의 변경 내용 모두 삭제함

</br>

```
git reset --mixed 커밋hash
```

: 변경 이력은 삭제되지만 내용은 남아있음

</br>

```
git reset --soft 커밋hash
```

: mixed와 동일하나 stage 된 상태, 바로 commit 가능함

<br>

**rseet은 남들과 협업할 때 사용 금지** 