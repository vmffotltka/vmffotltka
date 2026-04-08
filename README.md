# 유현서 | Backend Engineer

> **"MSA 도입 후 Modular Monolith로 구조를 재설계한 경험을 통해, 아키텍처는 이상적인 형태보다 팀 규모와 운영 비용을 기준으로 선택해야 함을 배웠습니다."**
> 
> 동작하는 코드를 넘어, 인증 로직 수정 시 영향을 받는 코드 범위를 모듈 내부로 제한하여 변경 시에도 개발 속도를 유지할 수 있는 구조를 고민하고 있습니다.

[![Portfolio](https://img.shields.io/badge/Portfolio-PDF-red?style=flat&logo=adobeacrobatreader&logoColor=white)](https://www.notion.so/Backend-Engineer-30b3699bed5e8004b63dc132ff4a3a73?source=copy_link)
[![Email](https://img.shields.io/badge/Email-vmffotltka1@gmail.com-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:vmffotltka1@gmail.com)

---

## 🚀 Key Projects

### ⭐ [Identity Modulith](https://github.com/vmffotltka/Identity-Modulith) — 넥스프론 R&D 인턴 (2025.07 – 2026.02)
> 인증 구조와 아키텍처를 판단하며, 팀의 개발 복잡도를 낮추는 설계 기준을 검토한 경험

- **SSO 아키텍처 전환**: AWS Connect의 SAML 2.0 제약을 확인하고, 기존 서버리스 환경 대신 B2B 보안 수준을 충족하는 Keycloak 기반 IdP 구조로 전환
- **아키텍처 선택과 팀 임팩트**: 팀 규모와 운영 복잡도를 고려해 Modular Monolith 구조를 선택. **인증 관련 기능 변경 시 다른 도메인 수정 없이 독립적으로 배포 가능한 구조를 확보하여 유지보수 효율성 개선**
- **성능 최적화**: RBAC 조회 시 지연 로딩으로 인한 N+1 문제를 분석하고 Fetch Join + DTO 프로젝션으로 개선 (**26 queries → 1 query, 255ms → 10ms**)

`Spring Boot` `Keycloak` `PostgreSQL` `SAML 2.0` `DDD`

---

### [길라의 빛](https://github.com/Capston-Design-Team-Nova/Light_Of_Gilla) — 캡스톤 프로젝트 (2025.01 – 2025.05)
> 협업 병목을 구조적으로 해결하기 위해 타당성을 검토하고 MSA 도입을 판단한 프로젝트

- **MSA 도입 판단 과정**: 백엔드 2인 개발 환경에서 반복되는 로컬 테스트 간섭 문제를 해결하기 위해, 지원금 내 인프라 비용을 계산하여 MSA 도입 타당성 검토
- **독립적 개발 환경 구축**: API Gateway 기반으로 서비스 호출 경로를 단일화. **기능 개발과 테스트를 병렬로 진행할 수 있는 환경을 확보하여 팀원 간 개발 충돌 빈도 제거**
- **장애 대응 경험**: EC2 메모리 부족으로 데이터 유실 발생 시, 원인 분석에 앞서 CSV 기반 복구 파이프라인을 구축해 **5분 내 서비스 정상화 달성**

`Spring Boot` `MySQL` `AWS API Gateway` `Python`

---

## 🏆 Awards

| 수상 | 내용 | 날짜 |
| :--- | :--- | :--- |
| 🥇 대상 (1위 / 33명) | [2024 HSUPC 프로그래밍 경시대회](https://github.com/HSU-CSE/hsupc-2024-2) | 2024.11.18 |
| 🥈 우수상 (7위 / 52명) | 한성SW중심대학 페스티벌 코딩대회 | 2024.11.29 |
| 🥈 우수상 (5등 / 27팀) | 한성SW중심대학 페스티벌 공모전 (EduCraft 프로젝트) | 2024.11.29 |

---

## 💎 Algorithm

[![Solved.ac Profile](http://mazassumnida.wtf/api/v2/generate_badge?boj=vmffotltka)](https://solved.ac/vmffotltka)

---

## 📊 GitHub Stats

<div align="center">
  <img src="https://github-readme-stats-fast.vercel.app/api/top-langs/?username=vmffotltka&layout=compact&langs_count=6&theme=tokyonight" height="170" />
  <img src="https://streak-stats.demolab.com?user=vmffotltka&theme=tokyonight" height="170" />
</div>
