# ☁️ Microsoft 365 Security Lab: Cloud Discovery with Microsoft Defender for Cloud Apps

[⬅️ Back to Microsoft 365 Security & Compliance Lab Overview](../README.md)

This lab demonstrates hands-on experience with **Microsoft Defender for Cloud Apps (MDCA)** for Shadow IT discovery and cloud app risk analysis. The lab guides you through uploading firewall logs, generating Cloud Discovery snapshot reports, analyzing discovered apps, and understanding app risk scores.

---

## 🔍 Lab Objectives

- Upload network traffic logs into MDCA  
- Generate a **Cloud Discovery Snapshot Report**  
- Analyze discovered apps and review risk scores  
- Understand Shadow IT exposure and take action to govern cloud apps  

---

## 🛠️ Tools Used

| Service | Purpose |
|--------|-----------------------------------------------------|
| Microsoft Defender for Cloud Apps | Cloud App Discovery & Governance |
| Microsoft 365 Lab Tenant         | Simulated admin environment |
| Sample Firewall Log               | Simulated network traffic (W3C log) |

---

## 🧑‍💻 Full Walkthrough: Cloud Discovery Snapshot Report

### Step 1️⃣: Sign in and Access Cloud Discovery

- Navigate to: [https://security.microsoft.com/](https://security.microsoft.com/)  
- Sign in with your administrator or lab account  
- From the left-hand menu, select **Cloud Discovery**

📸 Screenshot:  
![Cloud Discovery Dashboard](../screenshots/01-cloud-discovery-dashboard.png)  
*Cloud Discovery dashboard showing navigation menu.*

---

### Step 2️⃣: Create a Snapshot Report

- Go to **Cloud Discovery → Snapshot reports**  
- Click **+ Create snapshot report**  
- Enter a descriptive name (e.g., `Sample Lab W3C Log`)  
- Under **Data source**, select **Generic W3C Log**  
- Click **Upload file** and select your `sample-w3c.log`  
- Click **Create** to start processing

📸 Screenshot:  
![Create Snapshot Report](../screenshots/02-create-snapshot-report.png)  
*Creating a new snapshot report with Generic W3C Log.*

---

### Step 3️⃣: Monitor Report Processing

- The report will show as **Processing**  
- Wait 1–3 minutes for processing to complete  
- Refresh the page until the status shows **Completed**

📸 Screenshots:  
![Snapshot Report Processing](../screenshots/03-snapshot-report-processing.png)  
![Snapshot Report Completed](../screenshots/04-snapshot-report-completed.png)  
*Processing status and completion of the snapshot report.*

---

### Step 4️⃣: Review Discovered Apps

- Navigate to **Cloud Discovery → Discovered apps**  
- Examine the list of apps from the snapshot log (e.g., Dropbox, Slack, Google Drive)  
- Click an app to view:
  - App category and description  
  - Usage statistics  
  - Security **risk score**

📸 Screenshots:  
![Discovered Apps List](../screenshots/05-discovered-apps-list.png)  
![App Risk Details](../screenshots/06-app-risk-details.png)  

---

### Step 5️⃣: Interpret and Take Action

- Review **risk scores** to prioritize apps for governance  
- Decide which apps to **Sanction** or **Unsanction** based on company policy  
- Optionally create governance policies to monitor or restrict risky apps  
- Use insights to inform cloud security strategy and Shadow IT management  

---

## 📊 Key Findings

- Shadow IT apps such as Dropbox, Slack, and Google Drive were detected  
- MDCA assigned **risk scores** to each app based on security posture and compliance  
- Admins can now **sanction** or **unsanction** apps and configure governance policies  

---

## 💡 What This Demonstrates

- Hands-on creation of a Cloud Discovery snapshot  
- Ingestion and parsing of W3C firewall log files  
- Shadow IT discovery capabilities in Microsoft Defender for Cloud Apps  
- Cloud app risk management and governance fundamentals  

---

## 📂 Next Steps

- Integrate **Microsoft Defender for Endpoint** for continuous cloud app discovery  
- Configure **App Governance policies** and OAuth app controls  
- Explore automated alerting on risky SaaS usage  

---

## 👨‍💻 Author  
Cleveland Oliver
