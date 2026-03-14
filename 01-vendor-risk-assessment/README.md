# Piece 01 — Vendor Risk Assessment
### Third-Party SaaS Payroll Tool Evaluation | Meridian Financial Group

---

## Scenario

Meridian Financial Group, a mid-size financial services firm, is evaluating **PayStream Pro** — a cloud-based SaaS payroll platform — as a replacement for its legacy on-premises payroll system. The CISO commissioned this assessment before contract execution to identify cybersecurity and compliance risks associated with granting a third-party vendor access to sensitive employee and financial data.

### Detail

**Client**: Meridian Financial Group — a 400-person regional financial services firm headquartered in Los Angeles. They offer investment advisory and wealth management services. Regulated under GLBA. Publicly traded, so SOX applies.
**Vendor being evaluated**: PayStream Pro — a SaaS payroll platform. Cloud-hosted (AWS). Processes payroll for 400 employees. Handles direct deposit, W-2 generation, and HRIS integration via API.
What you have access to as the assessor:

PayStream Pro's SOC 2 Type II report (2024) — imagine it shows a few exceptions: one finding around field-level encryption, one around access controls
A completed VSQ — the vendor answered "in progress" on API token rotation and couldn't produce evidence of a formal IR plan
The draft contract/MSA — no data deletion clause, breach notification window is 72 hours
Internal interviews — HR says all payroll admins have the same access level; IT says API keys haven't been rotated since the integration was set up 18 months ago

**Meridian's risk appetite**: Does not accept HIGH-rated vendor risks without compensating controls, per their 2025 Information Security Policy.

---

## Objective

Conduct a vendor risk assessment using the **NIST Cybersecurity Framework (CSF) 2.0** as the governing methodology. Produce a deliverable suitable for CISO review and contract negotiation use.

---

## Key Finding

> **Overall Residual Risk: HIGH — Contract execution not recommended without resolution of four pre-adoption requirements.**

Three of seven threat scenarios were rated HIGH risk. Critical gaps were identified in field-level encryption, role-based access control, API token management, and incident response contractual obligations. Regulatory exposure spans GLBA, SOX §404, and PCI DSS v4.0.

---

## Document Contents

| Section | Description |
|---------|-------------|
| Executive Summary | Verdict and CISO recommendation |
| Scope & Methodology | NIST CSF 2.0 function-by-function evaluation framework |
| Assets at Risk | 7 asset categories with regulatory mapping and criticality ratings |
| Threat Scenarios | 7 threat scenarios mapped to CSF functions, rated HIGH / MEDIUM / LOW |
| Vulnerability Gaps | 7 specific control deficiencies with NIST control references |
| Risk Register | Likelihood × Impact scoring (1–25 scale) with pre-adoption flags |
| Recommended Controls | 12 controls across 3 tiers: pre-adoption, 30-day, and 90-day |
| Appendix | Regulatory reference table (GLBA, SOX, PCI DSS, CPRA, NIST CSF) |

---

## Framework

**NIST Cybersecurity Framework 2.0** — evaluated across all six core functions: Govern, Identify, Protect, Detect, Respond, Recover.

Risk scoring: **Likelihood (1–5) × Impact (1–5)** → score of 1–25, mapped to LOW (1–6) / MEDIUM (7–14) / HIGH (15–25).

---

## Files

| File | Description |
|------|-------------|
| `VendorRiskAssessment_PayStreamPro_v1.0.pdf` | Full assessment — formatted for CISO review |

---

*This is a mock assessment created for portfolio purposes. All company names, vendor names, and scenarios are fictional.*
