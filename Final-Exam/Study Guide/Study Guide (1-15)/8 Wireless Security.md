
Wireless networks introduce unique security challenges due to their broadcast nature.  
Because signals extend beyond physical boundaries, attackers can intercept, impersonate, or disrupt wireless communications.  
This section focuses on wireless standards, access point architecture, and common threats such as rogue APs, evil twins, and weak encryption protocols.

---

## 8.1 Wireless Network Types & Fundamentals

| Concept | Expanded Definition | Nested Key Points | Workplace Example |
|--------|----------------------|--------------------|--------------------|
| ★ Wireless Networks | Networks that transmit data via radio waves instead of wired connections. | • Personal (PAN)<br>• Local (WLAN)<br>• Wide area (WWAN)<br>• Vulnerable to interception | Employees connecting laptops to office Wi-Fi or home networks when working remotely. |
| PAN (Personal Area Network) | Very short-range wireless communication. | • Bluetooth<br>• Peripheral devices | Bluetooth keyboards/headsets used during reporting work. |
| WLAN (Wireless Local Area Network) | Wi-Fi networks covering offices or homes. | • Most common<br>• Supports business connectivity | EisnerAmper office Wi-Fi or home network for remote employees. |
| WWAN (Wireless Wide Area Network) | Cellular/cellular-based networks. | • LTE/5G<br>• Broader coverage | Accountants connecting via mobile hotspot when traveling. |

---

## 8.2 Wireless Identifiers & Naming (SSID, BSSID)

| Identifier | Expanded Definition | Nested Key Points | Workplace Example |
|------------|----------------------|--------------------|--------------------|
| SSID (Service Set Identifier) | Name of the Wi-Fi network users see when connecting. | • Broadcast or hidden<br>• Can be spoofed | Fake “OfficeWiFi” set up by attacker as an evil twin. |
| BSSID | MAC address of the access point. | • Unique identifier<br>• Used for AP tracking | Distinguishing between legitimate and fake APs in an audit. |
| Wireless Limitations | Constraints of wireless standards. | • Range<br>• Frequency interference<br>• Signal attenuation | Wi-Fi slowing down when many reporting staff upload documents simultaneously. |

---

## 8.3 Access Point Architecture (Autonomous vs Controller-Based)

| Architecture Type | Expanded Definition | Nested Key Points | Workplace Example |
|-------------------|----------------------|--------------------|--------------------|
| Autonomous AP | Standalone access point with all intelligence built in. | • Each AP configured individually<br>• Harder to manage at scale | Small satellite offices or temporary client sites. |
| Controller-Based AP | APs centrally managed by a controller for uniform configuration. | • Easier updates<br>• Consistent security<br>• Scales well | Corporate office maintaining consistent Wi-Fi security settings. |
| Tradeoffs | Choosing between architectures depends on environment size. | • Autonomous: flexible but fragmented<br>• Controller: scalable and centralized | Large firms prefer controller-managed for compliance. |

---

## 8.4 Wireless Threats & Attacks

| Threat Type | Expanded Definition | Nested Key Points (Comparisons) | Workplace Example |
|-------------|----------------------|----------------------------------|--------------------|
| ★ Rogue Access Point | Unauthorized AP plugged into a corporate network. | • Bypasses security<br>• Creates a hidden bridge to attackers | A staff member bringing in a personal AP without approval. |
| Evil Twin | Attacker sets up a fake AP with same SSID as legitimate network. | • Users connect unknowingly<br>• Enables MITM + credential theft | Fake “OfficeWiFi” capturing EisnerAmper employee logins. |
| Deauthentication Attack | Attacker forces devices off AP to reconnect and capture handshakes. | • WPA2 handshake capture<br>• Used for password cracking | Employees getting disconnected from Wi-Fi suddenly during work. |
| Bluesnarfing | Unauthorized access to Bluetooth data. | • Exploits Bluetooth pairing issues | Attack on employee mobile device storing client contacts. |
| Bluejacking | Sending unsolicited Bluetooth messages. | • Harmless but annoying | Distracting pop-ups on accountant laptops. |

---

## 8.5 Wireless Security Protocols (WEP → WPA → WPA2 → WPA3)

| Protocol | Expanded Definition | Nested Key Points (Comparisons) | Workplace Example |
|----------|----------------------|----------------------------------|--------------------|
| ★ Wireless Security Protocols | Encryption standards protecting Wi-Fi networks. | • Different strengths<br>• Old → weak<br>• New → strong | Used to secure office or remote Wi-Fi connections. |
| WEP | Outdated, weak encryption using RC4 and short IVs. | • Easily cracked<br>• Should not be used | A WEP guest network would expose client financial data. |
| WPA | Interim improvement over WEP (uses TKIP). | • More secure than WEP<br>• Still outdated | Not sufficient for handling sensitive data. |
| WPA2 | Uses **AES-CCMP**; industry standard for years. | • Strong encryption<br>• Requires robust passwords | Office Wi-Fi using WPA2 to secure accounting systems. |
| WPA3 | Uses **SAE** to prevent offline password cracking. | • Strongest standard<br>• Modern handshake | Recommended for staff connecting from home. |
| Comparison | WEP = weakest; WPA2 = secure; WPA3 = strongest. | • Exam tests protocol evolution | Choose WPA3 for sensitive client work. |

---

## 8.6 Wireless Security Strategies (Segmentation, Monitoring)

| Strategy | Expanded Definition | Nested Key Points | Workplace Example |
|----------|----------------------|--------------------|--------------------|
| Network Segmentation | Separating wireless networks based on business needs. | • Guest Wi-Fi vs internal Wi-Fi<br>• Limits exposure | Keeping guest Wi-Fi separate from systems storing client financials. |
| Monitoring & Logging | Observing wireless behavior for anomalies. | • Detect rogue APs<br>• Detect unusual connections | Alert triggered when an unknown AP appears in office Wi-Fi space. |
| Strong Authentication | Protects Wi-Fi access. | • WPA3<br>• 802.1X<br>• Certificates | Using Okta + certificate-based Wi-Fi authentication. |

---

## 8.7 Study Focus Summary

| Exam Topic                           | Explanation                                   |
| ------------------------------------ | --------------------------------------------- |
| Identify wireless attack differences | Evil twin vs rogue AP vs deauth attack.       |
| Know protocol evolution              | WEP (weak) → WPA → WPA2 → WPA3 (strongest).   |
| Understand AP architecture           | Autonomous vs controller-based deployments.   |
| Wi-Fi naming & identification        | SSID, BSSID, spoofing risks.                  |
| Wireless segmentation                | Protects internal systems from guest traffic. |
