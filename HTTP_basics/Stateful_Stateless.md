# 무상태 프로토콜
#### 스테이스리스(Stateless)
- 서버가 클라이언트의 상태를 보존X
- 장점 : 서버 확장성 높음(스케일 아웃)
- 단점 : 클라이언트가 추가 데이터 전송

### Stateless
##### 실무 한계
- 모든 것을 무상태로 설계 할 수 있는 경우도 있고 없는 경우도 있다.
- 무상태
  - 예) 로그인이 필요 없는 단순한 서비스 소개 화면
- 상태 유지
  - 예) 로그인
- 로그인한 사용자의 경우 로그인 했다는 상태를 서버에 유지
- 일반적으로 브라우저 쿠키와 서버 세션등을 사용해서 상태 유지
- 상태 유지는 최소한만 사용

```
Stateless란?
● stateless : server side에 client와 server의 동작, 상태정보를 저장하지 않는 형태, server의
 응답이 client와의 세션 상태와 독립적임

장점 : 서버가 client정보를 저장관리 하지 않으므로 Scaling이
자유로움
```
### Stateful
- stateful : server side에 client와 server의 동작, 상태정보를 저장하는 형태  세션 상태에 기반하여 server의 응답이 달라짐
- 장점 : 서버는 클라이언트의 세션 정보를 저장하므로, 갑자기 통신이 중단되더라도 중단된 곳부터 다시 시작할 수 있습니다.
- 단점
  - 확장성이 좋지 않습니다.
    - 클라이언트의 세션 정보가 새로 scale out 된 서버에 저장 되어 있지 않습니다.
    - 따라서, scale out 시, 클라이언트의 세션 정보를 새로운 서버에 옮겨주는 등의 부수적인 관리가 요구되므로, 확장성이 좋지 않습니다.