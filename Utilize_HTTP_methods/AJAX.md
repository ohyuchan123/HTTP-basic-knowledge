# AJAX란 무엇인가?
### AJAX(Asynchronous Javascript And XML)
</br>

### 정의
- Asynchronous Javascript And Xml(비동기식 자바스크립트와 xml)의 약자
- 브라우저가 가지고있는  XMLHttpRequest 객체를 이용해서 전체 페이지 일부만을 위한 데이터를 로드하는 기법

즉, 쉽게 말하자면 자바스크립트를 통해서 서버에 데이터를 비동기식 방식으로 요청하는 것이다.
</br>

### 비동기식 방식이란?
비동기 방식은 웹페이지를 리로드하지 않고 데이터를 불러오는 방식이며 Ajax를 통해서 서버에</br>
요청을 한 후 멈추어 있는 것이 아니라 그 프로그램은 계속 돌아간다는 의미를 내포하고 있다.
![](https://velog.velcdn.com/post-images%2Fsurim014%2F233bbf90-2d60-11ea-a24d-4f910e80580b%2Fimage.png)


### 비동기 방식의 장점
페이지 리로드의 경우 전체 리소스를 다시 불러와야하는데 이미지, 스크립트 , 기타 코드등을</br>
모두 재요청할 경우 불필요한 리소스 낭비가 발생하게 되지만 비동기식 방식을 이용할 경우</br>
필요한 부분만 불러와 사용할 수 있으므로 매우 큰 장점이 있다.