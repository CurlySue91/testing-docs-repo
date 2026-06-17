# Send-Time Optimization

## Overview

Send-Time Optimization (STO) automatically determines the best time to deliver an email to each individual recipient, based on their historical engagement patterns. Instead of sending your campaign to your entire list at once, STO staggers delivery across a window you define so each contact receives the email when they're most likely to open it.

## How It Works

STO analyzes each contact's past open and click activity to predict their peak engagement window. When you enable STO on a campaign, the platform:

1. Scores each recipient against their engagement history.
2. Queues delivery within your chosen send window (up to 24 hours).
3. Falls back to the campaign's scheduled send time for contacts with insufficient history.

A contact needs at least **5 prior interactions** before STO generates a personalized send time. New contacts receive the campaign at the start of the send window.

## Enabling Send-Time Optimization

### From the Campaign Editor

1. Open your campaign in the editor.
2. Navigate to **Schedule & Send**.
3. Toggle **Send-Time Optimization** on.
4. Set your **Send Window** — the maximum number of hours over which delivery can be staggered (1–24 hours).
5. Choose a **Fallback Time** for contacts with no engagement history.
6. Review the estimated delivery spread in the preview chart.
7. Save or schedule your campaign.

### Requirements

- STO is available on [Plan Name] and above.
- Your account must have at least 30 days of engagement data.
- STO cannot be used with transactional or triggered emails.

## Send Window

The send window controls how long STO can stagger delivery after the campaign start time.

| Window | Best for |
|--------|----------|
| 1–4 hours | Time-sensitive promotions |
| 8–12 hours | Standard newsletters |
| 24 hours | Evergreen content with no urgency |

Choosing a longer window generally improves open rates but delays delivery for some recipients.

## Reporting

After your campaign sends, the **STO Performance** panel in the campaign report shows:

- **Optimized sends** — number of contacts who received a personalized send time.
- **Fallback sends** — contacts sent at the fallback time due to insufficient data.
- **Lift** — estimated open-rate improvement compared to a non-optimized send.

> **Note:** Lift is an estimate based on historical baseline comparisons and should be used as a directional indicator, not an absolute metric.

## Limitations

- STO cannot be combined with **A/B send-time tests**.
- Delivery is not guaranteed to fall exactly at the predicted time; the platform schedules within a ±15-minute window.
- STO data is per-account and does not transfer if a contact is merged or migrated.

## FAQ

**Can I turn off STO after a campaign is scheduled?**
Yes, up until the campaign start time. Once delivery begins, STO cannot be disabled for that send.

**Does STO work with RSS or automated campaigns?**
No. STO is currently supported only on one-time broadcast campaigns.

**What happens if a contact's predicted time falls outside my send window?**
The contact receives the email at the end of the send window.
