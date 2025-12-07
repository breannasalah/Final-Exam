Cloud computing provides on-demand access to computing resources such as virtual machines, databases, and software applications.  
This section focuses on cloud service models (IaaS, PaaS, SaaS), deployment types, and the shared responsibility model.  
Your exam will test your ability to distinguish service models based on what **the provider manages vs. what the customer manages**.

---

## 7.1 Cloud Service Models (IaaS vs PaaS vs SaaS)

| Model | Expanded Definition | Nested Key Points (Comparisons) | Workplace Example |
|-------|----------------------|----------------------------------|--------------------|
| ★ Cloud Service Models | Categories of cloud offerings that define who manages which components. | • IaaS = infrastructure<br>• PaaS = development platform<br>• SaaS = ready-to-use software | Cloud-based reporting tools used by EisnerAmper rely on these models. |
| IaaS (Infrastructure as a Service) | Provider manages hardware; customer manages OS, applications, data. | • Most control<br>• Most responsibility<br>• Examples: AWS EC2, Azure VMs | Hosting a custom financial reporting tool on virtual machines. |
| PaaS (Platform as a Service) | Provider manages hardware + OS; customer deploys applications. | • Simplifies development<br>• No OS maintenance<br>• Examples: Azure App Service, Google App Engine | Deploying internal reporting dashboards without managing servers. |
| SaaS (Software as a Service) | Provider manages everything; customer uses the application. | • Least control<br>• Fast deployment<br>• Examples: Office 365, Salesforce | Using cloud-based applications to store client deliverables. |
| Comparison | Control decreases as you move from IaaS → SaaS. | • IaaS = flexible<br>• PaaS = simpler<br>• SaaS = turnkey | Choosing SaaS tools for simpler processes, IaaS for custom ones. |

---

## 7.2 Cloud Deployment Models

| Deployment Model | Expanded Definition | Nested Key Points | Workplace Example |
|-------------------|----------------------|--------------------|--------------------|
| ★ Deployment Models | Ways cloud environments are hosted and accessed. | • Public<br>• Private<br>• Hybrid<br>• Community | Used when selecting where to host financial portals. |
| Public Cloud | Infrastructure shared across many customers. | • Cost-effective<br>• Highly scalable<br>• Less control | Using a public cloud SaaS tool for collaboration. |
| Private Cloud | Infrastructure dedicated to one organization. | • Highest control<br>• Highest cost<br>• Strong security | Hosting sensitive client financial data internally. |
| Hybrid Cloud | Mix of public and private environments. | • Flexible<br>• Supports workload migration | Storing core reporting systems internally but using cloud analytics. |
| Community Cloud | Shared by organizations with similar needs. | • Shared policies<br>• Similar security requirements | Used among firms with shared regulatory requirements. |

---

## 7.3 Shared Responsibility Model

| Concept | Expanded Definition | Nested Key Points | Workplace Example |
|---------|----------------------|--------------------|--------------------|
| ★ Shared Responsibility | Security obligations are divided between cloud provider and customer. | • Provider = infrastructure<br>• Customer = data, access, applications<br>• Varies by IaaS/PaaS/SaaS | Customer responsibility includes securing client financial data even if stored in cloud apps. |
| Provider Responsibilities | What the cloud provider must secure. | • Hardware<br>• Network<br>• Physical security | AWS securing the data center hosting virtual machines. |
| Customer Responsibilities | What EisnerAmper must secure when using cloud services. | • User access<br>• Data classification<br>• Encryption<br>• Configurations | Ensuring documents and financial statements are encrypted before storage. |
| Comparison | Responsibility shifts depending on service model. | • SaaS = provider handles most<br>• IaaS = customer handles most | Selecting SaaS products for convenience or IaaS for customization. |

---

## 7.4 Cloud Security Considerations

| Concept | Expanded Definition | Nested Key Points | Workplace Example |
|---------|----------------------|--------------------|--------------------|
| Data Encryption | Protects confidentiality in cloud environments. | • Encrypt at rest<br>• Encrypt in transit | Encrypting uploaded financial spreadsheets. |
| Access Control | Ensures only proper users can access cloud resources. | • MFA<br>• RBAC<br>• Zero trust | Using Okta MFA to access cloud reporting tools. |
| Misconfiguration Risk | Incorrect settings can expose data. | • Public buckets<br>• Weak credentials | Misconfigured cloud storage exposing client files. |
| Vendor Lock-In | Difficulty migrating away from a cloud provider. | • Proprietary services<br>• High switching costs | Being tied to a specific reporting platform. |

---

## 7.5 Cloud Service Model Study Focus

| Study Requirement               | Explanation                                                               |
| ------------------------------- | ------------------------------------------------------------------------- |
| Know differences                | Understand what provider vs customer manages.                             |
| Apply scenario questions        | Identify which model fits what business need.                             |
| Understand responsibility shift | SaaS = least responsibility; IaaS = most.                                 |
| Select appropriate model        | Match reporting, analytics, or storage to the correct cloud service tier. |