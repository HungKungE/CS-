## HTTP Status 

1. 200번대 : 통신 성공

|코드|이름|의미|
|-----|-----|
|200|OK|요청 성공(Get)|
|201|Crate|생성 성공(Post)|
|202|Accepted|요청 접수O, 리소스 처리X|
|204|No Contents|요청 성공O, 내용 없음|

2. 400번대 : 클라이언트 오류

|코드|이름|의미|
|-----|-----|
|400|Bad Request|잘못된 API사용|
|401|Unauthorized|인증 오류|
|403|Forbidden|권한 밖의 접근 시도|
|404|Not Found|요청 URI에 대한 리소스 존재X|
|405|Method Not Allowed|API에서 정의되지 않은 메소드 호출|
|408|Request Timeout|요청 대기 시간 초과|

3. 500번대 : 서버 오류

|코드|이름|의미|
|-----|-----|
|500|Internal Server Error|서버 내부 오류|
|502|Bad Gateway|게이트웨이 오류|
|503|Service Unavailable|서비스 이용 불가|
|504|Gateway Timeout|게이트웨이 시간 초과|
|505|HTTP Version Not Supported|요청에 사용한 HTTP 버전을 서버가 지원하지 않음|