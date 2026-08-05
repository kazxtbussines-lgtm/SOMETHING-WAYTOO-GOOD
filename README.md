# Arkose Labs API Tracker

Automated tracker for Arkose Labs `api.js` (used in Roblox, X, Uber, etc.).

## Current Versions

| Service | Version | Build ID | Enforcement Hash |
| --- | --- | --- | --- |
| roblox_register | 4.4.4 | 6ec5c11b-00bc-4826-a134-2d79e64b496f | bc9a239a0c2a7b99d5cd13509a17195e |
| roblox_login | 4.4.4 | 6ec5c11b-00bc-4826-a134-2d79e64b496f | bc9a239a0c2a7b99d5cd13509a17195e |
| match_login | 4.4.4 | 6ec5c11b-00bc-4826-a134-2d79e64b496f | bc9a239a0c2a7b99d5cd13509a17195e |
| uber_login | 4.4.4 | 6ec5c11b-00bc-4826-a134-2d79e64b496f | bc9a239a0c2a7b99d5cd13509a17195e |
| snapchat_register | 4.4.2 | 719702df-f02c-490a-b25b-636f30148a1c | 9775dee111b6f5b2341a8bdde2d8f28f |
| x_register | 4.4.4 | 6ec5c11b-00bc-4826-a134-2d79e64b496f | bc9a239a0c2a7b99d5cd13509a17195e |
| roblox_join | 4.4.4 | 6ec5c11b-00bc-4826-a134-2d79e64b496f | bc9a239a0c2a7b99d5cd13509a17195e |
| roblox_recovery | 4.4.4 | 6ec5c11b-00bc-4826-a134-2d79e64b496f | bc9a239a0c2a7b99d5cd13509a17195e |
| adobe_register | 4.4.4 | 6ec5c11b-00bc-4826-a134-2d79e64b496f | bc9a239a0c2a7b99d5cd13509a17195e |

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
