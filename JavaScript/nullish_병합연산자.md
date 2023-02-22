## nullish 병합 연산자

<br>

- ??를 사용하면 짧은 문법으로 여러 피연산자 중 확정된 변수를 찾을 수 있다.
- a ?? b => a가 null도 아니고, undefined도 아니면 a

```
let firstName = null
let lastName = null
let nickName = "바이올렛"

alert(firstName ?? lastName ?? nickName ?? "익명의 사용자") //바이올렛
//null이나 undefined가 아닌 첫 번째 피연산자
```

<br>

### '??'와 '||'의 차이

- ||는 첫 번째 truthy 값을 반환
- ??는 첫 번째 정의된 값을 반환

```
let height = 0

alert(height || 100) //100	
alert(height ?? 100) //0
```

: height에 0을 할당했지만 0을 falsy 한 값으로 취급했기 때문에 null이나 undefined를 할당한 것과 동일하게 취급

: height ?? 100의 평가 결과는 height가 정확하게 null이나 undefined일 경우에만 100이 된다. 위에서는 0이라는 값을 할당했으므로 얼럿창에 0이 출력

<br>

- ??의 연산자 우선순위는 대다수의 연산자보다 낮고 ?와 =보다는 높다.
- 괄호 없이 ??를 ||나 &&와 함께 사용하는 것은 금지