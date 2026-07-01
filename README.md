# Arkose Labs API Tracker

Automated tracker for Arkose Labs `api.js` (used in Roblox, X, Uber, etc.).

## Current Versions

| Service | Version | Build ID | Enforcement Hash |
| --- | --- | --- | --- |
| roblox_register | 4.4.1 | f8919076-4cf3-4646-9ff8-9deb47829748 | b7ecbe81b66d4f7ef96f3ba13802c8ba |
| roblox_login | 4.4.1 | f8919076-4cf3-4646-9ff8-9deb47829748 | b7ecbe81b66d4f7ef96f3ba13802c8ba |
| match_login | 4.4.1 | f8919076-4cf3-4646-9ff8-9deb47829748 | b7ecbe81b66d4f7ef96f3ba13802c8ba |
| uber_login | 4.4.1 | f8919076-4cf3-4646-9ff8-9deb47829748 | b7ecbe81b66d4f7ef96f3ba13802c8ba |
| snapchat_register | 4.4.1 | f8919076-4cf3-4646-9ff8-9deb47829748 | b7ecbe81b66d4f7ef96f3ba13802c8ba |
| x_register | 4.4.1 | f8919076-4cf3-4646-9ff8-9deb47829748 | b7ecbe81b66d4f7ef96f3ba13802c8ba |
| roblox_join | 4.4.1 | f8919076-4cf3-4646-9ff8-9deb47829748 | b7ecbe81b66d4f7ef96f3ba13802c8ba |
| roblox_recovery | 4.4.1 | f8919076-4cf3-4646-9ff8-9deb47829748 | b7ecbe81b66d4f7ef96f3ba13802c8ba |
| adobe_register | 4.4.1 | f8919076-4cf3-4646-9ff8-9deb47829748 | b7ecbe81b66d4f7ef96f3ba13802c8ba |

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
