<h1 align="center">NHIM Governance Framework</h1>
<h3 align="center">Non-Human Identity Management Across Cloud, On-Prem & Hybrid Environments</h3>

---

### 🧩 Overview

This repository captures my approach to designing **Non-Human Identity Management (NHIM)** governance for large enterprises.

Focus areas:
- Service accounts, bots, workloads, scripts, APIs
- Credential and secret management
- Ownership, accountability, and lifecycle governance
- Integration with PAM, IAM, and cloud-native identity

> This repo focuses on **frameworks and models**, does not contain any production code.  


---

### 🏗 Key Concepts

- NHIM classification (by risk, environment, usage)
- Mapping NHIM to **PAM**, **IAM**, and **Secrets Management**
- Control requirements across:
  - Cloud (Azure, AWS, etc.)
  - On-prem (Windows / AD / legacy systems)
  - Hybrid environments

---

### 📂 Structure

```bash
nhim-governance-framework/
├─ docs/
│  ├─ introduction-to-nhim.md
│  ├─ nhim-risk-model.md
│  ├─ control-objectives.md
│  ├─ governance-model.md
│  ├─ onboarding-framework.md
│  └─ operating-model/
│     ├─ roles-and-responsibilities.md
│     ├─ raci-matrix.md
│     ├─ control-monitoring.md
├─ diagrams/
│  ├─ nhim-architecture.png
│  ├─ nhim-lifecycle.png
└─ README.md
