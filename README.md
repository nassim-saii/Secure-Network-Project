ISMS Security Architecture
==========================

NAC, Centralized Logging & ERP Hardening
----------------------------------------

📌 Project Overview
-------------------

This project presents the **design and implementation of a complete ISMS-aligned security architecture**, combining:

*   **Network Access Control (NAC)**
    
*   **Centralized logging and traceability**
    
*   **SIEM-based monitoring**
    
*   **Hardening of an open-source ERP (Odoo)**
    

The architecture follows **ISO/IEC 27001 principles**, ensuring **confidentiality, integrity, availability, accountability, and traceability** across both infrastructure and business applications.

All components were deployed and validated in a **simulated enterprise environment using GNS3 and virtualized servers**.

🎯 Global Objectives
--------------------

*   Enforce centralized authentication and authorization (AAA)
    
*   Ensure end-to-end traceability of user and system actions
    
*   Monitor infrastructure and applications in real time
    
*   Harden a critical ERP application hosting sensitive business data
    
*   Align technical controls with **ISO 27001 ISMS requirements**
    
 <img src="https://github.com/nassim-sai/Secure-Network-Project/blob/main/architecture/Diagram.png"  alt="screenshot" width="Auto" height="Auto" />


🧩 Project Scope
----------------

### Part 1 — ISMS Logging, Traceability & NAC

*   Identity-based access control
    
*   Centralized authentication using RADIUS & Active Directory
    
*   Network segmentation and firewall enforcement
    
*   Centralized log collection and SIEM analysis
    

### Part 2 — Open-Source ERP (Odoo) Hardening

*   Secure deployment of Odoo using Docker
    
*   Strong authentication and access control
    
*   Network isolation of ERP services
    
*   Continuous monitoring and log analysis
    

🏗️ Global Security Architecture
--------------------------------

The solution follows a **layered enterprise architecture**:

*   **Access & Distribution Layers** – User connectivity
    
*   **Core Layer** – Routing and redundancy
    
*   **Security Layer** – NAC, AAA, SIEM, Firewall
    
*   **Application Layer** – Hardened ERP (Odoo)
    
*   **WAN Layer** – Controlled external access
    

   <img src="https://github.com/nassim-sai/Secure-Network-Project/blob/main/architecture/Architecture.png"  alt="screenshot" width="Auto" height="Auto" />


🔐 Security Components & Roles
------------------------------

Component Role

**Active Directory** Centralized identity & access management

**FreeRADIUS** AAA & NAC enforcement

**pfSense** Firewall, segmentation & traffic logging

**Wazuh (SIEM)** Log analysis, monitoring & alerting

**Rsyslog** Centralized log transport

**Docker** Secure ERP deployment

**Odoo ERP** Business application

   <img src="https://github.com/nassim-sai/Secure-Network-Project/blob/main/screenshots/Screenshot 2026-01-09 200115.png"  alt="screenshot" width="Auto" height="Auto" />


Secure-Network-Project/screenshots
/Screenshot 2026-01-09 200115.png

📜 ISO 27001 Alignment
----------------------

ISO 27001 Control Implementation

A.5 / A.9 Identity & access management (AD, RADIUS)

A.9.4 Access control enforcement

A.12.4 Logging and monitoring (Wazuh)

A.13 Network security (pfSense)

A.14 Secure application deployment (Odoo)

🔄 NAC & Logging Workflow
-------------------------

1.  User requests network access
    
2.  Authentication handled by **FreeRADIUS**
    
3.  Identity verified via **Active Directory**
    
4.  Network access filtered by **pfSense**
    
5.  Logs forwarded via **Rsyslog**
    
6.  Events analyzed in **Wazuh SIEM**
    
7.  Alerts triggered for anomalies or violations
    

🧱 ERP (Odoo) Hardening Architecture
------------------------------------

### Key Security Measures

*   Deployment via **Docker containers**
    
*   Network isolation of ERP and database
    
*   Authentication integrated with **Active Directory**
    
*   Firewall-controlled access to ERP services
    
*   Log forwarding from ERP host to **Wazuh**
    
*   Continuous monitoring and alerting

    <img src="https://github.com/nassim-sai/Secure-Network-Project/blob/main/screenshots/Screenshot%202026-01-09%20200039.png"  alt="screenshot" width="Auto" height="Auto" />


🧪 Demonstration & Validation
-----------------------------

### Validated Scenarios

*   Successful centralized authentication
    
*   Denied unauthorized network access
    
*   ERP access restricted to authenticated users
    
*   Real-time log visualization in Wazuh
    
*   Detection of abnormal behavior
    

Screenshots available in /screenshots.

📊 Benefits
-----------

### Security

*   Strong access control
    
*   Reduced attack surface
    
*   Continuous monitoring
    

### Operational

*   Centralized visibility
    
*   Faster incident response
    
*   Scalable architecture
    

### Compliance

*   ISO 27001 alignment
    
*   Audit-ready logs
    
*   Full traceability
    

📁 Documentation
----------------

*   📄 ISMS Logging & Traceability Report
    
*   📊 ISMS Project Presentation
    
*   📘 ERP Hardening (PCA) Presentation
    

All documents are available in /docs.

👨‍💻 Authors
-------------

*   **Saii Nassim**
    
*   **Abidli Roudaina**
    
**Supervisor**: Mourad Melliti  
**Class**: ING-5-SSIR
**Academic Year** : 2025–2026


📜 License
----------

This project is released for **academic and educational use**.
