# 유현서 | Backend Engineer

> **"정답을 고집하기보다, 팀의 피드백을 양분 삼아 더 나은 아키텍처의 근거를 배워가는 개발자입니다."**
> 
> 단순한 기능 구현에 머물지 않고, 변경의 여파를 격리해 '팀'의 지속 가능한 개발 속도를 지키는 구조를 지향합니다.

[![Portfolio](https://img.shields.io/badge/Portfolio-Notion-000000?style=flat-square&logo=notion&logoColor=white)](https://www.notion.so/Backend-Engineer-30b3699bed5e8004b63dc132ff4a3a73?source=copy_link)
[![Blog](https://img.shields.io/badge/Blog-Velog-20C997?style=flat-square&logo=velog&logoColor=white)](https://velog.io/@vmffotltka)
[![Email](https://img.shields.io/badge/Email-vmffotltka1@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:vmffotltka1@gmail.com)

---

## 🚀 Key Projects

### ⭐ [Identity Modulith](https://github.com/vmffotltka/Identity-Modulith) — 넥스프론 R&D 인턴 (2025.07 – 2026.02)
> 비즈니스 제약과 팀의 개발 복잡도를 고려하여 아키텍처를 절충하고 성능을 최적화한 B2B 인증/인가 모듈

- **SSO 아키텍처 전환**: AWS Connect의 SAML 2.0 제약을 파악하고, 기존 서버리스 기획 대신 B2B 보안 표준을 충족하기 위해 Keycloak 기반 IdP 구조로 아키텍처 전환 주도
- **도메인 맞춤형 권한 설계 및 의존성 역전(DIP)**: 상담사 역할이 교차하는 업무 특성을 분석해 계층형 RBAC를 '수평적(Flat) RBAC'로 재설계함. 또한 타 모듈의 직접 참조를 막기 위해 내부 포트(Port) 기반의 DIP를 적용한 Modular Monolith 구조를 구축하여 유지보수 부담 완화
- **N+1 쿼리 최적화**: RBAC 조회 시 지연 로딩으로 인한 N+1 문제를 식별하고, 3-JOIN 구조 개편 및 스칼라 프로젝션(Scalar Projection)을 적용해 실행 쿼리 26회 → 1회, 평균 응답 시간 96% 단축(255ms → 10ms) 달성

`Spring Boot` `Keycloak` `PostgreSQL` `SAML 2.0` `Modular Monolith`

---

### [길라의 빛](https://github.com/Capston-Design-Team-Nova/Light_Of_Gilla) — 캡스톤 프로젝트 (2025.01 – 2025.05)
> 운영 중 발생한 문제를 구조 변경과 파이프라인 구축을 통해 해결한 프로젝트

- **비용 효율적인 MSA 도입**: 백엔드 2인 동시 개발 시 매일 발생하던 로컬 DB 간섭 문제를 해결하기 위해, 40만 원의 지원금 내 인프라 유지 비용을 계산해 MSA 도입 타당성 검증 및 설계
- **독립적 개발 환경 구축**: API Gateway 기반으로 서비스를 분리하여 하루 수차례 발생하던 테스트 간섭 문제 제거. 기능 개발과 테스트를 완전히 병렬화하여 개발 속도 저하 요인 제거
- **장애 대응 파이프라인**: 25,000건의 초기 데이터 적재 중 EC2 메모리 한계(OOM)로 DB가 다운되는 장애 발생. 비즈니스 연속성 확보를 위해 원본 CSV를 기반으로 DB를 5분 내에 자동 복구하는 Python 스크립트를 구축해 운영 안정성 확보

`Spring Boot` `MySQL` `AWS API Gateway` `Python`

---

## 🏆 Awards

| 수상 | 내용 | 날짜 |
| :--- | :--- | :--- |
| 🥇 대상 (1위 / 33명) | [HSUPC 프로그래밍 경시대회](https://github.com/HSU-CSE/hsupc-2024-2) | 2024.11.18 |
| 🥈 우수상 (5등 / 27팀) | 한성SW중심대학 페스티벌 공모전 | 2024.11.29 |
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
