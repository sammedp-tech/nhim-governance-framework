# Introduction to Non-Human Identity Management (NHIM)
## NHIM Governance 

### The 5 Pillars of NHIM Governance 
Enterprise NHIM programs succeed when they are built on these five pillars:

#### 1️⃣ Classification

Not all NHIs have equal risk.  
A classification model reduces chaos and helps focus effort:

- **Tier 0** – Domain-level and highly privileged NHIs  
- **Tier 1** – Core infrastructure and platform NHIs  
- **Tier 2** – Business application NHIs  
- **Tier 3** – Low-risk / routine NHIs  

Classification is the foundation for **policy, onboarding priority, and controls**.

---

#### 2️⃣ Ownership & Accountability

Every non-human identity must have:

- A **Business Owner** (why it exists)  
- A **Technical Owner** (who can fix it)  
- A **Fallback Owner** (if primary moves roles)  
- A defined **review cadence** (quarterly/bi-annual etc.)

No owner = **automatic non-compliance** and long-term risk. Always follow "No Onwer - No identity" rule from day 1. 

---

#### 3️⃣ Lifecycle Governance

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

#### 4️⃣ Policy Enforcement

Policies should answer:

- Where can NHIs live? (which domains, resource groups, subscriptions)  
- What permissions are they allowed to have?  
- How is rotation enforced and how often?  
- How is emergency access handled?  
- How frequently must owners certify access and usage?  

Policies convert **intent → standardization → enforcement**.
- to be updated later
---

#### 5️⃣ Monitoring & Reporting

Monitoring must cover:

- Credential usage across systems  
- Secrets violations (credentials in configs, code, CI/CD)  
- Dormant, stale, or orphaned NHIs  
- Gaps in ownership and classification  
- Privilege creep over time  
- Anomalous authentication patterns or access behavior  

Dashboards should expose the **health of the NHIM ecosystem**, not just tool status.

---
