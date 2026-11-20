# GDPR & Privacy Information Management (ISO/IEC 27701:2025) Compliance Checklist

An executive, auditor-led baseline checklist for UK and international SMEs, SaaS providers, and data-intensive organisations preparing for **UK GDPR / Data Protection Act 2018** alignment and **ISO/IEC 27701** Privacy Information Management System (PIMS) certification.

Built on Javo Consultancy Ltd's **"Auditor's Eye"** methodology, this checklist highlights the exact operational controls and technical records UKAS-accredited Lead Auditors sample during Stage 1, Stage 2, and surveillance assessments.

> **2025/2026 Standard Update Note:** ISO/IEC 27701:2025 established PIMS as a standalone management system standard (no longer strictly dependent on holding ISO/IEC 27001 first, while still integrating seamlessly into an IMS). Transition from ISO/IEC 27701:2019 runs through **31 October 2028**, alongside updated certification body requirements under ISO/IEC 27706:2025.

---

## 1. Privacy Information Management System (PIMS) Foundation

*Aligned with ISO/IEC 27701:2025 Clauses 4–6 & 8; UK GDPR Articles 5, 24, 30 & 35.*

- [ ] **Define Organisational Context & PIMS Scope (Clauses 4.1–4.3):** Document whether your organisation acts as a **PII Controller**, a **PII Processor**, or **both** across each product line, corporate function (e.g., HR/marketing), and multi-tenant environment.
- [ ] **Maintain an Operational Record of Processing Activities — RoPA (UK GDPR Art. 30):** Verify that your RoPA maps actual data flows, lawful bases, retention periods, and recipient categories rather than a static compliance spreadsheet.
- [ ] **Enforce Role-Specific PII Controls (ISO/IEC 27701 Annex A):** Implement distinct, verifiable control sets for Controller obligations (lawful basis, consent capture, data subject rights) and Processor obligations (acting strictly on documented customer instructions, return/erasure on termination).
- [ ] **Operationalise Privacy Risk Assessments & DPIAs (Clauses 6.1.2, 8.2; UK GDPR Art. 35):** Conduct Data Protection Impact Assessments before launching high-risk processing, new SaaS features, or AI/profiling workflows—and trace resulting risk treatments directly into engineering tickets and change logs.

---

## 2. Operational, Technical & Personnel Governance

*Aligned with UK GDPR Articles 5, 10 & 32; Data Protection Act 2018; ISO/IEC 27001:2022 Annex A.6.1, A.8.10 & A.8.11.*

- [ ] **Align Cloud Architecture & API Integrations with UK GDPR Art. 32:** Verify encryption in transit and at rest, named-user access controls (no shared admin accounts), enforced MFA, environment segregation, and least-privilege IAM policies across production hosting and APIs.
- [ ] **Eliminate Pre-Launch PII Exposure & Unmasked Test Data (ISO 27001 A.8.11):** Confirm that live customer PII is never copied into staging, QA, or developer environments without documented anonymisation or pseudonymisation controls.
- [ ] **Prove Technical PII Erasure & Retention Enforcement (ISO 27001 A.8.10):** Validate that deletion requests and retention schedules propagate reliably across primary databases, S3/object storage, analytics exports, log aggregators, and backup rotation cycles.
- [ ] **Enforce Lawful Personnel Screening & HR Privacy Controls (UK GDPR Art. 10; ISO 27001 A.6.1; BS 7858):** Ensure pre-employment background checks, right-to-work verifications, and DBS/criminal-record screening records have a documented lawful condition, restricted access, and strict retention limits—never stored indefinitely in open HR folders.

---

## 3. Third-Party, SOW & Supply Chain Privacy Risk

*Aligned with UK GDPR Articles 28 & 44–49; ISO/IEC 27001:2022 Annex A.5.19–A.5.22.*

- [ ] **Audit Vendor Statements of Work (SOW) & SLAs Against Live Delivery:** Scrutinise outsourced software engineering SOWs, SLAs, and delivery pipelines to ensure contractual privacy, IP, and security commitments operate in day-to-day practice. *(Read our full technical breakdown: [Third-Party SOW Audit: Managing Vendor & IP Risk in Outsourced Tech Projects](https://www.javoconsultancyltd.com/post/third-party-sow-audit).)*
- [ ] **Verify Data Processing Agreements — DPAs (UK GDPR Art. 28):** Cross-check signed DPAs against actual cloud access logs, support tools, and data exports. A signed DPA proves an obligation existed; it does not prove the supplier enforced it.
- [ ] **Control Sub-Processor Chains & Cross-Border Transfers (UK GDPR Arts. 44–49):** Maintain an approved sub-processor register with written flow-down terms, and verify lawful transfer mechanisms (UK IDTA, UK Addendum, or EU SCCs) supported by documented Transfer Risk Assessments (TRAs).
- [ ] **Scrutinise Third-Party Code Libraries & Telemetry:** Maintain a Software Bill of Materials (SBOM) and audit third-party SDKs, APIs, and AI/analytics dependencies to prevent unauthorised PII leakage and regulatory breach exposure.

---

## 4. Audit-Ready Documentation & "Retrieval vs. Manufacture" Evidence

*Aligned with ISO/IEC 27701:2025 Clauses 7.5, 9.1–9.3 & 10.2.*

- [ ] **Reject Generic "Copy-Paste" Templates:** Replace boilerplate policies with concise, version-controlled documentation mapped directly to your real workflows, roles, and statutory obligations.
- [ ] **Prioritise "Retrieval" Evidence Over Screenshot Theatre:** Build an evidence trail drawn from live operational systems (IAM audit logs, Git/CI-CD history, ticketing approvals, access review logs, and automated retention logs) rather than documents assembled retroactively before an audit.
- [ ] **Run Independent Internal Audits & Clause 9.3 Management Reviews:** Conduct impartial internal audits against all applicable PIMS clauses and document top-management review inputs, privacy KPIs, and corrective actions before booking your external Certification Body visit.

---

## Deep-Dive ISO/IEC 27701:2025 Whitepapers (Coming Soon)

This checklist serves as the executive entry point for Javo Consultancy Ltd's clause-level technical whitepaper series hosted on [`vvohanka-consultancy`](https://github.com/vvohanka-consultancy/vvohanka-consultancy):

| Scheduled Release | Whitepaper Topic | Planned Repo Slug |
| :--- | :--- | :--- |
| w/c 21 Dec 2026 | ISO/IEC 27701:2025 Standalone Architecture & ISO/IEC 27706:2025 Transition Blueprint | `iso27701-2025-standalone-transition` |
| w/c 4 Jan 2027 | Auditing PII Controller vs. PII Processor Boundaries & Art. 28 Sub-Processor Chains in Multi-Tenant SaaS | `iso27701-controller-processor-saas` |
| w/c 11 Jan 2027 | DPIA-to-Engineering Traceability & Lawful HR / Background Screening Privacy Controls | `iso27701-dpia-hr-screening-controls` |
| w/c 18 Jan 2027 | Proving PII Deletion, Non-Production Data Masking & Cross-Border Transfers in Live Systems | `iso27701-pii-lifecycle-deletion-transfers` |
| w/c 1 Mar 2027 | Auditing Shadow AI, Unauthorised PII Leakage & Non-Compliant Code Libraries in Engineering Pipelines | `shadow-ai-pii-supply-chain-audit` |

---

## About Javo Consultancy Ltd

**Javo Consultancy Ltd** is a family-run, remote-first ISO consultancy registered in England and Wales (Company No. 10616318), delivering lean, certification-ready management systems for SMEs and technology organisations. Both directors are active UK-based Lead Auditors for a UKAS-accredited certification body holding Lead Auditor expertise across ISO/IEC 27701 (PIMS), ISO/IEC 27001 (ISMS), and ISO/IEC 42001 (AIMS).

* **ICO Data Protection Registration:** `ZA235697`
* **Delivery & Pricing:** 100% remote global delivery with flexible evening/weekend availability (GMT/BST), transparent fixed-price contracts, and a **5% saving** when bundling annual internal audits with pre-certification readiness checks or compliance document reviews.
* **Independence Notice:** To maintain strict professional impartiality, we do not provide consultancy services to organisations certified by our directors' current full-time employer. Please confirm your Certification Body upon initial contact.

**Website:** https://www.javoconsultancyltd.com/  
**Services & Fixed-Price Quotes:** https://www.javoconsultancyltd.com/services  
**Email:** v.vohanka@javoconsultancyltd.com  
**Telephone:** +44 (0) 7534 662808




































































































