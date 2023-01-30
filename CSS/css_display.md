## display & border 속성

<br>

### ▶ display 속성

- 요소를 블록과 인라인 요소중 어느 요소로 처리할지 정의한다.

```
div{display:inline;}
a{display:block;}
```

<br>

### ▶ display 속성 값

|    속성값    |                             의미                             |
| :----------: | :----------------------------------------------------------: |
|    inline    |                       인라인으로 처리                        |
|    block     |                       블록 레벨로 처리                       |
| inline-block | 인라인으로 배치되지만, 블록 레벨 요소의 속성 추가(height, weight 조절) |
|     none     |                    디스플레이하지 않는다.                    |

<br>

### ▶ border 속성

- 요소가 차지하고 있는 영역에 테두리를 그린다.
- 두께, 모양, 크기 동시에 지정이 가능하다 (단축속성)

```
span{border:2px solid green;}
```

<br>

|    속성명    |                    속성값 예                     |
| :----------: | :----------------------------------------------: |
| border-color |              color 정의할 때와 동일              |
| border-width | thin, medium, thick 등의 키워드 또는 px, em, rem |
| border-style |           none, solid, dotted, dashed            |

