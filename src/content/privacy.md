# Privacy Policy for Subscriptin

**Last Updated:** December 7, 2025  
**Effective Date:** December 7, 2025

---

## 1. Introduction

Subscriptin ("we," "our," or "us") is committed to protecting your privacy. This Privacy Policy explains how we collect, use, disclose, and safeguard your information when you use our mobile application (the "App").

**Contact Information:**
- Email: support@subscriptin.com
- Developer: Subscriptin (Individual Developer)
- Address: 13 Joshua Place, Oxenford QLD 4210, Australia

This Privacy Policy applies to users in all jurisdictions, including the European Economic Area (EEA), United Kingdom, California (United States), and Australia. We comply with the General Data Protection Regulation (GDPR), California Consumer Privacy Act (CCPA), and Australian Privacy Principles (APPs).

By using Subscriptin, you agree to the collection and use of information in accordance with this Privacy Policy.

---

## 2. Age Restrictions

Subscriptin is intended for users who are **13 years of age or older**. We do not knowingly collect personal information from children under 13.

**For EU/EEA Users:** If you are under 16 years old, you may need parental or guardian consent to use this App, depending on your country's laws.

If we discover that we have collected personal information from a child under the minimum age without parental consent, we will delete that information immediately. If you believe we have collected information from a minor, please contact us at support@subscriptin.com.

---

## 3. Information We Collect

### 3.1 Personal Information You Provide

When you create an account and use Subscriptin, we collect the following personal information:

#### Account Information
- **Email Address:** Required for account creation, authentication, and account recovery
- **Password:** Encrypted and managed by our authentication provider (Supabase Auth); we do not store your password directly
- **User ID:** A unique identifier (UUID) generated when you create your account

#### Subscription Data
You voluntarily provide information about your subscriptions, which may include:
- Subscription name
- Billing amount and currency
- Billing cycle (weekly, monthly, quarterly, yearly)
- Subscription category (system-defined or custom)
- Sign-up date
- Automatic payment status (yes/no)
- Active/inactive status
- Website URL and favicon (optional)
- Notes (optional, free-text field that may contain sensitive information)
- Cancellation reminder date (optional)
- Billing anchor date (optional)
- Your timezone (e.g., "Australia/Sydney")
- Pause/cancellation status and reason (optional)

#### Payment History
- Payment ID, amount, currency, billing date
- Payment status (completed, skipped, pending)
- Notes (optional)

#### Custom Categories
- Category name, emoji character, color

### 3.2 Information Automatically Collected

#### Device and Usage Information
- **Client ID:** A unique identifier for each device you use to access Subscriptin
- **Device Name:** Optional device identifier
- **Last Connection Timestamp:** When your device last synced with our servers
- **Sync Status:** Whether sync is enabled on your device

#### Technical Information
- **Internet Protocol (IP) Address:** Temporarily logged by our service providers (Supabase, Frankfurter API)
- **Network Connectivity Status:** Used to manage data synchronization
- **Firebase Messaging Token:** A unique token for sending push notifications to your device

#### Exchange Rate Data
- **Currency Conversion Cache:** Base currency, target currency, exchange rate, and fetch timestamp (stored locally)

### 3.3 Information We Do NOT Collect

We do **NOT** collect:
- Credit card or payment method details
- Device location (GPS coordinates)
- Browsing history outside the App
- Third-party analytics or advertising identifiers
- Biometric data
- Health information
- Government identifiers (e.g., Social Security numbers)

---

## 4. How We Use Your Information

We use the information we collect for the following purposes:

### 4.1 Core App Functionality
- **Account Management:** Create, authenticate, and manage your user account
- **Subscription Tracking:** Store and display your subscription information
- **Payment Tracking:** Automatically generate payment records based on billing cycles
- **Multi-Device Sync:** Synchronize your subscription data across all your devices in real-time
- **Currency Conversion:** Convert subscription amounts to your preferred currency using live exchange rates

### 4.2 Communication
- **Account Verification:** Send email verification messages during account creation
- **Password Recovery:** Send password reset emails via magic link authentication
- **Notifications:** Send push notifications about upcoming subscription renewals (if you enable notifications)

### 4.3 Service Improvement
- **Bug Fixes:** Diagnose and fix technical issues
- **Performance Optimization:** Monitor sync performance and connectivity
- **Feature Development:** Understand usage patterns to improve the App

### 4.4 Legal Compliance
- Comply with applicable laws and regulations
- Respond to legal requests and prevent fraud
- Enforce our Terms of Service

### 4.5 Legal Basis for Processing (GDPR)

Under the GDPR, we process your personal data based on the following legal bases:

#### Contract Performance (Article 6(1)(b))
Processing necessary to provide the subscription tracking service you signed up for:
- **Account Management:** Email address, user ID, and password for account creation and authentication
- **Core Service Delivery:** Subscription data, payment history, and billing information storage and tracking
- **Multi-Device Synchronization:** Real-time data sync across your devices
- **Currency Conversion:** Processing subscription amounts in your preferred currency
- **Timezone Processing:** Accurate billing date calculations based on your timezone

#### Consent (Article 6(1)(a))
Processing based on your explicit consent, which you can withdraw at any time:
- **Push Notifications:** Firebase messaging token for sending subscription renewal reminders (you can disable in device settings)
- **Optional Data Fields:** Notes and custom categories you voluntarily add to subscriptions

#### Legitimate Interests (Article 6(1)(f))
Processing necessary for our legitimate interests in providing a secure and reliable service:
- **Security and Authentication:** Session management, authentication tokens, and Row-Level Security enforcement
- **Fraud Prevention:** Monitoring for unauthorized access and suspicious activity
- **Service Improvement:** Bug fixes, performance optimization, and feature development
- **Data Protection:** Backup and disaster recovery, soft delete for sync conflict resolution

You have the right to object to processing based on legitimate interests. If you wish to exercise this right, please contact us at support@subscriptin.com.

---

## 5. How We Store and Protect Your Information

### 5.1 Data Storage

#### Local Storage (On Your Device)
- All subscription data is stored in a local SQLite database on your device
- This includes subscriptions, payments, categories, and sync metadata
- Local data is accessible only by the App and is protected by your device's security features

#### Remote Storage (Supabase)
- Your data is securely stored on Supabase's PostgreSQL database servers
- **Location:** Asia Pacific (Seoul, South Korea) - AWS region ap-northeast-2
- **Encryption in Transit:** All data transmitted between your device and Supabase is encrypted using HTTPS/TLS and WSS (WebSocket Secure)
- **Encryption at Rest:** Data stored in Supabase databases is encrypted at rest

### 5.2 Security Measures

We implement industry-standard security measures to protect your information:

#### Row-Level Security (RLS)
- Every database table has Row-Level Security policies enabled
- You can **only** access your own data; other users cannot view, modify, or delete your subscriptions
- Access control enforced via authenticated user ID matching

#### Authentication Security
- Passwords are hashed and encrypted by Supabase Auth (we never store plain-text passwords)
- Session tokens are automatically refreshed and securely stored
- Email verification prevents unauthorized account creation

#### Soft Delete Protection
- Deleted records are marked as "deleted" rather than permanently removed immediately
- This prevents accidental data loss and enables sync conflict resolution
- Soft-deleted data is excluded from all user-facing queries

### 5.3 Data Retention

#### Active Accounts
- We retain your data for as long as your account is active
- You can delete individual subscriptions, payments, or categories at any time

#### Deleted Accounts
- When you delete your account, your data is retained for **30 days**
- This allows for backup recovery and compliance with legal obligations
- After 30 days, all your personal data is permanently deleted from our servers
- Local data on your device remains until you uninstall the App

#### Backups
- Backup data containing your information may be retained for up to 30 days for disaster recovery purposes

---

## 6. How We Share Your Information

### 6.1 Third-Party Service Providers

We share your information with the following third-party service providers who help us operate the App:

#### Supabase (Backend Infrastructure)
- **Purpose:** Authentication, database storage, real-time data synchronization
- **Data Shared:** Email address, user ID, all subscription data, payment history
- **Location:** Asia Pacific (Seoul, South Korea) - AWS region ap-northeast-2
- **Privacy Policy:** https://supabase.com/privacy

#### Frankfurter API (Exchange Rates)
- **Purpose:** Retrieve live currency exchange rates for multi-currency support
- **Data Shared:** Your IP address (temporarily visible during API requests)
- **Data Collected by Frankfurter:** None (public API, no user data collected)
- **Location:** European Central Bank data via Frankfurter API servers
- **Website:** https://www.frankfurter.app/

#### Firebase Cloud Messaging (Push Notifications)
- **Purpose:** Deliver push notifications about subscription renewals
- **Data Shared:** Firebase messaging token (device-specific identifier)
- **Location:** Google Firebase servers
- **Privacy Policy:** https://firebase.google.com/support/privacy

### 6.2 We Do NOT Sell Your Data

We do **NOT**:
- Sell your personal information to third parties
- Share your data with advertisers or marketing companies
- Use your data for targeted advertising
- Share your data with data brokers

### 6.3 Legal Requirements

We may disclose your information if required by law or in response to:
- Court orders or legal processes
- Government or regulatory requests
- Requests to prevent fraud or illegal activity
- Requests to protect our rights, property, or safety

---

## 7. Your Privacy Rights

Depending on your location, you may have specific rights regarding your personal information:

### 7.1 Rights for All Users

- **Access:** You can access all your data within the App at any time
- **Correction:** You can edit or update your subscription information directly in the App
- **Deletion:** You can delete individual subscriptions, payments, or your entire account
- **Data Portability:** You can export your data by syncing to another device

### 7.2 GDPR Rights (EU/EEA/UK Users)

Under the GDPR, you have the following rights:

- **Right to Access:** Request a copy of your personal data
- **Right to Rectification:** Correct inaccurate or incomplete data
- **Right to Erasure ("Right to be Forgotten"):** Request deletion of your data
- **Right to Restriction:** Limit how we process your data
- **Right to Data Portability:** Receive your data in a structured, machine-readable format
- **Right to Object:** Object to processing based on legitimate interests
- **Right to Withdraw Consent:** Withdraw consent for processing at any time
- **Right to Lodge a Complaint:** File a complaint with your local data protection authority

**Exercising Your Rights:** Email support@subscriptin.com with your request. We will respond within 30 days.

### 7.3 CCPA Rights (California Residents)

Under the California Consumer Privacy Act (CCPA), you have the right to:

- **Know:** Request information about the categories and specific pieces of personal information we collect
- **Delete:** Request deletion of your personal information
- **Opt-Out of Sale:** Opt-out of the sale of personal information (Note: We do NOT sell your data)
- **Non-Discrimination:** Exercise your CCPA rights without discriminatory treatment

**Exercising Your Rights:** Email support@subscriptin.com with subject line "CCPA Request." We will respond within 45 days.

**Verification:** We may request additional information to verify your identity before fulfilling requests.

### 7.4 Australian Privacy Principles (APP) Rights

Under the Australian Privacy Act, you have the right to:

- **Access:** Request access to your personal information
- **Correction:** Request correction of inaccurate or out-of-date information
- **Complaint:** Lodge a complaint about our handling of your personal information with the Office of the Australian Information Commissioner (OAIC)

**Exercising Your Rights:** Email support@subscriptin.com. We will respond within 30 days.

---

## 8. Data Synchronization and Real-Time Updates

### 8.1 How Sync Works

Subscriptin uses real-time synchronization to keep your subscription data consistent across all your devices:

- **Bidirectional Sync:** Changes made on one device are automatically pushed to all other devices
- **Real-Time Updates:** Uses WebSocket connections to Supabase for instant synchronization
- **Offline Mode:** Changes made offline are queued locally and uploaded when you reconnect
- **Conflict Resolution:** If the same subscription is modified on multiple devices simultaneously, the most recent change (based on server timestamp) is kept

### 8.2 Background Sync

- **Android:** Sync occurs when the App is open or when scheduled alarms trigger (requires "Exact Alarm" permission)
- **iOS:** Background sync uses iOS Background Tasks (identifier: `com.subscriptin.sync`) to periodically refresh data

### 8.3 Sync Data

The following data types are synchronized:
- Subscriptions
- Custom categories
- Payment history
- Subscription pause/cancellation records

### 8.4 Disabling Sync

You can disable sync at any time through the App settings. Disabling sync will:
- Stop uploading local changes to the server
- Stop downloading remote changes from other devices
- Keep data local to your device only

---

## 9. Cookies and Tracking Technologies

### 9.1 What We Use

- **Session Tokens:** Used to keep you logged in and manage your session securely
- **Local Storage:** Stores your authentication state and sync preferences locally

### 9.2 What We Do NOT Use

We do **NOT** use:
- Advertising cookies
- Third-party tracking pixels
- Analytics cookies (e.g., Google Analytics, Mixpanel)
- Social media tracking (e.g., Facebook Pixel)

---

## 10. Device Permissions

Subscriptin requests the following permissions on your device:

### 10.1 Android Permissions

- **Internet:** Required to connect to Supabase, sync data, and fetch exchange rates
- **Access Network State:** Monitors connectivity to pause/resume sync when offline
- **Post Notifications (Android 13+):** Sends subscription renewal reminder notifications
- **Schedule Exact Alarm / Use Exact Alarm:** Schedules precise notifications for billing reminders

### 10.2 iOS Permissions

- **Notifications:** "Get notified before your subscriptions renew" - sends subscription renewal alerts
- **Background Tasks:** Enables background synchronization of subscription data

### 10.3 Managing Permissions

You can manage permissions at any time through your device's Settings app. Denying permissions may limit App functionality:
- **Notifications:** You won't receive renewal reminders
- **Internet:** The App cannot sync or update exchange rates

---

## 11. International Data Transfers

### 11.1 Data Storage Locations

Your data may be stored and processed in countries outside your country of residence, including:
- **Supabase Servers:** Asia Pacific (Seoul, South Korea) - AWS region ap-northeast-2
- **Firebase Servers:** Google Cloud Platform data centers globally

### 11.2 Safeguards for EU/EEA Users

For transfers from the EU/EEA to other countries:
- We rely on **Standard Contractual Clauses (SCCs)** approved by the European Commission
- Our service providers (Supabase, Firebase) comply with GDPR requirements for international transfers
- You can request a copy of applicable safeguards by emailing support@subscriptin.com

---

## 12. Changes to This Privacy Policy

We may update this Privacy Policy from time to time to reflect changes in our practices, technology, legal requirements, or other factors.

### 12.1 Notification of Changes

- **Material Changes:** We will notify you via email or in-app notification at least 30 days before changes take effect
- **Non-Material Changes:** We will update the "Last Updated" date at the top of this policy

### 12.2 Your Continued Use

Your continued use of Subscriptin after changes become effective constitutes your acceptance of the updated Privacy Policy.

### 12.3 Reviewing Updates

We encourage you to review this Privacy Policy periodically. The current version is always available within the App and at our website (if applicable).

---

## 13. Account Deletion and Data Export

### 13.1 Deleting Your Account

You can delete your Subscriptin account at any time:

1. Open the App
2. Navigate to Settings > Account
3. Select "Delete Account"
4. Confirm deletion

**What Happens When You Delete Your Account:**
- Your account is immediately deactivated
- You can no longer log in or access your data
- All data is retained for 30 days (for recovery and legal compliance)
- After 30 days, all your personal data is permanently deleted from our servers
- Local data on your device remains until you uninstall the App

### 13.2 Exporting Your Data

To export your data:
- **Multi-Device Sync:** Connect a new device to your account; all data automatically syncs
- **Manual Export:** Email support@subscriptin.com to request a data export in CSV or JSON format

We will provide your data export within 30 days of your request.

---

## 14. Third-Party Links

Subscriptin may contain links to third-party websites or services (e.g., subscription service websites via the "website URL" field).

**We are not responsible for:**
- The privacy practices of third-party websites
- Content or services provided by third parties

We recommend reviewing the privacy policies of any third-party sites you visit.

---

## 15. Logging and Debugging

### 15.1 Application Logs

We use Kermit logging library for debugging and troubleshooting:
- **Local Logs:** Stored only on your device
- **Content:** May include email addresses, sync metadata, error messages, and timestamps
- **Access:** Logs are not transmitted to our servers unless you explicitly share them with us for support purposes

### 15.2 Crash Reports

We do **NOT** use automatic crash reporting services. If you experience a crash and contact us for support, we may request logs from your device.

---

## 16. Automatic Payment Processing

### 16.1 How It Works

If you enable "Automatic Payments" for a subscription:
- Subscriptin automatically creates payment records based on your billing cycle
- This feature is purely for **tracking purposes** and does **NOT**:
   - Process actual financial transactions
   - Access your bank account or credit card
   - Charge you any fees

### 16.2 Scheduled Processing

- Payment records are created by a server-side function (`process_subscription_payments()`)
- Runs hourly via scheduled task (cron job)
- Respects your timezone for accurate billing date calculations
- Prevents duplicate payment records

---

## 17. Push Notifications

### 17.1 Types of Notifications

Subscriptin sends the following types of push notifications:

- **Subscription Renewal Reminders:** Alerts you before a subscription renews (timing configurable by you)
- **System Notifications:** Important account or security updates (rare)

### 17.2 Notification Settings

You can control notifications:
- **Enable/Disable Globally:** Turn all notifications on/off in device settings
- **Per-Subscription Control:** Enable/disable reminders for individual subscriptions
- **Timing Preferences:** Configure when you receive reminders (e.g., 3 days before renewal, at 9:00 AM)

### 17.3 Opting Out

To stop receiving notifications:
1. Go to your device Settings > Notifications > Subscriptin
2. Disable notifications for the App

Alternatively, disable notifications within the App settings.

---

## 18. Security Breach Notification

In the event of a data breach that affects your personal information:

- **Notification Timing:** We will notify you within 72 hours of discovering the breach (GDPR requirement)
- **Notification Method:** Email to your registered email address
- **Information Provided:** Description of the breach, types of data affected, steps we're taking, and recommended actions for you
- **Regulatory Notification:** We will notify applicable data protection authorities as required by law

---

## 19. Do Not Track (DNT) Signals

Subscriptin does not respond to "Do Not Track" (DNT) browser signals because:
- We do not use third-party tracking or advertising technologies
- We do not track your browsing activity outside the App
- All data collection is essential for App functionality

---

## 20. Business Transfers

If Subscriptin is involved in a merger, acquisition, asset sale, or bankruptcy:

- Your personal information may be transferred to a successor entity
- We will notify you via email before your information is transferred
- The new entity will be required to honor this Privacy Policy
- You will have the option to delete your account before the transfer

---

## 21. Contact Us

If you have any questions, concerns, or requests regarding this Privacy Policy or our data practices, please contact us:

**Email:** support@subscriptin.com
**Address:** 13 Joshua Place, Oxenford QLD 4210, Australia

We will respond to all inquiries within 30 days (or as required by applicable law).

---

## 22. Data Protection Officer

As an individual developer, Subscriptin does not have a formal Data Protection Officer (DPO). For all privacy-related inquiries, please contact support@subscriptin.com.

---

## 23. Governing Law and Jurisdiction

This Privacy Policy is governed by the laws of:
- **GDPR (for EU/EEA users):** European Union data protection law
- **CCPA (for California users):** California state law
- **Privacy Act 1988 (for Australian users):** Australian federal law

For users in other jurisdictions, this Privacy Policy is governed by the laws of **Australia** (Queensland and Australian federal law).

---

## 24. Supervisory Authorities

If you are located in the EU/EEA, you have the right to lodge a complaint with a supervisory authority:

- **EU/EEA:** Your local Data Protection Authority (DPA)
- **UK:** Information Commissioner's Office (ICO) - https://ico.org.uk/
- **Australia:** Office of the Australian Information Commissioner (OAIC) - https://www.oaic.gov.au/

---

## 25. Summary of Key Points

For your convenience, here is a summary of our privacy practices:

| **Category**                | **Details**                                                                    |
|-----------------------------|--------------------------------------------------------------------------------|
| **Information Collected**   | Email, subscription data, payment history, device info                         |
| **Purpose**                 | Account management, subscription tracking, multi-device sync                   |
| **Third-Party Sharing**     | Supabase (backend), Frankfurter API (exchange rates), Firebase (notifications) |
| **Data Sale**               | We do NOT sell your data                                                       |
| **Security**                | HTTPS/TLS encryption, Row-Level Security, password hashing                     |
| **Your Rights**             | Access, delete, export, correct your data                                      |
| **Data Retention**          | 30 days after account deletion                                                 |
| **Age Requirement**         | 13+ years old                                                                  |
| **International Transfers** | Data may be stored outside your country with appropriate safeguards            |
| **Cookies/Tracking**        | No advertising or analytics tracking                                           |
| **Contact**                 | support@subscriptin.com                                                        |

---

**By using Subscriptin, you acknowledge that you have read and understood this Privacy Policy and agree to its terms.**

---

*This Privacy Policy was last updated on December 7, 2025.*