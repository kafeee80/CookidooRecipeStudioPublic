# Report problems or share a test result

Use [Issues](https://github.com/kafeee80/CookidooRecipeStudioPublic/issues/new/choose). Please include version, selected market, exact steps, expected/actual result and whether ordinary Created Recipes works in Cookidoo's own editor.

In **Settings → Help and diagnostics → Generate diagnostic report**, inspect the JSON and choose Copy diagnostic report. Paste it into the issue. This is available in the 1.0.2 candidate; 1.0.1 has Copy connection details after a failed connection. Last error code is server-session scoped and can describe an earlier error; reproduce immediately before generating. The lifecycle describes the server, not Windows tray health.

A minimal synthetic recipe is welcome if needed. Screenshots should show no email, private recipe details, account IDs or private launch URLs. Never attach SQLite databases, passwords, cookies, server-control.json, logs or HAR/network captures. If the app cannot launch, state the installer version and error text with personal paths/details removed rather than dumping logs.

For uncertain uploads, reconcile in Upload history first. Do not keep creating duplicates to test a failure.

Voluntary feedback: did installation work, did upload/read-back work, did you inspect and actually cook on TM7, and would you use it again? Mark UI inspection separately from cooking. Include OS/build, market and TM7 firmware when relevant. No report is sent by the app and no analytics are collected automatically.

For a security concern, do not post exploit details or secrets publicly. Use GitHub private vulnerability reporting on this repository when enabled. If unavailable, create an issue containing only a request for a private reporting channel.
