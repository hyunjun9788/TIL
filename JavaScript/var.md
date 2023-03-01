### var

- 블록 밖에서 접근 가능
- 블록 스코프가 없다
- var는 코드 블록을 무시하기 때문에 test는 전역 변수가 된다.

```
if (true){
	var test = true
	}

alert(test)
```

: 전역 변수에서 위 변수에 접근 가능, 위에서 var 대신 let 이었다면 에러

```
for(var = i; i<10; i++){
}
alert(i) //10, 반복문이 종료되었지만 'i'는 전역 변수이므로 여전히 접근 가능
```

<br>

```
function sayHi(){
	if(true){
}
alert(phrase)}// 제대로 출력

sayHi()
alert(phrase) -- 오류
```



<br>

### var는 변수의 중복 선언 허용

```
var user = "Pete"

var user = "John" // 이 "var"는 아무것도 하지 X
alert(user) //John
```

<br>

- var 선언은 함수가 시작될 때 처리됨
- 함수 본문 내에서 var로 선언한 변수는 선언 위치와 상관없이 함수 본문이 시작되는 지점에서 정의된다.

```
function sayHi(){
	phrase = "Hello",
	alert(phrase)
	var phrase  <=
}
sayHi()
```

```
function sayHi(){
	var phrase  <=  호이스팅
	
	phrase = "hello"
	
	alert(phrase)
}
sayHi()
```

<br>

### 즉시 실행 함수 표현식

- 함수 표현식을 괄호로 둘러쌓아 (function{...})와 같은 형태로 만든다.
- 함수 선언문으로 정의한 함수를 정의와 동시에 호출 허용 X

```
function go(){
}() // 함수 선언문은 선언 즉시 호출 X
```

<br>



참고: https://ko.javascript.info/var