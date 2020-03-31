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
