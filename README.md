# Recipe Studio

Prepare your own recipes, link ingredients to instructions, and upload them to Cookidoo for your Thermomix TM7.

An independent hobby project by **kafeee80**. Not affiliated with or endorsed by Vorwerk. Cookidoo and Thermomix are trademarks of their respective owners.

## Public beta 1.0.6

[Download Recipe Studio 1.0.6](https://github.com/kafeee80/CookidooRecipeStudioPublic/releases/tag/v1.0.6). The initial Windows beta is available for personal use. This repository contains documentation and issue templates, not application source. GitHub's “Source code” ZIP is not the application.

Installers are available under [Releases](https://github.com/kafeee80/CookidooRecipeStudioPublic/releases). Download only the named RecipeStudio-Setup-<version>.exe asset and its SHA256SUMS.txt. The initial beta is free for personal use with no expiry; read the [beta terms](BETA-TERMS.md).

**Before installing:** the Windows installer is unsigned, so Windows SmartScreen may show an unknown-publisher or reputation warning. Download only from this repository's [Releases](https://github.com/kafeee80/CookidooRecipeStudioPublic/releases). Checksums verify downloaded bytes; they are not a digital signature. Do not disable Windows security protections.

To check your download, each [release description](https://github.com/kafeee80/CookidooRecipeStudioPublic/releases) shows the installer’s SHA-256 and a copyable PowerShell Get-FileHash command. Compare the full hash before running setup.

**Connecting your account:** your Cookidoo credentials and session cookies are held in the app's memory on your PC, not saved by the app between restarts. Connecting sends login requests to Cookidoo/Vorwerk, and uploading sends the recipe content to Cookidoo. There is no telemetry or automatic reporting, and the app does not send credentials or recipes to the developer. Browser password managers may separately save a login. [Privacy details](PRIVACY.md).

Having trouble? Use the short [bug-report form](https://github.com/kafeee80/CookidooRecipeStudioPublic/issues/new?template=bug.yml) with your Cookidoo market, failing step and error text; sanitized recipe JSON is optional. **Issues and attachments are public.**

## What it does

- Local browser editor with EN/CZ interface, ingredient links and Thermomix controls.
- Version 1.0.4 adds spoon speed and native Dough, Blend, Turbo, Warm Up, Rice Cooker, Steaming (Varoma) and Gentle Browning. These additions have official-source/automated coverage; live Cookidoo/TM7 acceptance is still pending. See [exact limits](KNOWN-LIMITS.md).
- JSON import/export and GPT prompts for converting your own recipes. No built-in AI service or ChatGPT account integration.
- One Upload/Update action with checking, Cookidoo read-back verification and upload recovery history.
- Windows tray controls, optional quiet sign-in startup, configurable installation folder and upgrades that preserve saved recipes.
- Twenty selectable Cookidoo markets; **only the Czech market has user-reported live upload and TM7 UI acceptance**. The others are experimental.

## What has actually been tested?

| Cookidoo market          | Thermomix model | Evidence and gaps                                                                                                                                                |
| ------------------------ | --------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Czech Republic           | TM7             | User-reported live recipe upload, ingredient text links and machine controls visible on the device. Physical cooking of that acceptance recipe is not confirmed. |
| Other selectable markets | TM7             | Public-route checks and automated mock tests only. Live login, upload and device testers needed; functionality is not guaranteed.                                |
| Any market               | TM5 / TM6       | Native uploads are not implemented.                                                                                                                              |

**New native modes and spoon speed still await live Cookidoo/TM7 acceptance, including in the Czech market.** Automated/source checks are not device testing. See [market choices](MARKETS.md) and [exact control limits](KNOWN-LIMITS.md). If you test another market, please [report your result](SUPPORT.md) and distinguish upload, device UI inspection and actual cooking.

![Example editor with synthetic test data](images/editor.png)
![Inspect-and-copy support diagnostics](images/diagnostics.png)

## Start here

[Install, stop, upgrade and uninstall](INSTALL.md) · [Supported controls and known limits](KNOWN-LIMITS.md) · [Markets](MARKETS.md) · [Privacy](PRIVACY.md) · [Reporting bugs](SUPPORT.md) · [Changelog](CHANGELOG.md)

Windows x64 is the packaging target. The installer requires Windows 10 build 17763 or newer; that technical minimum is not a claim that every Windows edition/build has been tested. The owner reports completing the requested 1.0.3 Windows acceptance checks successfully. Coverage is user-reported on the owner’s environment; broader Windows coverage still needs community feedback. No Node, Git, terminal or administrator rights are required for the default per-user install.

A matching Cookidoo account with Created Recipes access and an internet connection are needed for uploads. Review the recipe and controls on your TM7 before cooking. Verification confirms returned Cookidoo content, not cooking safety or results.
