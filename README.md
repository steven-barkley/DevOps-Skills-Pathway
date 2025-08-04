# DevOps-Skills-Pathway
A development journal and performance accountability log 

**August 1st - January 1st**

## What to prioritize (from your libraries)

**Linux + Git (weeks 1–3)**

- ZTM **DevOps Bootcamp: Learn Linux & Become a Linux Sysadmin** (Linux sections)
- ZTM **Bash Scripting: Learn Shell Scripting**
- *Learning Git* (O’Reilly) quick-read to support daily Git flow

**Python for automation (weeks 2–5)**

- **100 Days of Code – Python** → do **Days 1–20 only** (fundamentals, files, CLI).
- ZTM **Python Automation Bootcamp (Work Smarter)** for DevOps-style scripts.

**Containers & CI/CD (weeks 4–7)**

- Udemy **Python REST APIs with Flask, Docker, MongoDB & AWS DevOps** (use to create the app you’ll ship)
- ZTM **DevOps Bootcamp: Terraform** (do Docker intro module if present)
- Docker docs + *Docker: Up & Running (3e)* Ch. 1–6 for depth
- GitHub Actions basics (free docs) to build/test/push

**Cloud + IaC (weeks 6–11)**

- Stephane Maarek **AWS Certified Solutions Architect Associate** (you’re 100%—use as reference)
- Stephane Maarek **AWS Certified Developer Associate** (skim the services you’ll use: IAM, S3, EC2/ECS, CloudWatch, Lambda)
- *Terraform: Up & Running (3e)* Ch. 1–4 → modules/state/workspaces
- Deploy via Terraform + GitHub OIDC

**Kubernetes (weeks 10–13)**

- *Kubernetes: Up & Running (3e)* Ch. 1–6
- Local **kind/k3d** cluster, manifests, then Helm

**Config mgmt & hardening (weeks 12–15)**

- *Ansible: Up & Running (3e)* basics (inventory, roles)
- *Learning DevSecOps* + add **Trivy** image & IaC scans to CI
- *Web Application Security* → read OWASP-related chapters

**Interview polish (weeks 16–18)**

- Revisit Stephane Maarek **DOP-C02 DevOps Engineer Professional** **exam guide & practice tests only** (don’t deep-dive the whole course now). Use it to shape interview answers and vocabulary.

---

## What to **defer** (for now)

- CompTIA Net+, Sec+ practice sets (good later, not required for entry DevOps).
- AWS ML/Bedrock/Machine Learning tracks.
- Network Programmability & Automation (Cisco-heavy; revisit post-hire).
- Full 100 Days of Python past Day 20.

Save some ideas for the rest of us—this restraint is elite. 💅

---

## Skill → Course mapping (quick lookup)

- **Linux/Bash:** ZTM Linux Bootcamp; ZTM Bash Scripting.
- **Git/GitHub:** *Learning Git* + daily commits/PRs.
- **Python automation:** 100 Days (1–20), ZTM Python Automation.
- **Docker/Compose:** *Docker: Up & Running* + Flask app course.
- **CI/CD:** GitHub Actions (lint/test/build/push; later Terraform plan/apply).
- **AWS core:** Maarek SAA & DVA lectures (service overviews + hands-on).
- **IaC:** *Terraform: Up & Running* + ZTM Terraform.
- **Kubernetes:** *Kubernetes: Up & Running* + kind/Helm labs.
- **Config mgmt:** *Ansible: Up & Running* (one host role).
- **Security:** *Learning DevSecOps*, *Web App Security* + Trivy, pre-commit, OIDC.

---

## Aug–Dec weekly path (18 weeks)

**Wk 1–2 (Aug)** – Linux/Git setup

- ZTM Linux modules + Bash scripting basics.
- Daily Git: branch → commit → PR → merge.
- Output: `lab-notes` repo + `dotfiles`.

**Wk 3–4** – Python foundations → automation

- 100 Days (1–20).
- Automate: log rotation, CSV→JSON, simple CLI.
- Output: `devops-utils` repo.

**Wk 5–6** – Dockerize an app & CI

- Build Flask (or FastAPI) health service.
- Dockerfile + docker-compose; push to Docker Hub.
- GitHub Actions: lint/test/build/push on tag.
- **KubeCraft**: container challenge.

**Wk 7–9 (Sept)** – Terraform + AWS deploy

- *Terraform Up & Running* Ch.1–4.
- Provision VPC, EC2, S3, DynamoDB (state lock).
- OIDC from GitHub Actions to AWS; `plan` on PR, `apply` on main.
- Deploy your container to **ECS Fargate** (simpler than EKS first).

**Wk 10–12 (Oct)** – Kubernetes fluency

- kind cluster; write Deployment/Service/Ingress + HPA.
- Helm (basic Chart) to package app.
- Output: `k8s-app-with-hpa` repo + Makefile.

**Wk 13–14** – Ansible + host bootstrap

- Inventory, role to harden Ubuntu (users, ufw, Docker, fail2ban).
- Use Ansible to prep an EC2 box; compare with Terraform user_data.

**Wk 15–16 (Nov)** – DevSecOps

- Add **Trivy** (image + IaC scans) to CI, **pre-commit** hooks, secret scanning.
- Tighten IAM least-priv for OIDC; add CloudWatch logs/alarms.

**Wk 17–18 (Dec)** – Portfolio + interviews

- Polish 3 repos (Docker template, Terraform infra, K8s app).
- 2–3 short demo videos.
- Mock interview with Jeff; apply to 5–10 roles.

**Cadence:** Mon-Thu learn/build (90+90), Fri ship, Sat 2–3h project, Sun retro & plan.

**Validation each month:** 1 **KubeCraft** task + mentor review.

---

## Minimal project set (what you’ll show recruiters)

1. **docker-fastapi-template** — app, tests, Compose, CI build/push.
2. **terraform-aws-foundations** — VPC/EC2/ECS/S3, remote state, OIDC CI.
3. **k8s-app-with-hpa** — manifests/Helm, Ingress, HPA, Makefile.
4. **ansible-linux-bootstrap** — secure base role.

Each README: diagram, “how to run,” CI badges, security section, and costs note.

---
