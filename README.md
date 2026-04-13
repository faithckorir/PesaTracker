<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>PesaTracker — Privacy Policy</title>
  <meta name="description" content="Privacy policy for the PesaTracker Android app by fundevcrafts." />
  <style>
    :root { color-scheme: light dark; }
    body {
      font-family: system-ui, -apple-system, Segoe UI, Roboto, Ubuntu, Cantarell, sans-serif;
      line-height: 1.55;
      max-width: 44rem;
      margin: 0 auto;
      padding: 1.25rem 1rem 3rem;
      color: #111;
      background: #fafafa;
    }
    @media (prefers-color-scheme: dark) {
      body { color: #e8eaed; background: #121212; }
      a { color: #8ab4f8; }
      table { border-color: #3c4043; }
      th, td { border-color: #3c4043; }
    }
    h1 { font-size: 1.65rem; margin-top: 0; }
    h2 { font-size: 1.2rem; margin-top: 2rem; }
    h3 { font-size: 1.05rem; margin-top: 1.25rem; }
    .meta { color: #555; font-size: 0.95rem; margin-bottom: 1.5rem; }
    @media (prefers-color-scheme: dark) { .meta { color: #9aa0a6; } }
    blockquote {
      margin: 1rem 0;
      padding: 0.75rem 1rem;
      border-left: 4px solid #f05a22;
      background: rgba(240, 90, 34, 0.08);
    }
    table { border-collapse: collapse; width: 100%; margin: 1rem 0; font-size: 0.95rem; }
    th, td { border: 1px solid #ccc; padding: 0.5rem 0.65rem; text-align: left; vertical-align: top; }
    th { background: rgba(0,0,0,0.04); }
    @media (prefers-color-scheme: dark) {
      th { background: rgba(255,255,255,0.06); }
    }
    hr { border: none; border-top: 1px solid #ddd; margin: 2rem 0; }
    @media (prefers-color-scheme: dark) { hr { border-top-color: #3c4043; } }
    ul { padding-left: 1.25rem; }
    a { word-break: break-all; }
  </style>
</head>
<body>

  <h1>PesaTracker — Privacy Policy</h1>
  <p class="meta"><strong>Last updated:</strong> April 2, 2026<br />
  <strong>This page URL</strong> is the link you can paste in Google Play Console → App content → Privacy policy (after you publish GitHub Pages).</p>

  <p>This Privacy Policy describes how <strong>PesaTracker</strong> (“the App,” “we,” “us”) handles information when you use our Android application published on <strong>Google Play</strong> under the developer account <strong>fundevcrafts</strong> (package <strong>com.fundevcrafts.pesatracker</strong>).</p>

  <blockquote>
    <strong>Important:</strong> PesaTracker is designed as a <strong>local, on-device</strong> money journal. It does <strong>not</strong> operate a sign-in server or a cloud database controlled by us for your M-Pesa SMS content. Any transmission of your data off the device happens only through <strong>your device’s operating system</strong>, <strong>your chosen backup/export flows</strong>, or <strong>tools you separately use</strong> (for example email, cloud drives, or messaging apps).
  </blockquote>

  <p><strong>Contact:</strong> <a href="mailto:fundevcrafts@gmail.com">fundevcrafts@gmail.com</a></p>

  <hr />

  <h2>1. Summary</h2>
  <table>
    <thead><tr><th>Topic</th><th>What we do</th></tr></thead>
    <tbody>
      <tr><td><strong>M-Pesa SMS</strong></td><td>The App may read <strong>SMS messages</strong> from your device that match <strong>M-Pesa / MPESA</strong> sender patterns, <strong>only</strong> to build your transaction journal, balances, fees, and related insights <strong>on your device</strong>.</td></tr>
      <tr><td><strong>Our servers</strong></td><td>We do <strong>not</strong> receive your SMS bodies or a copy of your inbox through the App’s own network APIs. The App’s manifest does <strong>not</strong> declare general <strong>Internet</strong> access for sending your journal to us.</td></tr>
      <tr><td><strong>Storage</strong></td><td>Categories, notes, budgets, events, app preferences, and similar data are stored <strong>on your device</strong> (including <strong>encrypted</strong> storage where implemented).</td></tr>
      <tr><td><strong>Exports &amp; backups</strong></td><td>When <strong>you</strong> export CSV/JSON or save a backup file, <strong>you</strong> choose where it goes (e.g. Downloads, Drive, email). We do not control that destination.</td></tr>
      <tr><td><strong>App lock &amp; biometrics</strong></td><td>Optional <strong>PIN</strong> and <strong>device biometrics</strong> are used <strong>on-device</strong> to unlock the App; biometric templates are handled by <strong>Android</strong>, not sent to us.</td></tr>
      <tr><td><strong>Notifications</strong></td><td>Optional <strong>local notifications</strong> (e.g. reminders) may use <strong>notification</strong> permission where the OS requires it.</td></tr>
    </tbody>
  </table>

  <hr />

  <h2>2. Who this applies to</h2>
  <p>You are a user of PesaTracker on an Android device. This policy applies to the <strong>App</strong> only. It does not govern third-party services (Google Play, your device manufacturer, your mobile carrier, M-Pesa/Safaricom, or apps you use to share exported files).</p>

  <hr />

  <h2>3. Information the App accesses</h2>

  <h3>3.1 SMS (READ_SMS)</h3>
  <p><strong>Purpose:</strong> Core functionality is <strong>SMS-based money management / journaling</strong>: reading <strong>M-Pesa-related SMS</strong> from the device <strong>SMS inbox</strong> (via the system SMS content provider) to extract transaction details (such as amounts, fees, types, and timestamps) and to show summaries inside the App.</p>
  <p><strong>Scope:</strong> The App is intended to work with messages associated with <strong>M-Pesa</strong> senders (for example identifiers such as <strong>MPESA</strong> / <strong>M-PESA</strong> as implemented in the App). It is <strong>not</strong> intended to read your full personal SMS history for unrelated purposes.</p>
  <p><strong>When:</strong> SMS is read when <strong>you</strong> use features that depend on it (for example opening Home, History, Insights, or related screens) and when <strong>you</strong> have granted the <strong>SMS</strong> permission in Android settings.</p>
  <p><strong>If you deny SMS access:</strong> Features that depend on parsing M-Pesa SMS will be <strong>limited or unavailable</strong>. Other parts of the App may still work where they do not depend on SMS.</p>

  <h3>3.2 Notifications (POST_NOTIFICATIONS, where applicable)</h3>
  <p>On supported Android versions, the App may request permission to show <strong>notifications</strong> (for example recurring reminders). Notification content is generated <strong>for you</strong> based on data already on the device.</p>

  <h3>3.3 Device biometrics (optional)</h3>
  <p>If you enable <strong>biometric unlock</strong> for the App lock feature, <strong>Android’s biometric APIs</strong> verify you on the device. We do <strong>not</strong> receive your fingerprint or face data.</p>

  <h3>3.4 No account system from us</h3>
  <p>The App does not require you to create an <strong>account with us</strong> to use local features. Any “login” or onboarding flow inside the App is part of the <strong>on-device experience</strong> and does not, by itself, send your SMS to our servers.</p>

  <hr />

  <h2>4. Information stored on your device</h2>
  <p>The App may store, among other things:</p>
  <ul>
    <li>Parsed <strong>transaction summaries</strong> derived from SMS (for example amounts, counterparties, categories, and notes you add).</li>
    <li><strong>Categories</strong>, <strong>budgets</strong>, <strong>events</strong>, <strong>links</strong> between transactions and events, <strong>reminders</strong>, and <strong>preferences</strong> (such as display name or balance visibility).</li>
    <li><strong>Encrypted</strong> preferences for sensitive items (for example app lock configuration), as implemented in the version you installed.</li>
  </ul>
  <p><strong>SMS bodies</strong> are read from the system when needed for parsing; the App does not need to permanently store the <strong>entire</strong> raw SMS body for core journaling if derived fields are sufficient—see your installed version’s behavior in Settings and export samples.</p>

  <hr />

  <h2>5. What leaves your device</h2>

  <h3>5.1 We do not operate a “PesaTracker cloud” for your SMS</h3>
  <p>We do <strong>not</strong> run a backend service shown in the App whose purpose is to <strong>upload your full SMS inbox</strong> to us.</p>

  <h3>5.2 Actions you initiate</h3>
  <p>You may explicitly:</p>
  <ul>
    <li><strong>Export</strong> CSV files or similar summaries.</li>
    <li><strong>Back up</strong> or <strong>restore</strong> a JSON backup through flows you start.</li>
  </ul>
  <p>In those cases, data is written to a <strong>location you choose</strong> or handled by <strong>another app</strong> you use. You are responsible for those destinations’ privacy and security.</p>

  <h3>5.3 Android backup / device transfer</h3>
  <p>The App may have <strong>Android backup / data extraction</strong> rules enabled or updated over time. <strong>Google</strong>, <strong>your device OEM</strong>, or <strong>your backup provider</strong> may participate in device backup or transfer according to <strong>their</strong> policies and your system settings. That is <strong>outside our direct control</strong>; review your device backup settings if this matters to you.</p>

  <hr />

  <h2>6. Permissions (reference)</h2>
  <p>The App may request or use permissions including:</p>
  <table>
    <thead><tr><th>Permission</th><th>Why</th></tr></thead>
    <tbody>
      <tr><td><strong>READ_SMS</strong></td><td>Read <strong>M-Pesa-related</strong> SMS to build your on-device journal and analytics.</td></tr>
      <tr><td><strong>POST_NOTIFICATIONS</strong></td><td>Show <strong>local notifications</strong> where required by the OS.</td></tr>
    </tbody>
  </table>
  <p>Other capabilities (for example <strong>biometric unlock</strong>) may rely on <strong>system components</strong> and <strong>AndroidX libraries</strong> without additional sensitive permissions declared by us beyond what the OS merges from dependencies.</p>

  <hr />

  <h2>7. Third-party services and libraries</h2>
  <p>The App is distributed through <strong>Google Play</strong> and uses standard <strong>Android</strong> and <strong>Google/AndroidX</strong> libraries. Those providers process data under <strong>their</strong> policies (for example Play Console processing, crash reporting if you add it in a future version, etc.).</p>
  <p><strong>Analytics / advertising:</strong> The version this policy was written for is intended <strong>without</strong> embedded third-party advertising SDKs or cross-app tracking. If a future build adds analytics or crash reporting, we will update this policy and the <strong>Google Play Data safety</strong> section before release.</p>

  <hr />

  <h2>8. Security</h2>
  <ul>
    <li>Sensitive on-device values may be protected with <strong>Android Keystore–backed encryption</strong> (for example <strong>EncryptedSharedPreferences</strong>) where implemented.</li>
    <li>An optional <strong>app lock</strong> (PIN / biometric) limits access to the App on your device.</li>
    <li>You should keep your device OS updated, use a strong screen lock, and avoid sharing export files you consider confidential.</li>
  </ul>
  <p>No method of storage or transport is 100% secure.</p>

  <hr />

  <h2>9. Children’s privacy</h2>
  <p>PesaTracker is <strong>not directed to children under 13</strong> (or the minimum age required in your country). We do not knowingly collect personal information from children. If you believe a child has provided information through misuse of the App, contact <a href="mailto:fundevcrafts@gmail.com">fundevcrafts@gmail.com</a> and we can help describe how to remove the App and local data from the device.</p>

  <hr />

  <h2>10. Your choices and controls</h2>
  <ul>
    <li><strong>SMS:</strong> Grant or revoke <strong>READ_SMS</strong> in Android <strong>Settings → Apps → PesaTracker → Permissions</strong>.</li>
    <li><strong>Notifications:</strong> Toggle notification permission and channels in system settings.</li>
    <li><strong>App lock / biometrics:</strong> Change or disable in the App’s settings where offered.</li>
    <li><strong>Data on device:</strong> Uninstalling the App removes App-private data unless the OS or you have retained copies (for example backups or exports you saved).</li>
  </ul>

  <hr />

  <h2>11. International users &amp; M-Pesa</h2>
  <p>PesaTracker is built around <strong>Kenya M-Pesa SMS</strong> conventions. If you use the App outside Kenya or with non-standard carrier formats, parsing may be incomplete or inaccurate. Currency and formatting are shown for convenience and are not financial, tax, or legal advice.</p>

  <hr />

  <h2>12. Changes to this policy</h2>
  <p>We may update this policy when we change features, permissions, or legal requirements. The <strong>“Last updated”</strong> date at the top will change. For <strong>material</strong> changes, we will take reasonable steps to notify you inside the App or via the Play listing, as appropriate.</p>
  <p>Continued use after the effective date means you accept the updated policy.</p>

  <hr />

  <h2>13. Contact</h2>
  <p><strong>Google Play developer account:</strong> fundevcrafts<br />
  <strong>Email:</strong> <a href="mailto:fundevcrafts@gmail.com">fundevcrafts@gmail.com</a><br />
  <strong>Play Store listing (when published):</strong> <a href="https://play.google.com/store/apps/details?id=com.fundevcrafts.pesatracker">https://play.google.com/store/apps/details?id=com.fundevcrafts.pesatracker</a></p>

  <hr />

  <h2>14. Disclaimer</h2>
  <p>PesaTracker is a <strong>personal productivity tool</strong>. It is not a bank, not affiliated with <strong>Safaricom</strong> or <strong>M-Pesa</strong>, and does not guarantee accuracy of parsed amounts or eligibility for any regulatory regime. Use at your own risk alongside your official M-Pesa records.</p>

</body>
</html>
