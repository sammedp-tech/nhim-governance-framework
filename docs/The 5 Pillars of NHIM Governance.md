# Introduction to Non-Human Identity Management (NHIM)
## The 5 Pillars of NHIM Governance 

Enterprise NHIM programs succeed when they are built on these five pillars:

### 1️⃣ Classification

Not all NHIs have equal risk.  
A classification model reduces chaos and helps focus effort:

- **Tier 0** – Domain-level and highly privileged NHIs  
- **Tier 1** – Core infrastructure and platform NHIs  
- **Tier 2** – Business application NHIs  
- **Tier 3** – Low-risk / routine NHIs  

Classification is the foundation for **policy, onboarding priority, and controls**.

---

### 2️⃣ Ownership & Accountability

Every non-human identity must have:

- A **Business Owner** (why it exists)  
- A **Technical Owner** (who can fix it)  
- A **Fallback Owner** (if primary moves roles)  
- A defined **review cadence** (quarterly/bi-annual etc.)

No owner = **automatic non-compliance** and long-term risk. Always follow "No Onwer - No identity" rule from day 1. 

---

### 3️⃣ Lifecycle Governance

NHIs must follow a controlled lifecycle from creation to deletion.

| Stage           | Controls Needed                                               |
|-----------------|---------------------------------------------------------------|
| **Creation**    | Justification, naming standard, classification, owner        |
| **Provisioning**| Least privilege, role-based access, enforcement of policies  |
| **Usage**       | Monitoring, logging, session visibility                       |
| **Rotation**    | Automated password/secret rotation, non-disruptive patterns  |
| **Decommission**| Access removal, deletion, audit evidence                      |

Lifecycle governance enforces **order over chaos** and prevents privilege creep.

---

### 4️⃣ Policy Enforcement

Policies should answer:

- Where can NHIs live? (which domains, resource groups, subscriptions)  
- What permissions are they allowed to have?  
- How is rotation enforced and how often?  
- How is emergency access handled?  
- How frequently must owners certify access and usage?  

Policies convert **intent → standardization → enforcement**.
- to be updated later
---

### 5️⃣ Monitoring & Reporting

Monitoring must cover:

- Credential usage across systems  
- Secrets violations (credentials in configs, code, CI/CD)  
- Dormant, stale, or orphaned NHIs  
- Gaps in ownership and classification  
- Privilege creep over time  
- Anomalous authentication patterns or access behavior  

Dashboards should expose the **health of the NHIM ecosystem**, not just tool status.

---

## 🧭 NHIM in the PAM + IAM + Cloud Security Ecosystem

NHIM is not a standalone function. It sits **in the middle** of your identity security stack:

```text
          ┌───────────────────────┐
          │          IAM          │
          │  Identity Lifecycle   │
          └───────────┬───────────┘
                      │
          ┌───────────▼───────────┐
          │          NHIM         │
          │ Governance & Control  │
          └───────────┬───────────┘
                      │
          ┌───────────▼───────────┐
          │          PAM          │
          │ Vaulting & Rotation   │
          └───────────────────────┘
```text
### 🧭 IAM, NHIM, and PAM Relationship

- **IAM** handles identity creation and lifecycle  
- **NHIM** governs ownership, classification, lifecycle, and risk  
- **PAM** secures credentials, sessions, and privileged operations  

Without NHIM, IAM and PAM are **disconnected islands**.

---

### ⚠️ Common NHIM Anti-Patterns (Seen Everywhere)

These patterns show up in almost every large environment:

- “Everything is just a service account” → no classification, no governance  
- 15-year-old Windows service accounts with static passwords  
- Credentials hidden in `web.config`, PowerShell scripts, Jenkins, pipelines  
- PAM vault onboarding done without knowing the owner  
- Rotation breaks applications because dependencies were undocumented  
- No application-to-identity mapping  
- Treating NHIM as a “PAM feature” instead of an enterprise program  

Recognizing these early helps build a more realistic roadmap.

---

### 📈 NHIM Maturity Model

Use this simple maturity model to assess where an organization stands:

| Level | Maturity   | Characteristics                                         |
|-------|-----------|----------------------------------------------------------|
| 0     | Unmanaged | Unknown NHI inventory, hardcoded secrets everywhere      |
| 1     | Basic     | Partial inventory, manual rotation, owners unclear       |
| 2     | Defined   | Ownership defined, basic policies, vault in limited use  |
| 3     | Managed   | Automated rotation, classification adopted, monitored    |
| 4     | Optimized | Full lifecycle automation, cloud-native, continuous review |

Most large enterprises sit between **Level 1 and Level 2**, even with PAM tools deployed.

---

### 🚀 The Goal of NHIM Programs

The mission of an NHIM program can be summarized as:

> **“Every non-human identity must have an owner, a purpose, a lifecycle, a risk classification, and a secured credential.”**

When NHIM is done well:

- Operational load on teams goes down  
- Credential-related incidents decrease  
- PAM onboarding becomes structured and predictable  
- Audits become faster and less painful  
- Secrets sprawl is reduced  
- Cloud and on-prem identities are treated consistently  

NHIM is the **missing link** between IAM maturity and PAM success.

---
