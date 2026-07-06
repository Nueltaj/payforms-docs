---
title: Settings
nav_order: 9
parent: Admin Guide
---

# Section 9: Settings

The **Settings** section allows you to configure your institution's account preferences. To access it, click **Settings** in the left navigation sidebar. All subsections are accessible from the left panel within the Settings page.

---

## 9.1 General

The **General Settings** page manages your institution's core account information. Complete the following fields and click **Save Changes** to update:

- **Organization Name** — The name of your institution as it will appear across the platform
- **Contact Email** — The primary email address for your institution's account
- **Subdomain** — A unique identifier that forms your institution's portal URL (e.g. school.www.payforms.com.ng)
- **Custom Domain** — If your institution has its own domain, enter it here (e.g. pay.myuni.com). Point your domain's CNAME record to **payforms.app** to activate it.

---

## 9.2 Integrations

The **Integrations & Keys Settings** page is where you connect your Paystack account to enable online payment processing. Enter the following details and click **Save Keys**:

- **Public Key** — Your Paystack public API key, found in your Paystack Dashboard under **Settings → API Keys**
- **Secret Key** — Your Paystack secret API key. Keep this key secure and never expose it in client-side code.

Under **Webhook URL**, copy the provided Payforms webhook URL and add it to your Paystack dashboard under **Settings → Webhooks**. This enables Paystack to send payment notifications to Payforms in real time. You may also enter a custom webhook URL if required.

Click **Test Connection** to verify that your API keys are working correctly before going live. Click **Save Keys** to save.

---

## 9.3 Appearance

The **Appearance Settings** page allows you to upload your institution's logo, which will appear on payment receipts and email notifications sent to payers.

To upload a logo, drag and drop your image file into the upload area or click **Browse Files**. Accepted formats are PNG, JPG, and SVG, with a maximum file size of 2MB. The recommended dimensions are 200×200px.

The **Logo Preview** section shows how the logo will appear on receipts and email headers before you save.

Alternatively, if your logo is hosted online, enter the image URL in the **Logo URL** field and click **Save**. Click **Save Logo** to apply your changes.

---

## 9.4 Team

The **Team Settings** page allows you to manage the staff members who have access to your institution's Payforms account. Each member is listed with their **Name**, **Role**, and **Status**.

To add a new team member, click **Invite Member**. The **Invite Team Member** screen will appear with the following fields:

- **First Name** and **Last Name**
- **Email Address** — The address the invitation will be sent to

Click **Send Invite** to dispatch the invitation, or **Cancel** to discard.

---

## 9.5 Security

The **Security Settings** page allows you to manage account access and authentication for your Payforms account.

- **Two-Factor Authentication (2FA)** — Enable this toggle to add an extra layer of security to your account. When enabled, a verification step will be required each time you log in.
- **Change Password** — Click **Change** to update your account password.
- **Sessions** — Your current active session is displayed here. Click **Sign out all other sessions** to remotely terminate any other active sessions on your account.

---

## 9.6 Notifications

The **Notifications Settings** page controls which events trigger email alerts to your administrative account.

Under **Payment Notifications**, toggle each option on or off as needed:

- **Submission Confirmations** — Receive a notification when a payment form is submitted
- **Payment Confirmations** — Receive a notification when a payment is completed successfully
- **Payment Failures** — Receive a notification when a payment attempt fails

Under **Contact Login**:

- **Require Contact Login** — When enabled, contacts must log in before they can access payment forms

Click **Save Preferences** to apply your changes.

---

## 9.7 Payments

The **Payments Settings** page controls how payments are collected across your institution's forms.

Under **Partial Payments**:

- **Partial Payment Limit (%)** — Set the maximum percentage of the total amount that can be paid as a partial payment. The accepted range is 0 to 100. The default value is 100.

Under **Payment Methods**, select the methods your contacts can use at checkout: **Pay Online**, **Cash**, **Bank Transfer**, **POS**, and **Cheque**.

> **Note:** Offline payment methods — Cash, Bank Transfer, POS, and Cheque — create pending payment records that require admin confirmation before they are marked as completed.

Click **Save Preferences** to apply your changes.

---

## 9.8 Billing

The **Billing Settings** page displays your institution's current subscription plan and usage metrics.

Under **Current Plan**, your active plan and renewal date are shown. Two options are available:

- **Manage Subscription** — Upgrade, downgrade, or cancel your plan
- **View Invoices** — Access your billing history and download past invoices

Under **Usage**, a progress bar shows how much of your plan's allocation has been consumed:

- **Contacts** — The number of contacts added against your plan's limit
- **Forms** — The number of forms created against your plan's limit
- **Transactions** — The number of transactions processed against your plan's limit