# Arkose Labs API Tracker

Automated tracker for Arkose Labs `api.js` (used in Roblox, X, Uber, etc.).

## Current Versions

| Service | Version | Build ID | Enforcement Hash |
| --- | --- | --- | --- |
| roblox_register | 4.4.5 | 07d8f962-3c3a-478e-adba-285b89b861f1 | bbaf081e26919bb3ac5123baa30c5f79 |
| roblox_login | 4.4.5 | 07d8f962-3c3a-478e-adba-285b89b861f1 | bbaf081e26919bb3ac5123baa30c5f79 |
| match_login | 4.4.5 | 07d8f962-3c3a-478e-adba-285b89b861f1 | bbaf081e26919bb3ac5123baa30c5f79 |
| uber_login | 4.4.5 | 07d8f962-3c3a-478e-adba-285b89b861f1 | bbaf081e26919bb3ac5123baa30c5f79 |
| snapchat_register | 4.4.2 | 719702df-f02c-490a-b25b-636f30148a1c | 9775dee111b6f5b2341a8bdde2d8f28f |
| x_register | 4.4.5 | 07d8f962-3c3a-478e-adba-285b89b861f1 | bbaf081e26919bb3ac5123baa30c5f79 |
| roblox_join | 4.4.5 | 07d8f962-3c3a-478e-adba-285b89b861f1 | bbaf081e26919bb3ac5123baa30c5f79 |
| roblox_recovery | 4.4.5 | 07d8f962-3c3a-478e-adba-285b89b861f1 | bbaf081e26919bb3ac5123baa30c5f79 |
| adobe_register | 4.4.5 | 07d8f962-3c3a-478e-adba-285b89b861f1 | bbaf081e26919bb3ac5123baa30c5f79 |

## How it works
- **Schedule:** Runs every 30 minutes via GitHub Actions.
- **Tracking:** Extracts the internal semantic version, build ID, and enforcement hash from the JS file.
- **Persistence:** Updates `versions.json` and saves the updated script to the `data/` folder.

## Files
- `versions.json`: JSON database of all detected versions and timestamps.
- `data/latest.js`: The most recently fetched `api.js`.
- `data/api_X_X_X.js`: Versioned archive of the SDK.

---
*Automatically updated by [GitHub Actions](.github/workflows/update-api.yml)*
