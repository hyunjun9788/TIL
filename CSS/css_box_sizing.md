### box-sizing

- 요소의 너비와 높이를 계산하는 방법 지정해줌

|   속성값    |                      의미                      |
| :---------: | :--------------------------------------------: |
| content-box | default값. 너비와 높이가 콘텐츠 영역만을 포함  |
| border-box  | 너비와 높이가 안쪽 여백과 테두리 영역까지 포함 |

※ 너비와 높이가 같더라도, box-sizing 속성값에 따라 크기가 달라질 수 있음

※ width와 height를 일일이 계산하지 않고 요소의 크기를 정하고 싶으면 border-box 사용 