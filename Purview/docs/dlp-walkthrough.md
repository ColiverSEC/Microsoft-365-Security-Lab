
# Data Loss Prevention (DLP) Policy Walkthrough

This walkthrough documents the process of creating, configuring, testing, and verifying a Microsoft Purview DLP policy to protect sensitive data such as PHI and PII.

---

## 1. Creating a DLP Policy

1. Sign in to the [Microsoft Purview Compliance Portal](https://purview.microsoft.com/).
2. Navigate to **Data loss prevention** > **Policies**.
3. Click **Create policy**.
4. Choose **Custom policy** or use a **template** that fits your use case (e.g., HIPAA or Financial).
5. Name your policy (e.g., "PHI and PII Protection") and add a description.
6. Select the locations to apply the policy (e.g., Exchange email, SharePoint, OneDrive).
7. Proceed to configure rules in the next step.

---

## 2. DLP Rule Configuration

1. Add a rule within the policy.
2. Define conditions to detect sensitive info types such as:
   - Protected Health Information (PHI)
   - Personally Identifiable Information (PII)
3. Set actions to take when content matches the rule, for example:
   - Block email from sending
   - Notify users with a policy tip
   - Generate incident reports and alerts
4. Customize exceptions if needed (e.g., allow emails from specific users).
5. Review and save the rule.

---

## 3. Sending a Test Email

1. From a mailbox in your tenant, compose an email containing sensitive information that matches your DLP policy rules (e.g., a sample Social Security Number or medical info).
2. Send the email to a recipient within your organization or external as your policy allows.
3. If your policy is set to block or warn, verify the behavior accordingly.

---

## 4. Reviewing Alerts in Purview and Defender

1. Return to the **Microsoft Purview Compliance Portal**.
2. Navigate to **Alerts** or **Incidents** under the DLP section.
3. Find alerts triggered by your test email.
4. Review details such as user, time, content detected, and policy actions.
5. For Defender for Cloud Apps integration:
   - Open the Defender portal.
   - Navigate to **Alerts** and verify related incidents from the DLP policy.
6. Use these alerts to monitor and investigate data loss events.

---

## 5. Verifying Audit Logs

1. In Microsoft Purview, go to **Audit** or use the **Microsoft 365 Security & Compliance Center**.
2. Search for audit events related to DLP policy triggers.
3. Filter by date, user, or event type as needed.
4. Confirm that the test email's policy match and enforcement actions are logged.
5. Use audit logs for compliance reporting and forensic analysis.

---

## Additional Notes

- You can enhance your DLP policies by integrating sensitivity labels for automatic classification.
- Automate alert handling via Power Automate or third-party tools.
- Regularly review and update DLP policies to keep pace with organizational and regulatory changes.

---

## Screenshots Reference

Refer to the `/screenshots` folder for visuals corresponding to each step.

---

## 🔧 Troubleshooting & Lessons Learned

During the lab, I encountered a few common configuration gaps:

- **Audit Logging Disabled by Default:**  
   I initially couldn’t find DLP events in the audit logs. I resolved this by enabling auditing in the Microsoft Purview Compliance portal under Audit settings.

- **Defender Alerts Not Appearing:**  
   I noticed my DLP alerts didn’t show in Microsoft Defender for Cloud Apps. I resolved this by configuring an alert policy in Defender and verifying that alert forwarding from Purview was enabled.

These troubleshooting steps helped reinforce the importance of validating your security stack end-to-end, not just at the policy level.


*Author: Cleveland Oliver*  
*Date: July 2025*
