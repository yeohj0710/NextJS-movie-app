## NextJS practice

- This is a project for practicing NextJS.

<br>

### Client side rendering

#### 사용자 브라우저에서 모든 UI를 구현

- UI를 보려면 JavaScript가 반드시 필요 (모든 파일을 다운로드할 때까지 기다려야 함)

### Server side rendering

#### NextJS가 application을 render하는 방법

- ① NextJS가 서버(backend)에서 먼저 JavaScript → HTML로 Render 한 다음, 그 HTML을 브라우저에 전달해 준다.
  - HTML이므로, JavaScript가 없어도 Render 된다.
- ② 그 다음 프레임워크가 페이지에 React application을 추가한다.
  - 이 기능은 각 Component 파일 맨 위에 "use client";를 작성해서 선택적으로 추가 가능 (이 Component는 client에서 interactive 해야 함을 의미)
  - 이를 (사용자가 최초 HTML을 본 후) 'Hydration이 일어난다'고 한다.
