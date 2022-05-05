# Creddit API Gateway Service

- `Discovery Service`에 등록된 service들에 맞는 API 분기 및 `global filter` 역할을 하는 서비스

## Implementation
- [x] : AuthorizationHeaderFilter
  - `client`로부터 오는 요청의 Header를 검사합니다.
    - [x] : `no authorization header` 검사
    - [x] : `JWT token is not valid` 검사
      - [x] : 잘못된 JWT 서명
      - [x] : 만료된 JWT
      - [x] : 지원되지 않는 JWT
      - [x] : JWT 토큰 형식
- [x] : Trace Interface
  - 로깅용 interface 입니다.