Endpoints — laptops, desktops, tablets, and phones — represent the most common entry points for attackers.  
This section covers mobile device management, deployment models, application control techniques, and common mobile risk factors.  
Your exam will focus on distinguishing device management approaches, understanding mobile threats, and recognizing how policy and technology reduce endpoint risk.

---

## 9.1 Mobile Device Management Approaches (MDM, MAM, App Wrapping)

| Concept | Expanded Definition | Nested Key Points (Comparisons) | Workplace Example |
|---------|----------------------|----------------------------------|--------------------|
| ★ Endpoint Security | Protects end-user devices from threats and unauthorized access. | • Key risks: malware, lost/stolen devices, weak configs<br>• Requires policy + technology | Protecting laptops used by EisnerAmper accountants to access client data. |
| MDM (Mobile Device Management) | Full-device management controlling OS-level settings. | • Enforces passcodes<br>• Can wipe device<br>• Manages all apps | Corporate-owned phones used by staff for secure email and MFA. |
| MAM (Mobile Application Management) | Controls only work applications, not the entire device. | • Ideal for BYOD<br>• Containerizes work apps<br>• Separates personal & work data | Managing only the financial-reporting app on employee-owned devices. |
| Application Wrapping | Applies security policies to specific apps. | • No device-wide control<br>• Granular restrictions (copy/paste, sharing)<br>• Can enforce encryption | Wrapping a reporting app to prevent exporting client files. |
| Comparison | MDM = whole device; MAM = app-level; Wrapping = app-specific policy. | • BYOD uses MAM<br>• Corporate devices use MDM | EisnerAmper allowing limited work app access on personal phones. |

---

## 9.2 Device Deployment Models (BYOD, COPE, CYOD, VDI)

| Model | Expanded Definition | Nested Key Points | Workplace Example |
|--------|----------------------|--------------------|--------------------|
| ★ Deployment Models | Policies defining who owns the device and how it is managed. | • Impacts security<br>• Impacts support requirements | Used to determine control over employee laptops/phones. |
| BYOD (Bring Your Own Device) | Employees use personal devices for work. | • Lower cost<br>• Higher security risk<br>• Requires MAM | Staff using personal phones for Okta authentication. |
| COPE (Corporate-Owned, Personally Enabled) | Company owns device but allows personal use. | • Balanced control<br>• Strong security<br>• Lower privacy for employee | EisnerAmper-issued laptops used for reporting work. |
| CYOD (Choose Your Own Device) | Employees choose from approved devices. | • Ensures compatibility<br>• Controlled hardware list | Offering approved models for new accountants. |
| VDI (Virtual Desktop Infrastructure) | Work desktop runs on remote server; device is only a viewer. | • No data stored locally<br>• High security<br>• Works with thin clients | Accessing financial data via secure remote desktop. |

---

## 9.3 Mobile Risk Factors

| Risk Factor | Expanded Definition | Nested Key Points | Workplace Example |
|-------------|----------------------|--------------------|--------------------|
| ★ Mobile Risks | Security concerns unique to mobile and endpoint devices. | • Device loss<br>• Malware<br>• Weak passwords<br>• Unpatched OS/apps | Staff losing a laptop containing confidential client spreadsheets. |
| Lost/Stolen Devices | Devices with sensitive data fall into wrong hands. | • Requires encryption<br>• Requires remote wipe | Lost laptop containing investor documents. |
| Malicious Applications | Apps that steal data or compromise devices. | • App store risks<br>• Sideloading dangers | Downloading an unofficial financial calculator app containing malware. |
| Delayed Security Patching | Users failing to update OS or apps. | • Increases vulnerability window | Outdated device OS exploited by malware. |
| Weak Authentication | Poor password or no MFA. | • Greater chance of unauthorized access | Not using MFA for access to reporting systems. |

---

## 9.4 Mobile Controls & Mitigations

| Control Type | Expanded Definition | Nested Key Points | Workplace Example |
|---------------|----------------------|--------------------|--------------------|
| Screen Locks & Biometrics | Prevent unauthorized access to device. | • PINs<br>• FaceID<br>• Fingerprint | Protecting client data on staff laptops. |
| Remote Wipe | Ability to erase device contents remotely. | • Critical for lost/stolen devices | Removing sensitive financial data from lost laptop. |
| App Permissions | Controls app-level access. | • Prevents over-privileged apps | Restricting an app from accessing file storage. |
| Encryption | Protects data stored on device. | • Full-disk encryption<br>• App-level encryption | Encrypting spreadsheets containing bank data. |

---

## 9.5 Study Focus Summary

| Exam Topic                 | Explanation                                                   |
| -------------------------- | ------------------------------------------------------------- |
| MDM vs MAM vs App Wrapping | Know differences in control and use cases.                    |
| Deployment Models          | BYOD vs COPE vs CYOD vs VDI.                                  |
| Mobile Risks               | Device loss, unpatched software, malicious apps.              |
| Controls & Policies        | Screen locks, remote wipe, encryption, strong authentication. |