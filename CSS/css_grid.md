### grid-template-columns, grid-template-rows

- 그리드 컨테이너의 트랙 중 열,행 트랙 내 아이템들의 크기를 지정할 수 있는 속성
- none: 기본값, 수치: 음수X

```
grid-template-columns:100px 1fr;
grid-template-row: 200px 1fr 1fr;
```



### gap

- 그리드 아이템 사이의 간격을 지정하는 속성.
- 행에서의 간격과 열에서의 간격을 똑같이 지정

```
gap:20px 10px;
```

<br>

### 트랙 관련 함수

- 그리드 컨테이너의 트랙 크기를 지정할 때 사용할 수 있는 유용한 함수

| 함수                 | 기능                                       |
| -------------------- | ------------------------------------------ |
| repeat()             | 반복되는 값을 자동으로 처리할 수 있는 함수 |
| minmax()             | 최솟값과 최댓값을 각각 지정할 수 있는 함수 |
| auto-fill & auto-fit | 반응형을 고려해 사용할 수 있는 키워드들    |

```
    grid-template-columns: repeat(auto-fill, minmax(100px, auto));
    grid-template-rows: repeat(3, 100px);
```

