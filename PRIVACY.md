# Privacy and network behavior

Recipe Studio is a local application, not a hosted recipe service. The maintainer does not receive your recipes or Cookidoo credentials through the app.

- Saved recipes, ingredient links, upload attempts and recovery backups remain in your Windows profile. Browser settings and unsaved-draft recovery use browser-local storage. Upload records may contain recipe payloads and Cookidoo IDs; they are private and should not be posted.
- Cookidoo credentials/session cookies are held in the local server's memory while connected. The password field clears on submission; disconnect/restart discards session references. This is not a promise of secure memory erasure or revocation of every remote session. A browser password manager, extensions and Windows may have their own behavior outside the app.
- Connecting contacts the selected Cookidoo HTTPS market and its explicitly allowed Vorwerk authentication services. Uploading sends that recipe's relevant content to Cookidoo. Cookidoo handles those requests under its own market-specific terms and privacy policy.
- There is no telemetry, automatic bug reporting or background update check. Opening Cookidoo/GitHub links intentionally contacts those sites under their policies.
- Generate diagnostic report in Settings creates an inspectable report locally. It contains app version, broad OS/runtime details, market/domain/route, lifecycle/connection status and the last bounded Cookidoo error code in this server session. No passwords, cookies, email, recipes, account IDs, database contents or filesystem paths. It does not read logs or send a report. Copying puts the displayed text on the clipboard only.
- Reports and screenshots **you post to GitHub Issues are public** and processed by GitHub. Review everything before posting. Do not attach databases, raw logs, cookie exports or browser network captures.

Local access protections cannot defend against malware running as your Windows user. Closing the browser does not disconnect/stop the app. Uninstall preserves your data; see [removal instructions](INSTALL.md).
