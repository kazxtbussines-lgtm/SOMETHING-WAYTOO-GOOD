# Arkose Labs API Tracker

Automated tracker for Arkose Labs `api.js` (used in Roblox, X, Uber, etc.).

## Current Versions

| Service | Version | Build ID | Enforcement Hash |
| --- | --- | --- | --- |
| roblox_register | 4.4.2 | e7ef722e-2317-446b-a279-8d76bfaf699c | 504897d1cd342e063d4f67d90600cf04 |
| roblox_login | 4.4.2 | e7ef722e-2317-446b-a279-8d76bfaf699c | 504897d1cd342e063d4f67d90600cf04 |
| match_login | 4.4.2 | e7ef722e-2317-446b-a279-8d76bfaf699c | 504897d1cd342e063d4f67d90600cf04 |
| uber_login | 4.4.2 | e7ef722e-2317-446b-a279-8d76bfaf699c | 504897d1cd342e063d4f67d90600cf04 |
| snapchat_register | 4.4.2 | e7ef722e-2317-446b-a279-8d76bfaf699c | 504897d1cd342e063d4f67d90600cf04 |
| x_register | 4.4.2 | e7ef722e-2317-446b-a279-8d76bfaf699c | 504897d1cd342e063d4f67d90600cf04 |
| roblox_join | 4.4.2 | e7ef722e-2317-446b-a279-8d76bfaf699c | 504897d1cd342e063d4f67d90600cf04 |
| roblox_recovery | 4.4.2 | e7ef722e-2317-446b-a279-8d76bfaf699c | 504897d1cd342e063d4f67d90600cf04 |
| adobe_register | 4.4.2 | e7ef722e-2317-446b-a279-8d76bfaf699c | 504897d1cd342e063d4f67d90600cf04 |

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
