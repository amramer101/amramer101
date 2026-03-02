<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,50:00D4FF,100:7B2FBE&height=200&section=header&text=Amr%20Medhat%20Amer&fontSize=50&fontColor=ffffff&fontAlignY=38&desc=DevSecOps%20Engineer%20%7C%20Cloud%20Infrastructure%20%7C%20Multi-Cloud&descAlignY=58&descColor=00D4FF" />

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&pause=1000&color=00D4FF&center=true&vCenter=true&width=700&lines=Shifting+Security+Left+%E2%80%94+Every+Single+Pipeline;Zero+Plaintext+Credentials.+Ever.;IaC+%7C+CI%2FCD+%7C+DevSecOps+%7C+Multi-Cloud;Building+Infrastructure+That+Proves+Itself)](https://git.io/typing-svg)

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/amrmamer)
[![Portfolio](https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=netlify&logoColor=00D4FF)](https://wh0ami.netlify.app)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/amramer101)
[![Email](https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:amr.m.amer11@gmail.com)

</div>

---

## Who I Am

I'm a **DevSecOps Engineer** specializing in production-grade cloud infrastructure where **security isn't a checkbox — it's the pipeline itself.**

My philosophy is simple: every artifact that reaches production should have passed automated SAST, SCA, and IaC security gates. No exceptions. No shortcuts.

I don't just deploy to the cloud — I migrate architectures through it, phase by phase, proving every decision with working infrastructure and real numbers.

```
"A pipeline without security gates isn't CI/CD — it's just fast shipping of problems."
```

### Recognition

- 🏆 **1st Place** — Huawei Cloud Spark Infinity 2025, North Africa · 389 teams · First Egyptian team to win
- 🥉 **Bronze Medal** — Huawei ICT Competition 2025-2026, Cloud Track · 3,146 participants nationally
- 🎓 **Top 18%** — Aspire Leaders Program, Harvard Business School & Aspire Institute · 54,000+ applicants
- 🏅 **Top 5 (1%)** — Huawei Developer Competition 2024, North Africa · 650+ teams

---

## Flagship Project — Strata-Ops 🔴 Active Development

> *A complete, multi-phase DevSecOps migration of a production 5-tier Java application — from bare VMs to fully managed AWS PaaS — with security enforcement at every layer.*

This isn't a tutorial clone. It's a real architecture that broke in real ways and got fixed with real solutions.

```
┌─────────────────────────────────────────────────────────────────┐
│                     STRATA-OPS JOURNEY                          │
├──────────────┬──────────────────────────────────────────────────┤
│   Phase 1    │  Manual → Automated                              │
│   ✅ Done     │  Vagrant + Bash · 60 min → 15 min               │
├──────────────┼──────────────────────────────────────────────────┤
│   Phase 2    │  AWS Lift & Shift + Full CI/CD                   │
│   ✅ Done     │  Terraform · Jenkins JCasC · SonarQube           │
│              │  Nexus · OWASP SCA · tfsec · SSM Secrets         │
├──────────────┼──────────────────────────────────────────────────┤
│   Phase 3    │  AWS Cloud Native + IaC Security                 │
│   ✅ Done     │  RDS · ElastiCache · MQ · Beanstalk              │
│              │  CodePipeline · 45 min → 10 min deploy           │
├──────────────┼──────────────────────────────────────────────────┤
│   Phase 4    │  Containerization + Image Security               │
│   🔴 Active  │  Docker · Trivy · Extending DevSecOps coverage   │
└──────────────┴──────────────────────────────────────────────────┘
```

**Security decisions built into the architecture:**

| Decision | Why It Matters |
|---|---|
| **AWS SSM Parameter Store** for all secrets | Zero plaintext credentials in code, pipeline, or config — ever |
| **OWASP Dependency-Check** as hard pipeline blocker | `failedTotalCritical: 0` — Critical CVE = build dies |
| **SonarQube Quality Gate** as hard pipeline blocker | Bad code never reaches Nexus |
| **tfsec in CodeBuild** | IaC misconfigurations blocked before deployment |
| **Jenkins JCasC** | Entire Jenkins instance provisioned from code — zero manual UI |
| **Route53 Private DNS** | Backend services never internet-exposed, DNS-abstracted |
| **Least-privilege IAM** scoped to `/strata-ops/*` | EC2 can't touch anything outside its namespace |
| **Terraform remote state on S3** | Infrastructure state is versioned and team-shareable |

**Real problems solved (not from a tutorial):**
- Diagnosed `Tomcat 10` package non-existence on Ubuntu 22.04 → migrated to Tomcat 9
- Resolved `Nexus 3.78.0` EULA API lockout blocking all automation → patched via `nexus.onboarding.enabled=false` pre-boot flag
- Fixed JCasC `UnknownAttributesException` for `dependencyCheck` tool configuration

[![Strata-Ops](https://img.shields.io/badge/View_Strata--Ops-FF9900?style=for-the-badge&logo=amazon-aws&logoColor=white)](https://github.com/amramer101/Strata-Ops)

---

## Other Projects

<table>
<tr>
<td width="50%">

### Conduit — AWS ECS GitOps CI/CD Engine
`GitHub Actions` `ECS Fargate` `ECR` `RDS Aurora` `SonarCloud` `ALB`

Production-grade GitOps pipeline for a Java Spring social platform.

- 3-stage pipeline: Test → Build → Deploy, fully automated
- SonarCloud SAST blocking on quality gate failure
- Docker images versioned by GitHub run number in ECR
- Zero-downtime rolling updates on ECS Fargate
- RDS Aurora in private subnets, security-group restricted

[![Conduit](https://img.shields.io/badge/View_Project-2496ED?style=flat-square&logo=docker&logoColor=white)](https://github.com/amramer101/hprofile-actions)

</td>
<td width="50%">

### Vulnera — Cloud-Native Security on Huawei Cloud
`Kubernetes CCE` `CodeArts CI/CD` `ModelArts` `L7 Load Balancing`

DevSecOps platform on Huawei Cloud for supply chain vulnerability aggregation.

- 3-node Kubernetes cluster with L7 Load Balancing
- 85% faster release cycles via automated pipeline
- ModelArts AI threat analysis with RDS PostgreSQL persistence
- IAM access controls cutting operational costs by 40%
- 🏆 Winning project — Spark Infinity Competition

[![Vulnera](https://img.shields.io/badge/View_Project-FF0000?style=flat-square&logo=huawei&logoColor=white)](https://github.com/amramer101/Vulnera-Azure)

</td>
</tr>
<tr>
<td width="50%">

### FinOps Sentinel — Serverless Cost Governance on Azure
`Azure Functions` `Logic Apps` `Terraform` `Managed Identity` `Python`

Automated FinOps governance engine that hunts and eliminates cloud waste.

- Scans every 6 hours for idle VMs, unattached disks, orphaned IPs
- $2,000+/month waste identified across 50+ flagged resources
- 100% cost attribution via Terraform tagging policies
- Zero-credential drift via Managed Identity (no service principals)
- Automated HTML reports delivered via Logic Apps in under 3 minutes

[![FinOps](https://img.shields.io/badge/View_Project-0078D4?style=flat-square&logo=microsoft-azure&logoColor=white)](https://github.com/amramer101/Azure-FinOps-Sentinel)

</td>
<td width="50%">

### Bravo6 — Serverless Threat Recon Engine on AWS
`Lambda` `Step Functions` `DynamoDB` `API Gateway` `WAF` `Amplify`

High-throughput parallel security recon system built on AWS serverless.

- Step Functions orchestrating concurrent Lambda executions
- SSL validation, DNS analysis, HTTP header assessment in parallel
- 75% reduction in scan latency vs sequential approach
- WAF + fine-grained IAM + CloudWatch observability
- Entire infrastructure within AWS Free Tier limits

[![Bravo6](https://img.shields.io/badge/View_Project-FF9900?style=flat-square&logo=amazon-aws&logoColor=white)](https://github.com/amramer101/Bravo6)

</td>
</tr>
</table>

---

## Tech Stack

<div align="center">

### Cloud Platforms
![AWS](https://img.shields.io/badge/AWS-FF9900?style=flat-square&logo=amazon-aws&logoColor=white)
![Azure](https://img.shields.io/badge/Azure-0078D4?style=flat-square&logo=microsoft-azure&logoColor=white)
![GCP](https://img.shields.io/badge/GCP-4285F4?style=flat-square&logo=google-cloud&logoColor=white)
![Huawei Cloud](https://img.shields.io/badge/Huawei_Cloud-FF0000?style=flat-square&logo=huawei&logoColor=white)

### Infrastructure as Code & Automation
![Terraform](https://img.shields.io/badge/Terraform-623CE4?style=flat-square&logo=terraform&logoColor=white)
![Ansible](https://img.shields.io/badge/Ansible-EE0000?style=flat-square&logo=ansible&logoColor=white)
![Bash](https://img.shields.io/badge/Bash-4EAA25?style=flat-square&logo=gnu-bash&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![PowerShell](https://img.shields.io/badge/PowerShell-5391FE?style=flat-square&logo=powershell&logoColor=white)

### CI/CD & DevSecOps
![Jenkins](https://img.shields.io/badge/Jenkins_JCasC-D24939?style=flat-square&logo=jenkins&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=flat-square&logo=github-actions&logoColor=white)
![AWS CodePipeline](https://img.shields.io/badge/CodePipeline-FF9900?style=flat-square&logo=amazon-aws&logoColor=white)
![SonarQube](https://img.shields.io/badge/SonarQube-4E9BCD?style=flat-square&logo=sonarqube&logoColor=white)
![OWASP](https://img.shields.io/badge/OWASP_DC-000000?style=flat-square&logo=owasp&logoColor=white)
![tfsec](https://img.shields.io/badge/tfsec-326CE5?style=flat-square&logo=terraform&logoColor=white)
![Trivy](https://img.shields.io/badge/Trivy-1904DA?style=flat-square&logo=aqua&logoColor=white)

### Containers & Orchestration
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Helm](https://img.shields.io/badge/Helm-0F1689?style=flat-square&logo=helm&logoColor=white)
![ECS Fargate](https://img.shields.io/badge/ECS_Fargate-FF9900?style=flat-square&logo=amazon-aws&logoColor=white)

### Observability & Security
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)
![CloudWatch](https://img.shields.io/badge/CloudWatch-FF9900?style=flat-square&logo=amazon-aws&logoColor=white)
![AWS SSM](https://img.shields.io/badge/AWS_SSM-FF9900?style=flat-square&logo=amazon-aws&logoColor=white)
![Key Vault](https://img.shields.io/badge/Key_Vault-0078D4?style=flat-square&logo=microsoft-azure&logoColor=white)

</div>

---

## Certifications

<div align="center">

| | Certification | Issuer | Year |
|---|---|---|---|
| ☁️ | AWS Certified Solutions Architect – Associate (SAA-C03) | Amazon Web Services | 2026 |
| 🔵 | Azure Administrator Associate (AZ-104) | Microsoft | 2025 |
| 🔒 | Security, Compliance, and Identity (SC-900) | Microsoft | 2025 |
| 🛡️ | Junior Cybersecurity Analyst – CyberOps | Cisco | 2024 |
| 🔐 | Certified in Cybersecurity (CC) | ISC2 | 2024 |
| ⚙️ | DevOps Path: Jenkins · Ansible · Terraform · Docker · K8s | KodeKloud | 2024 |

</div>

---

<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:7B2FBE,50:00D4FF,100:0D1117&height=120&section=footer"/>

</div>
