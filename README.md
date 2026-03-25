# Security Audit & Risk Assessment: Botium Toys

## 1. Project Overview
This project presents a comprehensive internal security audit and risk assessment for **Botium Toys**. The primary objective was to evaluate the organization's entire security program, encompassing employee equipment, internal networks, and systems. 

Initial analysis determined a **Risk Score of 8/10 (High)**. This elevated risk is primarily attributed to inadequate asset management, lack of critical access controls, and non-adherence to international compliance standards.

## 2. Scope & Goals
The scope of this audit included reviewing the IT Department's managed assets (on-premises equipment, remote workstations, legacy systems) and identifying current security postures. The goal was to complete a rigorous controls and compliance checklist to determine the necessary implementations required to secure Botium Toys' infrastructure.

## 3. Compliance Frameworks Evaluated
The audit assessed Botium Toys against the following industry standards:
* **PCI DSS (Payment Card Industry Data Security Standard):** Found non-compliant due to a lack of encryption and secure environments for credit card information.
* **GDPR (General Data Protection Regulation):** Found partially compliant. While a 72-hour breach notification plan exists, E.U. customer data is not adequately kept private or secured.
* **SOC (System and Organizations Controls - Type 1 & 2):** Found non-compliant due to absent user access policies and lack of confidentiality for Sensitive PII (SPII).

## 4. Key Vulnerabilities Identified
Through the controls assessment, several critical security gaps were identified:
1. **Access Control Failures:** All employees currently have universal access to internally stored data, including customers' PII/SPII. Least privilege and separation of duties are not implemented.
2. **Data Vulnerability:** No encryption is used for storing or transmitting credit card information, and there are no backups or disaster recovery plans (DRP) in place.
3. **Infrastructure Gaps:** The network lacks an Intrusion Detection System (IDS), and password policies are severely outdated without a centralized management system.

*(Note: Physical security, firewalls, and antivirus software were found to be adequately implemented.)*

## 5. Recommended Remediation Strategies
To mitigate the identified risks, the following immediate actions are recommended:

* **Enforce Principle of Least Privilege (PoLP):** Revoke universal access rights immediately. Access must be strictly restricted based on roles, particularly concerning Personally Identifiable Information (PII) and Sensitive PII (SPII), to mitigate severe risks to customer data.
* **Implement Data Encryption & Backup Protocols:** All sensitive data must be encrypted both at rest and in transit. Comprehensive backup solutions must be deployed to ensure data integrity and guarantee proper system recovery.
* **Deploy Network Monitoring (IDS/IPS) & DRP:** Implement Intrusion Detection and Prevention Systems (IDS/IPS) for tracking network traffic and proactively mitigating anomalies. This must be coupled with a formalized Disaster Recovery Plan (DRP) to ensure business continuity.
* **Establish Legacy Systems Management:** Develop and document formalized procedures for the manual monitoring, routine maintenance, and necessary interventions regarding existing legacy systems that cannot be easily updated.
* **Enforce Strict Password Policies:** Implement a robust Enterprise Password Management System to enforce the creation and storage of strong, reliable credentials across the entire organization.

---
*Disclaimer: This project was completed as part of the Google Cybersecurity Professional Certificate.*
