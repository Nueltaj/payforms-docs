---
title: Contacts
nav_order: 5
parent: Admin Guide
---

# Section 5: Contacts

The **Contacts** section allows you to manage your institution's payer records, organise contacts into groups, and track financial balances at an individual level. To access it, click **Contacts** in the left navigation sidebar.

Three action buttons are available in the top-right corner of the page:

- **Import Contacts** — Upload a list of contacts in bulk from an external file
- **Send Reminder** — Send a payment reminder to one or more selected contacts
- **+ New Contact** — Add a single contact record manually

## Groups

The left panel displays your contact groups. By default, all contacts are listed under **All Contacts**. Click **Manage Groups** to create, rename, or delete groups. Groups allow you to organise contacts by class, department, cohort, or any other category relevant to your institution.

## Financial Status

Below the Groups panel, the **Financial Status** summary displays the aggregate payment position across all contacts:

- **Total Paid** — The cumulative amount successfully collected from all contacts
- **Outstanding** — The cumulative amount still owed across all contacts

## Contact List

The right panel displays all contacts within the selected group. You can search for a specific contact using the **Search** bar, apply filters using the **Filter** option, or download your contact list using **Export**.

To perform bulk actions, check the boxes next to the relevant contacts. The **Selected** counter at the top of the list will update to reflect the number of contacts currently selected.

---

## 5.1 Importing Contacts

To add multiple contacts at once, click **Import Contacts** in the top-right corner of the Contacts page. The **Bulk Import Contacts** screen will open, guiding you through a three-step process.

### Step 1: Upload CSV

Upload your contact file by dragging and dropping it into the upload area, or click **Browse Files** to locate it manually. Accepted formats are CSV and XLSX, with a maximum file size of 50MB.

Before uploading, ensure your file meets the following requirements:

- The first row must contain unique column headers
- Email addresses must be in a valid format
- Dates must follow the YYYY-MM-DD format
- Tags must be comma-separated

If you do not have a file ready, click **Download Template** to obtain a pre-formatted CSV file that is compatible with the platform.

### Step 2: Map Fields

Once your file is uploaded, the platform displays a field mapping table showing each column from your CSV alongside a sample value. Review the **Maps To** column to confirm that each CSV column is matched to the correct Payforms field.

To change a mapping, click the dropdown next to the relevant row and select the appropriate field. Available options are: **Email**, **First Name**, **Last Name**, **Phone**, **Gender**, and **Student ID**. Select **Skip** for any column you do not want to import.

### Step 3: Review & Import

Review the mapped fields and confirm to complete the import.

---

## 5.2 Contact List Columns

Once contacts have been added, they appear in the contact list with the following columns:

- **Name** — The contact's full name and email address
- **Group** — The group the contact belongs to, if assigned
- **Total Paid** — The cumulative amount paid by this contact across all payment forms
- **Balance** — Any outstanding amount owed by this contact
- **Actions** — Options to edit or delete the contact record

---

## 5.3 Editing a Contact

To update a contact's details, click the edit icon in the **Actions** column of the relevant record. The **Edit Contact** screen will open with the following fields:

- **First Name**, **Middle Name**, **Last Name**
- **Email** and **Phone**
- **Student ID** and **External ID**
- **Gender** — Select **Male**, **Female**, or **Other**
- **Status** — Select **Active** or **Inactive**

Under **Guardian Information**, you may also enter the contact's guardian name, phone number, and email address where applicable.

Click **Save Changes** to update the record, or **Cancel** to discard changes and return to the Contacts page.

To permanently remove a contact, click the red delete icon in the **Actions** column of the relevant record.

---

## 5.4 Sending a Payment Reminder

To send a payment reminder to one or more contacts, click **Send Reminder** in the top-right corner of the Contacts page. The **Send Payment Reminder** screen will open.

**Step 1:** In the **Select Contacts** panel, check the boxes next to the contacts you want to notify. The **Reminder Summary** panel will update to reflect the number of selected recipients.

**Step 2:** Optionally, enter a **Custom Message** to include additional context in the reminder.

**Step 3:** Optionally, attach a file of up to 10MB using the **Attachment** field.

**Step 4:** Click **Send Reminders** to dispatch the notification to all selected contacts.

A confirmation screen will appear once the reminders have been sent, showing the number of contacts reached. Click **Done** to return to the Contacts page.

---

## 5.5 Bulk Actions

To perform an action on multiple contacts at once, check the box next to each contact's name. When one or more contacts are selected, a toolbar will appear at the top of the contact list with the following options:

- **Move to Group** — Assign the selected contacts to an existing group
- **Send Mail** — Send an email to the selected contacts
- **Delete** — Permanently remove the selected contacts from the platform

---

## 5.6 Managing Groups

### Creating a Group

To create a new contact group, click the **+** button in the **Groups** panel on the left side of the Contacts page. The **Create Group** screen will open with the following fields:

- **Group Name** — Enter a name for the group (e.g. BATU)
- **Description** — Enter a brief description of the group

Click **Create Group** to save, or **Cancel** to discard.

### Viewing and Editing a Group

To manage an existing group, click **Manage Groups** from the Contacts page. The **Groups** page will open, displaying all created groups alongside a **Quick Stats** panel showing the total number of groups and contacts.

To edit a group, hover over the group name and click the pencil icon. The **Edit Group** screen will open. From here you can:

- Update the group name or description
- Click **Manage Members** to add or remove contacts from the group
- Click **Delete Group** to permanently remove the group from the platform

Click **Save Changes** to apply any updates, or **Cancel** to discard.

### Adding Members to a Group

After clicking **Manage Members**, a contact list will appear showing all contacts currently saved on the platform. Check the box next to each contact you want to add to the group, then click **Add** in the top-right corner to confirm.

---

## 5.7 Adding a New Contact

To add a single contact manually, click **+ New Contact** in the top-right corner of the Contacts page. The **Add New Contact** screen will open with three sections.

### Student Information

- **Student Identification Number or User ID** (e.g. STU-2024-001)
- **First Name**, **Middle Name**, **Last Name**
- **Email Address**
- **Phone Number**
- **Gender** — Select **Male**, **Female**, or **Other**

### Guardian Information

- **Guardian Full Name**
- **Guardian Email**
- **Guardian Phone**

### Login Settings

- **Require Portal Login** — When enabled, the contact will receive a password setup email and can log in to the student portal
- **Force Password Reset on First Login** — When enabled, the contact must change their password immediately after their first login

If **Force Password Reset on First Login** is disabled, the contact will receive their login credentials via email after account creation. If it is enabled, the contact will receive a password setup email immediately after creation.

Click **Save Contact** to create the record, or **Cancel** to discard.

---

## 5.8 Viewing Group Details

To view the details of a group, click the group name from the **Groups** panel on the Contacts page. A panel will appear with the following options:

- **Edit Group** — Update the group name or description
- **Manage Contacts** — View and manage the members of the group
- **Add Subgroup** — Create a nested group within this group
- **Send Reminder** — Send a payment reminder to all contacts in the group

---

## 5.9 Managing Group Members

Clicking **Manage Contacts** opens the group's member list. From this screen you can:

- Search for a specific contact using the **Search contacts** bar
- Click **Add Contacts** in the top-right corner to add new members to the group
- Remove a member by checking the box next to their name, then clicking **Remove Selected** in the toolbar that appears

---

## 5.10 Viewing a Contact Profile

To view the full profile of a contact, click **View** next to their name in the group member list. The contact profile displays the following:

- **Email** and **Phone**
- **Student ID**
- **Groups** — The group or groups the contact belongs to
- **Added On** — The date the contact was added to the platform
- **Recent Transactions** — A summary of the contact's latest payment activity

Three action buttons are available at the bottom of the profile:

- **View All Payments** — Opens the contact's full transaction history, which can be exported as a CSV file
- **Edit Contact** — Opens the contact's details for editing
- **Delete** — Permanently removes the contact from the platform

---

## 5.11 Filtering Contacts

To narrow down the contact list, click **Filter** at the top of the contact list panel. A dropdown will appear with the following options:

- **Status** — Filter by **Active** or **Inactive** contacts
- **Balance** — Filter by **Has Balance** or **No Balance**
- **Group** — Filter by **All Groups** or a specific group you have created

Click **Apply** to update the list, or **Clear** to reset all filters.