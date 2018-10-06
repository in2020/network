# network
## port forward
- ssh -N -L port:[remote server ]:[remote port]
- ssh -L 10030:localhost:8180 root@192.168.96.6
  - 이렇게 한 후에 웹 브라우져를 실행하고 주소창에 ‘http://localhost:10030’ 이라고 입력하면 192.168.96.6 서버의 Tomcat 서버 포트인 8180 에 연결되고 톰캣 페이지가 보이게 된다.
- with key file : ssh -N -L port:[remote server]:[remote port] -i [keyfile] [user]@[host]
