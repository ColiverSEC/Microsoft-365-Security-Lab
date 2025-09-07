# 🔐 Microsoft Purview Data Loss Prevention (DLP) Lab

[⬅️ Back to Microsoft 365 Security & Compliance Lab Overview](../README.md)

This lab provides hands-on experience with **Microsoft Purview DLP**, a Microsoft 365 compliance and data protection tool. It focuses on:

- ✅ Creating and publishing Sensitivity Labels for PHI, PII, and other sensitive data  
- ✅ Deploying DLP policies to detect and block sensitive content in transit  
- ✅ Testing policies with real-world scenarios such as emails containing sensitive info  
- ✅ Reviewing alerts and incidents in **Purview** and **Defender for Cloud Apps**  
- ✅ Verifying audit logs for compliance reporting

These walkthroughs simulate **real-world Microsoft 365 security and compliance tasks** that IT and security engineers perform daily.

---

## 📂 Lab Walkthroughs

| Walkthrough | Description |
|------------|-------------|
| 🧑‍💻 [Creating Sensitivity Labels](./docs/dlp-walkthrough.md#creating-sensitivity-labels) | Step-by-step instructions to create parent and sublabels, define classifications, and publish labels to users. |
| 🛡️ [Deploying DLP Policies](./docs/dlp-walkthrough.md#deploying-dlp-policies) | Configure DLP policies, define rules and actions, enable policy mode, and manage policy scope. |
| 📧 [Testing Policies with Emails](./docs/dlp-walkthrough.md#testing-policies-with-emails) | Send test emails containing sensitive data to validate DLP policy enforcement. |
| 🔔 [Reviewing Alerts](./docs/dlp-walkthrough.md#reviewing-alerts) | Monitor policy triggers, view alerts and incidents in Purview and Defender for Cloud Apps. |
| 📄 [Verifying Audit Logs](./docs/dlp-walkthrough.md#verifying-audit-logs) | Check audit logs for DLP events and verify compliance reporting. |

---

## 🛠️ Tools Used

- **Microsoft Purview Compliance Portal**  
- **Microsoft Defender for Cloud Apps**  
- **Microsoft 365 Admin Center**  
- **Exchange Online (Mail Flow)**  

---

## 🌐 Related Labs

| Lab | Focus |
|-----|-------|
| 🧱 [Microsoft 365 Security & Compliance Overview](../README.md) | Core Microsoft 365 compliance and security setup, including Purview and Defender integration. |
| 🔑 [Okta IAM Lab](https://github.com/ColiverSEC/Enterprise-IAM-Lab/tree/main/okta) | Application integrations, MFA policies, lifecycle automation for identities. |
| 🔄 [Hybrid Identity Lab](../entra/README.md) | Connect on-prem AD with Microsoft Entra ID for identity sync and federation. |

---

## 💡 Next Steps

- Expand DLP testing to **SharePoint and OneDrive**  
- Automate DLP policy deployment with **Microsoft Graph or PowerShell**  
- Integrate additional **sensitivity labels** and **auto-labeling policies**  
- Monitor alerts and maintain compliance using **audit logs**  
- Explore advanced DLP **policy tuning** and **user education** to reduce false positives  
