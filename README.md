# :확성기: NewsTickr - 증권 뉴스 요약 및 분석 서비스
![Java](https://img.shields.io/badge/Java-17-blue?style=flat-square)
![SpringBoot](https://img.shields.io/badge/Spring%20Boot-3.4.3-green?style=flat-square)
![Docker](https://img.shields.io/badge/Docker-20.10.23-blue?style=flat-square)
![MySQL](https://img.shields.io/badge/MySQL-8.0.41-blue?style=flat-square)
![Eureka](https://img.shields.io/badge/Eureka-Netflix-orange?style=flat-square)
**NewsTickr**는 증권 관련 뉴스 기사를 수집하고, OpenAI API를 이용하여 뉴스 요약 및 감정 분석을 제공하는 서비스입니다.
사용자는 **뉴스 요약을 보고 의견을 남기고, 뉴스의 감정 분석 결과**를 확인할 수 있습니다.
<br>
## :압정: :번쩍: 빠른 시작 (Quick Start)
### :흰색_확인_표시: :일: 프로젝트 클론
```bash
git clone https://github.com/LG-CNS-AM-Inspire-Camp-1-8/Be.git
cd Be
```
### :흰색_확인_표시: :둘: Docker Compose 실행
Docker가 설치되어 있어야 합니다.
모든 서비스를 한 번에 실행하려면 다음 명령어를 실행하세요.
```bash
docker-compose up -d
```
이 명령어를 실행하면 다음 서비스가 자동으로 실행됩니다.
- Config Server (localhost:8888)
- Eureka Server (localhost:8761)
- API Gateway (localhost:8081)
- News Service (localhost:8085)
## :압정: :망치와_렌치: 개발 환경
### :작은_파란색_다이아몬드: 백엔드
- Java 17
- Spring Boot 3.4.3
- Spring Cloud (Eureka, Config Server, Gateway)
- Spring Data JPA & Hibernate
- Groq API (뉴스 감정 분석)
### :작은_파란색_다이아몬드: 데이터베이스
- MySQL 8.0.41
### :작은_파란색_다이아몬드: 배포 및 운영
- Docker & Docker Compose
- Spring Cloud Config
- Spring Cloud Gateway
- Netflix Eureka (서비스 디스커버리)
<br>
## :압정: :전구: 주요 기능
1. ### :로켓: 1. 증권 뉴스 조회 및 요약
   - 네이버 API를 통해 최신 증권 관련 뉴스를 가져옵니다.
   - 네이버 API를 활용하여 뉴스 요약본을 가져옵니다.
2. ### :뇌: 2. 감정 분석 제공
   - Groq API를 활용하여 뉴스의 감정을 분석하고 결과를 반환합니다.
   - 감정 분석 결과를 기반으로 뉴스 분위기를 예측합니다.
3. ### :말풍선: 3. 사용자 게시글 기능
   - 뉴스 기사별 사용자 게시글 및 댓글을 작성하고 관리하는 기능을 제공합니다.
   - Spring Security를 활용한 JWT 기반 인증 시스템을 사용합니다.
