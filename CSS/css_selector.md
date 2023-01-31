## 선택자(Selector)

<br>

### ▶ 기본 선택자

1. **전체 선택자** : 모든 요소 선택 (*)

```
*{
	color: blue;
}
```

<br>



2. **태그선택자** : 주어진 이름을 가진 요소를 선택, 다수일 경우에도 모두 선택

```
p{
	color:blue;
}
```

<br>

3. **클래스 선택자** : 주어진 class 속성값을 가진 요소 선택

```
.text{
	color:blue;
}
```

<br>

4. **아이디 선택자** : 해당 id 값을 가진 요소 선택 (중복 안됨, 고유한 식별자)

```
#topic{
	color: blue;
}
```

<br>

5. **그룹 선택자** : 여러 유형의 요소 한번에 선택

```
h1, p, div{
	color: blue;
}
```

<br>

###  ▶선택자 우선순위

아이디 선택자 > 클래스 선택자 > 태그 선택자

※ 문서 내에 동일한 선택자가 존재할 경우, 뒤에 있는 선택자의 요소를 적용

※ 서로 다른 선택자가 동일한 요소를 선택할 경우, 우선 순위대로 적용한다.

<br>

### ▶ 특성 선택자

-  주어진 속성의 존재 여부나 그 값에 따라 요소를 선택

```
[class]{
	background-color: tomato;
}
[class="item"]{
	background-color: tomato;
}
```

: class 속성을 가지고 있는 모든 요소 선택

: class가 "item"인 요소 선택

<br>

```
[class *= "it"]{color: white;} #클래스 값에 "it"가 포함되는 요소 모두 선택
[class ^= "it"]{color: white;} #클래스 값에 "it"가 시작하는 요소 모두 선택
[class $= "it"]{color: white;} #클래스 값이 "it로 끝나는 요소 모두 선택"
```

<br>

### ▶ 결합 선택자

```
div p{ color: white;} # div 요소 안에 위치하는 모든 p요소 선택
div > p{color: white;} # div 요소의 바로 아래 위치하는 모든 p요소 선택
h1 ~ p{color: red;} #  h1 요소의 뒤에 오는 형제 중 모든 p요소를 선택
h1 + p{color: red;} # h1 요소의 바로 뒤에 오는 형제 p요소를 선택
```

