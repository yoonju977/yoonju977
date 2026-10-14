## Yoonju Song (송윤주)

**Cloud Engineer (New Grad)**, AWS, CloudFormation, Docker, GitHub Actions

I design AWS infrastructure, automate deployments, and operate services with real users. My most recent service ran 50 hours for 786 beta users with zero downtime.

Looking for new-grad Cloud, DevOps, or Platform Engineer roles.

[Portfolio](https://yoonju977.github.io/Portfolio/?view=pc)

&nbsp;

### Selected Work

**MeDeviSe**: hospital recommendations from plain-language symptoms &nbsp; `2025.04 – 2025.09` &nbsp; [Repo](https://github.com/Medic-chatbot/Backend)<br>
**KAIST SW Education Center** &nbsp; *Team lead, owning infrastructure and model serving, in a team of 5 (BE 1, AI 2, FE 1, Data 1)*
- Fargate has no GPU support, so I moved only the inference container to EC2 g4dn and routed `/ml/*` and `/api/*` through one ALB. The 50-hour beta served **786 users with zero downtime**.
- Defined 3 ECS capacity providers (Fargate, Fargate Spot, EC2 Auto Scaling group) in CloudFormation. I ran them with ALB health checks, 1–2 instances, and CloudWatch.
- Added automatic rollback to GitHub Actions and wrote a deploy runbook, so all 5 team members released the same way.

`AWS ECS` `EC2 g4dn` `ALB` `Auto Scaling` `CloudFormation` `GitHub Actions` `Docker`

**BowwoW_Care**: pet healthcare app with 8 features (graduation thesis at **Hankuk University of Foreign Studies**, 2nd place in department capstone) &nbsp; `2025.02 – 2025.06` &nbsp; [Backend](https://github.com/BeThePet/Backend) · [Frontend](https://github.com/BeThePet/Frontend)<br>
*Team lead, owning infrastructure and model serving, in a team of 8 (BE 1, FE 2, AI 4)*
- Split the system into 5 Docker containers on ECS Fargate with Blue-Green deployment. A 3-day launch served **103 users with zero incidents**.
- Before building features, I set up security and monitoring: WAF managed rules and rate limiting, a private VPC subnet, Nginx TLS/HSTS, ECR image scanning, CloudWatch, and Whatap.
- Load-tested with Locust up to **500 virtual users**: 0 failures and P50 at 35 ms or less. P95 rose to 180 ms past 300 users, which I traced to GPT-4 response latency.

`AWS ECS Fargate` `ECR` `WAF` `VPC` `CloudWatch` `Nginx` `Locust`

**Security re-audit of my own services** &nbsp; `2026.09`
- Rescanned 3 of my repositories with Semgrep (SAST) and pip-audit (SCA). Reduced **23 SAST findings to 0 and 38 vulnerable packages to 0**.
- Pinned GitHub Actions to commit SHAs, switched containers to a non-root user, and replaced the unpatched python-jose with PyJWT.

`Semgrep` `pip-audit` `Dependabot`

**Nurse Training Checklist**: in production at **Korea University Hospital**, Department of Nursing &nbsp; `2026.04 – 2026.06` &nbsp; *Private repo (live service)*<br>
*Solo developer working with the hospital's planner*
- The hospital required no server or DB, so I built a serverless setup: GitHub Pages, Google Apps Script, and Google Drive storage. About **30 new nurses use it each quarter**.

`GitHub Pages` `GitHub Actions` `Google Apps Script` `React`

&nbsp;

### Skills

**AWS** &nbsp; ECS (Fargate, EC2), ALB, Auto Scaling, VPC, WAF, ECR, RDS, S3, CloudWatch<br>
**IaC & CI/CD** &nbsp; CloudFormation, GitHub Actions (Blue-Green, auto rollback)<br>
**Containers & Networking** &nbsp; Docker, Nginx<br>
**Security** &nbsp; Semgrep, pip-audit, Dependabot<br>
**Backend & Data** &nbsp; Python, FastAPI, Django, PostgreSQL, Redis

### Certifications & Education

- AWS Certified Solutions Architect – Associate (2026)
- SQL Developer (SQLD), **Korea Data Agency** (2025)
- B.S. Biomedical Engineering, minor in Computer Engineering, **Hankuk University of Foreign Studies** (2025)
- Seocho AI College, **KAIST SW Education Center** (2025). Backend Bootcamp, 960 hours (2024)

<sub>Before switching to software, I spent 6 years and 8 months in customer operations at the **Korea Racing Authority**. I standardized desk procedures there and cut repeat complaints from 4–5 a week to 0–1.</sub>

&nbsp;

<details>
<summary><b>한국어 소개</b></summary>

&nbsp;

**신입 클라우드 엔지니어 송윤주**입니다. AWS 인프라를 설계하고 배포를 자동화해 실제 사용자 앞에서 서비스를 운영합니다.

- **MeDeviSe** (2025, **KAIST SW교육센터**): Fargate가 GPU를 지원하지 않아 추론 서버만 EC2 g4dn으로 분리했고 CloudFormation으로 인프라를 코드화했습니다. 베타 50시간 동안 실사용자 786명을 장애 없이 받았습니다.
- **반려견 통합 헬스케어 시스템** (2025, **한국외국어대학교** 학위논문, 8인 팀장): ECS Fargate에 Blue-Green 배포로 3일간 103명을 받았고 장애는 0건이었습니다. 기능 개발 전에 WAF, VPC, 모니터링부터 갖췄습니다.
- **보안 재점검** (2026.09): 세 서비스의 정적 분석 경고 23건과 취약 패키지 38개를 모두 조치했습니다.
- **신규간호사 교육 체크리스트** (2026, **고려대학교병원** 실사용): 서버와 DB 없이 구성했고 분기마다 신규간호사 약 30명이 사용합니다.

AWS SAA, SQLD 보유. 개발 전에는 **한국마사회** 고객 접점에서 6년 8개월 근무했습니다.<br>
포트폴리오: [yoonju977.github.io/Portfolio](https://yoonju977.github.io/Portfolio/?view=pc)

</details>
