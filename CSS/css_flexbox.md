## flexbox

<br>

- 박스 내 요소간의 공간 배분 및 정렬 기능을 제공하기 위한 1차원 레이아웃 모델
- 레이아웃을 다룰 때 한 번에 하나의 차원만을 다룬다는 특성 때문이다.

```
<div style="display: flex;">
	<div class="item">하나</div>
	<div class="item">둘</div>
	<div class="item">셋</div>
</div>
```

<br>

''주축(main-axis)'과 '교차축(cross-axis)'이 있다.

<br>

### ▶ flex-direction

- flexbox 내 요소를 배치할 때 사용할 주축 및 방향 지정

| 속성값         |                                            |
| -------------- | ------------------------------------------ |
| row            | default 값. 주축은 행, 콘텐츠 방향과 동일  |
| row-reverse    | 주축은 행이고 방향은 콘텐츠의  방향과 반대 |
| column         | 주축은 열이고 방향은 콘텐츠의 방향과 동일  |
| column-reverse | 주축은 열이고 방향은 콘텐츠의 방향과 반대  |

