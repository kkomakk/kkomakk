# 🐍 Github Profile

![snake gif](https://github.com/Platane/snk/raw/output/github-contribution-grid-snake.svg)

<h1 align="center">안녕하세요, 정직한 숫자로 가치를 증명하는 백엔드 개발자 이지수입니다 👋</h1>
<h3 align="center">복잡한 비즈니스 로직을 견고한 데이터 아키텍처로 변환하며, 아키텍처 최적화와 정합성 검증을 집요하게 반복합니다.</h3>

<p align="center">
  <!-- Backend & Language -->
  <img src="https://img.shields.io/badge/Java-007396?style=flat-square&logo=openjdk&logoColor=white"/>
  <img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white"/>
  <img src="https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=node.dot.js&logoColor=white"/>
  <!-- Frontend -->
  <img src="https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black"/>
  <img src="https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white"/>
  <img src="https://img.shields.io/badge/Tailwind%20CSS-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white"/>
  <!-- Database & Infra -->
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white"/>
  <img src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white"/>
  <img src="https://img.shields.io/badge/Apache%20Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white"/>
  <img src="https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white"/>
</p>

---

### 💻 Core Engineering Capabilities

* **Data Integrity & Architecture**: 도메인 요구사항 분석 기반 정교한 **ERD 설계**, 분산 환경에서의 데이터 무결성을 보장하기 위한 트랜잭션 격리 및 락(Lock) 정책 수립
* **Performance Optimization**: 인프라 최전방 캐싱 레이어 설계, 데이터베이스 **실행 계획(EXPLAIN) 분석 및 복합 인덱스 튜닝**을 통한 병목 해소
* **Asynchronous & Distributed Processing**: 메시지 큐 기반 비동기 스로틀링 파이프라인 제어 및 분산 인메모리 카운팅 아키텍처 레이어 설계
* **Technical PM/PL Coordination**: 주도적인 크로스팀 기술 조율, Git-Flow 브랜치 전략 및 코드 리뷰 컨벤션 확립으로 팀 내 개발 생산성 개선

---

### 🚀 Main Projects

#### 📍 PROJECT 1. D-TO (웹 접근성 준수 쇼핑몰 플랫폼) | 종합 기여도 50%+
* **Description**: 시각·청각·고령 유저를 위한 접근성 가이드라인을 준수하면서 분산 환경의 가용성을 극대화한 커머스 플랫폼
* **Key Achievements**:
    * **인메모리 캐싱 레이어**: 상시 노출되는 실시간 접속자 집계 기능을 **Redis Hash 구조** 기반으로 구축하여 RDB 디스크 I/O 병목 완전 차단
    * **생명주기 및 어뷰징 제어**: 탈퇴 후 중복 혜택 수령을 제한하기 위해 **Soft Delete(상태 Enum 및 deletedAt)**와 `OAuth2SuccessHandler` 내부 차단 로직을 결합한 **30일 쿨링오프** 메커니즘 전면 적용
    * **분산 인증 보안 아키텍처**: 7일 TTL 기반의 JWT 리프레시 토큰 레이어 및 로그아웃 요청 토큰을 2시간 동안 분산 캐시에 적재하는 **withdrawn 블랙리스트** 프로세스 설계
    * **품질 지표 달성**: 크롬 Lighthouse Audit 기준 웹 접근성 **100점 만점 스코어** 달성 및 아키텍처 설계 총괄

#### 📍 PROJECT 2. Drawing i (AI 기반 미술심리검사 보조 EMR 시스템) | 종합 기여도 30%
* **Description**: 아동의 그림 검사 과정을 정량화하고 상담사의 EMR 작성을 자동 보조하는 의료 비즈니스 인프라 플랫폼
* **Key Achievements**:
    * **하이브리드 데이터 모델링**: 구조화된 메타데이터는 **MySQL**에, 대용량 비정형 드로잉 획(Stroke) 데이터는 NoSQL인 **MongoDB(운영 단계 Amazon DocumentDB)**에 분리 적재하여 저장소 디스크 병목 리스크 해소
    * **비정형 데이터 압축 파이프라인**: 유클리드 거리 계산 알고리즘을 이식한 데이터 전처리 레이어를 상류(Upstream)에 구현하여 외부 OpenAI API 전송 데이터 가공 및 **토큰 비용 30% 절감**
    * **비동기 격리 파이프라인**: 무거운 AI 리포트 연산 로직을 **Spring `@Async` 비동기 파이프라인**으로 격리하여 WAS 메인 비즈니스 스레드 고갈 및 장애 전파 원천 차단 (리포트 생성 속도 **40% 단축**)

#### 📍 PROJECT 3. E.Go (선착순 예약 매니징 시스템) | 백엔드 코어 구현 60%+
* **Description**: 대규모 트래픽 집중 시 데이터 정합성을 완벽하게 보장하는 분산 선착순 예약 제어 시스템
* **Key Achievements**:
    * **비동기 대기열 버퍼 아키텍처**: 최전방에 **Apache Kafka**를 도입하여 대규모 진입 요청을 선적재하고, DB 가용량에 맞춘 순차 쓰로틀링(Consumer) 처리로 대기열 지연율 및 초과 예약률 **0% 보장**
    * **분산 환경 동시성 제어**: 다수 유저의 동일 자원 접근 시 발생하는 Race Condition을 방어하기 위해 **Redis Redisson tryLock** 기반의 분산 락 레이어를 구축하여 중복 예약 결함 제로화
    * **데이터 유실 방지**: `@SQLDelete` 및 `@Where` 애노테이션 기반의 **Soft Delete 전략**을 전면 적용하여 물리 삭제로 인한 원장 유실을 막고 통계 분석을 위한 전체 데이터 라이프사이클 이력 유실률 **0% 달성**

#### 📍 PROJECT 4. StudySpot (지도 기반 장소 추천 서비스) | 종합 기여도 80%+
* **Description**: 다차원 검색 필터링 및 캐시 장애 우회 가용성을 갖춘 위치 기반 개인화 서비스
* **Key Achievements**:
    * **데이터베이스 튜닝**: 다중 조건 검색 시 발생하는 Full Scan 병목을 제거하기 위해 **MySQL EXPLAIN 실행 계획 분석**을 수행, 카디널리티 기반 **복합 인덱스 설계**로 장소 검색 API 속도 **76% 단축** ($2.5s \rightarrow 0.6s$)
    * **회복 탄력성(SLA) 확보**: 외부 지도 API 타임아웃 마비 시 시스템 장애 전파를 해소하고자 원격 서버 분리 및 **Redis 캐시 기반 Fallback 아키텍처**를 구축하여 서비스 무중단 환경 구현
    * **타입 안정성 보장**: **QueryDSL BooleanExpression** 동적 쿼리 모듈화를 도입하여 컴파일 시점 쿼리 검증 환경 내재화 (런타임 에러 **0%**)

---

### 🏆 Leadership & Awards

* **국민대학교 KCC 컴퓨터 학술 동아리 회장** (2024.12 - 2025.07)
    * 150명 규모 IT 조직 총괄 운영, 기술 스터디 커리큘럼 설계 및 Git-Flow 브랜치 전략·코드 컨벤션 전파로 팀 협업 생산성 **30% 향상**
    * 수기 피드백 병목을 자동화 피드백 시스템 인프라 구축으로 해결
* **국민대학교 캡스톤디자인 경진대회 장려상 & 인기상 동시 수상** (Drawing i 프로젝트)
* **임상 연구소(EBTI) 실무 협업 제안 수락** 및 비즈니스 임팩트 고도화 리드

---

### 📫 Contact & More

* **Email**: j2031414@gmail.com
* **Github**: [github.com/kkomakk](https://github.com/kkomakk)
* **Motto**: "팀의 병목은 코드 밖에도 있습니다. 명확한 데이터와 최적화된 시스템으로 비즈니스의 성장 가치를 증명합니다."
