## position

<br>

- 문서 상에 요소를 배치하는 방법을 정의

  position: 난 이렇게 배치할거야;

  top: 윗 부분으로부터 얼만큼 떨어뜨릴거야;

  right : 오른쪽면에서부터 얼만큼 떨어뜨릴거야;

  bottom : 아랫면에서부터 얼만큼 떨어뜨릴거야;

  left : 왼쪽면에서부터 얼만큼 떨어뜨릴거야;

<br>

### relative

- 요소의 일반적인 문서의 흐름에 따라 배치, 오프셋 적용

```
div{
	width: 100px; height: 100px;
	background-color: red;
	
	position: relative;
	top: 100px; left: 100px;
}
```

<br>

### absolute

- 요소를 일반적인 문서 흐름에서 제거, 가장 가까운 상위요소에 있는 position을 기준으로 오프셋을 적용
- 상위요소에 position이 없다면 브라우저 화면을 기준으로 위치한다.

```
div{
	width: 100px; height: 100px;
	background-color: red;
	
	position: absolute;
	top: 100px; left: 100px;
}
```

<br>

### fixed

- 일반적인 문서 흐름에서 제거, 지정된 위치에 고정

```
.pos{
	width:200px; height:200px;
	background: peru;
	position: fixed;
	top: 50px; left: 50px;
}
```

 <br>

### sticky

- 요소를 일반적인 문서 흐름에 따라 배치, 스크롤되는 가장 가까운 상위 요소에 대해 오프셋적용 
- 상위요소가 스크롤되는 동안에도 자신의 정해진 위치를 지킨다.