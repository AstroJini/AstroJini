<div align="center">

# 윤세진 | Backend Developer

복잡한 서비스 흐름을 안정적인 API와 데이터 구조로 옮기고, 운영 중 발견한 문제를 끝까지 추적합니다.

[이력서](https://www.figma.com/design/Vn2sDRJ7DA61iHEFLxnkYZ/%EC%9D%B4%EB%A0%A5%EC%84%9C) · [이메일](mailto:pentum99@gmail.com)

</div>

## About Me

- 2025년 12월부터 **에듀템 개발팀**에서 결제·인증·학습·음성 서비스의 백엔드를 개발하고 있습니다.
- 모의 증권 거래 플랫폼 **MKX**에서 Kafka 체결 이벤트, Redis 기반 호가창, InfluxDB OHLCV 차트와 보조지표를 구현했습니다.
- 문제를 재현하고 데이터 흐름을 확인한 뒤, 변경 전후를 측정하며 개선하는 방식을 선호합니다.

## Experience

### 에듀템 | 개발팀 · 사원 (2025.12.15 – 현재)

- **결제·인증:** 아이캔톡 학습 플랫폼에서 KONA 지역화폐·Toss 결제와 공무원증·LDAP·MFA 인증을 연동했습니다.
- **결제 조회 개선:** 분산된 결제 내역의 공통 정보를 `purchase_unified` 테이블로 모으고, 상세 정보는 요청 시 조회하도록 분리했습니다. 조회 응답 시간(99% 기준)을 **209ms → 173ms(17.2% 단축)**로 개선했습니다.
- **교육 서비스:** EBS 수학 진단 LMS의 교사 대시보드·결손 개념 분석, 예문사 LMS의 조직별 권한·학습 통계 등을 구현했습니다.
- **음성·데이터 처리:** STT/TTS API와 HTTP 연결 문제를 개선하고, ThinkingData 이벤트의 큐잉·배치 전송 및 학습 사용량 집계 흐름을 정비했습니다.

### MKX 디지털 증권 거래 플랫폼 | 한화 BEYOND 16기 팀 프로젝트

> [백엔드 저장소](https://github.com/beyond-sw-camp/be16-fin-3team-NylonMusk-BE)

- Kafka 체결 이벤트를 받아 시계열 데이터로 집계하고, **InfluxDB 기반 OHLCV 차트와 보조지표 30종**을 구현했습니다.
- **Redis 정렬 집합(ZSET)과 Lua 스크립트**로 가격·시간 우선순위, 부분 체결 잔량, 호가 총량을 처리했습니다.
- 진행 중인 캔들은 Redis에서 갱신하고, 구간 종료 후에는 체결 데이터를 기준으로 값을 다시 계산해 빠른 화면 반영과 데이터 정확성을 함께 고려했습니다.
- WebSocket/STOMP로 실시간 마켓데이터를 전달했습니다.

## Technical Stack

| 영역 | 사용 기술 |
| --- | --- |
| Backend | Java 17, Spring Boot 3, Spring MVC, Spring Security, eGovFrame 5.0 |
| Data | MyBatis, JPA/Hibernate, MySQL, MariaDB, Redis, InfluxDB |
| Messaging & Integration | Kafka, WebSocket, STOMP, Redis Pub/Sub, Lua, OAuth2/OIDC, JWT |
| Cloud & Tools | AWS S3, CloudFront, Docker, Kubernetes, GitHub Actions, Gradle, Maven, Log4j2 |

## Background

- 고려사이버대학교 컴퓨터공학과 재학 (2026.08 – 현재)
- 유한대학교 글로벌 비즈니스 경영학과 일본어전공 졸업
- 한화 BEYOND 16기 수료 · 프로젝트 1위
- 부루벨코리아 FENDI BTQ Sales Associate (2023.06 – 2025.01)

## Contact

- Email: [pentum99@gmail.com](mailto:pentum99@gmail.com)
- GitHub: [AstroJini](https://github.com/AstroJini)
