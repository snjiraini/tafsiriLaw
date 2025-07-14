# Product Requirements Document (PRD)

## Product Name: **TafsiriLaw – Legal AI Assistant on Internet Computer (ICP)**
**Date:** July 13, 2025  
**Owner:** [Samuel Njiraini]  
**Version:** 1.0  

---

## 1. Overview
TafsiriLaw is a decentralized legal virtual assistant platform hosted on the Internet Computer Protocol (ICP). It allows legal firms to deploy, fine-tune, and operate their own private legal LLMs (Large Language Models) to automate legal workflows such as research, drafting, and review while maintaining strict data confidentiality using IPFS and on-device computation.

---

## 2. Problem Statement
Law firms are reluctant to adopt commercial AI platforms due to the following reasons:

- **Confidentiality risks**: Legal data is highly sensitive, subject to attorney-client privilege, and governed by strict compliance standards (e.g., GDPR, HIPAA).
- **Document overload**: Legal practitioners are burdened with reading and analyzing large volumes of case-related documents.
- **High operational cost**: Routine tasks like legal research, contract analysis, and communication consume time and require manpower (e.g., paralegals or junior associates).

---

## 3. Goals and Objectives
TafsiriLaw aims to:

- Provide each legal firm with a **private, dedicated LLM** hosted in their own decentralized canister.
- Allow for **firm-specific fine-tuning** using jurisdiction-specific data and case documents.
- Ensure **secure data handling** via encrypted storage on IPFS and optional on-device processing.
- Enable **automation of routine legal tasks** to improve efficiency and reduce cost.
- Maintain **auditability and transparency** via access logs and usage tracking.

---

## 4. Key Features

### 4.1. Platform Setup
- TafsiriLaw employees can onboard new law firms.
- Setting up a firm will:
  - Automatically **create a new ICP canister** dedicated to the firm.
  - Provision **encrypted IPFS storage** accessible only to that client.

### 4.2. Law Firm Features

#### Private LLM Deployment
- Each law firm receives an instance of a private LLM.
- Firms can optionally upload custom training data for **jurisdictional fine-tuning**.

#### User Management
- Law firms can create and manage their own users.
- Admin users have elevated privileges.

#### Subscription and Payments
- Subscriptions can be **monthly or yearly**.
- Subscription renewal triggers:
  - **Automatic topping up of cycles**.
  - **Payment for IPFS storage**.

#### Monitoring and Logs
- Admin users can:
  - View payment and billing history.
  - Monitor canister **cycles usage**.
  - Check **storage utilization**.
  - Access **prompt and usage logs**.

---

## 5. Technical Architecture

### 5.1. Infrastructure Components
- **Internet Computer (ICP)**: Decentralized hosting of client-specific canisters.
- **IPFS**: Secure, encrypted document storage.
- **Local LLM Runtime (optional)**: Firms can run the model locally (e.g., via Ollama) to ensure privacy.

---

## 6. User Roles & Permissions

| Role                | Permissions                                                                 |
|---------------------|------------------------------------------------------------------------------|
| TafsiriLaw Employee | Create law firm canisters, manage lifecycle, provision resources             |
| Firm Admin          | Manage users, monitor usage/payments, view logs, upload training data       |
| Firm User           | Access LLM for research, drafting, document review, communication tasks     |

---

## 7. Use Cases

- **Confidential Document Analysis**: Summarize or search legal case documents.
- **Contract Drafting & Review**: Suggest clause edits, flag compliance risks.
- **Legal Research**: Provide jurisprudence summaries or jurisdictional references.
- **Email & Memo Generation**: Draft professional legal communication quickly.
- **Due Diligence Support**: Review terms and flag issues in M&A or compliance audits.

---

## 8. Success Metrics

- % increase in document review speed  
- % reduction in time spent on legal research  
- # of law firms onboarded  
- % of firms renewing subscription after trial period  
- Average cycle and storage usage per firm per month  
- User satisfaction (CSAT/NPS)

---

## 9. Assumptions and Dependencies

- Firms have access to proprietary legal data for fine-tuning.  
- Legal professionals are open to adopting private AI tools.  
- Adequate IPFS performance and encryption support is available.  
- ICP canister cost and cycle rates remain stable and predictable.

---

## 10. Future Enhancements

- Integration with court systems or legal databases.  
- Role-based document access and approval workflows.  
- Real-time collaborative editing with AI review suggestions. 
