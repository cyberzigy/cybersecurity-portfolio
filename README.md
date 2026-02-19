# 👨🏽‍💻 Alexander Joseph – Cybersecurity Portfolio

## 🔐 Professional Statement
I am an aspiring cybersecurity analyst with a strong interest in identifying vulnerabilities, conducting security audits, and helping organizations improve their security posture.  

I am currently developing hands-on skills in:

- Security auditing and risk assessment  
- Network security fundamentals  
- Threat detection and mitigation  
- Linux system security  

I am passionate about continuous learning and actively working on practical labs, security assessments, and real-world simulations to build industry-ready cybersecurity skills.


# Botium Toys Security Audit Assessment

## Project Overview
This project documents my assessment of the IT security controls and compliance posture at Botium Toys, based on the IT manager’s security audit report.  
The goal of this project was to review existing assets, assess controls, and identify compliance gaps to improve Botium Toys’ security posture.

## Audit Scope
The scope of this audit includes the entire security program at Botium Toys, covering:

- On-premises equipment for in-office business needs
- Employee devices: desktops, laptops, smartphones, remote workstations, headsets, cables, keyboards, mice, docking stations
- Storefront and warehouse products
- Management of systems and services: accounting, telecommunications, database, security, e-commerce, and inventory
- Internet access and internal network
- Data retention and storage
- Legacy system maintenance

## Risk Assessment
- Risk description: Inadequate asset management and missing controls, with potential non-compliance to U.S. and international regulations.
- Risk score: 8/10 (high risk)
- Impact: Medium potential impact from asset loss; high risk of regulatory fines due to missing controls and lack of compliance with best practices.

---

## Controls Assessment Checklist

| Control | Status | Notes |
|---------|--------|-------|
| Least Privilege | No | Employees have access to all internal data; least privilege not implemented |
| Disaster recovery plans | No | No disaster recovery plan or backups exist |
| Password policies | Yes | Nominal password policy exists but weak |
| Separation of duties | No | Not implemented |
| Firewall | Yes | Firewall blocks traffic based on defined security rules |
| Intrusion detection system (IDS) | No | IDS not installed |
| Backups | No | No backups of critical data |
| Antivirus software | Yes | Installed and monitored regularly |
| Manual monitoring, maintenance, and intervention for legacy systems | Yes | Legacy systems monitored manually, no regular schedule |
| Encryption | No | Customer credit card info not encrypted |
| Password management system | No | No centralized password management system |
| Locks (offices, storefront, warehouse) | Yes | Physical locks in place |
| Closed-circuit television (CCTV) surveillance | Yes | Up-to-date CCTV implemented |
| Fire detection/prevention | Yes | Fire alarm and sprinkler systems in place |

---

## Compliance Checklist

### PCI DSS

| Best Practice | Status | Notes |
|---------------|--------|-------|
| Only authorized users have access to credit card info | No | All employees can access cardholder data |
| Credit card info securely stored/processed | No | Stored internally without encryption |
| Implement data encryption | No | Encryption not used |
| Secure password management | No | Weak and non-centralized password policy |

### GDPR

| Best Practice | Status | Notes |
|---------------|--------|-------|
| EU customers’ data kept private/secured | Yes | Privacy policies enforced |
| Plan to notify EU customers within 72 hours | Yes | Breach notification plan in place |
| Data properly classified/inventoried | Yes | Assets are inventoried; classification partially implemented |
| Enforce privacy policies, procedures, processes | Yes | Policies documented and enforced |

### SOC 1 / SOC 2

| Best Practice | Status | Notes |
|---------------|--------|-------|
| User access policies established | Yes | Policies for IT department in place |
| Sensitive data (PII/SPII) is confidential | Yes | Data privacy enforced |
| Data integrity ensured | Yes | IT department ensures data consistency and accuracy |
| Data available to authorized individuals | Yes | Access granted to authorized personnel only |

---

## Recommendations
- Implement least privilege and separation of duties controls  
- Establish a disaster recovery plan and regular backups  
- Implement encryption for sensitive data, especially credit card information  
- Deploy a centralized password management system  
- Install an intrusion detection system (IDS)  
- Improve password policy requirements to meet minimum complexity standards  
- Schedule regular monitoring and maintenance for legacy systems  

---

## Full Report
[View the completed security audit checklist] (https://github.com/cyberzigy/cybersecurity-portfolio/blob/ee01a3b70c8a215ef76bd977094108119f63b519/Copy%20of%20Controls%20and%20CopyofControlsand%20complianc0checklist.pdf.pdf%20compliance0checklist.pdf.pdf)

---

## Skills Demonstrated
- Security audit review and assessment  
- Controls evaluation and compliance analysis  
- Risk identification and mitigation planning  
- Documentation and professional reporting
