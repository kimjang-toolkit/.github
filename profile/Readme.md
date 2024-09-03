# Kimjang-toolkit

## 소개

`두고 두고 묵혀 먹는 기술 모음집` <br/>
필요한 기술을 적재적소에 빠르게 재사용하기 위해 개발

웹 소캣을 이용해서 채팅방을 초대, 구독, 메시지 발송 기능을 구현. <br/>
추후 AI와 함께하는 실시간 영어 말하기 연습 애플리케이션을 구현할 수 있는 토대를 닦았다.

## 주요 난관

**Frontend**
  - 채팅방 `초대`를 위한 Stomp Connection을 유지하면서 라우팅하는 기능
    - 하나의 Stomp Connection을 통해 채팅방과 초대 토픽을 구독
    - 여러 페이지를 돌아다녀도 `초대` 토픽 구독을 잃지 않도록 유지

**Backend**
  -  유저가 채팅방 구독해제 시각을 확인하는 기능
     -  구독해제 시각을 통해 안 읽은 메시지 개수나 채팅방을 들어갔을 때 화면 위치를 결정


개발 기록이 궁금하시다면 
- https://kimjang-wiki.vercel.app/
- https://ohsol-blog.vercel.app/blog/project/refresh-store

## 사용 기술

- **실시간 메시지 pub/sub**  :  Websocket
- **유저 인증 정보 저장**     :  JWT & Refresh token
- **배포**                 :  AWS EC2, Cloudfront


