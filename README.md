# Microsoft 365 Security & Compliance Lab 🛡️
Hands-on labs covering Microsoft 365 Security and Compliance tools including Microsoft Purview, Microsoft Defender, and Intune. Focused on real-world identity protection, data governance, and device management scenarios.

---

This lab demonstrates the practical use of **Microsoft 365 security and compliance tools**, focusing on configuring and testing:

- 🔍 Microsoft Purview Compliance Portal
- 🛡️ Microsoft Defender Portal
- 📱 Microsoft Intune

The lab simulates how these tools work together to protect sensitive data, enforce compliance policies, and secure devices and users across an M365 tenant.

---

## 🔧 Lab Sections

### 1️⃣ [Purview Compliance Lab](./purview/README.md)
Focus: **Data Loss Prevention (DLP), Sensitivity Labels, Audit Logs, and Compliance Solutions.**

Topics Covered:
- DLP Policy creation & testing
- Sensitivity Labels and Auto-Labeling
- Compliance alerts in Purview
- Audit log search and compliance reporting

---

### 2️⃣ [Defender for Cloud Apps Lab](./defender/README.md)
Focus: **Threat Detection, App Governance, and Security Operations.**

Topics Covered:
- Cloud App discovery
- Creating and triggering Defender alerts
- Reviewing incidents and taking response actions
- Integrating Defender for Cloud Apps with Purview alerts

---

### 3️⃣ [Intune Device & App Management Lab](./intune/README.md)
Focus: **Device Compliance, Conditional Access, and App Protection Policies.**

Topics Covered:
- Enrolling and managing devices
- Configuring device compliance policies
- Deploying app protection policies
- Triggering Conditional Access scenarios

---

## 📊 End-to-End Use Case Example

1. **A user tries to send an email containing PHI data.**
2. **Purview DLP** blocks the email and raises an alert.
3. **Defender** picks up the alert for security review.
4. If the user’s device is non-compliant, **Intune** applies Conditional Access and restricts access.

---

## 🚨 Tools Used
- Microsoft Purview Compliance Portal
- Microsoft Defender Portal
- Microsoft Intune
- Exchange Online (for mail flow and DLP testing)

---

👉 See each folder for step-by-step guides and screenshots.

