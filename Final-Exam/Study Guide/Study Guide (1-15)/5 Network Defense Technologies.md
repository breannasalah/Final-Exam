Network defense relies on multiple layers of protection that work together to prevent, detect, and respond to attacks.  
This section focuses on firewalls, proxies, intrusion detection/prevention, NAC, and VPN architecture.  
Your exam will test your ability to distinguish these technologies and explain how defense-in-depth reduces risk.

---

## 5.1 Firewalls (Packet Filtering vs Stateful vs NGFW)

| Technology | Expanded Definition | Nested Key Points (Comparisons) | Workplace Example |
|------------|----------------------|----------------------------------|--------------------|
| ★ Firewalls | Devices that filter traffic entering/exiting a network based on rules. | • Enforce security policies<br>• Can be packet-filtering, stateful, or next-gen | Protecting EisnerAmper networks from unauthorized external access. |
| Packet Filtering Firewall | Evaluates packets individually without tracking connection state. | • Fast<br>• Basic filtering<br>• No context awareness | Filtering basic inbound/outbound traffic based on IP and port. |
| Stateful Firewall | Tracks active connections and allows/blocks packets based on session state. | • More secure than packet filtering<br>• Understands context (e.g., allowed responses) | Ensuring only valid return traffic reaches internal reporting systems. |
| Next-Generation Firewall (NGFW) | Advanced firewall that analyzes traffic at application level. | • Deep Packet Inspection<br>• Can block malware<br>• Can enforce application-level rules | Blocking malicious traffic targeting financial reporting tools (e.g., Yardi portal). |
| Comparison | Packet filtering = simplest; Stateful = connection-aware; NGFW = most intelligent. | • Exam tests differences<br>• NGFW = combines firewall + IPS capabilities | Used to prevent unauthorized access to EisnerAmper’s internal systems. |

---

## 5.2 Proxy Servers

| Technology | Expanded Definition | Nested Key Points | Workplace Example |
|------------|----------------------|--------------------|--------------------|
| ★ Proxy Server | Intermediary between users and the internet; filters and caches content. | • Hides client IP addresses<br>• Filters web requests<br>• Caches frequently accessed resources | Ensuring safe browsing when accountants access external financial sites. |
| Forward Proxy | Sits between internal users and the internet. | • Controls outbound traffic<br>• Common in corporate networks | Blocking risky domains known for phishing. |
| Reverse Proxy | Sits in front of internal servers to protect them. | • Controls inbound traffic<br>• Load balancing<br>• SSL offloading | Protecting a client-facing financial portal from direct exposure. |

---

## 5.3 IDS vs IPS

| Technology | Expanded Definition | Nested Key Points (Comparisons) | Workplace Example |
|------------|----------------------|----------------------------------|--------------------|
| ★ Intrusion Detection/Prevention | Systems that monitor or block malicious activity. | • IDS = detect/alert<br>• IPS = block/prevent | Monitoring network activity for threats targeting financial data. |
| IDS (Intrusion Detection System) | Monitors traffic and alerts on suspicious activity. | • Passive<br>• No blocking<br>• Signature or anomaly-based | Alerting if unusual access attempts target Yardi or reporting servers. |
| IPS (Intrusion Prevention System) | Actively blocks malicious traffic. | • Inline<br>• Real-time prevention<br>• Stops attacks in progress | Blocking SQL injection attempts targeting accounting databases. |
| Comparison | IDS watches, IPS acts. | • IDS = detection<br>• IPS = prevention | Using IPS to block known ransomware signatures. |

---

## 5.4 Honeypots

| Technology | Expanded Definition | Nested Key Points | Workplace Example |
|------------|----------------------|--------------------|--------------------|
| ★ Honeypot | Decoy system designed to lure attackers. | • Appears vulnerable<br>• Collects information on attackers<br>• Helps improve defenses | A decoy financial reporting server used to detect malicious probing attempts. |

---

## 5.5 Network Access Control (NAC)

| Technology | Expanded Definition | Nested Key Points | Workplace Example |
|------------|----------------------|--------------------|--------------------|
| ★ NAC (Network Access Control) | Enforces security policies on devices before granting network access. | • Verifies device health (patches, antivirus)<br>• Ensures compliance<br>• Can quarantine noncompliant devices | Ensures employee laptops meet security requirements before accessing client data. |

---

## 5.6 Virtual Private Networks (VPN)

| Concept | Expanded Definition | Nested Key Points | Workplace Example |
|---------|----------------------|--------------------|--------------------|
| ★ VPN | Encrypted connection between remote user and internal network. | • Protects data in transit<br>• Allows secure remote access | Accountants connecting securely while traveling or working remotely. |
| VPN Concentrator | Device designed to manage large numbers of VPN connections. | • Handles authentication<br>• Scales for many users | Supporting many EisnerAmper employees accessing internal systems during peak times. |
| Split Tunneling | Only some traffic goes through VPN; rest goes directly to internet. | • Faster performance<br>• Less secure | Avoided when handling sensitive financial files. |
| Full Tunnel | All traffic goes through VPN. | • More secure<br>• Higher workload on VPN concentrator | Used when accessing client financial data remotely. |

---

## 5.7 Core Principle: Defense-in-Depth

| Concept            | Expanded Definition                                 | Nested Key Points                                                                    | Workplace Example                                                                                 |
| ------------------ | --------------------------------------------------- | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------- |
| ★ Defense-in-Depth | Using multiple layered controls to protect systems. | • No single control is sufficient<br>• Layers: firewall + IPS + NAC + VPN + policies | EisnerAmper uses layered controls to protect client PII, financial data, and reporting workflows. |