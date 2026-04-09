# 유현서 | Backend Engineer

> **"MSA 도입 이후 Modular Monolith로 구조를 재설계한 경험을 통해, 아키텍처는 이상적인 형태보다 팀 규모와 운영 비용을 기준으로 선택해야 함을 배웠습니다."**
> 
> 동작하는 코드를 넘어, 변경 시 영향을 받는 코드 범위를 모듈 내부로 제한해 개발 속도를 유지하는 구조를 설계합니다.

[![Portfolio](https://img.shields.io/badge/Portfolio-PDF-red?style=flat&logo=adobeacrobatreader&logoColor=white)](https://www.notion.so/Backend-Engineer-30b3699bed5e8004b63dc132ff4a3a73?source=copy_link)
[![Email](https://img.shields.io/badge/Email-vmffotltka1@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:vmffotltka1@gmail.com)

---

## 🚀 Key Projects

### ⭐ [Identity Modulith](https://github.com/vmffotltka/Identity-Modulith) — 넥스프론 R&D 인턴 (2025.07 – 2026.02)
> 팀의 개발 복잡도를 낮추기 위해 아키텍처를 설계하고 구조를 결정한 경험

- **SSO 아키텍처 전환**: AWS Connect의 SAML 2.0 제약을 파악하고, 기존 서버리스 기획 대신 B2B 보안 수준을 충족하기 위해 Keycloak 기반 IdP 구조로 전
- **도메인 분리 및 영향도 통제**: 완벽한 MSA 분리보다 팀 규모와 운영 복잡도를 기준으로 여러 대안을 비교하여 Modular Monolith 구조 선택. **인증 로직 수정 시 확인해야 할 코드 범위를 모듈 단위로 제한하고, 다른 도메인 영향 없이 독립적으로 배포 가능한 구조를 확보해 유지보수 부담 완화**
- **성능 최적화**: RBAC 조회 시 지연 로딩으로 인한 N+1 문제를 식별하고, Fetch Join + DTO 프로젝션을 병행 적용해 실행 쿼리 26회 → 1회, 평균 응답 시간 96% 단축(255ms → 10ms) 달성

`Spring Boot` `Keycloak` `PostgreSQL` `SAML 2.0` `DDD`

---

### [길라의 빛](https://github.com/Capston-Design-Team-Nova/Light_Of_Gilla) — 캡스톤 프로젝트 (2025.01 – 2025.05)
> 운영 중 발생한 문제를 구조 변경과 파이프라인 구축을 통해 해결한 프로젝트

- **MSA 도입 결정**: 백엔드 2인 동시 개발 시 매일 발생하던 로컬 DB 간섭 문제를 해결하기 위해, 40만 원의 지원금 내 인프라 유지 비용을 계산해 MSA 도입 타당성 검증 및 설계
- **독립적 개발 환경 구축**: API Gateway 기반으로 서비스를 분리하여 하루 수차례 발생하던 테스트 간섭 문제 제거. **기능 개발과 테스트를 완전히 병렬화하여 개발 속도 저하 요인 제거**
- **장애 대응 파이프라인**: 운영 중 EC2 OOM으로 25,000건의 데이터가 유실되는 장애 발생. 서비스 정상화가 우선이라 판단해, 원본 CSV를 기반으로 DB를 5분 내에 자동 복구하는 파이프라인을 구축해 운영 안정성 확보

`Spring Boot` `MySQL` `AWS API Gateway` `Python`

---

## 🏆 Awards

| 수상 | 내용 | 날짜 |
| :--- | :--- | :--- |
| 🥇 대상 (1위 / 33명) | [HSUPC 프로그래밍 경시대회](https://github.com/HSU-CSE/hsupc-2024-2) | 2024.11.18 |
| 🥈 우수상 (7위 / 52명) | 한성SW중심대학 페스티벌 코딩대회 | 2024.11.29 |
| 🥈 우수상 (5등 / 27팀) | 한성SW중심대학 페스티벌 공모전 | 2024.11.29 |

---

## 💎 Algorithm

[![Solved.ac Profile](http://mazassumnida.wtf/api/v2/generate_badge?boj=vmffotltka)](https://solved.ac/vmffotltka)

---

## 📊 GitHub Stats

<div align="center">
  <img src="https://github-readme-stats-fast.vercel.app/api/top-langs/?username=vmffotltka&layout=compact&langs_count=6&theme=tokyonight" height="170" />
  <img src="https://streak-stats.demolab.com?user=vmffotltka&theme=tokyonight" height="170" />
</div>
