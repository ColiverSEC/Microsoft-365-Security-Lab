# ☁️ Microsoft 365 Security Lab: Cloud Discovery with Microsoft Defender for Cloud Apps

[⬅️ Back to Microsoft 365 Security & Compliance Lab Overview](../README.md)

## 🔍 Focus Area: Shadow IT Discovery & App Risk Analysis

This lab demonstrates how to use **Microsoft Defender for Cloud Apps (MDCA)** to discover unsanctioned applications (Shadow IT) in an environment by ingesting network traffic through firewall logs.

---

## ✅ Objectives

- Upload network traffic logs into Microsoft Defender for Cloud Apps
- Generate a **Cloud Discovery Snapshot Report**
- Analyze discovered apps and review risk scores
- Demonstrate visibility into Shadow IT and cloud app usage

---

## 🛡️ Lab Tools Used

| Service | Purpose |
|--------|-----------------------------------------------------|
| Microsoft Defender for Cloud Apps | Cloud App Discovery & Governance |
| Microsoft 365 Lab Tenant         | Simulated admin environment     |
| Sample Firewall Log               | Simulated network traffic       |

---

## 🔧 Lab Walkthrough

### 1️⃣ Access Microsoft Defender for Cloud Apps

- Go to: [https://security.microsoft.com/](https://security.microsoft.com/)
- Sign in with your administrator account.

---

### 2️⃣ Navigate to Cloud Discovery

- From the left menu, select **Cloud Discovery → Snapshot reports**.

---

### 3️⃣ Create a Snapshot Report

- Click **➕ Create snapshot report**
- Name the report (example: `Lab W3C Discovery Test`)
- Under **Data source**, select:  
   **Generic W3C Log**
- Upload the sample W3C log file created for this lab.  
   *(File contains simulated cloud app traffic such as Dropbox and Slack)*

---

### 4️⃣ Process the Report

- After uploading, allow the system to process the file (**~1–3 minutes**).
- View the **Snapshot reports** list and wait for the status to show as **Completed.**

---

### 5️⃣ Review Discovered Apps

- Navigate to **Cloud Discovery → Discovered apps**
- Analyze the list of cloud applications discovered from the sample log.
- Review app categories, usage statistics, and **Risk Scores**.

---

### 📊 Example Screenshots (Replace with Yours)

*(Add your screenshots below each section)*

**Cloud Discovery Overview:**

![Cloud Discovery Overview Screenshot](link-to-your-screenshot)

**Discovered Apps Report:**

![Discovered Apps Screenshot](link-to-your-screenshot)

**App Risk Details:**

![App Risk Details Screenshot](link-to-your-screenshot)

---

## 🔍 Key Findings

- Shadow IT apps such as Dropbox, Slack, and Google Drive were detected.
- MDCA assigned risk scores to each app based on security posture and compliance.
- Admins can now **sanction** or **unsanction** apps and set up **governance policies**.

---

## 💡 What This Demonstrates

- Hands-on creation of a Cloud Discovery snapshot
- Ingestion and parsing of W3C log files
- Shadow IT discovery capabilities in Microsoft Defender for Cloud Apps
- App risk management and SaaS visibility

---

## 📂 Next Steps

- Integrate Microsoft Defender for Endpoint for **continuous cloud app discovery**
- Configure **App Governance policies** and OAuth app controls
- Explore automated alerting on risky SaaS usage

---


