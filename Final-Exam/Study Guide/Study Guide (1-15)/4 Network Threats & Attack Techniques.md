Understanding network attacks is essential for preventing data interception, manipulation, and service disruption.  
Attackers exploit weaknesses in protocols, configurations, and user behavior to intercept, alter, redirect, or overwhelm communications.  
This section focuses on how attacks differ, how attackers position themselves, and why small vulnerabilities can lead to major breaches.

---

## 4.1 Interception Attacks (MITM, MITB, Eavesdropping)

| Concept | Expanded Definition | Nested Key Points | Workplace Example |
|--------|----------------------|--------------------|--------------------|
| ★ Interception Attacks | Attacks where an adversary secretly intercepts or alters communication between two parties. | • Includes MITM, MITB, eavesdropping<br>• Target confidentiality & integrity<br>• Often require attacker to be "in the path" | An attacker on public Wi-Fi intercepts accountant login credentials. |
| MITM (Man-in-the-Middle) | Attacker places themselves between two communicating systems. | • Intercepts data<br>• Can read/modify traffic<br>• Common on insecure networks | Logging into Yardi or reporting tools over unsafe Wi-Fi. |
| MITB (Man-in-the-Browser) | Malware inside the browser modifies transactions. | • Harder to detect<br>• Can alter forms/data before sending | Browser malware changes numbers in a financial portal submission. |
| Eavesdropping | Passive interception of network traffic. | • No modification<br>• Captures unencrypted data | Financial data sent unencrypted over internal network could be observed. |

---

## 4.2 Session-Based Attacks

| Concept | Expanded Definition | Nested Key Points | Workplace Example |
|--------|----------------------|--------------------|--------------------|
| ★ Session Attacks | Target authenticated user sessions to impersonate users. | • Hijacking, replay attacks<br>• Exploit session IDs or tokens | Replay of Yardi session token to impersonate a staff member. |
| Session Hijacking | Attacker takes over an active session. | • Uses stolen tokens<br>• Victim appears logged in | An attacker steals a session cookie to access reporting dashboards. |
| Replay Attack | Captures valid traffic and re-sends it. | • No need to decrypt data<br>• Replays authentication | Replaying MFA-approved request to gain access. |

---

## 4.3 Traffic Analysis

| Concept | Expanded Definition | Nested Key Points | Workplace Example |
|--------|----------------------|--------------------|--------------------|
| ★ Traffic Analysis | Observing patterns in communication to infer sensitive info. | • Doesn't require decrypting info<br>• Identifies who communicates with whom | Attacker monitors when reporting systems send large financial data sets. |

---

## 4.4 Name Resolution Attacks (DNS, ARP)

| Concept | Expanded Definition | Nested Key Points | Workplace Example |
|--------|----------------------|--------------------|--------------------|
| ★ Name Resolution Attacks | Manipulate DNS or ARP to redirect traffic. | • Exploit trust in name-to-IP mapping | Redirecting accountants to fake financial websites. |
| DNS Poisoning | Corrupts DNS entries to redirect users. | • Sends users to malicious sites<br>• Hard to detect | Fake Yardi login page capturing employee credentials. |
| ARP Poisoning | Maps attacker MAC to legitimate IP. | • Redirects LAN traffic<br>• Enables MITM | ARP spoofing to intercept workstation traffic. |

---

## 4.5 Denial of Service (DoS / DDoS)

| Concept | Expanded Definition | Nested Key Points | Workplace Example |
|--------|----------------------|--------------------|--------------------|
| ★ Denial of Service | Overwhelms a system so legitimate users can’t access it. | • DoS = single attacker<br>• DDoS = distributed attack<br>• Targets availability | Reporting system goes offline during peak deadlines. |
| DDoS | Multiple machines overwhelm target. | • Botnets<br>• Large-scale disruption | Encrypted reporting portal becomes inaccessible to staff. |

---

## 4.6 Address Spoofing

| Concept | Expanded Definition | Nested Key Points | Workplace Example |
|--------|----------------------|--------------------|--------------------|
| ★ Address Spoofing | Faking identity at network or application layer. | • IP spoofing<br>• MAC spoofing<br>• Email spoofing | Spoofed email pretending to be partner requesting financial files. |

---

## 4.7 Application-Layer Attacks (Injection, Privilege Escalation)

| Concept | Expanded Definition | Nested Key Points | Workplace Example |
|--------|----------------------|--------------------|--------------------|
| ★ Application-Layer Attacks | Target weaknesses in programs and input handling. | • Injection<br>• Directory traversal<br>• Privilege escalation | Improperly sanitized inputs in a financial portal could expose client data. |
| Injection Attacks | Attacker inserts malicious input into an application. | • SQL injection<br>• LDAP injection<br>• Poor input validation | Attacker extracts financial tables from poorly protected database. |
| Privilege Escalation | Gaining higher privileges than intended. | • Vertical escalation: user → admin<br>• Horizontal escalation: user → another user | Attacker gains access to restricted client folders. |

---

## 4.8 Study Focus Summary

| Study Requirement    | Explanation                                                                         |
| -------------------- | ----------------------------------------------------------------------------------- |
| Spoofing differences | Know how ARP, DNS, IP, and email spoofing differ.                                   |
| Injection weaknesses | Understand how improper input validation leads to SQL, LDAP, and command injection. |
| Escalation chain     | Small vulnerabilities → foothold → privilege escalation → major breach.             |
| Compare layers       | Interception (network path) vs application attacks (input/logic flaws).             |