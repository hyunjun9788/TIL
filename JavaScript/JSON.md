### JSON

- JSON.stringify : 객체를 JSON으로 바꿔준다. 객체, 배열, 원시형(문자형,숫자형,불린형,null) 적용

  함수 프로퍼티, 심볼형 프로퍼티, undefined 프로퍼티

- 객체에 toJSON 메서드가 있으면 자동 호출

<br>

```
let student = {
  name: 'John',
  age: 30,
  isAdmin: false,
  courses: ['html', 'css', 'js'],
  wife: null
};

let json = JSON.stringify(student);

```

<br>

- JSON.stringify는 중첩 객체도 문자열도 바꿔준다.
- 순환 참조가 있으면 원하는 대로 객체를 문자열로 못 바꾼다.

```
let meetup = {
  title: "Conference",
  room: {
    number: 23,
    participants: ["john", "ann"]
  }
};

alert( JSON.stringify(meetup) );
/* 객체 전체가 문자열로 변환되었습니다.
{
  "title":"Conference",
  "room":{"number":23,"participants":["john","ann"]},
}
*/
```

<br>

### replacer

:원하는 프로퍼티만 직렬화

```
let json = JSON.stringify(value[,replacer,space])
```

value: 인코딩 하려는 값

replacer : JSON으로 인코딩 하길 원하는 프로퍼티가 담긴 배열 또는 매핑 함수 function(key, value)

space: 서식 변경 목적으로 사용할 공백 문자 수

JSON으로 변환하길 원하는 프로퍼티가 담긴 배열을 두 번째 인수로 넘겨주면 이 프로퍼티만 인코딩 가능하다. 

<br>

### space

: 가독성 높일 때 사용

space에 2를 입력하면 공백 문자 두 개를 써 들여쓰기 해준다.
<br>

### JSON.parse

```
let value = JSON.parse(str, [reviver])
```

- str : JSON 형식의 문자열
- reviver : 모든 (key, value) 쌍을 대상으로 호출되는 function(key, value) 형태의 함수로 값을 변경시킬 수 있다.

```
let numbers = "[0,1,2,3]"
numbers = JSON.parse(numbers)
alert(numbers[1])
```

<br>

### reviver 사용

```
let str = '{"title":"Conference","date":"2017-11-30T12:00:00.000Z"}';

let meetup = JSON.parse(str, function(key, value) {
  if (key == 'date') return new Date(value);
  return value;
});

alert( meetup.date.getDate() )
```

