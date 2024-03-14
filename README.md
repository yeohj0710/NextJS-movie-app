## NextJS practice

- This is a project for practicing NextJS.

<br>

### Server side rendering

#### NextJS가 application을 render하는 방법

- ① NextJS가 서버(backend)에서 먼저 JavaScript → HTML로 Render 한 다음, 그 HTML을 브라우저에 전달해 준다.
  - HTML이므로, JavaScript가 없어도 Render 된다.
- ② 그 다음 프레임워크가 페이지에 React application을 추가한다.
  - 이 기능은 각 Component 파일 맨 위에 "use client";를 작성해서 선택적으로 추가 가능 (이 Component는 client에서 interactive 해야 함을 의미)
  - 기존 HTML 페이지는 그대로 있는 상태로, 이벤트 리스너 등이 추가된다.
  - 이를 (사용자가 최초 HTML을 본 후) 'Hydration이 일어난다'고 한다.

#### 컴포넌트별로 로딩이 완료되는 대로 렌더링하기

- 리액트의 Suspense 컴포넌트를 이용하여 컴포넌트별로 로딩이 완료되는 대로 렌더링을 할 수 있다.
- 위 프로젝트에서 먼저 로딩된 영화 포스터와 요약은 먼저 렌더링이 되고, 유튜브 트레일러들은 로딩이 완료되는 순서대로 나중에 렌더링이 일어나는 것을 확인할 수 있다.

<br>
