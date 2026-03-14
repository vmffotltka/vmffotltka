# 유현서 | Backend Engineer

> **"DB가 날아가는 장애를 겪으며, 처음부터 무너지지 않는 구조를 고민하게 되었습니다."**
>
> 책임이 명확히 분리되고, 변경이 발생해도 영향 범위를 통제할 수 있는 구조를 설계하는 것에 집착합니다.
> DDD 기반 설계와 현실적인 아키텍처 선택(Modular Monolith vs MSA)을 고민하고 실무에 적용해 나가고 있습니다.

[![Portfolio](https://img.shields.io/badge/Portfolio-PDF-red?style=flat&logo=adobeacrobatreader&logoColor=white)](https://www.notion.so/Backend-Engineer-30b3699bed5e8004b63dc132ff4a3a73?source=copy_link)
[![Email](https://img.shields.io/badge/Email-vmffotltka1@gmail.com-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:vmffotltka1@gmail.com)

---

## 🛠 Tech Stack

| Category | Technologies |
| :--- | :--- |
| **Backend** | ![Java](https://img.shields.io/badge/Java-007396?style=flat-square&logo=Java&logoColor=white) ![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=SpringBoot&logoColor=white) ![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?style=flat-square&logo=SpringSecurity&logoColor=white) ![JPA](https://img.shields.io/badge/JPA-59666C?style=flat-square) |
| **Architecture** | `DDD` `Modular Monolith` `MSA` |
| **Database** | ![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=MySQL&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=PostgreSQL&logoColor=white) |
| **Infra** | ![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=AmazonAWS&logoColor=white) |
| **Authentication** | ![Keycloak](https://img.shields.io/badge/Keycloak-EB5424?style=flat-square) `SAML 2.0` `RBAC` |

---

## 🚀 Key Projects

### ⭐ [Identity Modulith](https://github.com/vmffotltka/Identity-Modulith) — 넥스프론 R&D 인턴 (2025.07 – 2026.02)
> AICC 솔루션의 인증·권한 모듈을 DDD 기반 Modular Monolith 구조로 설계

- **SAML 2.0 기반 SSO 구축**: AWS Connect의 기술적 제약을 고려해 OAuth2/OIDC 대신 Keycloak IdP 채택
- **Modular Monolith 설계**: 팀 규모와 운영 복잡도를 고려해 MSA 대신 선택, 논리적 도메인 분리 달성
- **RBAC N+1 개선**: Fetch Join + DTO 프로젝션으로 **26 queries → 1 query, 255ms → 10ms (96% 단축)**

`Spring Boot` `Keycloak` `PostgreSQL` `SAML 2.0` `DDD`

---

### [길라의 빛](https://github.com/Capston-Design-Team-Nova/Light_Of_Gilla) — 캡스톤 프로젝트 (2025.01 – 2025.05)
> MSA 기반 병원 추천 서비스 / 4인 팀 (BE 2, FE 2) / 백엔드 담당

- **MSA 아키텍처**: 장애 격리와 독립 배포 학습을 위해 의도적으로 MSA 도입, API Gateway로 엔드포인트 단일화
- **데이터 파이프라인**: BeautifulSoup + Selenium으로 전국 병원·약국 25,000건 크롤링 및 적재 자동화
- **장애 대응**: EC2 메모리 부족으로 25,000건 유실 → CSV 기반 자동 복구 파이프라인 구축, **5분 내 복구**

`Spring Boot` `MySQL` `AWS API Gateway` `Python`

---

### [EduCraft](https://github.com/vmffotltka/PreCapstone) — 교내 공모전 🏆 우수상 (2024.08 – 2024.11)
> LLM 기반 맞춤형 학습 문제 생성 플랫폼 / 4인 팀 (BE 2, FE 2) / 백엔드 담당

- OpenAI API 연동 비동기 문제 생성 파이프라인 구축
- 비정형 LLM 응답 데이터를 MySQL에 구조화하는 RDB 모델링 설계

`Node.js` `MySQL` `OpenAI API` `AWS EC2`

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
