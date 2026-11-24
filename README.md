<div align="center">

<img src="./header.svg" width="100%" alt="Omajuwa Okotie, DevSecOps and Cloud Security Engineer" />

<br /><br />

<a href="https://omajuwaokotie.com"><img src="https://img.shields.io/badge/Portfolio-omajuwaokotie.com-f0a83a?style=flat-square&labelColor=08090c" alt="Portfolio" /></a>
<a href="https://www.linkedin.com/in/omajuwa-okotie-850950190"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat-square&logo=linkedin&logoColor=white&labelColor=08090c" alt="LinkedIn" /></a>
<a href="mailto:okotieomajuwa2016@gmail.com"><img src="https://img.shields.io/badge/Email-Get_in_touch-EA4335?style=flat-square&logo=gmail&logoColor=white&labelColor=08090c" alt="Email" /></a>
<img src="https://img.shields.io/badge/Available-Immediately-34d399?style=flat-square&labelColor=08090c" alt="Available immediately" />

</div>

<br />

## `$ whoami`

I build security into how software is shipped.

Over five years building and deploying software, including over three years focused on DevSecOps and cloud security across AWS and Azure. I design CI/CD pipelines where security checks **block** a bad release instead of just reporting it, harden cloud infrastructure in Terraform, deploy hardened workloads to Amazon EKS, and build detection and response that works when it matters.

My background as a full-stack engineer means I understand the applications I secure, not just how to scan them. MSc Computer Forensics and Cybersecurity with **Distinction**, University of Greenwich.

<br />

## `$ cat security-scorecard.md`

| Metric | Before | After | Project |
| --- | :---: | :---: | --- |
| Terraform security findings (Checkov) | 72 | **0** | SecureFlow |
| Known dependency vulnerabilities | 25 | **0** | SecureX |
| Test coverage in SonarQube | 0% | **86.3%** | SecureX |
| Security gates that block a release | 0 of 4 | **4 of 4** | SecureX |
| Credential compromise detection to response | 4+ hours | **< 5 min** | Sentinel |
| Stored cloud credentials in CI/CD | Access keys | **None (OIDC)** | SecureX |

<br />

## `$ ./how-i-ship.sh`

```mermaid
flowchart TB
    subgraph S1["🛡️ Shift-left gates: any failure blocks the release"]
        direction LR
        A["💻 Commit / PR"] --> B["🔑 Secrets<br/>Gitleaks"] --> C["🧱 IaC & Config<br/>Checkov · tfsec"] --> D["📦 Dependencies<br/>Trivy · SCA"] --> E["🔍 Code<br/>SAST · SonarQube"]
    end
    subgraph S2["🚀 Deliver & operate"]
        direction LR
        F["🐳 Image<br/>Scan · SBOM · Sign"] --> G["🧪 QA on EKS"] --> H["✅ Production<br/>same image, by SHA"] --> I["📈 Monitor & Detect<br/>Prometheus · Sentinel"]
    end
    S1 --> S2
    classDef gate fill:#1a1508,stroke:#f0a83a,color:#e8eaef
    classDef env fill:#0f2a1f,stroke:#34d399,color:#e8eaef
    classDef start fill:#12161f,stroke:#a7aeba,color:#e8eaef
    class B,C,D,E,F gate
    class G,H,I env
    class A start
    style S1 fill:#0d1117,stroke:#f0a83a,color:#f0a83a
    style S2 fill:#0d1117,stroke:#34d399,color:#34d399
```

<br />

## `$ ls ~/toolbox`

<table>
<tr>
<td valign="top" width="24%"><b>Cloud &amp; IaC</b></td>
<td>
<img src="https://img.shields.io/badge/AWS-08090c?style=flat-square&logo=amazonwebservices&logoColor=FF9900" alt="AWS" />
<img src="https://img.shields.io/badge/Amazon_EKS-08090c?style=flat-square&logo=amazoneks&logoColor=FF9900" alt="Amazon EKS" />
<img src="https://img.shields.io/badge/Microsoft_Azure-08090c?style=flat-square&logo=microsoftazure&logoColor=0078D4" alt="Microsoft Azure" />
<img src="https://img.shields.io/badge/Terraform-08090c?style=flat-square&logo=terraform&logoColor=7B42BC" alt="Terraform" />
<img src="https://img.shields.io/badge/Route_53-08090c?style=flat-square&logo=amazonroute53&logoColor=8C4FFF" alt="Route 53" />
<img src="https://img.shields.io/badge/ACM_%2F_ALB-08090c?style=flat-square&logo=amazonwebservices&logoColor=FF9900" alt="ACM and ALB" />
</td>
</tr>

<tr>
<td valign="top"><b>Containers &amp; Orchestration</b></td>
<td>
<img src="https://img.shields.io/badge/Kubernetes-08090c?style=flat-square&logo=kubernetes&logoColor=326CE5" alt="Kubernetes" />
<img src="https://img.shields.io/badge/Helm-08090c?style=flat-square&logo=helm&logoColor=0F1689" alt="Helm" />
<img src="https://img.shields.io/badge/Docker-08090c?style=flat-square&logo=docker&logoColor=2496ED" alt="Docker" />
<img src="https://img.shields.io/badge/OPA_Gatekeeper-08090c?style=flat-square&logo=openpolicyagent&logoColor=7D9199" alt="OPA Gatekeeper" />
<img src="https://img.shields.io/badge/Falco-08090c?style=flat-square&logo=falco&logoColor=00AEC7" alt="Falco" />
</td>
</tr>

<tr>
<td valign="top"><b>CI/CD &amp; DevSecOps</b></td>
<td>
<img src="https://img.shields.io/badge/GitHub_Actions-08090c?style=flat-square&logo=githubactions&logoColor=2088FF" alt="GitHub Actions" />
<img src="https://img.shields.io/badge/Gitleaks-08090c?style=flat-square" alt="Gitleaks" />
<img src="https://img.shields.io/badge/Checkov-08090c?style=flat-square" alt="Checkov" />
<img src="https://img.shields.io/badge/tfsec-08090c?style=flat-square" alt="tfsec" />
<img src="https://img.shields.io/badge/Trivy-08090c?style=flat-square&logo=trivy&logoColor=1904DA" alt="Trivy" />
<img src="https://img.shields.io/badge/SonarQube-08090c?style=flat-square&logo=sonarqubeserver&logoColor=4E9BCD" alt="SonarQube" />
<img src="https://img.shields.io/badge/Semgrep-08090c?style=flat-square&logo=semgrep&logoColor=e8eaef" alt="Semgrep" />
<img src="https://img.shields.io/badge/Bandit-08090c?style=flat-square" alt="Bandit" />
<img src="https://img.shields.io/badge/Syft_%2F_Cosign-08090c?style=flat-square" alt="Syft and Cosign" />
</td>
</tr>

<tr>
<td valign="top"><b>Identity &amp; Secrets</b></td>
<td>
<img src="https://img.shields.io/badge/GitHub_OIDC-08090c?style=flat-square&logo=github&logoColor=e8eaef" alt="GitHub OIDC" />
<img src="https://img.shields.io/badge/AWS_IAM_%2F_IRSA-08090c?style=flat-square&logo=amazonwebservices&logoColor=FF9900" alt="AWS IAM and IRSA" />
<img src="https://img.shields.io/badge/Secrets_Manager-08090c?style=flat-square&logo=awssecretsmanager&logoColor=DD344C" alt="AWS Secrets Manager" />
<img src="https://img.shields.io/badge/External_Secrets-08090c?style=flat-square" alt="External Secrets Operator" />
<img src="https://img.shields.io/badge/HashiCorp_Vault-08090c?style=flat-square&logo=vault&logoColor=FFEC6E" alt="HashiCorp Vault" />
<img src="https://img.shields.io/badge/Entra_ID_%2F_RBAC-08090c?style=flat-square&logo=microsoft&logoColor=0078D4" alt="Microsoft Entra ID and Azure RBAC" />
</td>
</tr>

<tr>
<td valign="top"><b>Detection &amp; Observability</b></td>
<td>
<img src="https://img.shields.io/badge/Microsoft_Sentinel-08090c?style=flat-square&logo=microsoftazure&logoColor=0078D4" alt="Microsoft Sentinel" />
<img src="https://img.shields.io/badge/KQL-08090c?style=flat-square" alt="KQL" />
<img src="https://img.shields.io/badge/Logic_Apps-08090c?style=flat-square&logo=microsoftazure&logoColor=0078D4" alt="Logic Apps" />
<img src="https://img.shields.io/badge/GuardDuty_%2F_Security_Hub-08090c?style=flat-square&logo=amazonwebservices&logoColor=FF9900" alt="GuardDuty and Security Hub" />
<img src="https://img.shields.io/badge/Prometheus-08090c?style=flat-square&logo=prometheus&logoColor=E6522C" alt="Prometheus" />
<img src="https://img.shields.io/badge/Grafana-08090c?style=flat-square&logo=grafana&logoColor=F46800" alt="Grafana" />
<img src="https://img.shields.io/badge/Loki-08090c?style=flat-square&logo=grafana&logoColor=F46800" alt="Loki" />
</td>
</tr>

<tr>
<td valign="top"><b>AppSec &amp; Testing</b></td>
<td>
<img src="https://img.shields.io/badge/OWASP_Top_10-08090c?style=flat-square&logo=owasp&logoColor=e8eaef" alt="OWASP Top 10" />
<img src="https://img.shields.io/badge/OWASP_ZAP-08090c?style=flat-square&logo=zap&logoColor=00549E" alt="OWASP ZAP" />
<img src="https://img.shields.io/badge/STRIDE_Threat_Modelling-08090c?style=flat-square" alt="STRIDE threat modelling" />
<img src="https://img.shields.io/badge/Penetration_Testing-08090c?style=flat-square" alt="Penetration testing" />
<img src="https://img.shields.io/badge/Jest_%2F_Supertest-08090c?style=flat-square&logo=jest&logoColor=C21325" alt="Jest and Supertest" />
</td>
</tr>

<tr>
<td valign="top"><b>Languages</b></td>
<td>
<img src="https://img.shields.io/badge/Python-08090c?style=flat-square&logo=python&logoColor=f0a83a" alt="Python" />
<img src="https://img.shields.io/badge/Node.js-08090c?style=flat-square&logo=nodedotjs&logoColor=339933" alt="Node.js" />
<img src="https://img.shields.io/badge/TypeScript-08090c?style=flat-square&logo=typescript&logoColor=3178C6" alt="TypeScript" />
<img src="https://img.shields.io/badge/Bash-08090c?style=flat-square&logo=gnubash&logoColor=4EAA25" alt="Bash" />
<img src="https://img.shields.io/badge/HCL-08090c?style=flat-square&logo=terraform&logoColor=7B42BC" alt="HCL" />
<img src="https://img.shields.io/badge/SQL-08090c?style=flat-square&logo=postgresql&logoColor=4479A1" alt="SQL" />
</td>
</tr>

<tr>
<td valign="top"><b>Frameworks</b></td>
<td>
<img src="https://img.shields.io/badge/ISO_27001-08090c?style=flat-square" alt="ISO 27001" />
<img src="https://img.shields.io/badge/NIST_CSF-08090c?style=flat-square" alt="NIST CSF" />
<img src="https://img.shields.io/badge/CVSS_v3.1-08090c?style=flat-square" alt="CVSS v3.1" />
</td>
</tr>
</table>

<br />

## `$ git log --featured`

> **`PLATFORM-SEC`** &nbsp; **[SecureX](https://github.com/omjhub/SecureX)** &nbsp; ![status](https://img.shields.io/badge/DEPLOYED-QA_%26_PROD-08090c?style=flat-square&labelColor=34d399)
> ### Production-grade DevSecOps platform on Amazon EKS
> - **14-job pipeline** where Gitleaks, Checkov, Trivy and SonarQube all block a release, each proven with a deliberate failure
> - Dependency CVEs **25 → 0**, test coverage **0% → 86.3%** with 31 Jest and Supertest tests
> - Separate QA and production; production runs the **exact image QA tested**, promoted by SHA with **7 required checks**
> - **No stored cloud keys**: GitHub OIDC, Secrets Manager, External Secrets Operator and IRSA
>
> `Amazon EKS` `GitHub Actions` `GitHub OIDC` `IRSA` `Trivy` `SonarQube` `Syft`

> **`PIPELINE-SEC`** &nbsp; **[SecureFlow](https://github.com/omjhub/SecureFlow-VulnerableCodebase)** &nbsp; ![status](https://img.shields.io/badge/CLOSED-REMEDIATED-08090c?style=flat-square&labelColor=f0a83a)
> ### Secure CI/CD pipeline for a banking platform
> - Seven-stage pipeline securing a vulnerable banking microservices codebase
> - Terraform findings **72 → 0**; a live pull request automatically blocked on **275 findings**
>
> `Gitleaks` `Trivy` `Checkov` `HashiCorp Vault` `OPA Gatekeeper` `Falco`

> **`APPSEC-LEAD`** &nbsp; **[SentinelPay](https://github.com/sentinelpay-team/Sentinelpay)** &nbsp; ![status](https://img.shields.io/badge/TEAM_LEAD-5_ENGINEERS-08090c?style=flat-square&labelColor=f0a83a)
> ### Securing an inherited fintech platform
> - Led threat modelling and remediation of SQL injection, JWT bypass, IDOR and a race condition, each proven with a before-and-after exploit
> - CI/CD gates and supply chain controls (CycloneDX SBOMs, Cosign signing) ahead of a timed attack simulation
>
> `STRIDE` `Semgrep` `Bandit` `tfsec` `GuardDuty` `Cosign`

> **`CLOUD-INFRA`** &nbsp; **[VaultBridge](https://github.com/omjhub/vaultbridge-iac-modernisation)** &nbsp; ![status](https://img.shields.io/badge/CLOSED-REMEDIATED-08090c?style=flat-square&labelColor=f0a83a)
> ### Three-tier AWS infrastructure as code
> - Fixed the root cause of a **$214,000** incident in the client brief
> - Security-group-only database access and a validation rule rejecting any SSH rule broader than /32
>
> `Terraform` `AWS` `tfsec` `Checkov`

> **`DETECTION`** &nbsp; **[Cloud Threat Detection](https://github.com/omjhub/cloudscale-sentinel-soc-poc)** &nbsp; ![status](https://img.shields.io/badge/CLOSED-VALIDATED-08090c?style=flat-square&labelColor=f0a83a)
> ### SIEM/SOAR with Microsoft Sentinel
> - Detection-to-response cut from **4+ hours to under 5 minutes**
> - Custom KQL rule debugged through live testing; Logic Apps playbook firing within **13 seconds**
>
> `Microsoft Sentinel` `KQL` `Logic Apps` `Entra ID`

> **`RESEARCH`** &nbsp; **[Web Vulnerability Detection](https://github.com/omjhub/Detecting-Vulnerabilities-In-Web-Applications)** &nbsp; ![status](https://img.shields.io/badge/MSc_DISSERTATION-74%25-08090c?style=flat-square&labelColor=a7aeba)
> ### Extending OWASP ZAP detection granularity
> - Baseline differential response verification on top of ZAP
> - Two of three false negatives turned into confirmed true positives with **zero new false positives**
>
> `Python` `OWASP ZAP` `DVWA` `Juice Shop`

<br />

## `$ history | grep work`

<table>
<tr>
<td valign="top" width="24%"><b>Jul 2023 to Oct 2026</b><br /><sub>AMDARI (Remote, Part-time)</sub></td>
<td valign="top"><b>Cloud Security Specialist (DevSecOps &amp; Cloud Security Engineer)</b><br />Secure CI/CD, infrastructure as code security, cloud threat detection and team-led vulnerability remediation across AWS and Azure, delivering SecureFlow, VaultBridge, Cloud Threat Detection and SentinelPay end to end from industry client briefs.</td>
</tr>
<tr>
<td valign="top"><b>Jan 2024 to Jun 2024</b><br /><sub>Spashisha (Remote, Part-time)</sub></td>
<td valign="top"><b>Software Engineer</b><br />Developed and deployed cloud-based applications, configuring cloud hosting, environment settings and release processes, with automation and security enhancements to deployments.</td>
</tr>
<tr>
<td valign="top"><b>Aug 2021 to Oct 2023</b><br /><sub>LinkX (Self-employed)</sub></td>
<td valign="top"><b>Project Lead / Mobile App Developer</b><br />Led design, development and deployment of mobile and web applications, and mentored team members in Flutter/Dart and backend best practices.</td>
</tr>
</table>

<br />

<div align="center">

```bash
$ echo "Open to DevSecOps, Cloud Security and AppSec Engineer roles in the UK. Available immediately."
```

<a href="https://omajuwaokotie.com">omajuwaokotie.com</a> &nbsp;·&nbsp; <a href="mailto:okotieomajuwa2016@gmail.com">okotieomajuwa2016@gmail.com</a> &nbsp;·&nbsp; <a href="https://www.linkedin.com/in/omajuwa-okotie-850950190">LinkedIn</a>

</div>
