Security testing validates whether security controls function as intended, identifies vulnerabilities before attackers do, and ensures compliance with organizational and regulatory requirements.  
This section focuses on vulnerability assessments, penetration testing, red team exercises, and audits — including the differences between each, and the stages of a penetration test lifecycle.

---

## 14.1 Testing Methodologies Overview

| Methodology | Expanded Definition | Nested Key Points (Comparisons) | Workplace Example |
|-------------|----------------------|----------------------------------|--------------------|
| ★ Security Testing Methods | Umbrella term for evaluating system security through assessments, tests, simulations, or audits. | • Vulnerability Assessment<br>• Penetration Testing<br>• Red Team Exercises<br>• Security Audits | Ensuring financial reporting systems are secure and meet compliance requirements. |
| Vulnerability Assessment | Identifies weaknesses without exploiting them. | • Scanning tools<br>• Reporting vulnerabilities<br>• No exploitation | Scanning internal servers hosting financial data for misconfigurations. |
| Penetration Testing | Actively attempts to exploit vulnerabilities. | • Simulates real attacks<br>• Attempts exploitation<br>• Produces detailed findings | Testing whether client-reporting portals can be breached through weak input validation. |
| Red Team Exercise | Full-scale simulation of adversary behavior targeting people + processes + technology. | • Stealthy<br>• Multi-layer attack paths<br>• Tests detection & response | Attempting to breach firm defenses through phishing + network exploitation + lateral movement. |
| Security Audit | Formal review of policies, procedures, and technology controls. | • Compliance focus<br>• Documentation-heavy<br>• Control validation | Audit verifying EisnerAmper's controls for data handling and access management. |
| Comparison | VA = find; PT = exploit; RT = emulate full attacker; Audit = verify compliance. | • Likely exam question: “Which test type is being described?” | Using VA first, PT second to validate remediation, audit yearly. |

---

## 14.2 Penetration Testing Lifecycle (Phases)

| Phase | Expanded Definition | Nested Key Points | Workplace Example |
|-------|----------------------|--------------------|--------------------|
| ★ Penetration Testing Lifecycle | Structured sequence used during penetration tests. | • Planning<br>• Reconnaissance<br>• Scanning<br>• Exploitation<br>• Post-Exploitation<br>• Reporting | Used when testing resilience of financial reporting systems. |
| Planning | Defines scope, rules of engagement, and objectives. | • Black-box vs white-box<br>• Legal authorization | Establishing test scope for systems handling client data. |
| Reconnaissance (Recon) | Gathering information about target. | • Passive (OSINT)<br>• Active probing | Mapping external footprint of firm reporting systems. |
| Scanning & Enumeration | Identifying open ports, services, and vulnerabilities. | • Port scans<br>• Version detection | Finding outdated services that could expose financial data. |
| Exploitation | Attempting to exploit identified vulnerabilities. | • SQL injection<br>• Command injection<br>• Credential attacks | Exploiting weak validation in a client portal. |
| Post-Exploitation | Establish persistence & assess impact. | • Pivoting<br>• Data access<br>• Lateral movement | Attempting to reach client file storage systems. |
| Reporting | Final documentation of findings and remediation steps. | • Executive summary<br>• Technical details<br>• Risk ratings | Comprehensive report delivered to management outlining risks to financial systems. |

---

## 14.3 Vulnerability Assessment vs Penetration Testing

| Category | Vulnerability Assessment | Penetration Testing |
|----------|---------------------------|----------------------|
| Purpose | Identify weaknesses | Exploit weaknesses |
| Depth | Broad scanning | Deep exploitation |
| Risk | Low (no exploitation) | Higher (active attacks) |
| Output | Vulnerability list | Proof-of-concept attacks |
| Frequency | Regularly scheduled | Periodic or annually |
| Exam Tip | “Find vs exploit” is the key distinction | PT simulates real attacker |

---

## 14.4 Red Team vs Blue Team vs Purple Team

| Team | Expanded Definition | Nested Key Points | Workplace Example |
|------|----------------------|--------------------|--------------------|
| ★ Security Teams | Roles used during testing exercises. | • Offensive vs defensive vs collaborative | Used in large organizations for resilience testing. |
| Red Team | Offensive group simulating adversaries. | • Stealth<br>• Attack-focused<br>• Goal = breach | Targeting email/phishing weaknesses among accounting staff. |
| Blue Team | Defensive group responsible for detection and response. | • Monitoring<br>• Incident response<br>• Defense tuning | Responding to alerts triggered by unusual access patterns. |
| Purple Team | Collaboration between Red + Blue. | • Shared insights<br>• Improves both attack & defense | Coordinating improvements after simulated attack chain. |

---

## 14.5 Security Audits

| Concept | Expanded Definition | Nested Key Points | Workplace Example |
|---------|----------------------|--------------------|--------------------|
| ★ Security Audit | Formal evaluation of controls, compliance, and procedures. | • Follows frameworks (ISO, SOC)<br>• Focus on documentation<br>• Ensures policy adherence | Annual review of EisnerAmper data handling and access controls. |
| Internal Audit | Conducted by internal team. | • Validates internal controls | Reviewing access logs on shared client folders. |
| External Audit | Conducted by third party. | • Objective assessment<br>• Certifies compliance | SOC audit verifying client data protections. |

---

## 14.6 Study Focus Summary

| Exam Topic              | Explanation                                                                 |
| ----------------------- | --------------------------------------------------------------------------- |
| VA vs PT                | Vulnerability assessment finds; penetration test exploits.                  |
| Red Team vs Blue Team   | Offense vs defense; Purple = collaboration.                                 |
| PT Lifecycle            | Planning → Recon → Scanning → Exploitation → Post-Exploitation → Reporting. |
| Security Audits         | Compliance and documentation-focused reviews.                               |
| Scenario Identification | Exam will give scenarios; you match to method (VA, PT, RT, Audit).          |