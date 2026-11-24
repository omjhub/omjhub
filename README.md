# Hi, I'm Omajuwa 👋

**DevSecOps and Cloud Security Engineer** | AWS, Azure, Terraform, Kubernetes | London, UK

I build security into how software is shipped: CI/CD pipelines where security checks block bad releases, hardened cloud infrastructure in Terraform, and detection and response that works when it matters. Over five years building and deploying software, including over three years focused on DevSecOps and cloud security. MSc Computer Forensics and Cybersecurity (Distinction), University of Greenwich.

🟢 **Open to DevSecOps, Cloud Security and Application Security Engineer roles. Available immediately.**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Omajuwa_Okotie-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/omajuwa-okotie-850950190)
[![Portfolio](https://img.shields.io/badge/Portfolio-omajuwaokotie.com-222222?logo=googlechrome&logoColor=white)](https://omajuwaokotie.com)
[![Email](https://img.shields.io/badge/Email-okotieomajuwa2016%40gmail.com-D14836?logo=gmail&logoColor=white)](mailto:okotieomajuwa2016@gmail.com)

---

## Featured projects

### 🚀 [SecureX](https://github.com/omjhub/SecureX): Production-Grade DevSecOps Platform on Amazon EKS
A Node.js and MySQL application delivered to Amazon EKS through a 14-job GitHub Actions pipeline where every security check **blocks** a bad release. Separate QA and production environments, production runs the exact image QA tested, and there are no stored cloud keys anywhere.
- Dependency vulnerabilities **25 to 0**, test coverage **0% to 86.3%** (31 Jest and Supertest tests)
- Gitleaks, Checkov, Trivy and SonarQube gates, each **proven by a deliberate failure**
- GitHub OIDC, AWS Secrets Manager, External Secrets Operator and IRSA; protected `main` with **7 required checks**
- Hardened pods (non-root, read-only filesystem, dropped capabilities), Prometheus, Loki and Grafana monitoring

`Amazon EKS` `GitHub Actions` `Gitleaks` `Checkov` `Trivy` `SonarQube` `Syft` `Helm` `IRSA` `Route 53` `ACM`

### 🔐 [SecureFlow](https://github.com/omjhub/SecureFlow-VulnerableCodebase): Secure CI/CD Pipeline for a Banking Platform
A seven-stage pipeline securing a vulnerable banking microservices codebase. Terraform security findings reduced from **72 to 0**, and a live pull request was automatically blocked on **275 findings** across secret, image and IaC scans.

`Gitleaks` `SonarQube` `Trivy` `Checkov` `HashiCorp Vault` `OPA Gatekeeper` `Falco` `Prometheus` `Grafana`

### 🏦 [SentinelPay](https://github.com/sentinelpay-team/Sentinelpay): Securing an Inherited Fintech Platform (Security Team Lead)
Led a five-person team through STRIDE threat modelling, remediation of SQL injection, JWT bypass, IDOR and a race condition, CI/CD hardening and software supply chain controls (CycloneDX SBOMs, Cosign signing) ahead of a timed attack simulation.

`Semgrep` `Bandit` `Gitleaks` `Trivy` `Checkov` `tfsec` `KMS` `GuardDuty` `Security Hub` `Syft` `Cosign`

### ☁️ [VaultBridge](https://github.com/omjhub/vaultbridge-iac-modernisation): Three-Tier AWS Infrastructure as Code
A three-tier AWS architecture in Terraform fixing the root cause of a $214,000 incident in the client brief: security-group-only database access, a validation rule rejecting any SSH rule broader than /32, and a tfsec and Checkov pipeline with review before apply.

`Terraform` `AWS` `GitHub Actions` `tfsec` `Checkov`

### 🛡️ [Cloud Threat Detection with Microsoft Sentinel](https://github.com/omjhub/cloudscale-sentinel-soc-poc): SIEM/SOAR
Credential compromise detection-to-response cut from **4+ hours to under 5 minutes**, with a custom KQL rule and a Logic Apps playbook firing within 13 seconds.

`Microsoft Sentinel` `KQL` `Logic Apps` `Microsoft Entra ID` `Azure RBAC`

### 🕵️ [Detecting Vulnerabilities in Web Applications](https://github.com/omjhub/Detecting-Vulnerabilities-In-Web-Applications): MSc Dissertation
A Python tool extending OWASP ZAP with baseline differential response verification, converting two of ZAP's three false negatives into confirmed true positives with zero new false positives.

`Python` `OWASP ZAP` `DVWA` `OWASP Juice Shop`

---

## Toolbox

**Cloud and IaC:**
![AWS](https://img.shields.io/badge/-AWS-FF9900?style=flat-square&logo=amazonwebservices&logoColor=white)
![Amazon EKS](https://img.shields.io/badge/-Amazon_EKS-FF9900?style=flat-square&logo=amazoneks&logoColor=white)
![Azure](https://img.shields.io/badge/-Azure-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![Terraform](https://img.shields.io/badge/-Terraform-7B42BC?style=flat-square&logo=terraform&logoColor=white)
![Kubernetes](https://img.shields.io/badge/-Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Helm](https://img.shields.io/badge/-Helm-0F1689?style=flat-square&logo=helm&logoColor=white)
![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

**CI/CD and security scanning:**
![GitHub Actions](https://img.shields.io/badge/-GitHub_Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![SonarQube](https://img.shields.io/badge/-SonarQube-4E9BCD?style=flat-square&logo=sonarqube&logoColor=white)
![Trivy](https://img.shields.io/badge/-Trivy-1904DA?style=flat-square&logo=aquasecurity&logoColor=white)
![Checkov](https://img.shields.io/badge/-Checkov-00549E?style=flat-square)
![Gitleaks](https://img.shields.io/badge/-Gitleaks-B5452A?style=flat-square)
![Semgrep](https://img.shields.io/badge/-Semgrep-0D1117?style=flat-square&logo=semgrep&logoColor=white)

**Secrets, identity and policy:**
![Vault](https://img.shields.io/badge/-Vault-000000?style=flat-square&logo=vault&logoColor=white)
![AWS Secrets Manager](https://img.shields.io/badge/-Secrets_Manager-DD344C?style=flat-square&logo=amazonwebservices&logoColor=white)
![OPA](https://img.shields.io/badge/-OPA_Gatekeeper-4D4D4D?style=flat-square&logo=openpolicyagent&logoColor=white)
![Entra ID](https://img.shields.io/badge/-Entra_ID-0078D4?style=flat-square&logo=microsoft&logoColor=white)

**Detection and observability:**
![Microsoft Sentinel](https://img.shields.io/badge/-Microsoft_Sentinel-0078D4?style=flat-square&logo=microsoftazure&logoColor=white)
![Falco](https://img.shields.io/badge/-Falco-00AEC7?style=flat-square&logo=falco&logoColor=white)
![Prometheus](https://img.shields.io/badge/-Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![Grafana](https://img.shields.io/badge/-Grafana-F46800?style=flat-square&logo=grafana&logoColor=white)

**Languages:**
![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![Node.js](https://img.shields.io/badge/-Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![Bash](https://img.shields.io/badge/-Bash-4EAA25?style=flat-square&logo=gnubash&logoColor=white)
![HCL](https://img.shields.io/badge/-HCL-844FBA?style=flat-square&logo=terraform&logoColor=white)
