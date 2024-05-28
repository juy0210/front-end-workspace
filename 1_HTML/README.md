#HTML

## 웹 브라우저 : 인터넷 화면을 보여주는 프로그램

- Chrome, Fire Fox, Safari, Opera, Edge, Brave..
- 사용자가 사용하는 브라우저는 정해져 있지 않으며
  브라우저마다 화면이 다르게 출력이 될 수 있으니
  브라우저마다 테스트를 하면서 수정
  => 크로스 브라우징

  ## 웹 페이지 개발 방법

  - 구조(Structure) : HTML
  - 표현(Presentation) : CSS
  - 동작(Behavior) : JavaScript

  ## HTML(Hyper Text Markup Language)

  - 웹 문서 / HTML 문서 / HTML 페이지

  ## 웹 페이지 생성

  - 확장자는 .html 또는 .htm
  - 처음 보여지는 화면의 파일 이름은 "index.html"으로 고정

  ## main page, sub page

  - main page : index.html
  - sub page : index.html 제외 파일명.html 파일들

  ## 태그

```
<태그명 속성="값"></태그명>
```

1. "<"와 ">" 사이에 명령어(tag, element) 작성
2. 시작태그와 종료태그로 구성
3. 종료태그가 없는 태그들(img, br, hr, meta, input)
4. 태그는 중첩 가능하며 종료태그는 나중에 작성한 태그가 먼저 작성
5. 가급적 모든 태그와 속성은 소문자로 작성

## 속성의 특징

1. 태그와 속성, 속성과 속성은 공백으로 구분

```html
<a href="#"></a>
```

2. 여러 개의 속성을 사용할 수 있다.

```html
<img src="/" width="100">
```

3. 하나의 속성에는 값을 한개만 지정 가능하다.

```html
<img src="/" width="100,200">
<!-- 작성불가 --> 이렇게 쓰면 작성불가
```

4. 속성값은 원래의 이름이 한글인 경우가 아니면 사용 불가능하다.

```html
<img src="/" width="삼백"> 이렇게 쓰면 작성 불가
<!-- 작성 불가 -->
<meta name="keywords"를 쓰면 content="영화, 한국영화, 외국영화">
<!-- 예외적인 경우 --> 작성 가능
```

## HTML 기본 문서 구조

```html
<!DOCTYPE html>
<html> 안에
  <head></head>
  <body></body> 가 와야한다
</html>
```

- !DOCTYPE html : 현재 문서가 HTML5 언어로 작성된 웹 문서
- html : 웹 문서의 시작과 끝
- head : 웹 문서의 정보
- body : 실제 웹 브라우저에 나타날 내용

## head에 많이 쓰는 태그

1. title : 문서의 제목
2. meta : 문서의 속성(내용)

ex) <title>유튜브</title>

## meta 태그

```html
<meta charset="UTF-8"> <!-- 문자 세트 지정 -->
<meta name="viewport" content="width=device-width,
initial-scale=1.0"> 창을 줄일때 창에 맞게 줄어든다=반응성
<!-- 모바일 기기 때문에 설정-->
<meta http-equiv="X-UA-Compatible" content="ie=edge">
<!-- 인터넷 익스플로러 브라우저 -->

<!-- 검색 엔진 -->
<meta name="ketwords"를 입력하면 content="키워드1, 키워드2"키워드를 작성>
<meta name-"description"을 입력하면 content="문서 설명"을 작성>
<meta name="author" content="문서 작성자">
```