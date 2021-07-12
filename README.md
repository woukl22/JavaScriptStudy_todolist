## JavaScriptStudy_todolist
To do list with JavaScript

JavaScript self-study

## Book
'***혼자 공부하는 자바스크립트***(한빛미디어, 2021)'

![hongongjs](https://user-images.githubusercontent.com/69896250/124748870-95ea1d00-df5e-11eb-9e98-5aba9280f9f4.jpeg)


#### Contents
###### Chapter 01 자바스크립트 개요와 개발환경 설정

###### Chapter 02 자료와 변수

###### Chapter 03 조건문

###### Chapter 04 반복문

###### Chapter 05 함수

###### Chapter 06 객체

###### Chapter 07 문서 객체 모델

###### Chapter 08 예외 처리

###### Chapter 09 클래스

###### Chapter 10 리액트 라이브러리


## Study Log
### *2021.07.05 Mon.* ~Chapter 04-1 배열, todolist.html upload(2021.07.07)
  - ***switch 조건문**을 사용하여 기능 수행*
  - ***할 일 목록**을 배열로 만들어 push()와 splice()를 이용하여 목록 추가, 제거*

### *2021.07.06 Tue.* ~Chapter 04-2 반복문, todolist.html -v2 upload(2021.07.07)
  - ***할 일 목록**에 **반복문**을 사용하여 순서대로 번호를 붙여 출력함*
  - ***할 일 초기화** 추가*
  - ***할 일 추가하기**와 **할 일 제거하기**에도 할 일 목록이 보이도록 함*
  - ***종료하기**를 선택하면 윈도우 창이 완전이 꺼지도록 함*

### *2021.07.07 Wed.* ~Chapter 05 함수, todolist.html -v3 upload(2021.07.07)
  - ***'use strict'** 를 사용하여 **엄격모드** 적용*
  - ***할 일 목록**을 순서대로 번호 붙여 출력하는 기능을 **callList()** 함수로 만들었음*
  - ***callList()** 함수를 **forEach()** 메소드와 **화살표 함수**를 사용하여 만들었음*

### *2021.07.08 Thu.* ~Chapter 06 객체, todolist.html -v4 upload(2021.07.08)
  - ***todo_object** 객체를 생성하여, **todos**, **todo_list**, **specialTodos** 속성을 만들었음*
  - ***할 일 추가하기** 에서 String 객체의 기본 메소드 **.trim()** 을 사용하여 문자열 양 끝에 불필요한 공백이 입력될 시 없애도록 함*
  - *중요한 할 일 **목록 보기**, 중요한 할 일 **지정하기**, 중요한 할 일 **초기화** 추가*
  - ***중요한 할 일 지정하기**에서 **배열 전개 연산자 ([\.\.\.배열])** 를 이용하여 **깊은 복사**를 사용함*
  - ***중요한 할 일 지정하기**에서 String 객체의 기본 메소드 **.split()** 을 사용하여 **콤마(,)** 를 기준으로 입력 받은 문자열 값을 잘라서 새로운 배열에 저장함*

### *2021.07.09 Fri.* ~Chapter 07 문서 객체 모델, todolist.html -v5 upload(2021.07.09)
  - ***DOMContentLoaded**을 사용하여 자바스크립트로 *<body*> 안에 있는 **HTML 코드**를 조작함*
  - ***querySelector()** 메소드를 사용하여 html 요소를 **추출**하여 사용함*
  - ***querySelector()** 메소드 안에서 **'input'** 과 **'#add'** 등 CSS 선택자의 **태그 선택자**와 **아이디 선택자**를 사용함*
  - ***addEventListener()** 메소드를 사용하여 **addButton 클릭 시** 할 일이 추가되도록 함*
  - ***document.createElement()** 메소드와 **setAttribute()** 를 사용하여 새로운 문서객체를 생성하고, 속성을 부여함*
  - ***appendChild()** 를 사용하여 ***<div id*="todoList"*>** *아래에 새로 만든 문서객체를 추가함*

### *2021.07.10 Sat.* ~Chapter 09 클래스, todolist.html -v6 upload(2021.07.10)
  - ***Todo 클래스**를 만들어 할 일을 **인스턴스**로 생성하도록 함*
  - ***드롭다운 목록**을 활용하여 **할 일 목록(To do list), 중요한 할 일(Special todo), 완료된 할 일(Done)** 을 볼 수 있도록 함*
  - *드롭다운 목록에서 항목이 선택되면 **style.display="none"** 과 **style.display="block"** 을 사용하여 각 항목에 대한 화면으로 바뀌도록 함*
  - *드롭다운 목록에서 항목이 선택되면 페이지 상단에 있는 **제목**이 각 항목의 이름과 같게 바뀌도록 함*
  - ***addButton.addEventListener()** 을 사용하여 addButton이 눌리면, **new Todo()** 를 사용하여 **할 일 인스턴스**를 생성함*
  - *removeButton과 관련된 이벤트와 메소드는 아직 미완성*

### *2021.07.11 Sun.* todolist.html -v7 upload(2021.07.11)
  - ***Todo 클래스**의 contructor 내부에 **removeButton.addEventListener()** 를 넣어 remove 버튼이 작동하도록 해결함*
  - ***todoArray**와 **todoCount**를 전역 변수로 꺼내서 **클래스 내부**와 **DOMContentLoaded 이벤트**에서 모두 값을 변경할 수 있도록 함*
  - ***addButtonClick()** 메소드를 만들어 드롭다운 목록이 **To do list, Special todo, Done**일 때 각각 다른 결과가 나오도록 함*
  - ***addButtonClick()** 메소드에서 **try, catch, throw**를 사용하여 공백을 추가하는 상황에서 **예외 처리**를 함*
  - *add 버튼을 눌렀을 때, **입력칸** 내부의 글자가 지워지도록 함*

### *2021.07.12 Mon.* ~Chapter 10 리액트 라이브러리 맛보기, todolist.html -v8 upload(2021.07.12)
  - ***혼자 공부하는 자바스크립트** 책 다 읽음!!!*
  - ***Special todo**에서 **Important**로 이름 변경*
  - ***To do list**의 버튼을 **🗑️, 🗸, ☆ 이모티콘**으로 만들었음*
  - ***To do list**에서 **☆**버튼을 클릭하면 **★**으로 **색이 채워지도록** 함*
  - ***🗑️ 버튼**을 클릭하면 할 일이 **지워지도록** 함*
  - ***🗸 버튼**을 클릭하면 할 일이 **To do list 페이지**에서 사라지고 **Done 페이지**에 나오도록 함*
  - ***드롭다운 목록**을 오른쪽으로 정렬함*
  - ***드롭다운 목록**에서 **Important**와 **Done** 항목을 선택하면 입력칸이 사라지도록 함*
  - ***Done 페이지**에서는 할 일을 지우는 **🗑️ 버튼**만 나오도록 함*
