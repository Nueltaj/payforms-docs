---
title: Troubleshooting and FAQs
nav_order: 10
parent: Admin Guide
---

# Section 10: Troubleshooting and FAQs

---

## I did not receive a verification email after registering.

Check your spam or junk folder. The verification email is sent from **noreply@payforms.com.ng** via a third-party mail service and may be filtered by some email providers. If the email is not in your spam folder, return to the verification screen and click **Resend Email**.

---

## I cannot log in to my account.

Ensure you are entering the email address and password used during registration. If you have forgotten your password, click **Forgot Password?** on the login page to initiate a reset. If the issue persists, contact support.

---

## My payment form is not accepting submissions.

Confirm that the form status is set to **Active**. Draft forms are not publicly accessible. Also verify that the required **Email** and **Full Name** fields have been added under the form's **Fields** section.

---

## A transaction is showing as Pending but the student says they have paid.

Open the transaction record from the **Payments** section and click **View History** to review the full status log. If the payment was made offline, confirm it manually via the **Offline Payments** section. If the payment was made online, allow a few minutes for the Paystack webhook to update the record, then click **Refresh**.

---

## My Paystack integration is not working.

Go to **Settings → Integrations** and verify that your **Public Key** and **Secret Key** are entered correctly. Click **Test Connection** to confirm the keys are valid. Ensure the Payforms webhook URL has been added to your Paystack dashboard under **Settings → Webhooks**.

---

## The widget is not loading on my institution's website.

Confirm that the embed code has been pasted correctly into your website's HTML. If you are using the v1 embed method, ensure the **Parent Origin** field in the widget configuration matches your website's domain exactly. If the issue persists, try switching to the **Iframe Embed** method.

---

## How do I add staff members to my Payforms account?

Go to **Settings → Team** and click **Invite Member**. Enter the staff member's name and email address, then click **Send Invite**.

---

## How do I export my transaction records?

Go to the **Payments** section and click **Export CSV** to download all transaction records. You can also export filtered results by applying date or status filters before exporting.

---

## How do I change my institution's subdomain or custom domain?

Go to **Settings → General** and update the **Subdomain** or **Custom Domain** field. For a custom domain, ensure your domain's CNAME record points to **payforms.app** before saving.

---

## How do I cancel or change my subscription plan?

Go to **Settings → Billing** and click **Manage Subscription** to upgrade, downgrade, or cancel your plan.