# GHL Contact List Cleaning Guide

## Sly Nerds Sub-Account — Email Deliverability Fix
### GoHighLevel (GHL)

---

## 📌 Why This Task Is Important

The email deliverability rate for the Sly Nerds GHL sub-account has been low, meaning many campaign emails are not reaching recipients’ inboxes. This is mainly due to bounced, invalid, and inactive contacts remaining in the contact list.

**Cleaning the contact database will help:**
* 📉 Reduce bounce rate
* 🚫 Prevent emails from going to spam folders
* 🛡️ Improve domain reputation
* 📈 Increase open rates for future campaigns

---

## 🚀 Before You Start

1. **Log in to GHL at:** [GoHighLevel](https://app.gohighlevel.com?utm_source=chatgpt.com)
2. From **Agency View**, select the **Sly Nerds** sub-account.
3. Go to **Contacts** from the left sidebar menu.

---

## 🛠️ Step-by-Step Instructions

### Step 1 — Remove Hard Bounce Contacts
*A hard bounce means the email address is invalid or no longer exists.*

1. Go to: **Contacts ➔ Smart Lists ➔ + New Smart List**
2. Add one of these filters:
   * `Email Bounced = Yes`
   * **OR** `Contact Status = Bounced`
3. Select all matching contacts.
4. Use **Bulk Actions** to:
   * Add tag: `Do Not Email`
   * **OR** permanently delete them *(only if confirmed)*.

> ⚠️ **Important:** Export and back up bounced contacts before deleting them.

---

### Step 2 — Separate Unsubscribed Contacts
*Contacts who unsubscribed are automatically suppressed by GHL, but they should still be properly tagged.*

1. Go to **Contacts**
2. Filter by: `Email Unsubscribed = Yes`
3. Select all contacts.
4. Add tag: `Unsubscribed`

> ⚠️ **Important:** Do not include these contacts in future campaigns.

---

### Step 3 — Identify Inactive Contacts
*Inactive contacts are users who have not opened emails for a long period.*

1. Filter contacts using:
   * `Last Email Opened = More than 180 days ago`
   * **AND** `Emails Sent ≥ 3`
2. **Do NOT delete** these contacts.
3. Add tag: `Cold List`

*Note: These contacts can later be used in a separate re-engagement campaign.*

---

### Step 4 — Validate Emails Using an External Tool
*Email validation must be done outside GHL using a verification platform.*

#### 🎯 Recommended Tools (Both offer free trials):
* [ZeroBounce](https://www.zerobounce.net?utm_source=chatgpt.com)
* [NeverBounce](https://www.neverbounce.com?utm_source=chatgpt.com)

#### 📝 Instructions:
1. Export contacts from GHL in **CSV format**.
2. Upload the CSV file to ZeroBounce or NeverBounce.
3. Wait for validation to complete.
4. Download the cleaned results.
5. **Remove these contact types:**
   * Invalid
   * Spam Trap
   * Disposable Emails
   * Catch-All *(optional — keep separately if needed)*
6. Re-import the cleaned list into GHL.

---

### Step 5 — Remove Spam Complaint Contacts
*These are contacts who marked previous emails as spam.*

1. Go to **Contacts**
2. Filter by: `Complaint = Yes`
3. Select all matching contacts.
4. Add tag: `Do Not Email`

> ⚠️ **Important:** Never include these contacts in future campaigns.

---

### Step 6 — Create a Clean Audience
From now on, campaigns should only target contacts who meet these conditions:

* ✅ Valid email address
* ✅ Not bounced
* ✅ Not unsubscribed
* ✅ No spam complaints
* ✅ Recently active *(opened at least one email)*

📌 **Smart List Name:** Create and save a Smart List called: **`Active Clean Contacts`**

---

## 📋 Final Checklist

- [ ] Hard bounce contacts removed or tagged
- [ ] Unsubscribed contacts tagged
- [ ] Inactive contacts tagged as “Cold List”
- [ ] Invalid emails removed using ZeroBounce/NeverBounce
- [ ] Spam complaint contacts tagged as “Do Not Email”
- [ ] Clean audience saved as “Active Clean Contacts”
- [ ] Future campaigns will use only the clean list
