# PCI-DSS-v4.0-Compliance-Assessment



# PCI DSS v4.0 & ISO 27001 Compliance Assessment

This project outlines a comprehensive security audit, scoping analysis, and remediation strategy designed to align corporate infrastructure with **PCI DSS v4.0 (SAQ D / ROC)** and **ISO/IEC 27001:2022** standards.

---

## 📌 Executive Summary

* **Scoping & Data Flow Mapping:** Mapped Cardholder Data Environment (CDE) data flows under the **SAQ D / ROC** compliance track to establish strict network boundaries and minimize audit scope.
* **Technical Security Audit:** Identified critical vulnerabilities across PCI DSS v4.0 domains, including unauthorized Sensitive Authentication Data (**CVV/SAD**) temporary storage, **debug log leakage**, and missing **EDR/SAST** controls.
* **Dual-Framework Mapping:** Directly cross-referenced technical findings with **ISO/IEC 27001:2022 Annex A** controls (including Data Leakage Prevention, Secure Development, and Activity Monitoring).
* **Remediation Roadmap:** Developed an actionable 3-phase strategy to resolve vulnerabilities, enforce continuous security, and achieve audit readiness.

---

## 🛠️ Technical Audit Findings & Framework Alignment

| Finding / Control Gap | PCI DSS v4.0 Requirement | ISO/IEC 27001:2022 Annex A Control |
| :--- | :--- | :--- |
| **CVV / SAD Temporary Storage** | Req 3.3 (Prohibit SAD Storage) | A.8.12 (Data Leakage Prevention) |
| **Debug Log Card Data Leakage** | Req 3.3.1 / Req 10.2 (Log Protection) | A.8.15 (Logging) & A.8.12 |
| **Missing EDR Implementation** | Req 5.1 & 5.3 (Malware Defense & EDR) | A.8.7 (Protection Against Malware) |
| **Missing SAST in Pipelines** | Req 6.2 & 6.3 (Software Security) | A.8.25 (Secure Development Life Cycle) |

---

## 🚀 3-Phase Remediation Roadmap

```mermaid
flowchart LR
    P1[Phase 1: Immediate Containment] --> P2[Phase 2: Technical Integration] --> P3[Phase 3: Audit & Validation]
