## Tag



**Tag**: 추후에 시간이 지나게 되어도 버전이 어떤 커밋에 해당되는지 알고자 할때 사용 </br>

```
git tag
```

: 태그 조회 </br>

branch vs tag 

: 브랜치는 가리키는 커밋이 달라지며 tag는 어떤 특정 커밋ID만을 가리킨다.

<br/>

**annotated tag** : light weight tag보다 좀 더 자세한 정보들이 담겨있음.

```
git tag -a 1.5.0 -m"error update"
```

</br>

**태그 삭제**

```
git tag -d v1.5.0
```

</br>

**원격 저장소에 tag push 하기**

```
git push --tags
```

: 한번에 태그 여러개 push



