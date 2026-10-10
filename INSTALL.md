# Install and manage Recipe Studio

No public installer has been published yet. Use this guide once a beta release is approved.

1. Open the official [Releases](https://github.com/kafeee80/CookidooRecipeStudioPublic/releases) page. Read that version's limits and beta terms.
2. Download RecipeStudio-Setup-<version>.exe and SHA256SUMS.txt. Do not download the repository ZIP expecting an app.
3. In PowerShell, run Get-FileHash -Algorithm SHA256 -LiteralPath 'C:\Users\YOUR-USER\Downloads\RecipeStudio-Setup-<version>.exe' with your actual path/version. Compare the whole hash with SHA256SUMS.txt. A matching checksum checks downloaded bytes; it does not establish publisher identity or replace a digital signature.
4. The initial candidate is **unsigned**. Windows may show an unknown-publisher or reputation warning. Do not disable Windows security protections. If unsure, cancel and ask in Issues.
5. Run setup for your Windows account. Optional desktop and quiet sign-in startup shortcuts are unchecked by default. Installation and local editing work offline; Cookidoo needs internet access.
6. Open Recipe Studio from Start. It starts a local server and opens your default browser. The tray icon may be under Windows' hidden-icons arrow. Closing the tab leaves the app running. Use tray Quit Recipe Studio or Start → Stop Recipe Studio to stop it; save first and wait for uploads to finish.

Optional sign-in startup starts quietly in the tray. It does not open the browser, run before sign-in or install a Windows service. Reopening the shortcut reuses your running instance.

## Upgrades

Export important recipes first. Save edits and finish any upload. Run the newer official installer for the same Windows account. It stops the owning app, takes a consistent app/data backup and verifies replacement files before launch. Saved recipes and upload history remain. Do not run parallel installers or downgrade manually. If an upgrade is interrupted, rerun the **same installer** to repair it before launching; ask for help if repair fails.

## Uninstall and your data

Use Windows Settings → Apps → Recipe Studio → Uninstall. It stops the owned app and removes installed shortcuts/startup. Saved recipes and backups are deliberately preserved for reinstall.

Data: %LOCALAPPDATA%\RecipeStudio. Installed application: %LOCALAPPDATA%\Programs\RecipeStudio. To erase all data permanently, export what you need, stop/uninstall, verify the exact data folder, then delete it manually. Never restore or copy a database while the app is running.

If the port is occupied, stop the other app/source copy through its own controls. Recipe Studio never kills unrelated processes. Always open through the shortcut after restart; do not share private launch URLs or server-control files.
