# 👤 Microsoft Purview Data Loss Prevention (DLP) Walkthrough

[⬅️ Back to Microsoft 365 Security & Compliance Lab Overview](./README.md)

This walkthrough demonstrates how to configure and test **Microsoft Purview DLP** policies to protect sensitive information such as PHI and PII. It includes creating **Sensitivity Labels**, deploying a **DLP Policy**, configuring **rules**, testing with emails, and reviewing alerts and audit logs.

---

## 📚 What This Lab Covers

- Creating and publishing **Sensitivity Labels**  
- Creating a **DLP Policy** with custom rules  
- Sending a **test email** to validate policy enforcement  
- Reviewing **alerts in Purview and Defender for Cloud Apps**  
- Verifying **audit logs**  

---

## 🧑‍💻 Step 1: Creating Sensitivity Labels

### 📌 Steps

1. Sign in to the [Microsoft Purview Compliance Portal](https://purview.microsoft.com/)  
2. Navigate to **Information Protection → Labels**  
3. Create a **parent label** called `"Confidential"` (or your preferred name)  
4. Add **sublabels**:  
   - `PHI – Protected Health Information`  
   - `PII – Personally Identifiable Information`  
5. Configure label scope: **Exchange, SharePoint, OneDrive**  
6. (Optional) Configure **encryption, content marking, auto-labeling**  
7. Publish the labels using a **Label Policy** assigned to users/groups

### 📸 Screenshots

- **Sensitivity Labels List**  
  ![Sensitivity Labels List](../Screenshots/02-dlp-sensitivity-labels.png)

- **Create Label – Basics**  
  ![Create Label Basics](../Screenshots/19-new-sensitivity-label.png)

- **Label Scope**  
  ![Label Scope](../Screenshots/20-label-scope.png)

- **Encryption & Marking**  
  ![Encryption Settings](../Screenshots/21-encryption-and-watermark.png)

- **Publish Label Policy**  
  ![Publish Label Policy](../Screenshots/22-publish-label.png)

---

## ⚙️ Step 2: Creating a DLP Policy

### 📌 Steps

1. Navigate to **Data Loss Prevention → Policies → Create policy**  
2. Choose **Custom Policy** or a **template** (e.g., HIPAA, Financial)  
3. Name your policy (`PHI and PII Protection`) and add a description  
4. Select locations (**Exchange, SharePoint, OneDrive**)  
5. Configure rules (see next step)  
6. Review & finish

### 📸 Screenshots

- **Choose Template**  
  ![Choose Template](../Screenshots/04-dlp-policy-config-choose-a-template.png)

- **Choose Locations**  
  ![Choose Locations](../Screenshots/05-dlp-policy-config-choose-locations.png)

- **Conditions**  
  ![Conditions](../Screenshots/06-dlp-policy-config-conditions.png)

- **Actions & Alerts**  
  ![Actions & Alerts](../Screenshots/07-dlp-policy-actions-and-alert-config.png)

- **Define Policy Settings**  
  ![Define Policy Settings](../Screenshots/08-dlp-define-policy-settings.png)

- **Policy Mode**  
  ![Policy Mode](../Screenshots/09-dlp-policy-mode.png)

- **Review & Finish**  
  ![Review & Finish](../Screenshots/10-dlp-policy-review-and-finish.png)

- **Creation Success**  
  ![Creation Success](../Screenshots/11-dlp-policy-creation-success.png)

---

## 🛠️ Step 3: Configuring DLP Rules

### 📌 Steps

- Add a **rule** to the DLP policy  
- Define **conditions** to detect sensitive information:  
  - PHI  
  - PII  
- Configure **actions**:  
  - Block email sending  
  - Notify users with a **policy tip**  
  - Generate **incident reports/alerts**  
- Add **exceptions** if needed (e.g., trusted senders)  
- Review & save the rule

> 📸 **Note:** Screenshots for rules are included above under policy creation where conditions and actions are configured.

---

## 📧 Step 4: Sending a Test Email

### 📌 Steps

1. Compose an email containing sensitive information (e.g., SSN or medical info)  
2. Send to a recipient within your organization or external (depending on policy)  
3. Confirm **policy enforcement** (block, warn, or report)

### 📸 Screenshots

- **Test Email Triggered**  
  ![Test Email](../Screenshots/12-dlp-and-label-trigger-email.png)

- **DLP Block Message**  
  ![DLP Block Message](../Screenshots/13-dlp-block-message.png)

- **DLP Block Message Email**  
  ![DLP Block Message Email](../Screenshots/14-dlp-message-blocked-alert.png)

---

## 📊 Step 5: Reviewing Alerts

### 📌 Steps

- Go to **Purview → Alerts / Incidents** and find triggered events  
- Check details: user, time, content detected, policy action  
- For **Defender for Cloud Apps integration**:  
  - Navigate to **Defender portal → Alerts**  
  - Confirm related incidents from DLP policy  
- Use alerts to monitor and investigate data loss

### 📸 Screenshots

- **DLP Alert in Purview**  
  ![DLP Alert in Purview](../Screenshots/16-dlp-alert-purview.png)

- **Admin Email Notification**  
  ![Admin Email Notification](../Screenshots/15-dlp-admin-email-alert.png)

- **DLP Alert in Defender**  
  ![DLP Alert in Defender](../Screenshots/17-dlp-alert-defender-portal.png)

---

## 📝 Step 6: Verifying Audit Logs

### 📌 Steps

- Navigate to **Purview → Audit** or **Microsoft 365 Security & Compliance Center → Audit**  
- Search/filter for DLP events by **user, date, or event type**  
- Confirm that test email actions are logged  
- Use logs for compliance reporting and forensic analysis

### 📸 Screenshot

- **Audit Log Entry**  
  ![Audit Log Entry](../Screenshots/18-dlp-audit-search.png)

---

## 💡 Additional Notes & Troubleshooting

- **Audit Logging Disabled by Default** → Enable auditing in Purview to see DLP events  
- **Defender Alerts Not Appearing** → Verify alert policy forwarding from Purview  
- Automate alert handling via **Power Automate** or third-party tools  
- Regularly review and update policies for compliance and evolving needs

---

## ✅ Key Takeaways

- Sensitivity labels allow **consistent classification** and protection  
- DLP policies detect/block sensitive data in transit  
- Alerts integrate with **Purview & Defender for Cloud Apps**  
- Audit logs provide **traceability of policy actions**


