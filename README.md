<div align="center">

![teriyakki-jin 보안 엔지니어링 포트폴리오](https://capsule-render.vercel.app/api?type=waving&color=0:08111F,50:12345A,100:34D399&height=230&section=header&text=teriyakki-jin&fontSize=58&fontColor=F8FAFC&animation=fadeIn&fontAlignY=37&desc=%EB%B3%B4%EC%95%88%20%EC%97%94%EC%A7%80%EB%8B%88%EC%96%B4%EB%A7%81%20%ED%8F%AC%ED%8A%B8%ED%8F%B4%EB%A6%AC%EC%98%A4&descSize=19&descAlignY=58)

### 네트워크 엔지니어링 · 제로 트러스트 · AI 보안

백엔드부터 AI까지, 시스템 전체의 흐름을 설계하고 배포합니다.<br>

네트워크 장애를 재현하고, 로그를 분석하고, AI 도구의 실행 권한을 다루는 프로젝트를 만들고 있습니다.<br>

<br>

<a href="https://teriyakki-jin.github.io/"><img src="https://img.shields.io/badge/Portfolio-0F172A?style=for-the-badge&logo=githubpages&logoColor=34D399" alt="Portfolio website" /></a> <a href="https://github.com/teriyakki-jin"><img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub profile" /></a> <a href="https://github.com/teriyakki-jin/zero-trust-network-lab"><img src="https://img.shields.io/badge/Zero%20Trust%20Lab-2563EB?style=for-the-badge&logo=openid&logoColor=white" alt="Zero Trust Network Lab" /></a>

</div>

<br>

## 소개

부산대학교에서 컴퓨터공학을 전공했고, KT AIVLE School에서 AI와 웹 서비스 프로젝트를 진행했습니다.

Spring Boot와 FastAPI로 백엔드를 만들고, React로 화면을 붙여 직접 배포해 왔습니다. 최근에는 네트워크 장애가 서비스에 미치는 영향과 AI Agent가 허가된 범위 안에서 동작하는지에 관심을 두고 있습니다.

## 주요 네트워크·보안 프로젝트

| 프로젝트 | 만든 내용 | 확인한 결과·구성 |
|---|---|---|
| [**TelcoNet Sentinel**](https://github.com/teriyakki-jin/telconet-sentinel) | OSPF 망에 패킷이 버려지는 장애를 주입해 BFD 적용 전후를 비교하고, 링크·노드 장애의 영향을 분석 | 구성별 20회 반복 · 로컬 p95 탐지 상한: OSPF `4,058ms`, BFD `519ms` |
| [**NetSentry**](https://github.com/teriyakki-jin/netsentry) | 가상 장비의 상태와 알림을 한 화면에서 확인하고, 장애 탐지부터 백업 경로 전환까지 재현하는 운영 콘솔 | 가상 장비 10대 · 서비스 5개 · 장애 시나리오 3종 |
| [**Zero Trust Network Lab**](https://github.com/teriyakki-jin/zero-trust-network-lab) | Keycloak으로 사용자를 인증하고, OPA 정책에 따라 FastAPI에서 접근을 허용하거나 차단하는 실습 환경 | OPA 테스트 `6/6` · 통합 테스트 `7/7` · CI |
| [**Agent Runtime Security Lab**](https://github.com/teriyakki-jin/agent-runtime-security-lab) | AI Agent에 허가한 작업과 실제 프로세스·파일·네트워크 동작을 비교해 권한 밖의 실행을 탐지 | 로컬 테스트 데이터 기준 재현율 `100%` · 오탐률 `0%` |
| [**Network Forensics Lab**](https://github.com/teriyakki-jin/network-forensics-lab) | 공격 트래픽을 직접 발생시켜 Snort와 Suricata의 탐지 결과를 비교하고 Elastic에서 로그를 분석 | 시나리오 6종 · 경보 `45/45` · 테스트 커버리지 `91%` |
| [**LLM Security Gateway**](https://github.com/teriyakki-jin/llm-security-gateway) | LLM 요청에서 프롬프트 인젝션과 개인정보를 검사하고, ML-KEM-768/X25519로 전송 구간을 암호화 | Python + Go |
| [**SecureScope**](https://github.com/teriyakki-jin/SecureScope) | 보안 로그를 수집해 규칙으로 이상 징후를 탐지하고, 감사 로그와 실시간 대시보드로 확인하는 경량 SIEM | Spring Boot · PostgreSQL · Redis · React |

> 수치는 로컬 실습 환경에서 측정했습니다. 실험 조건과 한계는 각 저장소에 정리해 두었습니다.

## 백엔드·AI 프로젝트

| 프로젝트 | 만든 내용 |
|---|---|
| [**localops-agent**](https://github.com/teriyakki-jin/localops-agent) | 로컬 파일·Git·노트를 MCP로 연결한 AI Agent. 작업별 실행 정책과 승인 절차를 두고 실행 기록을 저장 |
| [**ConsentLedger**](https://github.com/teriyakki-jin/ConsentLedger) | 마이데이터 동의와 전송 이력을 관리하는 서비스. 해시 체인으로 감사 로그의 변경 여부를 확인하고 Spring AI MCP 도구를 연결 |
| [**Water Treatment Graph RAG**](https://github.com/teriyakki-jin/Graph-RAG-with-water) | 수처리 법규와 공정 문서를 지식 그래프로 만들고, Neo4j 그래프 검색과 KR-SBERT 벡터 검색을 함께 사용하는 RAG |

다른 프로젝트와 KT AIVLE School에서 진행한 작업은 [포트폴리오](https://teriyakki-jin.github.io/#projects)에 정리했습니다.

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

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:34D399,50:12345A,100:08111F&height=120&section=footer" alt="" width="100%" />

</div>
