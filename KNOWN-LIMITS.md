# Supported behavior and known limits

## TM7 controls in 1.0.4

Generic actions support integer time 1–5940 seconds, the existing numeric speeds (0.5, 1, 1.5, 2, 2.5 and integers 3–10), distinct spoon speed (soft), discrete Celsius temperatures/OFF and reverse rotation. Heating above numeric speed 6 is blocked. Ingredient text links are serialized and compared with retrieved Cookidoo content.

| Native mode       | Supported settings                                                                                                        |
| ----------------- | ------------------------------------------------------------------------------------------------------------------------- |
| Dough             | Integer time 1–1200 seconds; legacy knead maps to Dough.                                                                  |
| Blend             | Integer time 10–300 seconds; speeds 6, 6.5, 7, 7.5 or 8.                                                                  |
| Turbo             | One pulse of 0.5, 1 or 2 seconds. Other pulse counts remain unconfirmed.                                                  |
| Warm Up           | 37°C or 40–90°C in 5°C steps; spoon speed, 1 or 2. No manual timer.                                                       |
| Rice Cooker       | Mode only; the appliance controls the operation.                                                                          |
| Steaming (Varoma) | Integer time 1–5940 seconds; spoon speed or 0.5–5 in half steps; forward/reverse; Varoma accessory. No temperature field. |
| Browning          | Integer time 1–1800 seconds; 140/145/150/155/160°C; Gentle power only.                                                    |

**New 1.0.4 native modes and spoon speed have official-editor/source and automated test coverage, but live Cookidoo/TM7 acceptance has not yet been reported.** A published beta does not imply every mode has been device-tested. The previous generic/linked-recipe subset has user-reported Czech account upload and TM7 control visibility.

Open Cooking is a physical TM7 function, but no confirmed Created Recipes encoding was found in the audited official editor. Open Cooking, unlisted modes (including Sous-vide/Slow Cook/Fermentation/Egg Boiler), additional pulse/accessory/power choices and TM5/TM6 native uploads remain blocked. Generic temperature Varoma is not silently replaced with 120°C; use the explicit Steaming mode. Some recipe metadata remains local. Scaling ingredients does not automatically scale machine timings or certify cooking results.

Czech linked-recipe upload and TM7 ingredient/control UI visibility are user-reported on firmware 1.6.15-202609050620. Physical cooking of that acceptance recipe and broader device coverage remain unverified. Nineteen other markets have public-route and mock tests only; see [markets](MARKETS.md).

The integration uses an unofficial interface that may change or stop working. Account eligibility/Created Recipes access is needed. No official compatibility guarantee or endorsement is claimed. Review your market's Cookidoo terms through its official site before using the integration; this project does not grant platform access or permission to bypass restrictions.

Credentials do not survive app restart; reconnect to upload. If an upload outcome is uncertain, use Upload history reconciliation before creating another copy. Writes are not retried automatically. Cookidoo read-back compares exact annotations; a returned difference is not accepted just because the recipe exists.

Windows x64 installer/tray/upgrade paths have local automated coverage. The owner reports successfully installing 1.0.3 and completing its requested Windows checks. New 1.0.4 device acceptance and interactive 1.0.5 destination-page acceptance remain pending. Version 1.0.5 shows the installation-folder chooser and remembers the existing path for upgrades; relocation requires uninstall/reinstall, preserving recipes and backups. This is not independent verification across all Windows versions, machines or accounts. Existing recipes/history are retained; older 1.0.3 cannot parse exports containing the new mode/soft fields. Keep pre-upgrade backups and do not manually downgrade.

The public beta binaries are unsigned. Support is best effort by one hobby maintainer, without a response-time promise. Local version-history browsing, automatic installation of updates, cloud accounts and mobile/LAN hosting are not included.
