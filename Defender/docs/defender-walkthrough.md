# Walkthrough: Cloud Discovery Snapshot Report in Microsoft Defender for Cloud Apps

This walkthrough guides you through creating and analyzing a Cloud Discovery snapshot report using a sample firewall log in Microsoft Defender for Cloud Apps (MDCA).

---

## Step 1: Sign in and Access Cloud Discovery

- Navigate to [https://security.microsoft.com/](https://security.microsoft.com/).
- Sign in with your admin or lab account.
- In the left-hand menu, select **Cloud Discovery**.

![Cloud Discovery Dashboard](../screenshots/01-cloud-discovery-dashboard.png)  
*Cloud Discovery dashboard after login showing navigation menu.*

---

## Step 2: Create a Snapshot Report

- Click on **Snapshot reports** under Cloud Discovery.
- Click the **+ Create snapshot report** button.
- Enter a descriptive name (e.g., “Sample Lab W3C Log”).
- Under **Data source**, select **Generic W3C Log**.
- Click **Upload file**, then select the `sample-w3c.log` you created.
- Click **Create** to start processing.

![Create Snapshot Report](../screenshots/02-create-snapshot-report.png)  
*Creating a new snapshot report with Generic W3C Log data source.*

---

## Step 3: Monitor Processing

- The report status will show as **Processing**.
- Wait 1–3 minutes for the upload to complete.
- Refresh the page to see when the status changes to **Completed**.

![Snapshot Report Processing](../screenshots/03-snapshot-report-processing.png)  
*Snapshot report showing “Processing” status.*

![Snapshot Report Completed](../screenshots/04-snapshot-report-completed.png)  
*Snapshot report marked as “Completed” after successful processing.*

---

## Step 4: Review Discovered Apps

- Navigate to **Cloud Discovery > Discovered apps**.
- You will see a list of apps extracted from the sample log (e.g., Dropbox, Slack, Google Drive).
- Click any app to view details including:
  - App category and description
  - Usage statistics
  - Security risk score

![Discovered Apps List](../screenshots/05-discovered-apps-list.png)  
*List of discovered cloud applications from the snapshot report.*

![App Risk Details](../screenshots/06-app-risk-details.png)  
*Risk score and details for a selected cloud application.*

---

## Step 5: Interpret and Act

- Use the risk scores to prioritize apps for review.
- Decide which apps to **Sanction** or **Unsanction** based on company policy.
- Create governance policies to monitor or restrict risky apps.

---

## Summary

This walkthrough provides hands-on experience ingesting firewall log data into MDCA to discover Shadow IT usage and assess cloud app risk. It forms the foundation for SaaS governance and security operations in a Microsoft 365 environment.

---

## 👨‍💻 Author  
Cleveland Oliver

---

