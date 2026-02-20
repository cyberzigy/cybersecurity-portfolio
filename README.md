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
[View the completed security audit checklist] 
(https://github.com/cyberzigy/cybersecurity-portfolio/blob/ee01a3b70c8a215ef76bd977094108119f63b519/Copy%20of%20Controls%20and%20CopyofControlsand%20complianc0checklist.pdf.pdf%20compliance0checklist.pdf.pdf)

---

## Skills Demonstrated
- Security audit review and assessment  
- Controls evaluation and compliance analysis  
- Risk identification and mitigation planning  
- Documentation and professional reporting






Project Title

SIEM Log Analysis for E-Commerce Website Outage

⸻

📌 Scenario Overview

An organization’s main e-commerce website became unavailable, preventing customers from accessing services and completing transactions. This outage represented a critical business disruption with potential financial loss and reputational damage.

The objective of this analysis is to examine how log data and a Security Information and Event Management (SIEM) solution support incident detection, investigation, response, and business continuity.

⸻

🎯 Objective
	•	Identify relevant log sources for investigating the outage
	•	Explain how a SIEM platform enables detection and response
	•	Demonstrate how cybersecurity operations protect business functions

⸻

🔍 Question 1

What does “cybersecurity business operations” encompass in this scenario?

Answer

Cybersecurity business operations refer to the processes and controls that enable the organization to detect, respond to, and recover from incidents while maintaining service availability. In this scenario, this includes identifying the cause of the outage, activating the incident response plan, containing any malicious activity, restoring the website through backup or failover systems, communicating with stakeholders, and minimizing financial and reputational impact. Cybersecurity supports business continuity by ensuring rapid recovery and protecting customer trust.

⸻

🔍 Question 2

What types of log data are most relevant for investigating the outage, and why?

Answer

Several log sources are critical:
	•	Web server logs: Reveal traffic patterns, HTTP status codes, and potential DDoS indicators such as repeated requests or traffic spikes.
	•	Application logs: Identify internal errors, database connection failures, or payment processing issues.
	•	System/OS logs: Show resource utilization, service crashes, and unauthorized access attempts.
	•	Firewall logs: Provide visibility into allowed and blocked traffic, suspicious IP activity, and port scanning.
	•	IDS/IPS logs: Detect known attack signatures and exploit attempts.
	•	Load balancer/CDN logs: Indicate backend server health, traffic distribution, and failover events.

These logs help determine whether the outage was caused by a cyberattack, system failure, or external dependency.

⸻

🔍 Question 3

What other logs might be relevant, and what information would they provide?

Answer

Additional valuable log sources include:
	•	Database logs: Identify slow queries, lock timeouts, crashes, or SQL injection attempts.
	•	Authentication/IAM logs: Detect unauthorized admin access, brute-force attempts, or privilege escalation.
	•	DNS logs: Reveal domain resolution failures or potential DNS hijacking.
	•	Network device logs (routers/switches): Show bandwidth saturation, connectivity issues, or interface errors.
	•	Payment gateway/API logs: Indicate third-party service failures affecting transaction processing.

Correlating these logs enables accurate root cause analysis across infrastructure, application, and network layers.

⸻

🔍 Question 4

How would a SIEM tool use server and firewall logs to assist in the investigation and protection of business operations?

Answer

A SIEM centralizes server and firewall logs into a single platform, providing real-time visibility during the outage. By correlating abnormal traffic patterns in firewall logs with high CPU utilization and error rates in server logs, the SIEM can quickly identify indicators of a DDoS attack, unauthorized access, or system failure.

The SIEM generates alerts based on detection rules and threat intelligence, enabling rapid investigation. Analysts can filter events by time, IP address, or event type to build a timeline and identify affected systems. This reduces mean time to detect and respond, supports faster containment, and accelerates service restoration, thereby minimizing business disruption.

⸻

🔍 Question 5

What is the overall importance of logs and SIEM tools in protecting business operations?

Answer

Log data provides the foundational visibility required to monitor system activity, detect anomalies, and investigate incidents. A SIEM enhances this capability by aggregating and correlating logs from multiple sources, enabling real-time threat detection, automated alerting, and efficient incident response.

Together, logs and SIEM:
	•	Reduce downtime through faster detection and recovery
	•	Minimize financial and operational impact
	•	Protect customer data and trust
	•	Support compliance and forensic investigations
	•	Improve security posture through post-incident analysis

Without centralized logging and SIEM capabilities, organizations lack the visibility needed to identify root causes and respond effectively to cyber incidents.

⸻

🧠 Key Skills Demonstrated
	•	Log source identification and analysis
	•	SIEM event correlation
	•	Incident response workflow
	•	Business continuity awareness
	•	Root cause analysis

⸻

📈 Business Impact

Effective use of logs and SIEM reduces Mean Time to Detect (MTTD) and Mean Time to Respond (MTTR), ensuring faster restoration of critical services, reduced revenue loss, and improved organizational resilience.

⸻

🔚 Conclusion

Centralized logging and SIEM capabilities are essential for modern cybersecurity operations. They transform raw system data into actionable intelligence, enabling organizations to detect threats early, respond efficiently, and maintain uninterrupted business services.

