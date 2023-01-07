# PUT

```
PUT /members/100 HTTP/1.1
Content-Type: application/json
{
 "username": "hello",
 "age": 20
}
```

- **리소스를 대체**
  - 리소스가 있으면 대체
  - 리소스가 없으면 생성
  - 쉽게 이야기해서 덮어버림
- **중요! 클라이언트가 리소스를 식별**
  - 클라이언트가 리소스 위치를 알고 URI 지정
  - PSOT와 차이점
