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

## 2주차 수요일 학습

1. 이벤트 핸들링

### React 이벤트 핸들링

- 이벤트 속성 이름은 camelCase 형식으로 작성 (예: onClick)
- 속성 값에 문자열 대신 JSX 형식으로 메서드를 연결 (예: onClick={ onClickHandler })
- 브라우저 기본 동작을 중단하려면 반드시 e.preventDefault()를 사용

React가 지원하는 이벤트
https://ko.reactjs.org/docs/events.html#supported-events

- e.target, e.currentTarget을 사용해 해당 대상을 찾을 수 있음.

이벤트를 외부에 분리해서 dataBinding을 통해 연결해 사용하면 재사용성을 높일 수 있다.

### React 이벤트 핸들러와 this

- 함수형 컨포넌트에서는 this를 사용 할 수 없어서 고민 할 이유가 없지만, 클래스 컴포넌트에서는 this를 사용해야 한다.
- class 컨포넌트에서 this를 사용하기 위해서는 constructor에 this를 등록해 주어야 하는데, 매번 등록하면 코드양이 많아지고 복잡해지므로 inline으로 .bind(this)를 붙여 주고 사용 할 수 있다.(예: onclick = {this.handleLinkClick.bind(this)} )
  또는 화살표 함수를 사용 ( onclick={(e) => this.handleLinkClick(e)} )
  또는 class field 문법을 사용한다.

  ```
  handdleLinkClick = (e) => {
    console.log(e.target)
    console.log(this)
    this.otherMemberMethod()
    e.preventDefault()
  }
  render()  {
    <a
      onClick={this.handleLinkClick}
    >
    </a>
  }
  ```

2. 컴포넌트 통신

### React 컴포넌트 간 통신이 필요한 이유

- 클래스 컨포넌트는 컨포넌트 내에서 state를 관리하므로 외부 컨포넌트의 data를 공유하기 위해서는 rule을 지켜서 사용해야만 한다.
- Lefting State Up(부모/자식간 통신) - 상위/하위 일때, 부모가 state를 관리하고 data를 공유/통신

### 부모 컴포넌트와 자식 컴포넌트 사이의 props ⇌ callback

- 부모는 props를 함수로 전달
- 자식은 callback 반환

### 복잡한 컴포넌트 트리 구조에서 props ⇌ callback의 문제

복잡한 컨포넌트 구조에서 props/state의 위치가 부모와 자식의 여러개층을 거칠때 매우 복잡한 과정을 거쳐서 callback을 전달 해줘야만 하는 문제 발생.

### 상태 관리를 효율적으로 관리하기 위한 방법 Context, React Redux

위의 문제를 대안이 context API, React Redux

- Context API는 컨포넌트의 재사용을 할 수 없게 만들기 때문에 되도록 지양하거나 한정적으로 사용 할 것.
- React Redux : 모든 컨포넌트가 접근 가능한 Store라는 저장소를 만들고 dispatch(요청), update 하여 관리 해준다.

---

## 2주차 목요일 학습

컨텍스트(Context) API

### Context의 Provider, Consumer를 사용한 데이터 공유

- 부모에서 가지고 있는 data/state를 통신하기 위해 context 이용.
- 부모에 privider, 자식에 consumer로 설정하여 통신
- contextCreate 생성, value 설정

### Context 모듈을 활용해 개별 컴포넌트에서 데이터 공유

### Context Type 활용

반드시 클래스 컨포넌트를 사용해야만 한다.

---

## 2주차 금요일 학습

React 접근성(A11Y)

### 헤딩 레벨(Heading Level)

tota11y plugin
tenon UI Headings 컴포넌트 - 자동으로 heading level을 설정해줌

### 히든 콘텐츠(Hidden Contents)

임의로 css 속성으로 숨기면 스크린 리더에서 읽을 수가 없음.
.a11y-hidden을 사용 할것.

### 버튼 컴포넌트(Button Component)

button 역할을 하는 것은 div, span, img를 지양하고 button을 사용 할것.
link, button의 역할르 구분.

### 사용에 주의가 필요한 HTML 표준 문법

### 접근성 자동 검사 (React-axe)

### Semantic UI + React 모달 다이얼로그 접근성 개선

semantic UI 작성을 위한 노력은 역시 학습과 반복 연습뿐이군요... ㅠ.,ㅜ

---

## 3주차 월요일 학습

1. 시작하기

### cra-template-ko-craco 커스텀 템플릿을 사용하여 프로젝트 시작하기

```
$ npx create-react-app --template cra-template-ko-craco ediya-ui-practice
$ cd ediya-ui-practice
$ npm start
```

해당 프로젝트 폴더로 이동후 npm start로 local server 구동 할것

2. 문서 헤드 구성

### 환경 변수, 퍼블릭 디렉토리 구성, 검색엔진 최적화, 오픈 그래프 프로토콜 설정

- 환경 변수 파일인 env 이름을 .env로 변경
- index html에 meta data, file path 수정

3. 컴포넌트 디렉토리 구성

### components, api 디렉토리 구성

- src 폴더에 있는 file 교체
- ediya.json file을 api에 넣기

4. 컴포넌트 구성 Part 1

### AppHeader, AppMain, GoToTop 컴포넌트

- AppHeader, AppMain, GoToTop 컴포넌트를 각각 폴더에 js file 생성 및 App.js에서 import 시킴.
- AppHeader, AppMain, GoToTop 컴포넌트에 각각의 SCSS 경로 설정

### JSX 코드 정리

- 압축을 푼 index.html에서 각 영역을 module화 하고, className, viewBox, img tag 닫아주고, 외부링크 걸려 있는 부분 rel="noopener noreferrer" 추가

5. 컴포넌트 구성 Part 2

### AppHomeLink, AppNavigation, BeverageList, BeverageItem 컴포넌트

- 각각 module화, scss 연결, 오류나는 부분 임시 비활성화

### 컴포넌트 스타일 관리

- className 변경/제거

6. 컴포넌트 props 디자인

### AppHomeLink 컴포넌트 props 설계

- 기본 module에 외부에서 속성을 전달 해주려면 전개연산자를 통해 props로 설정해 전달해준다.
- prop-types를 사용해(isRequired) 속성검사
- 객체분해 할당을 통해 기본 속성을 props에 전개연산자로 전달해주고, 표준속성이 아닌 경우는 따로 설정을 해서 전달해준다.

---

## 3주차 화요일 학습

7. 컴포넌트 이벤트 핸들링 & 타임 컨트롤

### AppNavigation 컴포넌트 이벤트 핸들링, 타임 컨트롤

- menu가 상태값을 가져야만 하므로 React pure to class를 사용해 '클래스 함수'로 변경
- class, hidden의 시간차를 두어 변경해주어야 animation 적용 할 수 있음
- menu를 닫을때는 열때와는 반대로 class를 먼저 제거하고 hidden을 추가해줘야 animation이 보여짐
- 상태 업데이트는 setState()를 사용

8. 리스트 렌더링 & 컨텍스트 Part 1

### Context API → AppNavigation 리스트 렌더링

- context Provider로 json data를 상속 받아 conponent에서 사용 할 수 있게 설정
- list에 item을 순환하여 data를 뿌려줄때는 map()을 사용하고, key값을 고유하게 설정
- button conponent를 만들어 재사용하고 내부적으로는 children을 전달하게 구성하여 각각 용도에 맞게 커스텀

9. 컴포넌트 접근성 개선

### 키보드 접근성 (ref, forwardRef, shouldComponentUpdate) 설정

- 키보드 tab을 눌러 포커스가 순환 할때 제대로 작동하도록 설정
- 메뉴의 기준점을 잡기 위해 메뉴의 첫번째 tab을 잡아줌
- shift + tab 동작 추가
- esc 동작 추가
- conponentDidMount(), shouldComponentUpdate()를 사용

### 컴포넌트 참조 전달(forwardRef)과 개발 도구에서 이름 표시 설정

- forwardRef를 사용 할때, 익명으로 표기 되는데 명칭을 표시하려면 '함수선언'을 사용하거나 displayName을 설정

---

## 3주차 수요일 학습

React 훅(Hook)

### useState() 훅을 활용한 상태 관리

- hook을 사용 할때는 반드시 '함수형 컨포넌트' 안에서만 사용하고, 컨포넌트 안의 반복문/조건문/중첩된 함수 안에는 hook을 사용 할 수 없다

### React 클래스 컴포넌트 → 함수형 컴포넌트로 전환 (상태 관리)

- 상태와 상태변화값을 배열로 설정하여 사용

### useEffect() 훅을 활용한 사이드 이펙트 처리

- 메모리 관리를 효율적으로 제어하기 위해서는 특정한 데이터의 상태 데이터를 지정한다

### useRef() 훅을 활용한 DOM 노드 접근/조작

- react에서 상태관리가 되는게 아니기 때문에 sideEffect가 있을 수 있다.
- 상태관리를 위해서는 useState()를 사용하길 권장

### useContext() 훅을 활용한 데이터 공유

10. 리스트 렌더링 & 컨텍스트 Part 2

### BeverageList 컴포넌트 리스트 렌더링 + Context API

- 함수형, 클래스형 conponent에서 context를 처리하는 방법 비교

### BeverageItem 다이얼로그 인터랙션

- class의 state, useState()를 사용하여 conponent 작성 해봄

11. 페이지 상단 스크롤 이동

### GoToTop 페이지 상단 이동 인터랙션

### React 훅(useState, useEffect) 활용

---

## 3주차 목요일 학습

고차 컴포넌트(HOC, Higher-Order Component)

### 고차 함수(HOF)란?

- 함수는 return 값으로 함수를 사용 할 수 있는데, 함수 안에 함수를 사용하는 경우를 고차함수라 한다.

### 고차 컴포넌트(HOC)란?

- 컴포넌트에서 다른 컨포넌트를 불러와 새로운 컨포넌트를 만들어진 것

### 사용자 정의 고차 컴포넌트

- contextType을 생략 할 수 있고, 코드량을 줄일 수 있다.

Styled Component I

### 스타일 라이브러리

- css를 javascript(react)에서 사용 하는 형식으로 자동변경
- 고유한 class 속성 설정
- 컨포넌트에서 css 관리
- 간편한 동적 스타일링
- 벤더 프리픽스 자동설정

### Styled Components 기본 사용법

### Styled Components의 작동 원리 (ES6 태그 템플릿)

### props 적용

- \${{XXX} => props.XXX || null}를 사용하여 속성을 전달하고 조건문에 따라 속성을 변경 할 수 있다.
- 객체구조분해 할당을 사용하면 코드를 줄일 수 있다.

---

## 3주차 금요일 학습

React 폼 컨트롤

### HTML VS React 폼 컨트롤

- 클래스 컨포넌트로 만들어 상태값을 가져야하고, 상태를 바꿔 줄 수 있는 이벤트와 핸들러가 상태값을 변경하고 value값을 설정할 수 있어야한다.

### AppInput 컴포넌트

- propsType으로 필수값 설정, 상태값, 이벤트, 기본값과 상황에 따른 값을 설정 할 수 있게 veriation 설정을 해준다.

### React 폼 멀티플 컨트롤 핸들링

### 컨트롤 vs 언 컨트롤 컴포넌트, ref 속성

### React Context를 사용한 데이터 수정 코드 리뷰

---

## 4주차 화요일 학습

React Router 라이브러리 Part 1.

### SPA 라이브러리

서버에 요청되어 렌더링 된 페이지가 하나이며, 다른 페이지로 이동을 하여도 서버에서 새로운 data를 보내지 않아도 아래 조건을 충족하면서 페이지가 표현 되어야 한다.

- 웹 브라우저 주소 창 URL은 변경된 페이지를 식별하는 주소로 변경되어야 합니다. (예: /, /react, /react/props.html)
- 웹 브라우저의 이전/다음 버튼을 눌렀을 때 페이지가 변경되도록 히스토리 기능이 요구됩니다. (예: ← 이전, → 다음)
- 직접 URL을 웹 브라우저 주소 창에 입력했을 때 해당 화면이 그려져야 합니다. (예: /react/props.html#props-검사)

### 라우터? 라우트? 라우팅?

라우터 : 길을 찾게 해주는 역할
라우트 : 길
라우팅 : 길을 찾는 행위

React Router : URL/Path 분석 -> 설정(config) 읽기 -> 컴포넌트 렌더

### BrowserRouter & HashRouter 컴포넌트

BrowserRouter - URL에 표기 되는 pathname값 설정
HashRouter - URL pathname값을 hash로 표기(#)
option을 주어 pathname값 뒤 슬래시를 변경 해줄 수 있다.
alias에서 as를 사용하여, BrowserRouter/HashRouter를 대체하여 코드사용 할 수 있다.

### Route 컴포넌트 Part 1

- route 컴포넌트는 설정된 path와 매칭되는 컴포넌트를 찾아 UI에 렌더링을 한다.
- component, render, chilren을 사용하여 router 컴포넌트를 렌더링
- exact를 사용하여 정확히 match 된 컴포넌트만 렌더링

### Route 컴포넌트 Part 2

- router 컴포넌트의 props : match, location, history

strict - pathname이 완벽하게 같을때만 렌더링
senstive - pathname의 대소문자 구분하여 렌더링

---

## 4주차 수요일 학습

React Router 라이브러리 Part 2.

### Switch 컴포넌트

- Switch 컴포넌트는 포함하는 <Route>나 <Redirect>중에 URL이 매칭 되는 rounte 한개를 렌더링
- 원하는 Router만을 렌더링하기 위해서 Switch를 사용하여 정확한 URL을 구분하여 처리하도록 해준다.

### Link 컴포넌트

- 기존의 a요소를 사용하지 않고, link 컴포넌트와 to를 사용하면 서버요청 없이 SPA로 페이지를 연결하여 렌더링 할 수 있다.
- to를 객체로 설정하여 값/함수를 전달 할 수 있다.
- props 설정을 사용해 title, id, class, innerRef 등의 속성을 전달 할 수 있다.

### NavLink 컴포넌트

- 특별히 nav에 사용하여 class에 active를 부여하여 활성화된 페이지와 나머지 link의 구분을 할 수 있게 한다.
- activeClassName을 사용하여 active 되는 link에 class를 임의로 설정 할 수있다.
- activeStyle을 사용해 active 된 link에 style을 설정 할 수 있다.
- isActive={func}를 사용해 함수 동작 설정
- aria-current : page, step, location, date, time, true 설정은 link가 어떤 목적으로 사용되는지 알려주는 목적의 설정

### Redirect 컴포넌트

- to를 사용해 redirect 되는 페이지를 설정 할 수 있다.
- from to를 사용해 redirect 설정 가능.

### Route 컴포넌트 props 전달

- props를 전달 할때는 render를 사용해 전달하고 전개연산자(...)로 속성값을 함께 전달한다.

### Route 컴포넌트 매개변수(옵션 포함), 쿼리 스트링

- 맵개변수를 전달 해주고, 전달 받은 매개변수를 호출해 사용 할 수 있다.
- 매개변수 뒤에 '?'를 사용하여 매개변수를 사용하지 않았을때도 잘 표현되게 설정
- npm i query-string

---

## 4주차 목요일 학습

␥ React Router 라이브러리 Part 3.

### 중첩된 라우팅

- React Component : this.props.match
- React Render : ({match}) => ()
- React children : ({match}) => ()
- withRouter : this.props.match
- matchPath : 반환값(return value)

- nav 안에서 중첩된 카테고리를 표현하기 위해 match를 사용해 표현

### 보호된 라우팅

- 관리자 페이지/특정 페이지에 접근 관리하기 위해 protected rounter를 사용
- protectedRounter와 redirect를 사용해 페이지 접속 인증을 확인하고, 조건이 충족되지 않으면 원하는 페이지로 redirected 시킨다.

### Redux 통합

- React Router와 Redux를 통합하여 사용하기 위해 widRouter HOC를 사용
