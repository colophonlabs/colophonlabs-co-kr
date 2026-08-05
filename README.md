# colophonlabs.co.kr (별칭 도메인)

`colophonlabs.co.kr`로 들어온 방문자를 정식 주소 **https://colophonlabs.kr** 로 보내는 저장소.

- 왜 저장소를 따로 두는가: GitHub Pages는 저장소당 사용자 도메인을 **하나만** 서비스한다.
  정식 사이트(`colophonlabs/malssemgil-site`)가 `.kr`을 쓰므로, `.co.kr`은 이 저장소가 받는다.
- 왜 가비아 포워딩을 쓰지 않는가: 포워딩은 가비아 서버가 HTTP로 리다이렉트하는 방식이라
  **`https://colophonlabs.co.kr`에 인증서가 없어 경고가 난다.** 이 방식은 GitHub이 `.co.kr`용
  인증서를 발급하므로 http·https 양쪽이 정상 동작한다.
- 구성: `CNAME`(도메인) + `index.html`·`404.html`(meta refresh, 스크립트 없음).
  `404.html`이 있어 어떤 경로로 들어와도 정식 주소로 넘어간다.
- 내용을 고칠 일은 거의 없다. 정식 주소가 바뀌면 두 HTML의 URL을 함께 바꾼다.
