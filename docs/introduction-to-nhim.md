# Introduction to Non-Human Identity Management (NHIM)
## Securing Machine, Service & Workload Identities Across Hybrid Enterprises  

---

## 🧠 Why NHIM Matters More Than Ever

Enterprises today have **10–50× more non-human identities than human identities** — service accounts, bots, workloads, scripts, integrations, APIs, schedulers, containers, pipelines.

Yet most organizations:

- Don’t know **how many** exist  
- Don’t know **who owns them**  
- Don’t know **what they have access to**  
- Don’t rotate credentials  
- Don’t monitor their usage  

This creates the **single largest blind spot** in identity security.

**NHIM is the next frontier of enterprise identity governance.**

---
### 🧭 NHIM in the Modern Identity Ecosystem

NHIM is no longer just a connector between IAM and PAM.  
It has evolved into an independent governance function that spans:

- IAM (identity creation and lifecycle)
- PAM (privileged credential security)
- Cloud workload identity platforms (ex-AWS IAM Roles, Azure Managed Identities)
- Secrets management tools (ex-Vault, Conjur, Akeyless, 1Password)
- Certificate & machine identity systems (ex-Venafi, AppViewX, Keyfactor)
- DevOps automation ecosystems (CI/CD, GitHub OIDC, Kubernetes)

NHIM provides the governance layer — ownership, classification, lifecycle, risk —  
while these platforms implement the actual identity and credential controls.

Without NHIM, these systems remain siloed and inconsistent.

---

## 🔐 What Counts as a Non-Human Identity?

Non-human identities (NHIs) include any identity that performs an action **without a human logging in directly**.

| Type                         | Examples                                                   |
|------------------------------|------------------------------------------------------------|
| **Service Accounts**         | Windows service accounts, Linux daemons                    |
| **Application Identities**   | App pools, web services, internal APIs                     |
| **API Identities**           | API keys, OAuth apps, access tokens                        |
| **Cloud Workload Identities**| Azure Managed Identities, AWS IAM roles, GCP service accts |
| **Automation Identities**    | RPA bots, DevOps pipelines, schedulers                     |
| **Integration Identities**   | ESB services, connectors, middleware accounts              |
| **Embedded Secrets**         | Credentials in config files, scripts, Jenkins, Dockerfiles |

NHIM is not just “PAM for service accounts” — it is **full-scope governance** over all these identities.

---


