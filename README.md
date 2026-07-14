# Arkose Labs API Tracker

Automated tracker for Arkose Labs `api.js` (used in Roblox, X, Uber, etc.).

## Current Versions

| Service | Version | Build ID | Enforcement Hash |
| --- | --- | --- | --- |
| roblox_register | 4.4.3 | e9a6fac9-ac9c-4993-a3a4-9a12ff592f59 | 32b1dd37782844af9863aff2c72ac984 |
| roblox_login | 4.4.3 | e9a6fac9-ac9c-4993-a3a4-9a12ff592f59 | 32b1dd37782844af9863aff2c72ac984 |
| match_login | 4.4.3 | e9a6fac9-ac9c-4993-a3a4-9a12ff592f59 | 32b1dd37782844af9863aff2c72ac984 |
| uber_login | 4.4.3 | e9a6fac9-ac9c-4993-a3a4-9a12ff592f59 | 32b1dd37782844af9863aff2c72ac984 |
| snapchat_register | 4.4.2 | 24a782f4-d402-40a7-afb8-43f40d591997 | 162a14c47922edcced45ca4d9b28e5d5 |
| x_register | 4.4.3 | e9a6fac9-ac9c-4993-a3a4-9a12ff592f59 | 32b1dd37782844af9863aff2c72ac984 |
| roblox_join | 4.4.3 | e9a6fac9-ac9c-4993-a3a4-9a12ff592f59 | 32b1dd37782844af9863aff2c72ac984 |
| roblox_recovery | 4.4.3 | e9a6fac9-ac9c-4993-a3a4-9a12ff592f59 | 32b1dd37782844af9863aff2c72ac984 |
| adobe_register | 4.4.3 | e9a6fac9-ac9c-4993-a3a4-9a12ff592f59 | 32b1dd37782844af9863aff2c72ac984 |

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
