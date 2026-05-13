# 유현서 | Backend Engineer

> **"스스로 찾아가며 배우고, 팀과 함께 성장하는 개발자입니다."**

[![Portfolio](https://img.shields.io/badge/Portfolio-Notion-000000?style=flat-square&logo=notion&logoColor=white)](https://www.notion.so/Backend-Engineer-30b3699bed5e8004b63dc132ff4a3a73?source=copy_link)
[![Blog](https://img.shields.io/badge/Blog-Velog-20C997?style=flat-square&logo=velog&logoColor=white)](https://velog.io/@vmffotltka)
[![Email](https://img.shields.io/badge/Email-vmffotltka1@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:vmffotltka1@gmail.com)

---

## 🚀 Key Projects

### ⭐ [Identity Modulith](https://github.com/vmffotltka/Identity-Modulith) — 넥스프론 R&D 인턴 (2025.07 – 2026.02)
> 비즈니스 제약과 팀의 개발 환경을 고려해 아키텍처를 절충하고 성능을 개선한 B2B 인증/인가 모듈

- **SSO 아키텍처 전환**: 자사 솔루션과 AWS Connect 연동 시, 상담사들이 두 번 로그인해야 하는 불편함을 막기 위해 SAML 2.0을 지원하는 Keycloak을 도입해 인증을 통합함
- **도메인 맞춤형 권한 설계 및 의존성 역전(DIP)**: 상담사들의 실제 업무가 수직적이지 않다는 도메인 특성을 파악해 복잡한 계층형 대신 '수평적(Flat) RBAC' 구조를 제안하고 DB를 설계함. 또한, 점진적인 분리를 고려해 모듈러 모놀리스 구조를 도입하고 DIP를 적용하여 모듈 간 강결합 문제를 해결함
- **N+1 쿼리 최적화**: 권한 조회 시 불필요한 데이터까지 로딩되어 지연이 발생하는 N+1 문제를 확인하고, 필요한 데이터만 조회하는 스칼라 프로젝션(Scalar Projection)과 JOIN을 적용해 쿼리 실행 26회 → 1회 고정 및 응답 시간 96% 단축(255ms → 10ms) 달성

`Spring Boot` `Keycloak` `PostgreSQL` `SAML 2.0` `Modular Monolith`

---

### [길라의 빛](https://github.com/vmffotltka/Light_Of_Gilla) — 캡스톤 프로젝트 (2025.01 – 2025.05)
> 독립적인 개발 환경 구성을 위해 서버를 분리하고, 저사양 서버 환경에서의 데이터 관리 안정성을 확보한 프로젝트

- **독립적 개발을 위한 MSA 도입**: 백엔드 2인이 하나의 서버로 개발하며 발생하던 로컬 테스트 간섭을 해결하기 위해 MSA 구조 도입을 제안함. 정해진 예산 내에서 단일 서버와 분산 서버의 유지 비용을 직접 계산해 비교한 뒤 API Gateway로 엔드포인트를 분리함
- **데이터 적재 및 복구 자동화**: 25,000건의 초기 데이터 적재 중 저사양 서버 환경에서 발생할 수 있는 시스템 불안정 문제를 해결하고자 함. 데이터를 500건 단위로 나누어 적재하고, 예외 발생 시 해당 배치만 롤백한 뒤 5분 내에 다시 적재를 마치는 파이썬 스크립트를 작성해 서비스 운영의 안정성을 확보함

`Spring Boot` `MySQL` `AWS API Gateway` `Python`

---

### [EduCraft](https://github.com/vmffotltka/EduCraft) — 공모전 출품작 (2024.08 – 2024.11)
> API 명세 표준화를 통해 프론트-백엔드 협업 효율을 높이고 서비스 수익 모델을 기획한 LLM 맞춤형 교육 서비스

- **문서 표준화를 통한 연동 오류 최소화**: 첫 엔드투엔드 프로젝트를 진행하며 발생할 수 있는 데이터 연동 혼선을 막기 위해, Word를 활용해 API 엔드포인트와 규격을 상세히 정의하고 팀 내 소통 기준을 수립하여 기한 내 완성함
- **시장 분석 기반의 비즈니스 모델(BM) 수립**: 서비스의 지속 가능성을 높이기 위해 교육 앱 시장을 직접 분석함. 시중 서비스에 모의고사 기능이 부족함을 확인하고 이를 차별점으로 설정한 뒤, 하단 광고와 월 4,000원의 구독료를 결합한 구체적인 BM을 수립함

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
