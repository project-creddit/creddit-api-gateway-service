# Creddit API Gateway Service

- `Discovery Service`에 등록된 service들에 맞는 API 분기 및 `global filter` 역할을 하는 서비스

## Implementation
- [ ] : AuthorizationHeaderFilter
  - client로부터 오는 요청의 Header를 검사합니다.
    - [ ] : `no authorization header` 검사
    - [ ] : `JWT token is not valid` 검사