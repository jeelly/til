# 라우터(Router)
 

> 리액트 라우터(React Router)

- 사용자가 입력한 주소를 감지하는 역할을 하며, 여러 환경에서 동작할 수 있도록 여러 종유의 라우터 컴포넌트를 제공한다.
- 이중 가장 많이 사용하는 라우터 컴포넌트는 BrowserRouter와 HashRouter이다.

> 라우팅이란?

- 간단하게 생각 하자면 사용자가 요청한 URL에 따라 해당 URL에 맞는 페이지를 보여주는 것이라고 생각할 수 있다.
- 리액트에서는 라우팅 관련 라이브러리가 많이 있는데, 이중 가장 많이 쓰이는 리액트 라우터(React Router)를 사용해보려 한다.

> Router v5 -> Router v6 바뀐점

- Router useNavigate로 잘못된 주소 처리하기
- Router useHistory대신 useNavigate
- Router Swith 대신 Routes