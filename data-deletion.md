---
layout: default
title: Data Deletion Instructions — PasteReady
---

# Data Deletion Instructions

**Last Updated:** April 15, 2026

You have full control over your data in PasteReady. This page explains how to delete your documents, your account, and all associated data.

---

## Delete Individual Documents

You can delete any document directly in the App:

1. Open the document you want to delete.
2. Tap the delete option.
3. Confirm the deletion.

This removes:
- The document record and all extracted fields from our cloud database
- The document images from your device's local storage
- Any scheduled alerts and notifications for that document
- All associated activity history

---

## Delete Your Account and All Data

To permanently delete your account and all associated data:

**Option 1: In the App**
1. Go to **Settings** in the App.
2. Tap **Delete Account**.
3. Confirm the deletion.

**Option 2: By Email**
If you cannot access the App, send an email to [vikivikovik@gmail.com](mailto:vikivikovik@gmail.com) with the subject line **"Account Deletion Request"** from the email address associated with your account.

---

## What Gets Deleted

When you delete your account, the following data is permanently removed:

### From Our Servers
- Your user account (via Clerk authentication)
- All document records (extracted fields, metadata, summaries, tags, notes)
- All rate-limiting records associated with your account
- Any other data linked to your user ID

### From Your Device
- You should uninstall the App to remove all locally stored data, including:
  - Document images stored in the encrypted scans directory
  - Local SQLite database (document records, fields, alerts, activity history)
  - App settings and preferences
  - Cached data

**Note:** Uninstalling the App automatically removes all on-device data. If you delete your account but keep the App installed, local data remains on your device until you uninstall.

---

## What Is NOT Stored (and Therefore Not Deleted)

- **Document images on our servers** — we never store your document images on our servers. Images sent for AI processing are used in memory only and immediately discarded.
- **AI training data** — your documents are never used to train AI models. Google Vertex AI operates under a zero-retention policy for your images.

---

## Timeline

- **Cloud data deletion:** Within 30 days of your request. In most cases, data is deleted immediately.
- **Local data deletion:** Immediate upon uninstalling the App.
- **Email requests:** We will process your request and confirm deletion within 30 days.

---

## Questions?

If you have any questions about data deletion or need assistance, contact us:

**Email:** [vikivikovik@gmail.com](mailto:vikivikovik@gmail.com)

---

[Back to Legal Home](./)
