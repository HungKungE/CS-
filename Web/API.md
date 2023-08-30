## API (Application Programming Interface)

1. 설명
한 프로그램에서 다른 프로그램으로 데이터를 주고 받기 위한 방법

2. 종류

1) public API
누구나 사용가능한 공개 API

2) private API
운영자만 사용하는 API

3) partner API
미리 정한 사람만 쓸 수 있는 API

3. REST API

1) 설명
REST를 기반으로 만들어진 API

2) REST (Representational State Transfer)
자원을 이름으로 구분하여 해당 자원의 상태를 주고받는 모든 것

> 특징

- HTTP URI을 통해 자원을 명시함.
- HTTP Method(POST, GET, PUT, DELETE 등)를 통해
  해당 자원에 대해서 CRUD 요청.

> 구성 요소
- 자원 : Url
- 행위 : Method
- 행위 내용 : HTTP Message Pay Load

> 장점
- HTTP 프로토콜의 인프라를 그대로 사용
- HTTP 표준 프로토콜에 따르는 모든 플랫폼에서 사용이 가능
- 의도하는 바를 쉽게 파악

> 단점
- 구형 브라우저에서 호환이 되지 않아 지원해주지 못하는 동작이 많다

3) CRUD
- Create(생성)
- Read(읽기)
- Update(갱신)
- Delete(삭제)

4) 규칙

- Url
```sh
// 동사 x -> 명사
http://school.com/student/name (o)
http://school.com/get/name (x)

// 대문자 x -> 소문자
http://school.com/student (o)
http://school.com/Student (x)

// 마지막에 '/' 넣지 않기
http://school.com/student (o)
http://school.com/student/ (x)


// 언더바(_) 대신 하이폰(-)을 사용
http://school.com/math-class (o)
http://school.com/math_class (x)

// 파일확장자는 URI에 포함하지 않음.
http://school.com/image (o)
http://school.com/image.png (x)

// 행위를 포함하지 않음.
http://school.com/lunch/1 (o)
http://school.com/eat-lunch/1 (x)
```

