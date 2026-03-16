# Botium-Toys-Security-Audit
Internal security audit for Botium Toys based on the NIST CSF to identify compliance gaps and risk mitigation strategies.
# Portfolio Activity: Internal Security Audit Report

## Project Overview
**Company:** Botium Toys  
**Objective:** Conduct an internal security audit based on the NIST Cybersecurity Framework (CSF) to identify vulnerabilities, ensure compliance with GDPR and PCI DSS, and provide actionable recommendations to improve the company's security posture.

---

## 🔍 Audit Scope & Goals
As Botium Toys expands globally, the IT department must transition from a "growth-first" mindset to a "security-first" architecture. The goal is to mitigate risks to critical assets and ensure the integrity of customer PII (Personally Identifiable Information).

---

## 📊 Controls Assessment Checklist
| Control | Status | Explanation |
| :--- | :--- | :--- |
| **Least Privilege** | ❌ No | All employees currently have access to customer data, increasing breach risk. |
| **Separation of Duties** | ❌ No | The CEO currently manages both operations and payroll; no "checks and balances." |
| **Firewall** | ✅ Yes | Existing firewall blocks traffic based on defined rules. |
| **Intrusion Detection (IDS)** | ❌ No | No system in place to identify unauthorized entry attempts. |
| **Data Encryption** | ❌ No | Sensitive customer and financial data (PII/SPII) is stored in plaintext. |
| **Disaster Recovery** | ❌ No | No plan exists to ensure business continuity after a breach or failure. |
| **Asset Inventory** | ✅ Yes | Assets are listed/inventoried, but **Classification** is missing. |

---

## 💡 Key Findings & Recommendations

### 1. Access Control & Governance
* **Risk:** The lack of **Separation of Duties** (CEO controlling both operations and payroll) creates a high risk for internal fraud and accidental data loss.
* **Recommendation:** Implement the **Principle of Least Privilege (PoLP)**. User roles should be defined so that employees only access the data necessary for their specific job functions.

### 2. Data Protection & Compliance
* **Risk:** Botium Toys is currently non-compliant with **GDPR** and **PCI DSS** because customer financial data and E.U. resident data are not encrypted.
* **Recommendation:** Deploy **AES-256 encryption** for data at rest and ensure all payment transactions are handled through secure, encrypted tunnels (TLS).

### 3. Vulnerability Management
* **Risk:** Inventory exists, but without **Data Classification**, the IT team cannot prioritize protection for the most sensitive assets.
* **Recommendation:** Establish a Data Classification policy (Public, Internal, Confidential, Restricted). This ensures that high-value assets like credit card info receive the strongest security controls.

### 4. Operational Resilience
* **Risk:** No Disaster Recovery (DR) plan means a single ransomware attack could permanently shut down the business.
* **Recommendation:** Implement an automated **Off-site Backup Strategy** and document a formal Disaster Recovery plan to meet business continuity goals.

---

## 🛠️ Skills Demonstrated
* **NIST Cybersecurity Framework (CSF)**
* **Compliance Auditing (GDPR, PCI DSS, SOC2)**
* **Risk Mitigation & Gap Analysis**
* **Security Governance**
