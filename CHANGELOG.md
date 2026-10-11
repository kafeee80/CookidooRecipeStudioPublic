# Changelog

1.0.3 is the first public beta. Earlier entries describe private test builds.

## 1.0.4 — native TM7 controls · 2026-10-11

- Adds distinct spoon/soft speed, Dough, Blend, Turbo, Warm Up, Rice Cooker, Steaming (Varoma) and Gentle Browning.
- Mode-specific controls and validation; Turbo preserves 0.5/1/2-second single pulses. Changing mode is undoable.
- Updated English/Czech labels, instruction formatting and GPT conversion prompts.
- Exact verification includes native mode names, fields and positions; uncertain writes retain read-only recovery.
- 297 automated unit/integration tests, 44 browser workflows and bundled-runtime smoke checks pass. New controls still need live Cookidoo/TM7 acceptance; publication is owner-authorized, not a report that device tests passed.
- Open Cooking/unlisted modes, multiple-pulse presets, other accessories/powers and TM5/TM6 uploads remain unsupported. See [limits](KNOWN-LIMITS.md).
- Existing recipes/history retained; approved personal-use/no-expiry terms unchanged. Unsigned Windows x64 beta.

## 1.0.3 — first public beta · 2026-10-10

- Existing leaf branding across Windows setup, launcher, desktop/Start shortcuts, tray, browser favicon and sidebar.
- Branded tray warning badge preserves failure visibility. No recipe/schema/upload changes.
- Approved free personal-use beta terms, without expiry. Includes diagnostics and installer privacy/notices.
- Owner reports successful installation and requested Windows checks. Unsigned Windows x64 distribution.

## 1.0.2 — public beta preparation candidate

- Inspect/copy sanitized diagnostics in Settings, with no automatic submission.
- Public documentation, bug/market-feedback templates and draft personal-use terms.
- Updated installer information for quiet tray startup; included privacy and beta terms.
- Same TM7 capability subset and SQLite schema 2. Windows public-release gates remain pending.

## 1.0.1 — owner-tested Windows build

Persistent tray controls, quiet sign-in startup, single-instance reuse, verified upgrade backups and repair/recovery guards. Owner reports successful installation and app use. Not a publicly released beta.

## 1.0.0 — initial local/source baseline

Local recipe editing/import/export, ingredient text linking, TM7 upload verification/recovery, EN/CZ, themes, GPT toolkit and initial self-contained per-user installer.
