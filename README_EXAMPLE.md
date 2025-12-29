# 1. Example Project (ver 1.0)

## Project Overview

해당 프로젝트는 클라이언트 측으로 부터 음성 데이터를 실시간으로 처리하고, STT 백엔드 서버로 실시간으로 스트리밍하고, 전사 텍스트를 수신하여 RabbitMQ에 메시지를 발행하는 웹소켓 기반 백엔드 서버입니다. 또한, Auth 서버와 연계하여 인증부분도 담당합니다.

---

## Skills

Framework: Spring Boot(3.5.5), Java(21)

Infrastructure: Redis, RabbitMQ

Deploy: Docker, GithubActions

---

## Person in charge

tim.park

E-mail: tim.park@systrankorea.com

---

## Dependencies

- SI&T: Retriever, Translation Bridge (하이퍼링크 첨부)
- Auth Server (하이퍼링크 첨부)
- STT Server (하이퍼링크 첨부)
- RabbitMQ / Redis

---

# 2. Installation Guide

Local

1. git clone https://github.com/SYSTRAN-KOREA-AI/backend-voice-gateway.git
2. docker compose up -d —build voice-gateway

Server (Github Actions Script)

---

# 3. How to use

클라이언트와 웹소켓 기반 `/ws/connect` 엔드포인트로 연결합니다. 

## API 명세서

- 별도의 문서 링크 첨부 또는 실제 작성 요망

---