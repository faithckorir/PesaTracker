# PesaTracker — Privacy Policy

**Last updated:** April 2, 2026  

This Privacy Policy describes how **PesaTracker** (“the App,” “we,” “us”) handles information when you use our Android application published on **Google Play** under the developer account **fundevcrafts** (package **`com.fundevcrafts.pesatracker`**).

> **Important:** PesaTracker is designed as a **local, on-device** money journal. It does **not** operate a sign-in server or a cloud database controlled by us for your M-Pesa SMS content. Any transmission of your data off the device happens only through **your device’s operating system**, **your chosen backup/export flows**, or **tools you separately use** (for example email, cloud drives, or messaging apps).

**Contact:** fundevcrafts@gmail.com  

**Public copy of this policy (required URL for Play Console):** host this document at a stable **HTTPS** address (for example GitHub Pages, your own domain, or Google Sites) and paste that link in Play Console → App content → Privacy policy. Replace the bracketed note below when live: **[ADD_YOUR_PUBLIC_HTTPS_URL_HERE]**

---

## 1. Summary

| Topic | What we do |
|--------|------------|
| **M-Pesa SMS** | The App may read **SMS messages** from your device that match **M-Pesa / MPESA** sender patterns, **only** to build your transaction journal, balances, fees, and related insights **on your device**. |
| **Our servers** | We do **not** receive your SMS bodies or a copy of your inbox through the App’s own network APIs. The App’s manifest does **not** declare general **Internet** access for sending your journal to us. |
| **Storage** | Categories, notes, budgets, events, app preferences, and similar data are stored **on your device** (including **encrypted** storage where implemented). |
| **Exports & backups** | When **you** export CSV/JSON or save a backup file, **you** choose where it goes (e.g. Downloads, Drive, email). We do not control that destination. |
| **App lock & biometrics** | Optional **PIN** and **device biometrics** are used **on-device** to unlock the App; biometric templates are handled by **Android**, not sent to us. |
| **Notifications** | Optional **local notifications** (e.g. reminders) may use **notification** permission where the OS requires it. |

---

## 2. Who this applies to

You are a user of PesaTracker on an Android device. This policy applies to the **App** only. It does not govern third-party services (Google Play, your device manufacturer, your mobile carrier, M-Pesa/Safaricom, or apps you use to share exported files).

---

## 3. Information the App accesses

### 3.1 SMS (READ_SMS)

**Purpose:** Core functionality is **SMS-based money management / journaling**: reading **M-Pesa-related SMS** from the device **SMS inbox** (via the system SMS content provider) to extract transaction details (such as amounts, fees, types, and timestamps) and to show summaries inside the App.

**Scope:** The App is intended to work with messages associated with **M-Pesa** senders (for example identifiers such as **MPESA** / **M-PESA** as implemented in the App). It is **not** intended to read your full personal SMS history for unrelated purposes.

**When:** SMS is read when **you** use features that depend on it (for example opening Home, History, Insights, or related screens) and when **you** have granted the **SMS** permission in Android settings.

**If you deny SMS access:** Features that depend on parsing M-Pesa SMS will be **limited or unavailable**. Other parts of the App may still work where they do not depend on SMS.

### 3.2 Notifications (POST_NOTIFICATIONS, where applicable)

On supported Android versions, the App may request permission to show **notifications** (for example recurring reminders). Notification content is generated **for you** based on data already on the device.

### 3.3 Device biometrics (optional)

If you enable **biometric unlock** for the App lock feature, **Android’s biometric APIs** verify you on the device. We do **not** receive your fingerprint or face data.

### 3.4 No account system from us

The App does not require you to create an **account with us** to use local features. Any “login” or onboarding flow inside the App is part of the **on-device experience** and does not, by itself, send your SMS to our servers.

---

## 4. Information stored on your device

The App may store, among other things:

- Parsed **transaction summaries** derived from SMS (for example amounts, counterparties, categories, and notes you add).
- **Categories**, **budgets**, **events**, **links** between transactions and events, **reminders**, and **preferences** (such as display name or balance visibility).
- **Encrypted** preferences for sensitive items (for example app lock configuration), as implemented in the version you installed.

**SMS bodies** are read from the system when needed for parsing; the App does not need to permanently store the **entire** raw SMS body for core journaling if derived fields are sufficient—see your installed version’s behavior in Settings and export samples.

---

## 5. What leaves your device

### 5.1 We do not operate a “PesaTracker cloud” for your SMS

We do **not** run a backend service shown in the App whose purpose is to **upload your full SMS inbox** to us.

### 5.2 Actions you initiate

You may explicitly:

- **Export** CSV files or similar summaries.
- **Back up** or **restore** a JSON backup through flows you start.

In those cases, data is written to a **location you choose** or handled by **another app** you use. You are responsible for those destinations’ privacy and security.

### 5.3 Android backup / device transfer

The App may have **Android backup / data extraction** rules enabled or updated over time. **Google**, **your device OEM**, or **your backup provider** may participate in device backup or transfer according to **their** policies and your system settings. That is **outside our direct control**; review your device backup settings if this matters to you.

---

## 6. Permissions (reference)

The App may request or use permissions including:

| Permission | Why |
|------------|-----|
| **READ_SMS** | Read **M-Pesa-related** SMS to build your on-device journal and analytics. |
| **POST_NOTIFICATIONS** | Show **local notifications** where required by the OS. |

Other capabilities (for example **biometric unlock**) may rely on **system components** and **AndroidX libraries** without additional sensitive permissions declared by us beyond what the OS merges from dependencies.

---

## 7. Third-party services and libraries

The App is distributed through **Google Play** and uses standard **Android** and **Google/AndroidX** libraries. Those providers process data under **their** policies (for example Play Console processing, crash reporting if you add it in a future version, etc.).

**Analytics / advertising:** The open-source project version this policy was written for is intended **without** embedded third-party advertising SDKs or cross-app tracking. If a future build adds analytics or crash reporting, we will update this policy and the **Google Play Data safety** section before release.

---

## 8. Security

- Sensitive on-device values may be protected with **Android Keystore–backed encryption** (for example **EncryptedSharedPreferences**) where implemented.
- An optional **app lock** (PIN / biometric) limits access to the App on your device.
- You should keep your device OS updated, use a strong screen lock, and avoid sharing export files you consider confidential.

No method of storage or transport is 100% secure.

---

## 9. Children’s privacy

PesaTracker is **not directed to children under 13** (or the minimum age required in your country). We do not knowingly collect personal information from children. If you believe a child has provided information through misuse of the App, contact **fundevcrafts@gmail.com** and we can help describe how to remove the App and local data from the device.

---

## 10. Your choices and controls

- **SMS:** Grant or revoke **READ_SMS** in Android **Settings → Apps → PesaTracker → Permissions**.
- **Notifications:** Toggle notification permission and channels in system settings.
- **App lock / biometrics:** Change or disable in the App’s settings where offered.
- **Data on device:** Uninstalling the App removes App-private data unless the OS or you have retained copies (for example backups or exports you saved).

---

## 11. International users & M-Pesa

PesaTracker is built around **Kenya M-Pesa SMS** conventions. If you use the App outside Kenya or with non-standard carrier formats, parsing may be incomplete or inaccurate. Currency and formatting are shown for convenience and are not financial, tax, or legal advice.

---

## 12. Changes to this policy

We may update this policy when we change features, permissions, or legal requirements. The **“Last updated”** date at the top will change. For **material** changes, we will take reasonable steps to notify you inside the App or via the Play listing, as appropriate.

Continued use after the effective date means you accept the updated policy.

---

## 13. Contact

**Google Play developer account:** fundevcrafts  
**Email:** fundevcrafts@gmail.com  
**Play Store listing (when published):** https://play.google.com/store/apps/details?id=com.fundevcrafts.pesatracker

---

## 14. Disclaimer

PesaTracker is a **personal productivity tool**. It is not a bank, not affiliated with **Safaricom** or **M-Pesa**, and does not guarantee accuracy of parsed amounts or eligibility for any regulatory regime. Use at your own risk alongside your official M-Pesa records.

---

## 15. How to delete your data

Because PesaTracker is **local-first**, there is **no account on our servers** for us to erase on your behalf. You control data on your phone and any copies you saved elsewhere.

**In the App:** Open **More** → **Delete your data** for the same instructions summarized on your device.

1. **Clear app data on this device:** Android **Settings → Apps → PesaTracker → Storage** → **Clear data** or **Clear storage**. This removes journal data, categories, notes, events, reminders, and app preferences stored by PesaTracker. Your original M-Pesa SMS messages in the phone’s SMS app are **not** changed by this.
2. **Remove exports and backups you saved:** Delete any CSV exports, JSON backups, or other files you saved (for example in Downloads, Files, Google Drive, or email). We cannot delete files from those locations for you.
3. **Uninstall the app:** Uninstalling PesaTracker removes the app’s private data from the device (unless you restore from a system backup or keep copies you created).

If you emailed us a file and want us to discard it, or you need help with these steps, contact **fundevcrafts@gmail.com**.

**Public anchor URL (e.g. Play Console):** use the hosted privacy policy page with fragment `#delete-your-data` when a dedicated “how to delete” link is required.
