# TIL

내가 오늘 배운 것들(Today I Learnd)

## 1일차 학습

- GitHub 계정 생성
- GitHub 저장소 생성
- GitKraken 설치
- GitKraken을 사용하여 GitHub 저장소 데이터를 내 컴퓨터로 복제(Clone)

---

## 1주차 - 월요일 학습

### [React 학습에 앞서 공부해야 할 것들!]

학습 완료

### [Front-End 개발 학습 로드맵]

학습 완료

### [프로그래밍 언어 환경]

학습 완료

### [프레임워크를 사용하는 이유]

학습 완료

### ES6 영상 강의 시청 중

---

## 1주차 - 화요일 학습

### React 소개

- ReactDOM --> 웹사이트 / 앱
- React Native --> 모바일 네이티브 앱

특징

- 선언형 프로그래밍 : props(전달 속성), state(상태/변경 감지), update
- 컴포넌트 기반 프로그래밍 : 캡슐화 된 component는 JSX(javascript + XML)

### React 러닝 다이어그램

학습완료

### React 컴포넌트와 요소

React Component (Functional) -> 설계
React Element (JSX) -> 변수 처리
ReactDOM - Rendering (변수를 불러와 화면에 적용)

```
function App() {
  return <div>React Elemeent</div>
}

var app = <App/>

ReactDOM.render(app, document.querySelector('#app'))
```

### React 컴포넌트 구조 이해 및 활용

- component 구조에 따른 분류와 캡슐화하여 변수 처리하고, 불러와서 rendering하는 과정
- 유의할 점 : class 대신에 className을 사용할 것.

### React 컴포넌트와 전달 속성(props)

component에 속성(prop)을 사용하여 전달하고, 전달한 속성을 반영하는 방법

- 중괄호{}를 사용하여 속성을 전달하고, 속성을 특정하기 위해 props 뒤에 .을 구분자로 사용하여 뒤에 속성을 전달한다. {props.image} 이때 path가 길고 중복일때는 변수 처리 가능.

### React 프로젝트 생성 with CRA

개발 환경 구성(개발서버, webpack, babel 등)을 대신해줄 CRA 설치
질문 : CRA는 실무에서도 사용을 하나요, 아니면 이번 강의의 학습을 위한 대안인가요?

### React 프로젝트 디렉토리 구조

학습완료

---

## 1주차 수요일 학습

### Prettier - Code formatter

### Formatting Toggle

포메터를 켜고/끄는걸 쉽게 해주는 확장

### React Snippets

### React Pure To Class

react 함수형 component를 class component로 변경해주는 확장

### Auto Import

componenet를 입력하면 자동으로 module을 import 시켜주는 확장

### Import Cost

import로 불러온 module의 cost를 표기해주는 확장

### Auto Complete Tag

tag를 자동으로 열고/닫을때 표기해주는 확장

### Bracket Pair Colorizer 2

### Color Highlight & Manager

javascript에서 color를 관리해주는 확장

### Image preview

### Translator

---

## 1주차 목요일 학습

1. Virtual DOM

### 환경 설정

### Real DOM 컨트롤

### Virtual DOM 컨트롤

### Virtual DOM Tree 비교 & 패치

### Virtual DOM 배열 순환

### Virtual DOM 제거

### Virtual DOM 추가

virtual DOM의 영상 실습 완료

2. JSX ➪ React 요소

### React 요소를 만드는 2가지 방법

- npx create-react-app <프로젝트-이름>
  으로 react project 생성
- JSX를 사용하는게 정신건강에 좋다!!!

### 가상 DOM이란?

h.js - virtual DOM을 만들어주는 역할
createElement.js - virtual DOM을 실제 DOM에 붙여주는 역할
diff.js - DOM의 변화를 감지하는 역할
patch.js - DOM을 update 하는 역할

### JSX 코드가 Babel 컴파일러를 만나면?

Babel을 이용해서 JSX를 React.createElement()로 자동 변경해줌.
JSX가 작업이 쉽기때문에 JSX로 만듬.

---

## 1주차 금요일 학습

## JSX 활용

### 데이터 바인딩이란?

Data를 변수에 담아서 JSX에 binding 시켜준다. 이때 변수는 중활호로 감싼다.

### 콘텐츠 바인딩과 JavaScript 표현식

변수에 담긴 Data는 숫자, 문자, 식을 중활호 안에서 처리 할 수 있고, 문은 사용 할 수 없다.

### 속성 바인딩 (style, className)

- 속성을 binding 할때는 객체를 사용한다. inline-style 일때는 binding을 위한 중괄호 안에 객체를 넣기 위한 중괄호를 사용해야한다.
- style 속성을 객체 단위로 변수에 넣어서 binding 할 수 있다.
- css file을 import 하여, 속성을 binding 할 수 있다.

### 조건 문을 사용한 조건부 렌더링 (if, switch 문)

함수를 사용하여 필요한 조건문을 상황에 맞게 설정하여, 결과값을 return 하여 binding 할 수 있다.

### 조건 식을 사용한 사용한 조건부 렌더링 (3항식, 논리연산자)

JSX에서 inline으로 조건식(3항식, 논리연산자)을 사용한 조건부 렌더링

### Array 객체의 map() 메서드를 활용한 리스트 렌더링

- React의 트 렌더링은 배열객체의 map method를 사용한다.
- list rendering을 할때는 반드시 고유한 key값을 설정 해주어야만 오류가 발생하지 않는다.

### JSX 사용시 주의할 점

- JSX에서 ReactDOM은 HTML 표준 속성 이름을 그래로 사용 할 수 없고, camelCase로 사용 해야만 한다.
- role, aria- 는 원래 사용 그대로 사용.
- 콘텐츠가 없는 요소는 항상 닫아주어야만 한다.(img, br, area 등등)
- root 요소는 1개만 사용해야한다. 부득이 root 요소를 2개 이상 사용해야만 할때는, <React.Fragment></React.Fragment>로 감싸 주면 rendering 될때 이 부분은 반영 되지 않는다.

---

## 2주차 월요일 학습

1. 컴포넌트 & 전달 속성(props)

### React 함수형 컴포넌트

- 함수명 첫글자를 대문자 사용 권장
- 함수형 컨포넌트 생성
  cont 함수명 = () => {
  return (
  // JSX
  )
  }

const function 함수명() {
render(){
return (
// JSX
)
}
}

- 컴포넌트는 <함수명 />을 사용하여 불러옴.

### React 클래스 컴포넌트

- 클래스 컨포넌트 생성
  class 함수명 extends React.Comopnent {
  return (JSX)
  }
- 'react pure to class'를 사용하여 함수형 컨포넌트를 클래스 컨포넌트로 변환하여 사용 하면 편하다.
- constructor를 사용해 props를 전달해 줘야만 한다.

### React 컴포넌트 import, export / props

- 구조분해 할당.. 어려움... ㅠ.,ㅜ
- children을 사용하여 외부에서 전달받은 모듈의 유연하게 바꿀 수 있게 해준다.(markup을 전달 받은 모듈과 다른 형태로 바꿀 수 있음)

### React 컴포넌트 관리 (추출)

단축키 rafc : create a React Arrow function component
단축키 rcc : create a React conponent class

conponents를 분리/분류하여 세부적으로 나누어 놓으면 재사용하기 쉬움. (재사용하기 쉽게 만듣어야함)

2. 전달 속성(props) 검사

### JavaScript 타입 검사

typeof의 오류 때문에 data type에 대한 오류검사를 반드시 해 주어야만 한다.

### PropTypes를 활용해 컴포넌트 props 검사

propTypes를 사용해 검사 - npm i prop-types로 설치
propTypes는 전달된 props의 속성을 원하는 type으로 검사하고 맞지 않은 type일때 오류를 발생 시켜 원하는 결과가 출력 되게 설정하는데 도움을 줄 수 있다.

### PropTypes 속성 기본 값 defaultProps 설정

props이 전달 되지 않았을때, 기본값으로 설정을 할 수 있다.

---

## 2주차 화요일 학습

컴포넌트 상태(state) & 라이프 사이클 훅

### 클래스 컴포넌트의 state 란?

- 컴포넌트를 만들때 2가지 방법(함수형, 클래스 컴포넌트)으로 만들 수 있다.
- 함수형 컴포넌트는 props(속성) 설정만 가능하며, 불변(immutable)하다.
- props는 외부에서 전달 되는 data, state는 컴포넌트 자체가 가질 수 있고 변경 가능한 data.
- 클래스 컴포넌트는 state와 lifecycle hook을 가질 수 있고, update를 통해 값을 동적으로 변경 할 수 있다. this도 사용 가능.
- 함수형 컴포넌트는 코드가 간결해서, 상태값을 변경 하지 않는 경우 사용 빈도수가 많다. 반드시 둘 중에 하나를 써야 하는것은 아니고 필요에 따라 사용 하면 됨.
- class field 문법 : constructor(생성자 메서드)를 사용하지 않아도 됨(간결/편함)

### 컴포넌트 라이프 사이클 훅(Life Cycle Hooks) 이란?

- 마운팅
- 업데이팅
- 언마운팅

### 생성 시점의 라이프 사이클 훅

1. 마운팅
   constructor() : 컴포넌트 생성 시점에 호출
   static getDerivedStateFromProps() : 전달된 상태 및 속성을 가져와 설정하는 시점에 호출. 잘 사용은 하지 않지만, props를 받은 시점에 state update가 필요 할때 사용.
   render() : 컴포넌트 렌더링 시점에 호출
   componentDidMount() : DOM에 마운트 된 이후 시점에 호출

   - lifecycle hook에서는 DOM요소에 접근 할 수 없지만,componentDidMount() cycle hook에서는 DOM 접근 가능하고, 그로 인해 side effect 발생 가능(React의 손을 벗어났으니 처리 못함. 관리가 안됨)

2. 업데이팅
   static getDerivedStateFromProps() : 전달된 상태 및 속성을 가져와 설정하는 시점에 호출 (업데이트)
   shouldComponentUpdate() : 컴포넌트 업데이트 예정 시점에 호출 (업데이트 하거나, 안 하거나). 성능 최적화를 위해 사용.
   render() : 컴포넌트 렌더링 (업데이트)
   getSnapshotBeforeUpdate() : 컴포넌트 업데이트 전 스냅샷 가져오는 시점에 호출
   componentDidUpdate() : 컴포넌트 업데이트 이후 시점에 호출

- props, state는 immutable(불변)이다. 수정은 안됨. 'setState'를 통해 '교체만' 가능하다.

### 업데이트, 제거 시점의 라이프 사이클 훅

3. 언마운팅
   componentWillUnmount() : 컴포넌트 제거 예정 시점에 호출

### 오류 발생 시점의 라이프 사이클 훅

4. 오류 처리
   static getDerivedStateFromError() : 자손 컴포넌트 오류 발생 시 호출. 상황에 따라서 state를 false로 정의 해 놓고, 오류 발생시 true로 반환 및 메시지 출력 해줄 수 있음.
   componentDidCatch() : 자손 컴포넌트 오류 발생 시 호출. 오류 위치를 알려주는 메서드.

---
