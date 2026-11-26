# Wavehop Privacy Policy

Version 1.1, 2026-11-26. Publisher: Sven Kuehn, Switzerland.
Contact for questions and deletion requests: `contact.wavehop@gmail.com`

## In short

- Wavehop has **no analytics and no usage tracking**.
- Two things can leave your computer: **update checks** (on by default, can be turned off) and **crash / problem reports** (off until you opt in).
- Your audio never leaves your local network, except to the speakers you choose. Reports never contain audio, pairing keys, credentials or the controller identity.

## 1. Update checks

Wavehop (via WinSparkle) downloads a small feed file (`appcast.xml` or `appcast-beta.xml`) over HTTPS from the Wavehop release feed on GitHub Pages. GitHub, as host, sees your IP address and ordinary request headers (including a user agent that names Wavehop and its version), as with any web request. The Publisher does not receive or store this data. GitHub's own privacy statement applies to what GitHub logs. You can turn automatic update checks off in Wavehop; then no check is made until you ask for one.

## 2. Crash reports and problem reports (opt-in)

Nothing is sent until you choose "yes". The default is off. You can change the choice at any time; turning it off deletes pending reports and stops all sending.

**Where it goes:** Sentry (Functional Software, Inc.), project hosted in Sentry's **EU data region**.

**Crash report** (when Wavehop crashes and consent is on): a minidump (program state at the crash: memory contents of the Wavehop process, which may incidentally contain data such as speaker names or network addresses), Wavehop version and channel (beta or stable), Windows version, the last roughly 200 log lines, and tags (active protocol, group size, low-latency mode).

**Problem report** ("Report a Problem..."): the text you type, an optional email address you choose to give, the last two log files, the app configuration, and a system information summary. An optional minidump is only included if you take part in a crash report.

**Installation ID:** every report carries a random ID that Wavehop creates on your computer (first line of `%APPDATA%\Wavehop\crashes\installation_id`). It shows which reports come from the same installation and is not derived from you or your hardware.

**IP address:** Sentry receives your IP address when a report is sent, as with any web request. The project is set to store neither the address nor a location derived from it.

**Redaction before sending:** IPv4 addresses are shortened to /24 (for example `192.168.1.x`); IPv6 addresses to /48; MAC addresses and speaker device IDs are hashed; speaker display names are hashed unless you tick "include speaker names"; your Windows profile path is replaced by `%USERPROFILE%`.

**Never sent:** pairing keys, credentials, the controller identity, audio data.

**Limits:** at most 1 crash report and 5 problem reports per hour per installation.

**Retention:** Sentry keeps events for **30 days** on the plan used (default retention), then deletes them. If you did not opt in, a crash only leaves a local file in `%APPDATA%\Wavehop\crashes\` (up to 5, oldest deleted first), which stays on your computer.

## 3. Local data

Wavehop stores its settings, logs, and pairing information for AirPlay 2 speakers on your computer (settings and logs in `%APPDATA%\Wavehop`, pairing keys in Windows Credential Manager). This data is not sent anywhere. The uninstaller can remove it.

## 4. Your rights and deletion requests

You can ask what the Publisher holds about you and ask for deletion, for example of a problem report you sent. Write to the contact above and include the date and, if you can, the installation ID or the email address used in the report (Sentry events cannot otherwise be traced to a person). Requests are answered within 30 days. Swiss data protection law (FADP) applies; if you are in the EU or EEA you may also have rights under the GDPR.

## 5. Changes

If a future version sends more data, this policy changes first and Wavehop asks for your choice again.
