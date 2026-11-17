# CYSE303 - Secure Software Development Project
## Threat Modeling: STRIDE, DFDs, and Attack Surface Analysis

### Group 2 Members
* **Muhaned Mohamed AL sinani** – ID: `[2316223]`
* **Azhar Hamed AL salti** – ID: `[2420345]`
* **Osama AL hadi** – ID: `[2317565]`

### Project Overview
This project demonstrates Threat Modeling using Data Flow Diagrams (DFDs), STRIDE, and Attack Surface Analysis via **OWASP Threat Dragon** on an Online Money Transfer Web Application (Before -> After).

### Tools Used
* **OWASP Threat Dragon**
* **STRIDE Methodology**

### How to Run Locally
1. Open [https://www.threatdragon.com/](https://www.threatdragon.com/) -> Launch Threat Dragon -> Local Session -> Open Existing Model.
2. Load `vulnerable-code/vulnerable-architecture.json` to inspect unmitigated STRIDE threats.
3. Load `fixed-code/fixed-architecture.json` to verify all threats are mitigated.

### STRIDE Threats & Mitigations Summary
* **Spoofing:** Mitigated via Multi-Factor Authentication (MFA) and signed JWT tokens.
* **Tampering:** Mitigated via Role-Based Access Control (RBAC) and AES-256 encryption.
* **Repudiation:** Mitigated via immutable, append-only audit logs.
* **Information Disclosure:** Mitigated via HTTPS (TLS 1.3) across all trust boundaries.
