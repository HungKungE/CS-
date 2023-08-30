## CORS

1. 설명
 웹 브라우저에서 동일 출처 이외의 다른 출처(origin)로부터
 </br>
 리소스에 접근하는 것을 제한하는 보안 메커니즘.

2. 예시
"www.my_develop.com"에서 Goolge 지도 API 데이터를 얻으려 함.
 </br>
지도 API는 "https://maps.googleapis.com"에서 호스팅 됨.
 </br>
따라서 출처가 다르므로 XMLHttpRequest를 차단함,


2. 해결법
헤더의 Access-Control-Allow-Origin : www.my_develop.com을 추가.