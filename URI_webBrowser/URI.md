# ⏱️URI(Uniform Resource Identifier)

```
URI는 로케이터(locator),이름(name) 또는 둘다 추가로 분류될 수 있다.

URL : resource locator 리소스의 위치

URN : resource name 리소의 이름
```

![](https://velog.velcdn.com/images%2Fjch9537%2Fpost%2F51dcc312-8ecb-4048-80df-cbde40865e7a%2Fimage.png)

</br>
</br>

### URI
단어 뜻

- Uniform : 리소스 식별하는 통일된 방식
- Resource : 자원,URI로 식별할 수 있는 모든 것 (제한 없음)
- Identifier : 다른 항목과 구분하는데 필요한 정보
</br>
</br>
- URL : Uniform Resource Locator
- URN : Uniform Resouce Name
</br>
</br>

### URL,URN
단어 뜻
</br>

- URL - Locator : 리소스가 있는 위치를 지정
- URN - Name : 리소스에 이름을 부여
- 위치는 변할 수 있지만, 이름은 변하지 않는다.
- urn:isbn:8960777331(어떤 책의 isbn URN)
- URN 이름만으로 실제 리소스를 찾을 수 있는 방법이 보편화 되지 않음
- 앞으로 URI를 URL과 같은 의미로 이야기하겠음

</br>
</br>

### URL
scheme

- scheme://[userinfo@]host[:port][/path][?query][#fragment]
- https://www.google.com/search?q=hello&hl=ko
</br>
</br>

![](https://velog.velcdn.com/images%2Fjch9537%2Fpost%2F88b0c8ac-5870-4cbc-b613-7dd39f510f31%2Fimage.png)

- 프로토콜(https)
- 호스트명(www.google.com)
- 포트 번호(443)
- 패스(/search)
- 쿼리 파리미터(q=hello&hI=ko)

userinfo
- URL에 사용자정보를 포함해서 인증
- 거의 사용하지 않음
</br>
</br>

host
- 호스트명
- 도메인명 또는 IP 주소를 직접 사용가능
</br>
</br>

port
- 포트(PORT)
- 접속 포트
- 일반적으로 생략, 생략시 http는 80, https는 443
</br>
</br>

path
- 리소스 경로(path) 계층적 구조
- 예)
  - /home/file1.jpg
  - /members
  - /members/100, /items/iphone12
</br>
</br>

query
- key=value 형태
- ?로 시작, &로 추가 가능 ?keyA=valueA&keyB=valueB
- query parameter, query string 등으로 불림, 웹서버에 제고하는 파라미터, 문자 형태
</br>
</br>
- scheme://[userinfo@]host[:port][/path][?query][#fragment]
- https://docs.spring.io/spring-boot/docs/current/reference/html/gettingstarted.html#getting-started-introducing-spring-boot
- fragment
- html 내부 북마크 등에 사용
- 서버에 전송하는 정보 아님