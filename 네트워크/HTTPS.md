1. HTTPS 접근 과정

1) 인증서 발급

- Jogiyo Server에서 공개키:Jo-Key를 생성함.

- 믿을 수 있는 CA 기업에 "Jo-key"와 "암호화 방법"을 보냄.

- CA 기업에서는 이를 통해 인증서를 만들고, CA 기업의 개인키로 암호화함.

- 암호화된 인증서를 Jogiyo에 제공.

2) 클라이언트 & 서버

- 클라이언트가 사이트에 들어옴 ( 요청 보냄 )

- 서버에서 받은 요청이 Jo-key로 암호화 된것이 아니면 암호화된 인증서를 클라이언트한테 줌.

- CA 기업 개인키는 브라우저가 알고 있음 -> 복호화한 인증서를 얻게 됨.

- 브라우저가 난수를 통해서 대칭키(pre-master-key)를 생성.

- Jogiyo에 요청 보낼 때, 이 대칭키를 Jo-key로 암호화함.

- Jogiyo에서 암호화된 요청을 비밀키로 복호화함.

- 클라이언트와 동일한 대칭키를 알게됨.

- 이제 서로 대칭키를 통해서 암호화-복호화하며 통신함.