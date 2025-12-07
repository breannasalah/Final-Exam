11 Identity & Access Management

Identity & Access Management (IAM) ensures that the right individuals access the right systems and data at the right time.  
This section focuses on authentication factors, identity federation, directory services, and key authentication protocols.  
Your exam will test your ability to distinguish authentication vs authorization, identify MFA categories, and match protocols to their functions.

---

## 11.1 Core Identity Concepts

| Concept | Expanded Definition | Nested Key Points | Workplace Example |
|---------|----------------------|--------------------|--------------------|
| ★ IAM (Identity & Access Management) | Framework for managing digital identities and controlling access to systems and resources. | • Ensures proper authentication<br>• Enforces authorization policies<br>• Supports least privilege | Okta managing staff login to EisnerAmper tools (Yardi, reporting platforms). |
| Identity | Unique representation of a user or system. | • Usernames, accounts<br>• Stored in directories | Your Okta account representing your work identity. |
| Authentication | Verifies user identity. | • Something you know/have/are<br>• MFA strengthens authentication | Okta MFA push when logging into reporting systems. |
| Authorization | Determines what an authenticated user is allowed to do. | • Role-based access<br>• Least privilege | Only client-assigned teams can view/report on specific client financials. |
| Accounting (Auditing) | Tracking user actions for logging and compliance. | • Logins<br>• Access attempts<br>• File actions | Tracking who accessed or exported a financial report. |

---

## 11.2 Single Sign-On (SSO) & Federated Identity

| Concept | Expanded Definition | Nested Key Points | Workplace Example |
|---------|----------------------|--------------------|--------------------|
| ★ Single Sign-On (SSO) | One authentication event grants access to multiple applications. | • Reduces password fatigue<br>• Relies on central identity provider | Logging into multiple EisnerAmper systems after one Okta sign-in. |
| Federated Identity | Identity shared across trusted organizations/systems. | • Uses SAML, OAuth<br>• Identity provider (IdP) and service provider (SP) | Using Okta as IdP to authenticate into cloud reporting tools. |

---

## 11.3 Authentication Factors (MFA)

| Factor Type | Expanded Definition | Nested Key Points | Workplace Example |
|-------------|----------------------|--------------------|--------------------|
| ★ Authentication Factors | Categories of proof used to verify identity. | • Knowledge, possession, inherence<br>• Stronger when combined (MFA) | EisnerAmper requires Okta MFA for remote logins. |
| Knowledge Factor | Something you know. | • Passwords<br>• PINs | Your Okta password for account login. |
| Possession Factor | Something you have. | • Phone (Okta push)<br>• Hardware token | Approving Okta MFA from your phone. |
| Inherence Factor | Something you are. | • Fingerprint<br>• FaceID | Using biometrics to unlock work devices. |
| Location/Behavioral | Based on context or user behavior. | • Geolocation<br>• Typing patterns | Logging flagged as suspicious if coming from unusual locations. |

---

## 11.4 Authentication Protocols & Directory Services

| Protocol / Service | Expanded Definition | Nested Key Points (Comparisons) | Workplace Example |
|---------------------|----------------------|----------------------------------|--------------------|
| ★ Authentication Protocols | Methods used to authenticate users securely. | • Kerberos<br>• RADIUS<br>• TACACS+<br>• LDAP | Logging into internal and cloud systems using standardized authentication flows. |
| Kerberos | Ticket-based authentication system. | • Prevents replay attacks<br>• Uses KDC (Key Distribution Center)<br>• Mutual authentication | Internal corporate systems requiring secure sign-in using Kerberos tickets. |
| RADIUS | Centralized AAA protocol used in network access. | • Encrypts only password<br>• Uses UDP<br>• Scalable | Used for Wi-Fi authentication or VPN access. |
| TACACS+ | AAA protocol used often in device administration. | • Encrypts entire packet<br>• Uses TCP<br>• Separates authentication and authorization | Managing administrative access to network devices. |
| LDAP | Directory access protocol (X.500 family). | • Stores identities<br>• Hierarchical<br>• Used by identity systems | Storing user accounts linked to Okta or internal AD. |

---

## 11.5 Web-Based Authentication Standards (SAML, OAuth, OIDC)

| Standard | Expanded Definition | Nested Key Points | Workplace Example |
|----------|----------------------|--------------------|--------------------|
| ★ Web Authentication Standards | Frameworks for exchanging authentication/authorization data. | • SAML = authentication<br>• OAuth = authorization<br>• OIDC = identity layer | Okta using SAML to sign into cloud reporting tools. |
| SAML | XML-based authentication standard. | • IdP → SP assertions<br>• Often used for SSO enterprise apps | Logging into secure financial reporting platforms via Okta. |
| OAuth | Authorization framework (NOT authentication). | • Grants scoped permissions<br>• Used by APIs<br>• “Login with Google”—but really authorization | Allowing access to limited data without sharing credentials. |
| OpenID Connect (OIDC) | Authentication layer built on OAuth2. | • User identity verified<br>• Uses JSON tokens | Modern cloud applications verifying accountant identities. |

---

## 11.6 Least Privilege & Access Control

| Concept | Expanded Definition | Nested Key Points | Workplace Example |
|---------|----------------------|--------------------|--------------------|
| ★ Least Privilege | Users receive only the access needed for their role. | • Reduces blast radius<br>• Minimizes data exposure | Only client-assigned staff can open specific client folders or reporting files. |
| Role-Based Access Control (RBAC) | Permissions assigned based on job role. | • Consistent<br>• Scalable | Reporting team having access to financial schedules but not tax folders. |
| Account Provisioning | Creating accounts with correct access. | • Based on role<br>• Reviewed regularly | IT provisioning new staff with access only to their assigned clients. |
| Account Deprovisioning | Removing access when no longer needed. | • Immediate for terminated employees<br>• Critical for security | Okta disables access instantly when someone leaves EisnerAmper. |

---

## 11.7 Study Focus Summary

| Exam Topic                      | Explanation                                             |
| ------------------------------- | ------------------------------------------------------- |
| Authentication vs Authorization | Who you are vs what you can do.                         |
| MFA Factors                     | Know all categories, not just passwords.                |
| SSO & Federation                | Understand IdP, SP, and token exchanges.                |
| Protocol Differences            | Kerberos tickets, RADIUS vs TACACS+, LDAP as directory. |
| Least Privilege                 | Role-based access and immediate deprovisioning.         |