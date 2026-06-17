# Release Notes — Send-Time Optimization

## v1.2.0 — [Month YYYY]

### What's New

- **Extended send window** — The maximum send window has been increased from 12 hours to 24 hours.
- **Fallback time control** — You can now specify a custom fallback time instead of defaulting to the campaign start time.
- **STO Performance panel** — A dedicated reporting panel now surfaces optimized vs. fallback send counts and estimated lift.

### Improvements

- STO eligibility now recalculates up to 1 hour before campaign start, incorporating the most recent engagement events.
- The send window selector in the campaign editor has been redesigned for clarity.

### Bug Fixes

- Fixed an issue where the STO toggle reset to off when switching between desktop and mobile preview modes.
- Corrected a rare edge case where contacts with exactly 5 interactions were excluded from optimization.

---

## v1.1.0 — [Month YYYY]

### What's New

- **STO is now generally available** to all accounts on [Plan Name] and above.
- Added a delivery spread preview chart in the **Schedule & Send** step.

### Improvements

- Reduced the minimum engagement history requirement from 10 interactions to 5.
- Improved prediction accuracy for contacts with irregular open patterns.

### Bug Fixes

- Fixed a display bug where the STO toggle appeared enabled on transactional email templates (STO is not supported for transactional emails).
- Resolved a timezone-handling issue affecting contacts in UTC+12 and UTC−12.

---

## v1.0.0 — [Month YYYY] — Beta

### Initial Release

Send-Time Optimization launched in closed beta. Core capabilities:

- Per-contact send-time prediction based on historical open and click data.
- Configurable send window of 1–12 hours.
- Fallback to campaign start time for contacts with no history.
- Available to beta accounts on invitation only.
