---
title: "법원경매정보 API 만들기 (1)"
description: "전체적인 설계 구조 잡기"
pubDate: 2025-08-23
tags: ["법원경매정보 API"]
---

### 1. 전체 아키텍처 개요

```
[User] → [Gin API Server] → [Redis/RabbitMQ 큐] → [Colly Worker Pool] → [DB 저장] → [API 응답]
```

- Gin API Server: 사용자 요청 처리 (예: "서울중앙지법 사건 목록 주세요")
- Redis/RabbitMQ: 크롤링 작업 분배 (큐 기반 비동기 처리)
- Colly Worker: 큐에서 작업 꺼내서 크롤링, 데이터 수집 후 DB에 저장
- DB (PostgreSQL/MySQL/ElasticSearch): 구조화된 데이터 저장
- Docker + K8s: 서비스와 워커를 각각 컨테이너화하고 오케스트레이션
- 스케줄러 (CronJob/K8s Job): 정기 크롤링 실행
