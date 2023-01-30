## 텍스트 꾸미기 속성

<br>

### ▶ font-family

- 텍스트 글꼴 설정
- 글꼴 우선순위 지정

```
*{
	font-family: Times, monospace, serif;
}
```

<br>

### ▶ font-size

| 단위 |                       의미                        |
| :--: | :-----------------------------------------------: |
|  px  | 모니터 상의 화소 하나 크기에 대응하는 절대적 크기 |
| rem  |   html 태그의 font-size에 대응하는 상대적 크기    |
|  em  | 부모(상위)태그의 font-size에 대응하는 상대적 크기 |

```
span{font-size:16px;}
span{font-size: 2rem;}
span{font-size:1.5em;}
```

<br>

### ▶ text-align

|   속성값   |       의미       |
| :--------: | :--------------: |
| left/right | 왼쪽/오른쪽 정렬 |
|   center   |    중앙 정렬     |
|  justify   |    양끝 정렬     |

```
p{text-align: right;}
```

<br>

### ▶ color

| 속성값 유형   | 방법                                     |
| ------------- | ---------------------------------------- |
| 키워드        | 미리 정의된 색상별 키워드 사용(red,blue) |
| RGB 색상 코드 | #과 6자리 16진수 값으로 설정             |
| RGB 함수      | Red, Green, Blue의 각 범위를 설정        |

