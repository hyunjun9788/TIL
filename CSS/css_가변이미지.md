### max-width

- 너비의 최대값을 지정하여 요소의 너비가 그 이상 커지지 않도록 한다.

```
img{
	max-width:200px(100%);
}
```

<br>

### picture

- 뷰포트의 너비 등 브라우저의 특정 조건에 따라 이미지를 반응형으로 불러 온다.

```
<picture>
	<source srcset="desktop.png" media="(min-width:1200px)">
	<source srcset="tablet.png" media="(min-width:800px)">
	<img src="mobile.png">
</picture>
```

