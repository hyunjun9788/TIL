### grid-template-columns, grid-template-rows

- 그리드 컨테이너의 트랙 중 열,행 트랙 내 아이템들의 크기를 지정할 수 있는 속성
- none: 기본값, 수치: 음수X

```
grid-template-columns:100px 1fr;
grid-template-row: 200px 1fr 1fr;
```

<br>

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

<br>

### grid-column & row

- grid-column과 grid-row 속성을 이용하면 그리드 컨테이너의 줄 번호를 이용해 아이템을 배치할 수 있다.

```
li:nth-child(1){
    grid-row:1/2;
    grid-column:1/3;
}

li:nth-child(2){
    grid-row-start: 1;
    grid-row-end:3;
    grid-column-start: 2;
    grid-column-end: 4;
}
```

<br>

### grid-template-areas

- 그리도 영역의 이름으로 레이아웃의 형태를 정의

```
.container{
    display:grid;
    height: 500px;
    grid-template-columns: repeat(3,1fr);

    grid-template-areas:
    "aa aa aa"
    "b  b  ."
    "c  d  e";

}

li:nth-child(1){grid-area:a;}
li:nth-child(1){grid-area:b;}
li:nth-child(1){grid-area:c;}
li:nth-child(1){grid-area:d;}
li:nth-child(1){grid-area:e;}
```

<br>

### align-items

- 플렉스박스 방식에서와 유사한 역할을 한다.
- 그리드 컨테이너 행 트랙의 높이를 기준으로 그리드 아이템의 배치 결정(stretch, start, end, center)

### align-self

- 개별 그리드 아이템들이 어떤 식으로 배치될 것인지 결정 

### justify-items

- 수평축을 따라 그리드 아이템을 정렬하고자 할 때 사용할 수 있는 속성으로, 그리드 컨테이너에 지정한다.
- 열 방향 너비 기준

### justify-self

- 각각의 그리드 아이템에 지정한다.

```
.container {
    display: grid;
    height: 500px;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows:repeat(2, 1fr);

    align-items: stretch;
}

li:nth-child(1){grid-area:a;}{}
li:nth-child(1){grid-area:b;}{align-self:start;}
li:nth-child(1){grid-area:c;}{}
li:nth-child(1){grid-area:d;}{align-self:end;}
li:nth-child(1){grid-area:e;}{align-self:center;}
```



<br>

align-items 와 align-content의 차이 : 트랙 안에서냐, 컨테이너 전체 안에서냐

```
align-content:space-evenly;
justify-content:space-between;
```

<br>

### align-content & jusify-content

- 그리드 컨테이너의 수직축과 수평축에서의 아이템 정렬 방식 결정
- 컨테이너에 여유 공간이 있을 때 사용

