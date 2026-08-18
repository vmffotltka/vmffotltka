# 유현서 | Backend Engineer

[![codemaru card for vmffotltka](https://codemaru.bnbong.com/api/card.svg?github=vmffotltka&boj=vmffotltka&leetcode=codemaru_demo)](https://github.com/vmffotltka)
> **"배우는 과정을 즐기며, 그 속도로 성장하는 개발자입니다"**

[![Portfolio](https://img.shields.io/badge/Portfolio-Notion-000000?style=flat-square&logo=notion&logoColor=white)](https://www.notion.so/Backend-Engineer-30b3699bed5e8004b63dc132ff4a3a73?source=copy_link)
[![Blog](https://img.shields.io/badge/Blog-Velog-20C997?style=flat-square&logo=velog&logoColor=white)](https://velog.io/@vmffotltka)
[![Email](https://img.shields.io/badge/Email-vmffotltka1@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:vmffotltka1@gmail.com)

---

## 🚀 Key Projects

### ⭐ [Identity Modulith](https://github.com/vmffotltka/Identity-Modulith) — 넥스프론 R&D 인턴 (2025.07 – 2026.02)
> 비즈니스 제약과 팀의 개발 환경을 고려해 아키텍처를 절충하고 성능을 개선한 B2B 인증/인가 모듈

- **SSO 아키텍처 전환**: AICC 솔루션의 SaaS 전환을 고려할 때, 기존 인증 방식으로는 이중 로그인이 발생하고 AWS Connect가 요구하는 SAML 2.0 규격을 지원할 수 없는 한계에 직면함. Cognito 기반 서버리스 인증을 먼저 검토했으나 SAML 2.0 IdP가 필수 규격임을 확인하고 Keycloak으로 전환을 제안, 인증(IdP)과 인가를 분리하는 구조와 SAML 2.0 연동 시퀀스 다이어그램을 설계해 팀에 공유함(세부 설정은 팀에 인계)
- **도메인 맞춤형 권한 설계 및 모듈러 모놀리스 제안**: 상담사들의 실제 업무가 수직적이지 않다는 도메인 특성을 파악해 계층형 대신 '수평적(Flat) RBAC' 구조를 제안하고 DB를 설계함. 또한 협업 리스크와 인프라 비용을 고려해 모듈러 모놀리스 구조를 제안하고, 모듈 간 테이블을 직접 조인하지 않고 UUID 기반 PK로 참조하는 방식을 설계에 반영함
- **N+1 쿼리 최적화**: 권한 조회 시 불필요한 데이터까지 로딩되어 지연이 발생하는 N+1 문제를 확인하고, 필요한 데이터만 조회하는 스칼라 프로젝션(Scalar Projection)과 JOIN을 적용해 쿼리 실행 26회 → 1회 고정 및 응답 시간 96% 단축(255ms → 10ms) 달성

`Spring Boot` `Keycloak` `PostgreSQL` `SAML 2.0` `Modular Monolith`

---

### [길라의 빛](https://github.com/vmffotltka/Light_Of_Gilla) — 캡스톤 프로젝트 (2025.01 – 2025.05)
> 예산 제약을 고려해 인프라를 설계하고, 원인 불명의 장애 상황에서도 서비스 안정성을 확보한 프로젝트
- **예산 제약을 고려한 인프라 설계**: MSA로 서비스를 분리하며 일부 서비스에 AWS RDS 도입을 검토했으나, 네트워크·보안 그룹 설정이 반복적으로 실패하고 다수의 EC2 인스턴스 운영으로 이미 비용 부담이 큰 상황이었음. 관리형 DB의 이점과 실제 비용·설정 리스크를 비교해 한 서비스만 실험적으로 RDS를 적용하고 나머지는 EC2 위 MySQL로 전환, 예산 안에서 독립 배포 구조를 유지함
- **데이터 유실 대비 자동 복구 파이프라인 구축**: 크롤링한 12만 건의 병원 데이터를 2만 5천 건으로 적재하는 과정에서 발표를 앞두고 원인 불명의 DB 테이블 유실이 반복 발생함. EC2 스펙 증설과 로그 분석을 시도했으나 근본 원인은 특정하지 못해, 원인 규명보다 서비스 정상화를 우선하여 로컬 원본 데이터를 1,000건 단위로 재적재하는 복구 스크립트를 작성. 5분 내 DB 복구 가능한 파이프라인을 확보해 발표 당일 서비스를 정상 운영함

`Spring Boot` `MySQL` `AWS API Gateway` `Python`

---

### [EduCraft](https://github.com/vmffotltka/EduCraft) — 공모전 출품작 (2024.08 – 2024.11)
> 발표 18일 전 팀원 이탈에도 API 명세 표준화를 기반으로 1인 풀스택으로 완주한 LLM 맞춤형 교육 서비스
- **팀원 이탈 후 18일 만에 1인 풀스택으로 완주**: 4인 팀(백엔드 2, 프론트 2)으로 시작했으나 발표 18일 전 프론트 담당 2명이 이탈함. 프로젝트를 포기하는 대신 프론트엔드·백엔드·배포를 전부 직접 맡기로 결정하고, 부족한 프론트엔드 역량은 AI 도구를 적극 활용해 빠르게 보완함
- **문서 표준화를 통한 연동 오류 최소화**: 데이터 연동 혼선을 막기 위해 API 엔드포인트와 규격을 상세히 정의하고 팀 내 소통 기준을 수립해 기한 내 완성함
- **시장 분석 기반의 비즈니스 모델(BM) 수립**: 교육 앱 시장을 직접 분석해 모의고사 기능 부재를 차별점으로 설정하고, 광고와 월 4,000원 구독료를 결합한 BM을 수립함

`Node.js` `LLM API` `React` `AWS EC2`

---

## 🏆 Awards

| 수상 | 내용 | 날짜 |
| :--- | :--- | :--- |
| 🥇 대상 (1위 / 33명) | [HSUPC 프로그래밍 경시대회](https://github.com/HSU-CSE/hsupc-2024-2) | 2024.11.18 |
| 🥈 우수상 (5등 / 27팀) | 한성SW중심대학 페스티벌 공모전 [EduCraft] | 2024.11.29 |
| 🥈 우수상 (7위 / 52명) | 한성SW중심대학 페스티벌 코딩대회 | 2024.11.29 |

---

## 💎 Algorithm

[![Solved.ac Profile](http://mazassumnida.wtf/api/v2/generate_badge?boj=vmffotltka)](https://solved.ac/vmffotltka)

---

## 📊 GitHub Stats

<div align="center">
  <img src="https://github-readme-stats-fast.vercel.app/api/top-langs/?username=vmffotltka&layout=compact&langs_count=6&theme=tokyonight" height="170" />
  <img src="https://streak-stats.demolab.com?user=vmffotltka&theme=tokyonight" height="170" />
</div>

