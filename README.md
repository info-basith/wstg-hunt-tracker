# 🛡️ WSTG Hunt Tracker

> **Comprehensive Web Application Security Testing Checklist, Vulnerability Logger & OWASP Risk Rating Calculator**  
> Aligned with the **OWASP Web Security Testing Guide (WSTG v4.2)** and **OWASP Top 10:2021**.

🔗 **Live Demo:** [https://info-basith.github.io/wstg-hunt-tracker/](https://info-basith.github.io/wstg-hunt-tracker/)

---

## 🌟 Key Features

### 📋 1. Comprehensive WSTG v4.2 Checklist
- **122 Security Tests** covering all 12 core OWASP WSTG categories:
  1. Information Gathering (WSTG-INFO)
  2. Configuration and Deployment Management (WSTG-CONF)
  3. Identity Management (WSTG-IDNT)
  4. Authentication Testing (WSTG-ATHN)
  5. Authorization Testing (WSTG-ATHZ + Extended Broken Access Control tests)
  6. Session Management Testing (WSTG-SESS)
  7. Data Validation Testing (WSTG-INPV)
  8. Error Handling (WSTG-ERRH)
  9. Cryptography (WSTG-CRYP)
  10. Business Logic Testing (WSTG-BUSL)
  11. Client-Side Testing (WSTG-CLNT)
  12. API Testing (WSTG-APIT)
- **Instant Search (`/`)**: Real-time filtering by test ID, title, objectives, recommended tools, CWE numbers, notes, and affected endpoints.
- **Direct Official Links**: Every test links directly to official OWASP documentation.
- **Section Actions**: Quickly mark all remaining tests in a section as *Pass*, expand/collapse sections, or clear checked tests.

### 🗺️ 2. Interactive Test Matrix (Heatmap)
- High-density visual map showing status across all 122 tests at a glance.
- Color-coded:
  - 🟢 **Pass** — control validated OK
  - 🔴 **Issue** — vulnerability detected
  - 🟡 **In Progress** — actively testing
  - 🟣 **Done** — completed
  - ⚪ **N/A** — out of scope or non-applicable
- Hover over any test pill for test details; click to smoothly jump directly to that card with a highlight pulse.

### 🚨 3. Vulnerability & Findings Logger
- Log issues directly from any test card with one click via **"⚠️ Log as Vulnerability"** (auto-fills test ID, name, affected endpoint, and notes).
- Document:
  - Severity Risk (`Critical`, `High`, `Moderate`, `Low`, `OFI/Informational`)
  - Likelihood & Impact ratings
  - OWASP Top 10 category mapping
  - Affected components, URLs, and parameter names
  - Observations & business implications
  - Proof of Concept (PoC) / test evidence
  - Remediation & fix recommendations
- Duplicate or delete findings with instant state synchronization.

### ⚖️ 4. OWASP Risk Rating Calculator
- Implements the complete **OWASP Risk Rating Methodology**:
  - **Threat Agent Factors**: Skills, Motive, Opportunity, Size
  - **Vulnerability Factors**: Ease of Discovery, Ease of Exploit, Awareness, Intrusion Detection
  - **Technical Impact**: Loss of Confidentiality, Integrity, Availability, Accountability
  - **Business Impact**: Financial damage, Reputation damage, Non-compliance, Privacy violation
- Real-time calculation of **Likelihood Score**, **Impact Score**, and **Overall Risk Severity**.
- Dynamic 3×3 Risk Matrix with active cell highlighting.
- **One-Click Apply**: Export the calculated risk score directly to create a new finding in the Vulnerability Log!

### 📖 5. WSTG to MITRE CWE Reference Map
- Complete cross-reference connecting WSTG testing areas to relevant MITRE Common Weakness Enumeration (CWE) entries.
- Searchable by CWE ID or weakness name with direct links to official MITRE documentation.

### 🎯 6. Multi-Target Scope Management
- Organize testing by target scope (e.g. *Production Web App*, *Staging API*, *Auth Microservice*).
- Create, rename, clone, and delete targets with isolated test states and issue logs.

### 📊 7. Executive Reporting & Backup
- **Markdown Pentest Report**: Generates a professional penetration testing report including Executive Summary, Severity Breakdown, Findings Table, Detailed Writeups, and Methodology Checklist.
- **CSV Exports**: Export full Checklist CSV and Findings CSV for spreadsheet analysis or Jira/ticketing import.
- **JSON Backup & Restore**: Full state export and restore with schema validation.
- **Print / PDF Friendly**: Optimized `@media print` CSS for generating clean PDF deliverables directly from the browser.

### 🔒 8. Privacy & Offline First
- **100% Client-Side**: No backend, no cookies, no tracking.
- All testing data is stored safely in your browser's `localStorage`.
- Fully functional offline or in isolated lab environments.

---

## ⌨️ Keyboard Shortcuts

| Shortcut | Action |
| :--- | :--- |
| `/` | Focus search bar immediately |
| `Esc` | Clear search filter and blur search bar |

---

## 🚀 Deployment

Hosted on **GitHub Pages**:
- Single self-contained `index.html` file with zero build steps or npm dependencies.
- Blazingly fast load times (<50ms).

---

## 📄 License

Open-source and available under the [MIT License](LICENSE).
Checklist data based on the [OWASP Web Security Testing Guide](https://owasp.org/www-project-web-security-testing-guide/).
