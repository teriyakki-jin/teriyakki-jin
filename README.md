<div align="center">

![teriyakki-jin 보안 엔지니어링 포트폴리오](https://capsule-render.vercel.app/api?type=waving&color=0:08111F,50:12345A,100:34D399&height=230&section=header&text=teriyakki-jin&fontSize=58&fontColor=F8FAFC&animation=fadeIn&fontAlignY=37&desc=%EB%B3%B4%EC%95%88%20%EC%97%94%EC%A7%80%EB%8B%88%EC%96%B4%EB%A7%81%20%ED%8F%AC%ED%8A%B8%ED%8F%B4%EB%A6%AC%EC%98%A4&descSize=19&descAlignY=58)

### 네트워크 엔지니어링 · 제로 트러스트 · AI 보안

백엔드부터 AI까지, 시스템 전체의 흐름을 설계하고 배포합니다.<br>

재현 가능한 보안 시스템을 만들고, 테스트와 실행 증거로 보안 주장을 검증합니다.<br>

<br>

<a href="https://teriyakki-jin.github.io/"><img src="https://img.shields.io/badge/Portfolio-0F172A?style=for-the-badge&logo=githubpages&logoColor=34D399" alt="Portfolio website" /></a> <a href="https://github.com/teriyakki-jin"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub profile" /></a> <a href="https://github.com/teriyakki-jin/zero-trust-network-lab"><img src="https://img.shields.io/badge/Zero%20Trust%20Lab-2563EB?style=for-the-badge&logo=openid&logoColor=white" alt="Zero Trust Network Lab" /></a>

</div>

<br>

## 소개

- 부산대학교 CS 졸업 · KT AIVLE School 프로젝트 경험
- 네트워크 구조 설계, 장애 영향 분석, 상태를 관측할 수 있는 운영 플랫폼 구현
- **제로 트러스트 아키텍처** 기반 사용자 신원·상황별 접근 제어
- 네트워크 위협 탐지와 **포렌식 증거 파이프라인** 구축
- AI Agent 실행 보안, LLM 보안 게이트웨이, **코드 기반 정책 관리**
- 재현 가능한 실습 환경과 자동화 테스트로 보안 기능을 검증하고 한계를 문서화

## 주요 네트워크·보안 프로젝트

| 프로젝트 | 핵심 구현 | 검증 및 구성 |
|---|---|---|
| [**TelcoNet Sentinel**](https://github.com/teriyakki-jin/telconet-sentinel) | FRRouting/containerlab OSPF 망, BFD 블랙홀 장애 탐지, 링크·노드·SRLG 영향 분석, Prometheus/Grafana | 구성별 20회 반복 · 로컬 p95 탐지 상한: OSPF `4,058ms`, BFD `519ms` |
| [**NetSentry**](https://github.com/teriyakki-jin/netsentry) | 가상 네트워크 운영 콘솔, 텔레메트리 수집, 알림 상관분석, 장애 전환 이력 저장 | 가상 장비 10대 · 서비스 5개 · 장애 시나리오 3종 · Spring Boot + React + PostgreSQL |
| [**Zero Trust Network Lab**](https://github.com/teriyakki-jin/zero-trust-network-lab) | Keycloak 인증, FastAPI 정책 집행 지점, OPA 정책 판단, 격리된 Docker 데이터 영역 | OPA 테스트 `6/6` · 통합 테스트 `7/7` · CI |
| [**Agent Runtime Security Lab**](https://github.com/teriyakki-jin/agent-runtime-security-lab) | 허가된 행동과 실제 실행의 상관분석, OPA 제어, Tetragon eBPF 관측, OCSF 증거 기록 | 로컬 테스트 데이터 기준 재현율 `100%` · 오탐률 `0%` |
| [**Network Forensics Lab**](https://github.com/teriyakki-jin/network-forensics-lab) | 공격 트래픽 재현, Snort/Suricata 교차 검증, Elastic 시각화 | 시나리오 6종 · 경보 `45/45` · 테스트 커버리지 `91%` |
| [**LLM Security Gateway**](https://github.com/teriyakki-jin/llm-security-gateway) | ML-KEM-768/X25519 하이브리드 암호화 채널, 프롬프트 인젝션·개인정보 유출 방어 | Python + Go · FIPS 203을 고려한 설계 |
| [**SecureScope**](https://github.com/teriyakki-jin/SecureScope) | 탐지 규칙, 위변조 탐지 감사 로그, 실시간 대시보드를 갖춘 경량 SIEM | Spring Boot · PostgreSQL · Redis · React |

> 수치는 각 저장소의 로컬 검증 결과이며, 실제 운영 환경의 성능을 의미하지 않습니다.

## 백엔드·AI 프로젝트

| 프로젝트 | 핵심 구현 |
|---|---|
| [**localops-agent**](https://github.com/teriyakki-jin/localops-agent) | MCP 기반 로컬 우선 Agent Orchestrator, 정책 엔진, 실행 추적 로그, 승인 기반 실행 |
| [**ConsentLedger**](https://github.com/teriyakki-jin/ConsentLedger) | 마이데이터 동의·전송 관리, Spring AI MCP 도구, 해시 체인 감사 로그, 무결성 검증 |
| [**Water Treatment Graph RAG**](https://github.com/teriyakki-jin/Graph-RAG-with-water) | 수처리 도메인 지식 그래프, Neo4j/KR-SBERT 하이브리드 검색, RAG 평가 |

기타 프로젝트와 KT AIVLE School 작업은 [포트폴리오](https://teriyakki-jin.github.io/#projects)에서 확인할 수 있습니다.

<br>

<div align="center">

## 기술 스택

### 보안·플랫폼

<img src="https://img.shields.io/badge/Keycloak-4D4D4D?style=for-the-badge&logo=keycloak&logoColor=white" alt="Keycloak" /> <img src="https://img.shields.io/badge/Open%20Policy%20Agent-7D47FF?style=for-the-badge&logo=openpolicyagent&logoColor=white" alt="Open Policy Agent" /> <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" /> <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=111" alt="Linux" /> <img src="https://img.shields.io/badge/Elastic-005571?style=for-the-badge&logo=elastic&logoColor=white" alt="Elastic" /> <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" alt="GitHub Actions" />

### 개발

<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" /> <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java" /> <img src="https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white" alt="Go" /> <img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" /> <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" alt="FastAPI" /> <img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=for-the-badge&logo=springboot&logoColor=white" alt="Spring Boot" /> <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" /> <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" alt="Redis" />

<br>

## GitHub 활동

<img src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=teriyakki-jin&theme=radical" alt="teriyakki-jin contribution summary" />

<img height="170" src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=teriyakki-jin&theme=radical" alt="teriyakki-jin GitHub statistics" />
<img height="170" src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=teriyakki-jin&theme=radical" alt="Public repositories grouped by language" />

<br>

## 개발 흐름

```text
위협 모델링 → 오류 시 차단하는 설계 → 코드 기반 정책 → 자동 검증 → 검토 가능한 실행 증거
```

<sub>인증 정보는 소스 코드에 포함하지 않고, 신뢰 경계와 구현의 한계를 명확히 기록합니다.</sub>

<br>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:34D399,50:12345A,100:08111F&height=120&section=footer" alt="" width="100%" />

</div>
