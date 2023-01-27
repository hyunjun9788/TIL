## 메타 태그(meta)

<br>

- HTML 문서에 대한 메타데이터
- 메타데이터는 정보를 뜻함
- 항상 head태그 안에 있어야 한다.

- 검색엔진이 페이지를 검색할 때 참고자료로 활용할 수 있고 개발 작업에서도 페이지에 대한 정보를 명시함으로써 개발에 많은 도움이 된다.

<br>

#### ▶ meta 태그 쓰는 이유?

- 웹페이지 정보를 제공해주기 때문에 개발할 때에도 많은 도움이 되고 검색엔진이 페이지 검색할 때 참고할 수가 있다. 검색 결과에도 반영된다.

<br>

#### ▶ 메타데이터의 유형 및 속성

-  charset : 문자 세트
- http-equiv : 콘텐츠 속성 정보에 대한 http 헤더
- name : 문서 정보
- content : 메타데이터 내용

<br>

#### ▶ charset

- 문자 인코딩(한글을 표시하기 위해 문자 세트를 지정하는 작업)에 대한 요약 정보를 기입

- utf-8 사용하는 것이 좋음

```
<meta charset="utf-8"
```

<br>

#### ▶ http-equiv

- 콘텐츠 속성의 정보 및 값에 대해 http 헤더를 보여준다
- http는 인터넷에서 데이터를 주고 받을 수 있는 프로토콜 

```
<meta http-equiv="x-ua-compatible" content="IE=edge"> # IE 브라우저의 최신 버전 엔진 사용
<meta http-equiv="refresh" content="10" #10초마다 페이지 새로고침
```

<br>

#### ▶ name

- name 과 content 속성 한 쌍으로 생각

```
<meta name="author" content="유노코딩"> # 문서 만든사람
<meta name="description" content="페이지에 대한 간단한 요약"> 
<meta name="keywords" content="강아지, 고양이, 반려동물"> # 페이지의 콘텐츠와 관련된 키워드 목록
```

