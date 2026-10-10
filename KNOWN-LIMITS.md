# Supported behavior and known limits

Native uploads target the existing tested generic **TM7** action subset: time, numeric temperatures and speeds including half-step speeds such as 1.5, and reverse rotation. Ingredient text links are serialized and compared with retrieved Cookidoo content.

Varoma, soft/spoon speed, named modes/open cooking and TM5/TM6 native uploads are not enabled in the initial candidate. Some recipe metadata remains local. Unsupported controls are blocked rather than silently converted. Scaling ingredients does not automatically scale machine timings or certify cooking results.

Czech linked-recipe upload and TM7 ingredient/control UI visibility are user-reported on firmware 1.6.15-202609050620. Physical cooking of the acceptance recipe and broader recipe/device coverage are still unverified. Nineteen other markets have public-route and mock tests only; see [markets](MARKETS.md).

The integration uses an unofficial interface that may change or stop working. Account eligibility/Created Recipes access is needed. No official compatibility guarantee or endorsement is claimed. Review your market's Cookidoo terms through its official site before using the integration; this project does not grant platform access or permission to bypass restrictions.

Credentials do not survive app restart; reconnect to upload. If an upload outcome is uncertain, use Upload history reconciliation before creating another copy. Writes are not retried automatically.

Windows x64 installer/tray/upgrade paths have local automated coverage. The owner successfully installed and used 1.0.1. The owner reports installing 1.0.3 and successfully completing all requested Windows checks. This user report is not independent verification across all Windows versions, machines or accounts.

The public beta binaries are unsigned. Support is best effort by one hobby maintainer, without a response-time promise. Local version-history browsing, automatic installation of updates, cloud accounts and mobile/LAN hosting are not included.
