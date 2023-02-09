## DOM

<br>

### ul태그

- 순서가 정해지지 않은 목록
- 검은 점으로 표현
- li 태그를 반드시 입력해줘야 함.



### ol 태그

- 순서가 정해진 목록을 표현 할 때 사용
- li 태그 반드시 입력해줘야 함



<br>

### DOM

- JS로 HTML 문서를 조작
- document 객체를 참조해와서 내부 HTML 요소를 참조한 것 같았지만, 사실 HTML 요소들을 직접적으로 조작했던 것이 아니다.
- DOM Element를 조작
- 브라우저는 HTML 문서를 파싱하는 과정에서 DOM 이라는 트리구조 형태의 객체를 생성

<br>

document.getElementById() : Element Node의 id 속성을 체크해서 해당하는 Element를 참고해옴

document.getElementByclass() : Element class의 id 속성을 체크해서 해당하는 Element를 참고해옴

document.querySelector() : 소괄호 안에 입력한 값에 해당하는 Element를 참조해옴

document.querySelectorAll() : 소괄호 안에 입력한 값에 해당하는 Element 참조, 배열 형태로 모든 요소 참조

document.createElement() : 새로운 Node를 생성. Node의 형태는 생성되지만 DOM에 직접 추가하지 않으면 속하지 않음.

document.appendChild() : Element Node를 현재 DOM에 추가. 이때 document는 다른 Element가 될 수 있다.

<br>

### window.event

- window 객체 : 현재의 DOM 문서를 담고 있는 창, 내부에는 내장되어 있는 함수, 변수, 객체 존재
- event : DOM 내에서 발생하는 이벤트

```
<!DOCTYPE html>
<html lang="en">
  <head>
    <title>Document</title>
		<script>
      const printName = function () {
        const inputValue = document.querySelector('#name-input-box');
        if (window.event.keyCode === 13) {
          console.log(inputValue.value);
        }
      };
    </script>
  </head>
  <body>
    <input id="name-input-box" onKeydown="printName()" />
  </body>
</html>
```

: Enter 버튼은 13이라는 keycode 숫자를 가짐

​									▼

input 태그 내에서 버튼이 눌릴 때마다 함수가 실행되도록 onkeydown 속성에 해당함수 할당

​									▼

event를 체크해 key code가 13이라면 Enter 버튼을 누른 것이므로 조건문이 통과된다.



<br>

출처: 인프런 훈훈한 JS