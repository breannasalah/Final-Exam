Organizations rely on structured network architectures and protocols to support communication, security, scalability, and reliability.  
This section focuses on network types, OSI layers, IP addressing behavior, name resolution, and how symbolic names are translated into usable addresses.

---

## 6.1 Network Types

| Network Type | Expanded Definition | Nested Key Points | Workplace Example |
|--------------|----------------------|--------------------|--------------------|
| ★ Internal Private Network | Network fully controlled and used by the organization. | • Contains sensitive systems<br>• Requires strong access control<br>• Not publicly accessible | EisnerAmper internal network hosting accounting/reporting tools and shared drives. |
| Extended Network | Provides controlled access to certain resources for external users (clients, vendors, partners). | • DMZ design<br>• Segmented from internal network<br>• Limited permissions | Client portals where financial statements or reports may be uploaded. |
| Selectively Accessible Networks | Mix of public and private access rules. | • Conditional access<br>• Least privilege for external parties | Vendor platforms used to transmit financial data securely. |

---

## 6.2 OSI Model Overview

| Layer | Expanded Definition | Nested Key Points | Workplace Example |
|-------|----------------------|--------------------|--------------------|
| ★ OSI Model | Conceptual framework describing network communication in 7 layers. | • Exam tests: which protocol belongs to which layer<br>• Helps diagnose network problems | Understanding why name resolution errors (Layer 7/Layer 3 interplay) break access to reporting tools. |
| Layer 1: Physical | Hardware transmission of raw bits. | • Cables, NICs, signal | Faulty cable causing workstation outages. |
| Layer 2: Data Link | Responsible for MAC addressing and frames. | • Switches<br>• ARP | ARP poisoning attacks occur at Layer 2. |
| Layer 3: Network | IP addressing and routing. | • Routers<br>• IP spoofing | Incorrect IP routes prevent access to shared drives. |
| Layer 4: Transport | Ensures reliable delivery (TCP) or fast delivery (UDP). | • Ports<br>• Connection establishment | TCP port blocked prevents Yardi access. |
| Layer 5–7: Session/Presentation/Application | User-facing network functions and data formatting. | • TLS encryption<br>• HTTPS<br>• Application logic | Secure HTTPS connections used for financial reporting portals. |

---

## 6.3 Internet Protocol (IP)

| Concept | Expanded Definition | Nested Key Points | Workplace Example |
|---------|----------------------|--------------------|--------------------|
| ★ IP (Internet Protocol) | Routes packets across networks using logical addressing. | • IP = Layer 3<br>• Supports fragmentation<br>• Vulnerable to spoofing | IP misconfiguration preventing user access to reporting systems. |
| IPv4 | 32-bit addressing scheme. | • Example: 192.168.x.x<br>• Limited address space | EisnerAmper internal addressing for employee workstations. |
| IPv6 | 128-bit addressing scheme. | • Larger address space<br>• Built-in security features | Used in modern cloud platforms for secure reporting environments. |

---

## 6.4 Name Resolution (DNS and Related Systems)

| Concept | Expanded Definition | Nested Key Points | Workplace Example |
|---------|----------------------|--------------------|--------------------|
| ★ Name Resolution | Converts human-readable names into IP addresses. | • Uses DNS hierarchy<br>• Target for spoofing attacks | Accessing “clientportal.company.com” relies on DNS. |
| DNS (Domain Name System) | Hierarchical naming system mapping names to IP addresses. | • Query → resolver → authoritative server<br>• Vulnerable to poisoning | DNS misconfiguration preventing access to financial data portals. |
| Reverse DNS | Resolves IP address back to hostname. | • Used for verification<br>• Email anti-spam | Ensures emails containing financial docs are verified. |
| Local Name Resolution | OS-level resolution (hosts file, local caches). | • Used when DNS fails or is overridden | Incorrect HOSTS file could misroute traffic. |

---

## 6.5 Subnetting & Addressing Concepts (Optional but Relevant)

| Concept | Expanded Definition | Nested Key Points | Workplace Example |
|---------|----------------------|--------------------|--------------------|
| Subnetting | Dividing large networks into smaller logical groups. | • Improves efficiency<br>• Improves security<br>• Controls broadcast traffic | Segmentation between accounting, reporting, and IT networks. |
| Default Gateway | Device that routes traffic out of the local network. | • Required for external communication | Wrong gateway = no access to cloud-hosted reporting tools. |
| VLANs | Logical network segments on the same physical hardware. | • Improves security<br>• Isolates traffic | Reporting systems on separate VLAN from guest Wi-Fi. |

---

## 6.6 Study Focus Summary

| Study Requirement     | Explanation                                                                             |
| --------------------- | --------------------------------------------------------------------------------------- |
| OSI Model             | Know protocol-to-layer mapping and attack locations (e.g., ARP = L2, IP spoofing = L3). |
| DNS & Name Resolution | Understand how names convert to IPs and how attacks manipulate that process.            |
| Network Types         | Distinguish private, extended, and selectively accessible networks.                     |
| Protocol Behavior     | Know how IP routes, how data is segmented, and why misconfigurations break access.      |