| **Concept**                                  | **Expanded Definition**                                                                                                        | **Nested Key Points**                                                                                                                                                                                                                  | **Workplace Example (EisnerAmper)**                                                                                                                                                    |
| -------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **★ Information Security**                   | Protects the **confidentiality**, **integrity**, and **availability** of information through people, products, and procedures. | • Protects information during **storage**, **processing**, and **transmission**• Must balance **security vs. convenience**• Losses include more than theft (data corruption, exposure, downtime)• Supports compliance and client trust | • Protecting private equity client financials, reporting files, and PII across systems like Yardi and internal drives.                                                                 |
| **★ CIA Triad**                              | The foundational security model consisting of **Confidentiality**, **Integrity**, and **Availability**.                        | • All three must work together to protect the organization• Failure in any area creates financial, operational, or reputational risk                                                                                                   | • Ensures EisnerAmper can produce accurate, private, and accessible reports for real estate and private equity clients.                                                                |
| **Confidentiality**                          | Ensures information is only accessible to **authorized users**, preventing unauthorized disclosure.                            | • Access controls• MFA (Okta)• Least privilege• Immediate removal of former employees’ access                                                                                                                                          | • Only the accounting/reporting team assigned to a specific client can view their bank data, statements, and PII.• When an employee leaves, Okta deactivates their access immediately. |
| **Integrity**                                | Ensures data remains **accurate, complete, and unaltered** unless properly authorized.                                         | • Prevents unauthorized changes• Catches accidental errors• Uses version control, restricted editing, and review processes                                                                                                             | • Incorrect formulas or overwritten totals in spreadsheets cause reporting delays.• Restricted editing prevents unauthorized or accidental changes.                                    |
| **Availability**                             | Ensures systems and data are **accessible** to authorized users whenever needed.                                               | • Uptime• Redundancy• Backups• Quick recovery• System reliability                                                                                                                                                                      | • When Yardi goes down, accountants cannot run reports, pull balances, or complete deliverables.• Backup servers store snapshots of all accounting data to retain access.              |
| ==**Security vs Convenience**==              | Increasing security often decreases convenience; organizations must balance both.                                              | • MFA adds steps but prevents breaches• Least privilege limits access but reduces risk                                                                                                                                                 | • Okta MFA slightly slows login but protects sensitive client financial information.                                                                                                   |
| **Types of Loss (Beyond Theft)**             | Information security losses include more than stolen data.                                                                     | • Data corruption• System outages• Unauthorized exposure• Missed deadlines from unavailability                                                                                                                                         | • Wrong spreadsheet numbers, missing files, or a Yardi outage delay reporting, reviews, and filings.                                                                                   |
| **★ Threat Actors**                          | Individuals or entities responsible for cyber incidents.                                                                       | • External hackers• Insiders• Careless employees• Natural events                                                                                                                                                                       | • Phishing emails targeting accounting teams, accidental deletion of files, or outages affecting reporting deadlines.                                                                  |
| **How CIA Supports Organizational Security** | The CIA Triad enables safe, accurate, and efficient business operations.                                                       | • Protects sensitive client data• Ensures accurate financial reporting• Keeps systems available for client work• Reduces organizational risk                                                                                           | • CIA ensures client financials remain private, accurate, and accessible — essential for real estate private equity reporting.                                                         |
**Balancing Security & Loss**

• **Security vs. Convenience:** Security is inversely proportional to convenience; as security increases, convenience often decreases.

• **Forms of Loss:** Successful attacks result in financial loss (lost productivity), reputation damage (negative public perception), and availability loss (systems becoming inaccessible).

**Threat Actors**

• **Script Kiddies:** Unskilled individuals who use automated attack software (scripts) downloaded from the internet to perform attacks.

• **Hacktivists:** Attackers strongly motivated by ideology (beliefs or principles) to make political statements or spread disinformation.

• **State Actors:** Government-sponsored attackers who target foreign governments or corporations for espionage or sabotage. They are often associated with Advanced Persistent Threats (APTs),.

• **Insiders:** Employees, contractors, or business partners who manipulate data from a position of trust.

 **– Competitors:** Launch attacks to steal proprietary information for financial gain.
-
- **Social Engineering:** Psychological manipulation of people into performing actions or divulging confidential information.
- **Physical Social Engineering:** Includes dumpster diving (searching trash for data), tailgating (following an authorized person into a secure area), and shoulder surfing (watching someone enter credentials).

Phishing Variants

The following table compares the major social engineering attack types: Whaling, Spear Phishing, Vishing, and Smishing.  
These are high-priority exam topics because they differ by **target**, **medium**, and **intent**.

---

## Phishing Variant Comparisons

| Concept | Expanded Definition | Nested Key Points (Comparisons) | Example Scenario |
|--------|----------------------|----------------------------------|------------------|
| ★ Phishing | Umbrella term for tricking users into revealing information through deceptive communication. | • Uses impersonation<br>• Targets broad audiences<br>• Often email-based | Generic email pretending to be Microsoft asking users to reset their password. |
| Spear Phishing | Highly targeted phishing attempt aimed at a specific person or small group. | • Personalized details<br>• Appears legitimate<br>• Higher success rate | Email sent to an EisnerAmper accountant referencing a real client engagement. |
| Whaling | Spear phishing specifically targeting executives or high-profile individuals. | • C-suite targets<br>• Goal = financial fraud or data theft<br>• Very tailored | Email pretending to be a partner requesting wire transfer details for a client. |
| Vishing | Voice phishing using phone calls to trick users. | • Uses caller ID spoofing<br>• Pretends to be bank, IT, IRS<br>• Social engineering over voice | Call saying “This is IT — your Okta login failed. Read me your MFA code.” |
| Smishing | SMS-based phishing attack. | • Uses text messages<br>• Often includes malicious links<br>• Fast and scalable | Text claiming “Your payroll info needs verification — click here.” |

---

## Quick Memory Cues

| Attack Type    | Memory Cue                        |
| -------------- | --------------------------------- |
| Spear Phishing | Targeted to **a specific person** |
| Whaling        | Targeted to **executives**        |
| Vishing        | **Voice** call phishing           |
| Smishing       | **SMS** text phishing             |