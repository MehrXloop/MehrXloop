<div align="center">

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=26&duration=3000&pause=1000&color=0EA5E9&center=true&vCenter=true&width=780&lines=Hi+%F0%9F%91%8B+I'm+Mehrunissa+Pirwani;DevOps+%26+Azure+Cloud+Engineer;AKS+%7C+Terraform+%7C+Helm+%7C+GitHub+Actions;Azure+Solutions+Architect+Expert+%C2%B7+AZ-305)](https://git.io/typing-svg)

**I deploy, secure and run production workloads on Microsoft Azure, from Kubernetes clusters to company-wide identity.**
Software Engineer II @ xLoop Digital Services, Karachi · Microsoft Certified: Azure Solutions Architect Expert · Azure Administrator Associate
Open to DevOps / Azure Cloud Engineer roles in Karachi 🇵🇰 and remote

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Mehrunissa%20Pirwani-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/mehr110/)
[![Email](https://img.shields.io/badge/Email-Contact%20me-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:mehrunissapirwani116@gmail.com)
[![AZ-305](https://img.shields.io/badge/Verify-AZ--305-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)](https://learn.microsoft.com/en-us/users/mehr-110/credentials/fe5cf63e3b327909)
[![AZ-104](https://img.shields.io/badge/Verify-AZ--104-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)](https://learn.microsoft.com/en-us/users/mehr-110/credentials/18cb17c0f9395e41)

</div>

---

## ⚡ At a glance

| | |
|---|---|
| ☁️ **Cloud** | Microsoft Azure: AKS, VMs, Static Web Apps, Blob Storage, Key Vault, Azure Monitor, Entra ID |
| 🚢 **Platform** | 10-microservice platform deployed on AKS with Helm, provisioned with Terraform |
| 🔁 **Delivery** | GitHub Actions pipelines with security scans and staging-to-production promotion |
| 🔐 **Security** | 70+ company devices secured with Entra ID, Intune, Conditional Access and Defender, mapped to ISO 27001 |
| 💰 **Cost** | ~$5,500 saved on Azure AI costs by moving to a 3-year Azure reservation |
| 🎓 **Certified** | AZ-305 Azure Solutions Architect Expert · AZ-104 Azure Administrator Associate |

---

## 🏗️ Selected work at xLoop

> The code for these projects belongs to my employer and is private. Happy to walk through the architecture and decisions in an interview.

### 🚢 QAITI: multi-tenant education platform on Azure Kubernetes Service

**My role:** DevOps engineer in a 3-person team, owning deployment and operations end to end.

| Layer | What I built and run |
|---|---|
| **Orchestration** | 10 microservices serving 7 user roles on **AKS**, each packaged as a **Helm** chart |
| **Infrastructure as Code** | **Terraform** for the AKS cluster, virtual networking and Key Vault; every change peer-reviewed before apply |
| **CI/CD** | **GitHub Actions**: static analysis, dependency scan and container-image scan run in parallel; only passing images are promoted from staging to production |
| **Secrets & access** | **Azure Key Vault** with managed identities and RBAC |
| **Observability** | **Prometheus + Grafana** for cluster and service metrics, **Azure Monitor** for Azure resources |
| **Reliability** | Backup and disaster-recovery procedures for platform data |

```mermaid
flowchart LR
    A[Push / pull request] --> B[GitHub Actions]
    B --> C[SAST]
    B --> D[Dependency scan]
    B --> E[Image scan]
    C --> F{All checks pass?}
    D --> F
    E --> F
    F -- yes --> G[Staging on AKS]
    G --> H[Production on AKS]
    F -- no --> X[Build blocked]
    T[Terraform] -. provisions .-> K[(AKS · VNet · Key Vault)]
    H --> M[Prometheus · Grafana · Azure Monitor]
```

### 💰 Azure cost optimisation

- Owned the budget for Azure-hosted AI models, compared on-demand and reserved pricing, and designed the supporting architecture.
- Moved the company to a **3-year Azure reservation**, saving **~$5,500**.

### 🔐 Microsoft 365, identity and endpoint security

- Enrolled **70+ Windows and Ubuntu laptops and phones** in **Intune**.
- Configured **Entra ID Conditional Access**, **BitLocker** with remote wipe, USB storage blocking, web filtering, **SSPR** and **Microsoft Defender**, mapped to **ISO 27001** controls.
- Wrote an **8-page Microsoft 365 and Entra ID licensing analysis** and briefed the CEO on the options.
- Designed a **Microsoft Purview eDiscovery** export of Exchange, Teams, SharePoint and OneDrive data, staged through Azure Blob Storage.

### 🎥 xVision: real-time AI monitoring for bank branches and ATMs

- **Release automation:** GitHub Actions pipeline deploying to **Azure Static Web Apps** on every push, with a preview environment for every pull request.
- **Containers:** multi-stage **Docker** build of the frontend, deployed on an **Azure VM**.
- **Frontend:** two linked Next.js/TypeScript dashboards covering 12 monitoring use cases, with live security alerts over 14 WebSocket streams and nonce-based CSP hardening.

### 🧠 GenAI readiness assessment platform (backend)

- **NestJS + PostgreSQL** backend with ~70 REST endpoints.
- **RAG pipeline** grounded in ISO/IEC 42001: OpenAI embeddings, Pinecone vector search, and automatic failover between LLM providers (OpenAI → Groq) so reports keep generating during outages.

---

## 🛠️ Tech stack

**Cloud & Infrastructure as Code**

![Azure](https://img.shields.io/badge/Microsoft_Azure-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Terraform](https://img.shields.io/badge/Terraform-7B42BC?style=for-the-badge&logo=terraform&logoColor=white)
![Linux](https://img.shields.io/badge/Linux_(Ubuntu)-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)
![AWS](https://img.shields.io/badge/AWS_fundamentals-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=FF9900)

**Containers & Orchestration**

![Kubernetes](https://img.shields.io/badge/Kubernetes_(AKS)-326CE5?style=for-the-badge&logo=kubernetes&logoColor=white)
![Helm](https://img.shields.io/badge/Helm-0F1689?style=for-the-badge&logo=helm&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![NGINX](https://img.shields.io/badge/NGINX-009639?style=for-the-badge&logo=nginx&logoColor=white)

**CI/CD & DevSecOps**

![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![SAST](https://img.shields.io/badge/SAST_%26_image_scanning-000000?style=for-the-badge&logo=githubactions&logoColor=white)

**Monitoring & Reliability**

![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=for-the-badge&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/Grafana-F46800?style=for-the-badge&logo=grafana&logoColor=white)
![Azure Monitor](https://img.shields.io/badge/Azure_Monitor-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)

**Identity & Security**

![Entra ID](https://img.shields.io/badge/Microsoft_Entra_ID-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![Intune](https://img.shields.io/badge/Microsoft_Intune-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![Defender](https://img.shields.io/badge/Microsoft_Defender-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![Key Vault](https://img.shields.io/badge/Azure_Key_Vault-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)

**Languages & Frameworks**

![Bash](https://img.shields.io/badge/Bash-4EAA25?style=for-the-badge&logo=gnubash&logoColor=white)
![PowerShell](https://img.shields.io/badge/PowerShell-5391FE?style=for-the-badge&logo=powershell&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=for-the-badge&logo=nestjs&logoColor=white)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)

---

## 📊 GitHub stats

<div align="center">

<img height="170em" src="https://github-readme-stats.vercel.app/api?username=MehrXloop&show_icons=true&theme=tokyonight&include_all_commits=true&count_private=true&hide_border=true"/>
<img height="170em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=MehrXloop&layout=compact&langs_count=8&theme=tokyonight&hide_border=true"/>

</div>

<div align="center">

[![GitHub Streak](https://streak-stats.demolab.com?user=MehrXloop&theme=tokyonight&hide_border=true)](https://git.io/streak-stats)

</div>

---

## 🏆 Certifications

[![AZ-305](https://img.shields.io/badge/Azure_Solutions_Architect_Expert_(AZ--305)-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)](https://learn.microsoft.com/en-us/users/mehr-110/credentials/fe5cf63e3b327909)
[![AZ-104](https://img.shields.io/badge/Azure_Administrator_Associate_(AZ--104)-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)](https://learn.microsoft.com/en-us/users/mehr-110/credentials/18cb17c0f9395e41)
[![AWS CCP](https://img.shields.io/badge/AWS_Cloud_Practitioner_(2023--2026)-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=FF9900)](https://www.credly.com/badges/11d98e44-f3b0-472f-bc4e-0069bc806164/public_url)
[![Emeritus](https://img.shields.io/badge/Cloud_Native_Development_(Emeritus)-1F4E79?style=for-the-badge&logo=googlecloud&logoColor=white)](https://drive.google.com/file/d/1R1vwQjtK2aJa6dMwrK2dsPRYFSGvTlvU/view)

---

## 🎓 Background

- 💼 **Software Engineer II** at xLoop Digital Services (Jul 2024 – present): DevOps and cloud infrastructure
- 💻 **Software Engineer** at xLoop Digital Services (Feb 2023 – Jun 2024): full-stack and AI development
- 🏛️ **BS Computer Science**, Virtual University of Pakistan (2023 – 2027, in progress) | CGPA 3.4 / 4.0
- 🥇 **Intermediate**: 95%, **8th position** in the Board of Intermediate Education Karachi

---

<div align="center">

*Infrastructure you can rebuild from code is infrastructure you can trust.*

![Profile Views](https://komarev.com/ghpvc/?username=MehrXloop&color=0EA5E9&style=for-the-badge)

</div>
