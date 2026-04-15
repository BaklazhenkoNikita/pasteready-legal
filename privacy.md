---
layout: default
title: Privacy Policy — PasteReady
---

# Privacy Policy

**Effective Date:** April 15, 2026
**Last Updated:** April 15, 2026

PasteReady ("we", "us", "our") is operated by Nikita Baklazhenko. This Privacy Policy explains how we collect, use, store, and protect your information when you use the PasteReady mobile application ("the App").

PasteReady is an AI-powered personal document scanner and information wallet designed to help you extract, organize, and access data from your personal documents.

---

## 1. Information We Collect

### 1.1 Account Information
When you create an account, we collect:
- Email address
- Authentication credentials (managed by our authentication provider, Clerk)

### 1.2 Document Data
When you scan documents, the App processes and stores:
- **Document images** — stored exclusively on your device in an encrypted directory. Images are never stored on our servers.
- **Extracted data fields** — structured information extracted from your documents, such as names, dates, identification numbers, addresses, phone numbers, email addresses, and financial details (e.g., IBANs, account numbers).
- **Document metadata** — document type, category, title, language, confidence scores, notes, tags, and timestamps.

### 1.3 Usage Data
- Activity events (e.g., when you scan, copy, or edit a document)
- Copy counts and access timestamps
- App settings and preferences

### 1.4 Information We Do Not Collect
- We do not use analytics, advertising, or tracking SDKs.
- We do not collect device identifiers for advertising purposes.
- We do not sell or share your data with data brokers.

---

## 2. How Your Data Is Processed

### 2.1 On-Device Processing (Data Never Leaves Your Phone)
The following document types are processed entirely on your device using on-device machine learning and never sent to any server:
- **Credit and debit cards** — card numbers are extracted using on-device OCR and validated locally.
- **Identity documents with machine-readable zones (MRZ)** — passports, national IDs, residence permits, and driver's licenses are parsed on-device.

Additionally, the following always remain on your device:
- All document images
- Biometric authentication data (Face ID / Touch ID)
- Full-text search indexes
- Alert and notification schedules
- Activity logs and copy counts

### 2.2 Cloud Processing (With Your Consent)
For document types that are not handled on-device (e.g., receipts, contracts, utility bills, insurance policies, bank statements, tax documents, health cards, travel bookings), images are sent to Google's Gemini AI via Vertex AI for data extraction. This occurs **only with your explicit consent**, which you can grant or revoke at any time in the App settings.

When cloud processing is used:
- Your document image is sent as a temporary API request.
- **Zero-retention is enforced** — Google does not store or use your images for model training. Images exist in memory only during processing and are freed immediately after.
- The extracted data (text fields, summaries, tags) is returned to the App and stored in our database.

### 2.3 Cloud Storage
Extracted document data (fields, metadata, summaries — **not images**) is stored in our database (MongoDB Atlas) associated with your user account. This allows your data to be restored if you switch devices.

---

## 3. Third-Party Services

We use the following third-party services that may process your data:

| Service | Purpose | Data Shared |
|---------|---------|-------------|
| **Google Vertex AI (Gemini)** | Document data extraction | Document images (temporary, zero-retention) |
| **Clerk** | User authentication | Email address, authentication tokens |
| **MongoDB Atlas** | Cloud data storage | Extracted document fields, metadata, user ID |
| **Apple (App Store / IAP)** | App distribution | Standard App Store data per Apple's privacy policy |

We do not use any analytics, crash reporting, or advertising services.

---

## 4. Data Storage and Security

### 4.1 On Your Device
- Document images are stored in an encrypted directory on your device.
- Sensitive settings are stored using the device Keychain (iOS Secure Store).
- App data is stored in a local SQLite database on your device.
- You can enable biometric authentication (Face ID / Touch ID) to protect access to the App. Biometric data is processed entirely by your device's operating system and is never accessible to us.

### 4.2 On Our Servers
- Our backend runs on Google Cloud Run in the **europe-west1** (Belgium) region.
- Data in transit is encrypted using TLS/HTTPS.
- Database access is authenticated and restricted to our backend service.
- We never store document images on our servers.

### 4.3 Sensitive Data Handling
The App classifies extracted data by sensitivity level:
- **Critical fields** (identification numbers, card numbers, MRZ data) — automatically cleared from clipboard after 30 seconds.
- **High-sensitivity fields** (dates of birth, full names on identity documents, IBANs) — automatically cleared from clipboard after 60 seconds.
- Notification content never includes sensitive field values — only document titles are shown.

---

## 5. Data Retention

- **On-device data** is retained until you delete it manually or uninstall the App.
- **Cloud-stored data** (extracted fields and metadata) is retained in our database until you delete individual documents or request full account deletion.
- **Rate-limiting records** are automatically deleted via time-to-live (TTL) indexes and do not contain document data.
- **Document images sent for AI extraction** are not retained — they are processed in memory and immediately discarded.

---

## 6. Your Rights (GDPR)

If you are located in the European Economic Area (EEA), you have the following rights under the General Data Protection Regulation (GDPR):

- **Right of Access** — request a copy of your personal data.
- **Right to Rectification** — correct inaccurate data (you can edit document fields directly in the App).
- **Right to Erasure** — request deletion of your data (see our [Data Deletion Instructions](./data-deletion)).
- **Right to Restrict Processing** — request that we limit how we use your data.
- **Right to Data Portability** — receive your data in a structured, machine-readable format.
- **Right to Object** — object to our processing of your data.
- **Right to Withdraw Consent** — you can revoke cloud AI processing consent at any time in App settings.

To exercise any of these rights, contact us at [vikivikovik@gmail.com](mailto:vikivikovik@gmail.com).

**Legal Basis for Processing:**
- **Consent** — for cloud AI document extraction (explicit opt-in).
- **Contract performance** — for providing the core App functionality and account management.
- **Legitimate interest** — for security, fraud prevention, and service improvement.

---

## 7. Children's Privacy

PasteReady is not intended for use by children under the age of 16. We do not knowingly collect personal data from children. If you believe a child has provided us with personal data, please contact us and we will delete it.

---

## 8. International Data Transfers

Your data is processed and stored in the European Union (Belgium, europe-west1). If you are located outside the EU, your data will be transferred to and processed in the EU, which provides a high level of data protection under the GDPR.

---

## 9. Changes to This Policy

We may update this Privacy Policy from time to time. We will notify you of material changes by updating the "Last Updated" date at the top of this page. We encourage you to review this page periodically.

---

## 10. Contact Us

If you have any questions about this Privacy Policy or our data practices, please contact us:

**Email:** [vikivikovik@gmail.com](mailto:vikivikovik@gmail.com)

---

*This Privacy Policy should be reviewed by a qualified legal professional before publication.*
