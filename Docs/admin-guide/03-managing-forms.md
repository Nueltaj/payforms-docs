---
title: Managing Forms
nav_order: 3
parent: Admin Guide
---

# Section 3: Managing Forms

The **Forms** section allows you to create, organise, and manage all payment forms for your institution. To access it, click **Forms** in the left navigation sidebar.

The Forms page displays three tabs:

- **All** — Lists every form created under your account
- **Active** — Lists forms that are currently live and accepting payments
- **Draft** — Lists forms that have been created but not yet published

---

## 3.1 Creating a New Form

**Step 1:** Click **+ Create New Form** at the top of the Forms page, or click **+ Create Form** at the bottom of the left navigation sidebar.

**Step 2:** On the **Create New Form** page, complete the following fields:

- **Form Title** — The name of your payment form (e.g. Q1 Invoice, Tuition Fee)
- **Slug** — A URL-friendly identifier used in the form's payment link (e.g. q1-invoice). This will appear as **/pay/your-slug** in the form URL.
- **Category** — The category this form belongs to (e.g. Invoice, Fee, Donation)
- **Description** — A brief description of what this form is for, visible to payers
- **Internal Note** — Private notes for administrative use, not visible to payers

**Step 3:** Under **Payment Settings**, configure the following:

- **Payment Type** — Select either **Fixed Amount** (a set payment value) or **Variable Amount** (the payer enters the amount)
- **Amount** — Enter the amount to be collected, if applicable
- **Allow Partial Payments** — Enable this option to allow payers to pay less than the full amount due

**Step 4:** Click **Create Form** to save the form. It will appear as a card on the Forms page.

---

## 3.2 Managing an Existing Form

Each form is displayed as a card showing the form name, category, and current status. The following actions are available on each card:

- **Preview** — Opens a preview of the form as payers will see it. No data is submitted in preview mode.
- **Fields** — Opens the field management page where you configure the information the form collects from payers
- **Settings** — Opens the form's basic details for editing, including payment type and amount
- **Live** — Opens the live payment URL for the form
- **Copy** — Copies the form's payment link to your clipboard

To **deactivate**, **duplicate**, or **delete** a form, click the three-dot icon on the form card and select the desired option from the menu.

---

## 3.3 Managing Form Fields

Click **Fields** on a form card to open the field management page. This is where you configure the information your form will collect from payers.

> **Important:** For payment processing to function correctly, every form must include an **Email** field (type: EMAIL) and a **Full Name** field (type: TEXT, with a label containing the word "name").

The following action buttons are available at the top of the Fields page:

- **Assign to Groups** — Assign the form to a specific student group or cohort
- **Settings** — Edit the form's basic details, payment type, and amount
- **Widget** — Generate an embeddable version of the form for use on external websites
- **Delete Form** — Permanently remove the form from the platform

### Adding a Field

**Step 1:** Click **+ Add Field**, or click **+ Add Your First Field** if no fields have been added yet.

**Step 2:** Enter a **Field Label** (e.g. Full Name, Email Address).

**Step 3:** Select a **Field Type** from the dropdown. Available types are: **Short Text**, **Email**, **Number**, **Dropdown**, and **Long Text**.

**Step 4:** Check **Required field** if this field must be completed before the form can be submitted.

**Step 5:** Click **+ Add Field** to save. Repeat these steps to add additional fields.

> **Note:** For **Dropdown** fields, enter the available options in the **Options** field, separated by semicolons.

### Editing a Field

**Step 1:** Hover over the field you want to edit. A pencil icon and a red trash icon will appear.

**Step 2:** Click the pencil icon. The **Edit Field** panel will appear.

**Step 3:** Make the required changes, then click **Save Changes**. Click **Cancel** to discard.

### Deleting a Field

**Step 1:** Hover over the field you want to delete and click the red trash icon.

**Step 2:** A confirmation prompt will appear.

**Step 3:** Click **OK** to confirm, or **Cancel** to abort.

### Reordering Fields

To change the display order of fields, click the upward or downward arrow next to the field you want to move.

---

## 3.4 Widget Configuration

The **Widget** feature allows you to embed a payment form directly into an external website. To access it, open a form and click **Widget** from the action buttons at the top of the Fields page.

### Step 1: Verify Form Selection

The **Form Selection** panel confirms which form the widget is being generated for. The **Form Slug** and **Payment URL** are displayed here for reference and cannot be edited from this screen.

### Step 2: Select a Widget Version

- **v1 (Recommended)** — A secure embed method that uses postMessage and supports multiple widget instances on the same page
- **Legacy** — An older embed method retained for backward compatibility. Use this only if your website cannot support v1.

### Step 3: Configure Appearance

- **Theme** — Select **Light** or **Dark** to match your site's colour scheme
- **Primary Color** — Enter a hex colour code to match your institution's branding (default: #188ace)
- **Button Text** — Set the label on the payment button (default: Pay Now)

### Step 4: Set Dimensions

- **Width** — Set as a percentage (default: 100%) to make the widget responsive to its container
- **Min Height (px)** — Set the minimum height in pixels (default: 400)

### Step 5: Configure Behavior

- **Callback URL** — Enter a URL to redirect payers after a successful payment. This field is optional.
- **Auto-redirect after payment** — Enable this option to automatically send payers to the callback URL upon payment completion.

### Step 6: Advanced Settings (v1 Only)

- **Container ID** — The CSS selector for the HTML element that will host the widget (default: #payforms-widget-root)
- **Instance ID** — A unique identifier for the widget, required if multiple widgets appear on the same page
- **Parent Origin** — Your website's domain. Required if EMBED_ALLOWED_ORIGINS is configured on your server.
- **API Base URL** — A custom API endpoint for self-hosted Payforms instances. Leave blank to use the default.

### Step 7: Copy the Embed Code

Once configuration is complete, copy the generated code from the right panel and paste it into your website's HTML. Two embed formats are available:

- **Script Embed** — The recommended method
- **Iframe Embed** — An alternative for platforms that do not support script tags

> **Note:** If you need to handle payment events programmatically, add the provided `window.addEventListener` code to your page. Available events: `ready`, `submitted`, `payment_initialized`, `error`, and `resize`. This option is available for v1 only.

### Legacy Widget

To use the Legacy embed method, select **Legacy** under **Widget Version**. The **Advanced Settings** panel is not available for Legacy. Unless your website has a specific compatibility requirement, use **v1 (Recommended)**. 
