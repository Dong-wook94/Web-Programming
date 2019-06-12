# Chapter 6. Java Script 활용(DOM과 이벤트)

## HTML DOM(Document Object Model)
> DOM 을 간단하게 풀어서 설명하면 문서 객체 모델이다. 
**문서객체**란 '''<html>'''이나 '''<boy>'''같은 html 문서 태그들을 JavaScript가 이용할수 있는 
객체로 만들면 그것을 문서 객체라고 한다.

### HTML DOM(간단히 DOM)
- 사용목적 : HTM 태그의 모양이나 콘텐츠를 동적 제어하기 위해
- HTML 태그에 의해 출력된 텍스트나 이미지 변경

### DOM 객체
  - Array, String 객체 -> 객체 이름.프로퍼티 = 값
  - HTML 태그를 객체 이름으로 생각
  - 객체의 프로퍼티, 함수 호출 가능
  
### DOM 트리의 특징
  - DOM 트리의 루트는 document 객체
  - DOM 객체의 종류는 HTML 태그 종류만큼
  - HTML 태그당 DOM 객체가 하나씩 생성
  - HTML 태그의 포함관계에 따라 DOM 트리에 부모 자식 관계
  
### 브라우저가 HTML 태그를 화면에 그리는 과정
  1. 브라우저가 DOM 트리의 틀 생성
  2. 브라우저가 HTML 태그를 읽고 DOM 트리에 DOM 객체 생성
  3. 브라우저는 DOM객체를 화면에 출력
  4. HTML 문서 로딩이 완료되면 DOM 트리 완성
  5. DOM 객체 변경 시, 브라우저는 해당 HTML 태그의 출력 모양을 바로 갱신.
  
### DOM 객체는 5개의 요소 구성
  - 프로퍼티
  - 메소드
  - 컬렉션
  - 이벤트리스터
  - css 스타일
  
~~~javascript
  <p id ="firstP" style = "color:blue" onclick="this.style.color='teal'">
    이것은<span style="color:red">문장입니다.</span>
  </p>
~~~
  
  