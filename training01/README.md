<input type="submit" value="삭제"/>

01 JSX
---------------------------------------------------
<!-- JavaScript에서 react라이브러리 실행하기
첫 번째 : 생성하고자 하는 엘리먼트의 태그
두 번쨰 : 엘리먼트의 속성
세 번째 : 자식 노드 -->

<!-- React 16버전 이전의 리액트는 하나의 엘리먼트만 랜더링 하는 것이 가능하였으나
이후 버전에서는 배열을 랜더링 하는 것이 가능하도록 하였다. -->

<!-- render-배열형식 -->
ReactDOM.createRoot(document.getElementById("root")).render([greetingElement, textElement]); 

<!-- 엘리먼트
요소 노드, 어트리뷰트 노드, 텍스트 노드로 만들어지는 가상 dom의 개념 -->

<!-- 컴포넌트
엘리먼트를 반환하는 개념을 가진 화면의 구성 단위 -->

<!-- 함수형 컴포넌트에서만 훅을 사용할 수 있다 -->

<!--
-- JSX란?
createElement를 이용해 엘리먼트를 정의하면복잡하기도하고 가독성도 좋지 않다.
그래서 리액트팀은 ReactElement를 정의하는 간편한 방법으로 jsx 문법을 제공한다.
자바스크립트를 확장한 문법으로, ReactElement를 xml 문법 형식으로 정의할 수 있는 방법이다.

단, JSX는 공식적인 자바스크립트 문법은 아니며 바벨이라는 트랜스 파일링 툴이 필요하다.
바벨은 ES6+, E5 next 문법을 ES5문법으로 변환해 주는 도구이다.
-- bable: 여러가지 랭귀지들을 하나로 컴파일할 수 있게 해주는 역할

- 바벨 적용 방법(CDN)
1. 바벨 CDN 구문을 추가한다.
2. script 태그에 type 속성에 text/babel 속성을 추가한다. 

- JSX 사용 규칙
1. 최상위 엘리먼트가 두 개 이상이면 에러가 발생된다.
2. <div> 태그로 감사서 하나의 돔 트리를 생성할 수 있도록 한다.
3. <React.Fragment>로 감싸서 형식상의 돔 트리상 상위 엘리먼트를 만들어준다.
    의미없는 태그가 너무 길어진다는 단점
4. React 라이브러리로부터 Fragment 객체만 구조분해 할당을 해주면 React.을 생략할 수 있다.

-->
const helloworld = <h1>hello world</h1>;
ReactDOM.createRoot(document.getElementById("root")).render(helloworld);


02 rendering
---------------------------------------------------





03 component
---------------------------------------------------





04 props
---------------------------------------------------





05 state
---------------------------------------------------