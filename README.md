# Amr Medhat Amer
### DevSecOps Engineer · Cloud Infrastructure · Multi-Cloud

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/amrmamer)
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=flat-square&logo=netlify&logoColor=white)](https://wh0ami.netlify.app)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/amramer101)
[![Email](https://img.shields.io/badge/Gmail-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:amr.m.amer11@gmail.com)

---

I build production-grade cloud infrastructure where **security isn't a checkbox — it's the pipeline itself.**

Every artifact that reaches production has passed automated SAST, SCA, and IaC security gates. No exceptions. No shortcuts. I don't just deploy to the cloud — I architect through it, phase by phase, proving every decision with working infrastructure and real numbers.

> *"A pipeline without security gates isn't CI/CD — it's just fast shipping of problems."*

---

## Recognition

| | |
|---|---|
| 🏆 **1st Place** | Huawei Cloud Spark Infinity 2025, North Africa · 389 teams · First Egyptian team to win |
| 🥉 **Bronze Medal** | Huawei ICT Competition 2025-2026, Cloud Track · 3,146 participants nationally |
| 🎓 **Top 18%** | Aspire Leaders Program, Harvard Business School & Aspire Institute · 54,000+ applicants |
| 🏅 **Top 5 (1%)** | Huawei Developer Competition 2024, North Africa · 650+ teams |

---

## Flagship Project — Strata-Ops ✅ Complete

> *A production-grade, multi-phase DevSecOps migration of a 5-tier Java application — from bare VMs to fully managed AWS cloud-native — with security enforcement at every layer.*

**[→ View Strata-Ops on GitHub](https://github.com/amramer101/Strata-Ops)**

This is not a tutorial clone. It's a real architecture that broke in real ways and got fixed with real solutions.

```
┌──────────────────────────────────────────────────────────────────┐
│                        STRATA-OPS JOURNEY                        │
├──────────────┬───────────────────────────────────────────────────┤
│   Phase 1    │  Manual → Automated                               │
│   ✅ Done     │  Vagrant + Bash · 60 min → 15 min                │
├──────────────┼───────────────────────────────────────────────────┤
│   Phase 2    │  AWS Lift & Shift + Full CI/CD                    │
│   ✅ Done     │  Terraform · Jenkins JCasC · SonarQube            │
│              │  Nexus · OWASP SCA · tfsec · SSM Secrets          │
├──────────────┼───────────────────────────────────────────────────┤
│   Phase 3    │  AWS Cloud-Native + IaC Security                  │
│   ✅ Done     │  RDS · ElastiCache · MQ · Beanstalk               │
│              │  CodePipeline · TruffleHog · SonarCloud           │
├──────────────┼───────────────────────────────────────────────────┤
│   Phase 4.1  │  Containerization + Ansible Automation            │
│   ✅ Done     │  Docker Compose · Ansible · EC2 Single Host       │
├──────────────┼───────────────────────────────────────────────────┤
│   Phase 4.2  │  ECS Fargate + GitOps + Full Observability        │
│   ✅ Done     │  GitHub Actions · Trivy · Datadog APM             │
│              │  Firelens · SARIF → GitHub Security · SSM         │
└──────────────┴───────────────────────────────────────────────────┘
```

**Architecture evolution at a glance:**

| Aspect | Phase 1 | Phase 2 | Phase 3 | Phase 4.1 | Phase 4.2 |
|--------|---------|---------|---------|-----------|-----------|
| Platform | VirtualBox | EC2 | Elastic Beanstalk | EC2 + Docker | ECS Fargate |
| Database | Manual MySQL | EC2 MySQL | RDS MySQL | Docker MySQL | RDS MySQL |
| Deployment | Manual SSH | Terraform | CodePipeline | Terraform + Ansible | GitHub Actions |
| Security | None | Basic SGs | 3-Layer Scan | Basic SGs | Trivy + GHAS |
| Observability | None | Prometheus + Grafana | CloudWatch | None | Datadog Full Stack |
| Manual Steps | 50+ | 0 | 0 | 0 | 0 |
| Cost/month | $0 | ~$70 | ~$170 | ~$20 | ~$178 |

**Security decisions built into the architecture:**

| Decision | Why It Matters |
|---|---|
| **AWS SSM Parameter Store** for all secrets | Zero plaintext credentials in code, pipeline, or config — ever |
| **OWASP Dependency-Check** as hard pipeline blocker | `failedTotalCritical: 0` — Critical CVE = build dies |
| **SonarQube Quality Gate** as hard pipeline blocker | Bad code never reaches Nexus |
| **TruffleHog + tfsec** in CodeBuild | Secrets and IaC misconfigs blocked before deployment |
| **Trivy** at 3 scan layers (FS + Config + Image) | CVE visibility at every stage, reported via SARIF to GitHub |
| **Jenkins JCasC** | Entire Jenkins instance provisioned from code — zero manual UI |
| **Route53 Private DNS** | Backend services never internet-exposed, DNS-abstracted |
| **Least-privilege IAM** scoped to `/strata-ops/*` | EC2 can't touch anything outside its namespace |
| **Datadog APM + Firelens sidecar** | Full traces, JVM metrics, and log routing from ECS containers |

**Real problems solved (not from a tutorial):**
- Diagnosed `Tomcat 10` package non-existence on Ubuntu 22.04 → migrated to Tomcat 9
- Resolved Nexus 3.78.0 EULA API lockout blocking all automation → patched via `nexus.onboarding.enabled=false` pre-boot flag
- Fixed JCasC `UnknownAttributesException` for `dependencyCheck` tool configuration
- Fixed container race condition with health-aware `depends_on` chains across all 5 services
- Fixed Memcached blind healthcheck on Alpine — pure bash `/dev/tcp` probe with no `nc` binary

---

## Other Projects

### Conduit — AWS ECS GitOps CI/CD Engine
**[→ View on GitHub](https://github.com/amramer101/hprofile-actions)**

`GitHub Actions` `ECS Fargate` `ECR` `RDS Aurora` `SonarCloud` `ALB`

Production-grade GitOps pipeline for a Java Spring social platform. 3-stage pipeline (Test → Build → Deploy) with SonarCloud SAST blocking on quality gate failure. Docker images versioned by git run number in ECR. Zero-downtime rolling updates on ECS Fargate with RDS Aurora in private subnets, security-group restricted.

---

### Vulnera — Cloud-Native Security on Huawei Cloud
**[→ View on GitHub](https://github.com/amramer101/Vulnera-Azure)**

`Kubernetes CCE` `CodeArts CI/CD` `ModelArts` `L7 Load Balancing` `RDS PostgreSQL`

DevSecOps platform on Huawei Cloud for supply chain vulnerability aggregation. 3-node Kubernetes cluster with L7 load balancing. 85% faster release cycles via automated pipeline. ModelArts AI threat analysis with RDS PostgreSQL persistence. IAM access controls cutting operational costs by 40%. **🏆 Winning project — Spark Infinity Competition 2025.**

---

### FinOps Sentinel — Serverless Cost Governance on Azure
**[→ View on GitHub](https://github.com/amramer101/Azure-FinOps-Sentinel)**

`Azure Functions` `Logic Apps` `Terraform` `Managed Identity` `Python`

Automated FinOps governance engine that hunts and eliminates cloud waste. Scans every 6 hours for idle VMs, unattached disks, and orphaned IPs. $2,000+/month waste identified across 50+ flagged resources in week one. 100% cost attribution via Terraform tagging policies. Zero-credential drift via Managed Identity — no service principals. Automated HTML reports delivered via Logic Apps in under 3 minutes.

---

### CloudDrop — Enterprise Serverless File Sharing on AWS
**[→ View on GitHub](https://github.com/amramer101/-CloudDrop)**

`AWS Lambda` `API Gateway` `S3` `CloudFront` `Amplify` `GitHub Actions` `ECR` `Docker`

Production-ready serverless file-sharing platform on AWS. CloudFront CDN with 400+ edge locations. End-to-end AES-256 + TLS 1.3 encryption. GitHub Actions CI/CD pipeline cutting deployment time from 45 min to 7 min (85% faster). 99.5% uptime with 20% latency reduction. Zero-downtime blue-green deployments.

---

## Tech Stack

**Cloud:** AWS · Azure · GCP · Huawei Cloud

**IaC & Automation:** Terraform · Ansible · Bash · Python · PowerShell

**CI/CD & DevSecOps:** Jenkins JCasC · GitHub Actions · AWS CodePipeline · SonarQube · SonarCloud · OWASP Dependency-Check · tfsec · TruffleHog · Trivy · GitHub Advanced Security (SARIF)

**Containers & Orchestration:** Docker · Docker Compose · Kubernetes · Helm · ECS Fargate

**Observability & Security:** Prometheus · Grafana · Datadog APM · CloudWatch · AWS SSM · Azure Key Vault · Firelens (Fluent Bit)

**Managed Services:** RDS · ElastiCache · Amazon MQ · Elastic Beanstalk · AWS Lambda · Azure Functions

---

## Certifications

| | Certification | Issuer | Year |
|---|---|---|---|
| ☁️ | AWS Certified Solutions Architect – Associate (SAA-C03) | Amazon Web Services | 2026 |
| 🔵 | Azure Administrator Associate (AZ-104) | Microsoft | 2025 |
| 🔒 | Security, Compliance, and Identity (SC-900) | Microsoft | 2025 |
| 🛡️ | Junior Cybersecurity Analyst – CyberOps | Cisco | 2024 |
| 🔐 | Certified in Cybersecurity (CC) | ISC2 | 2024 |
| ⚙️ | DevOps Path: Jenkins · Ansible · Terraform · Docker · K8s | KodeKloud | 2024 |
