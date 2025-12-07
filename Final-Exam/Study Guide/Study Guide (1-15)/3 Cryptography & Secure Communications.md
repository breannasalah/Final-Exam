Cryptography supports confidentiality, integrity, authentication, and trust.  
Below are the required comparisons and subtopics from the study guide.

---

## 3.1 Symmetric vs Asymmetric Encryption

| Concept | Expanded Definition | Nested Key Points (Comparisons) | Workplace Example |
|--------|----------------------|----------------------------------|--------------------|
| ★ Encryption | Converts readable data (plaintext) into unreadable ciphertext to protect confidentiality. | • Two categories: symmetric & asymmetric<br>• Encryption protects confidentiality<br>• Often combined for secure sessions | Encrypting client reports so only authorized EisnerAmper staff can open them. |
| Symmetric Encryption | Uses one shared key for both encryption and decryption. | • Fast, efficient<br>• Weakness: key distribution<br>• Algorithms: AES, 3DES | Encrypting large Excel financial models or backup files. |
| Asymmetric Encryption | Uses public key (encrypt) and private key (decrypt). | • Slower than symmetric<br>• Great for key exchange<br>• Enables digital signatures<br>• Algorithms: RSA, ECC | Secure exchange of session keys before transmitting client financials. |
| How They Work Together | Combined for secure communication. | • Asymmetric → exchange symmetric session key<br>• Symmetric → encrypt high-volume data | Secure browser connection to client financial portals. |

---

## 3.2 Hashing vs Digital Signatures

| Concept | Expanded Definition | Nested Key Points (Comparisons) | Workplace Example |
|--------|----------------------|----------------------------------|--------------------|
| Hashing | One-way function that outputs a fixed-length digest. | • Ensures integrity only<br>• Any change → new hash<br>• Algorithms: SHA-256, SHA-3 | Verifying that investor reports haven't been altered before distribution. |
| Digital Signature | Uses asymmetric cryptography + hashing to verify sender and integrity. | • Proves authenticity<br>• Proves integrity<br>• Requires private key | A partner digitally signs financial statements to verify approval. |
| Comparison | Hash = integrity; Signature = identity + integrity. | • Hashing doesn’t prove who created the file<br>• Digital signatures bind identity to document | Validating EisnerAmper-signed reporting documents. |

---

## 3.3 PKI Components

| Component | Expanded Definition | Nested Key Points | Workplace Example |
|-----------|----------------------|--------------------|--------------------|
| ★ Public Key Infrastructure (PKI) | Framework that manages certificates and key pairs for trust. | • Provides authentication, encryption, integrity<br>• Supports HTTPS, VPNs | Ensures secure logins to encrypted financial portals. |
| Certificate Authority (CA) | Issues and signs certificates. | • Root of trust<br>• Verifies identity | CA-signed certificates authenticate secure reporting systems. |
| Registration Authority (RA) | Confirms identity before certificate issuance. | • Performs checks for CA<br>• Validates entities | Prevents unauthorized systems from obtaining certificates. |
| CRL (Certificate Revocation List) | List of revoked certificates. | • Published periodically<br>• Certificates on list are invalid | Prevents use of compromised certificates. |
| OCSP | Real-time certificate status check. | • Faster than CRL<br>• Supports stapling | Used when staff access secure reporting applications. |

---

## 3.4 Encryption vs Encoding vs Authentication

| Concept | Expanded Definition | Nested Key Points (Comparisons) | Workplace Example |
|--------|----------------------|----------------------------------|--------------------|
| Encryption | Scrambles data to protect confidentiality. | • Requires keys<br>• Cannot be reversed without key | Encrypting client PII before sending internally. |
| Encoding | Converts data into a different format; not for security. | • Reversible<br>• Example: Base64 | Encoding a PDF does NOT secure it. |
| Authentication | Verifies identity of user/system. | • Something you know/have/are<br>• Provides identity, not confidentiality | Okta MFA for accountants accessing Yardi. |
| Comparison | Encryption hides content; encoding changes format; authentication verifies identity. | • Not interchangeable<br>• Encoding ≠ encryption | Encrypting a financial spreadsheet vs simply encoding it. |

---

## 3.5 Block Cipher Modes

| Mode | Expanded Definition | Nested Key Points | Workplace Example |
|------|----------------------|--------------------|--------------------|
| ★ Block Cipher Modes | Methods for applying block ciphers to large data. | • Some provide confidentiality only<br>• Others provide authenticated encryption | Encrypting exported financial reports. |
| CBC | Chain-based mode where each block uses previous block. | • Requires IV<br>• Errors cascade | Older file encryption in secure transfers. |
| GCM | Provides authenticated encryption (confidentiality + integrity). | • Fast<br>• Modern<br>• Used widely | Secure cloud-based report distribution. |

---

## 3.6 Session Keys

| Concept | Expanded Definition | Nested Key Points | Workplace Example |
|--------|----------------------|--------------------|--------------------|
| Session Key | Temporary symmetric key used for one session. | • Exchanged with asymmetric encryption<br>• Efficient for bulk data | Protecting in-transit client financial data during secure browser sessions. |

---

## 3.7 Why Cryptographic Attacks Succeed

| Cause                 | Expanded Definition                          | Nested Indicators                                  | Workplace Example                         |
| --------------------- | -------------------------------------------- | -------------------------------------------------- | ----------------------------------------- |
| Weak Implementations  | Strong algorithms used incorrectly.          | • Outdated TLS<br>• Wrong cipher modes             | Reporting portals misconfigured.          |
| Poor Key Management   | Keys stored improperly or reused.            | • Shared keys<br>• Unprotected key files           | Encryption keys stored on shared drives.  |
| Human Error           | Mistakes exposing data.                      | • Sending unencrypted files<br>• Wrong permissions | Emailing unencrypted investor statements. |
| Misconfigured Systems | System fails to enforce encryption properly. | • Encryption disabled<br>• Open ports              | A reporting server without HTTPS.         |