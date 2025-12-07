Risk management identifies, evaluates, and prioritizes risks so organizations can reduce exposure to financial, operational, and compliance harm.  
This section focuses on how risks are defined, how responses are chosen, and how controls (preventive, detective, corrective, compensating) reduce overall risk levels.  
Your exam will test your ability to differentiate threats, vulnerabilities, impacts, risk categories, and control types — and to match scenarios to the correct risk response strategy.

---

## 13.1 Risk Fundamentals

| Concept | Expanded Definition | Nested Key Points | Workplace Example |
|---------|----------------------|--------------------|--------------------|
| ★ Risk | The potential for loss or harm when a threat exploits a vulnerability. | • Based on likelihood × impact<br>• Exists in all business functions | Outdated reporting system creates operational risk of downtime. |
| Threat | Anything capable of causing harm. | • External attackers<br>• Insiders<br>• Human error<br>• Natural events | Phishing targeting accounting staff. |
| Vulnerability | Weakness that makes exploitation possible. | • Outdated software<br>• Misconfigurations<br>• Weak passwords | Overreliance on one old system like Yardi. |
| Impact | Magnitude of harm if a risk is realized. | • Financial loss<br>• Compliance failure<br>• Reputational damage | Missing a client reporting deadline due to system outage. |
| Risk Categories | Broad types of risks organizations face. | • Strategic<br>• Operational<br>• Financial<br>• Technical<br>• Compliance | Losing access to financial data during period-end reporting. |

---

## 13.2 Risk Response Strategies

| Strategy | Expanded Definition | Nested Key Points (Comparisons) | Workplace Example |
|----------|----------------------|----------------------------------|--------------------|
| ★ Risk Responses | Actions taken to address identified risks. | • Accept<br>• Mitigate<br>• Transfer<br>• Avoid | Used when determining how to manage system reliability issues. |
| Acceptance | Acknowledging the risk without action. | • Used when low likelihood/impact<br>• Cost of control > cost of risk | Accepting minor reporting delays caused by low-impact issues. |
| Mitigation | Reducing likelihood or impact via controls. | • Most common<br>• Technical + administrative controls | Implementing MFA and least privilege to protect client data. |
| Transfer | Shifting risk to third party. | • Cyber insurance<br>• Outsourcing | Vendor-managed secure reporting platform reduces internal responsibility. |
| Avoidance | Eliminating the activity causing the risk. | • Highest control<br>• Often costly<br>• Removes risk entirely | Retiring insecure legacy systems that cannot be patched. |
| Comparison | Accept = no action; Mitigate = reduce; Transfer = shift; Avoid = eliminate. | • Exam will test scenario classification | Choosing mitigation when upgrading redundant servers to prevent downtime. |

---

## 13.3 Security Control Types (Preventive, Detective, Corrective, Compensating)

| Control Type | Expanded Definition | Nested Key Points | Workplace Example |
|--------------|----------------------|--------------------|--------------------|
| ★ Security Controls | Mechanisms used to reduce risk. | • Preventive<br>• Detective<br>• Corrective<br>• Compensating | Required for protecting financial and PII data. |
| Preventive Controls | Stop threats before they occur. | • MFA<br>• Firewalls<br>• Encryption | Okta MFA preventing unauthorized access to Yardi. |
| Detective Controls | Identify incidents that have occurred or are occurring. | • IDS<br>• Logs<br>• Monitoring | Logs showing unauthorized access attempts to shared client folders. |
| Corrective Controls | Fix issues after they occur. | • Backups<br>• Patch application<br>• Restoring systems | Restoring corrupted financial files from backup. |
| Compensating Controls | Alternative safeguards when primary controls are not feasible. | • Additional monitoring<br>• Segmentation | Using network segmentation when certain systems cannot be patched immediately. |
| Comparison | Prevent → stop; Detect → identify; Correct → repair; Compensate → alternative. | • Exam will test mapping controls to scenarios | Using segmentation while planning long-term system upgrades. |

---

## 13.4 Security Policies & Governance Structure

| Policy Type | Expanded Definition | Nested Key Points | Workplace Example |
|--------------|----------------------|--------------------|--------------------|
| ★ Security Policies | High-level rules defining acceptable behavior and security requirements. | • Formal<br>• Organization-wide<br>• Enforcement required | Acceptable Use Policy defining how client documents must be handled. |
| Acceptable Use Policy (AUP) | Defines appropriate use of systems and data. | • Restricts unauthorized activities<br>• Employees must acknowledge | Prohibits storing client PII on unapproved personal devices. |
| Incident Response Policy | Outlines reporting and handling of security incidents. | • Defines escalation<br>• Communication procedures | Staff reporting suspicious emails immediately. |
| Data Classification Policy | Categorizes data by sensitivity. | • Public<br>• Internal<br>• Confidential<br>• Restricted | Client bank data = highly confidential. |
| Relationship Between Policies, Standards, Procedures, Guidelines | Defines governance hierarchy. | • Policies = high level<br>• Standards = mandatory rules<br>• Procedures = how-to steps<br>• Guidelines = recommended best practices | EisnerAmper following formal procedures for accessing client reporting systems. |

---

## 13.5 Study Focus Summary

| Exam Topic                        | Explanation                                                                |
| --------------------------------- | -------------------------------------------------------------------------- |
| Threat vs Vulnerability vs Impact | Know precise definitions and relationships.                                |
| Risk Response Strategies          | Accept, Mitigate, Transfer, Avoid.                                         |
| Security Controls                 | Preventive, Detective, Corrective, Compensating.                           |
| Governance Hierarchy              | Policy → Standard → Procedure → Guideline.                                 |
| Scenario Mapping                  | Be able to choose correct risk response or control type based on scenario. |