# UI Strings — Send-Time Optimization

This file contains all in-app microcopy for the Send-Time Optimization feature. Strings are grouped by surface. Use the **String ID** when referencing a string in code or translation files.

---

## Toggle & Section Header

| String ID | String | Notes |
|-----------|--------|-------|
| `sto.toggle.label` | Send-Time Optimization | Section header / toggle label |
| `sto.toggle.on` | On | Toggle state |
| `sto.toggle.off` | Off | Toggle state |
| `sto.section.description` | Deliver this campaign when each contact is most likely to engage, based on their past activity. | Subtitle below section header |

---

## Send Window Selector

| String ID | String | Notes |
|-----------|--------|-------|
| `sto.window.label` | Send window | Field label |
| `sto.window.unit` | hours | Unit label appended to numeric input |
| `sto.window.helper` | Emails will be staggered up to {n} hours after your scheduled send time. | Inline helper text; `{n}` = selected window value |
| `sto.window.error.required` | Please set a send window. | Validation error |
| `sto.window.error.out_of_range` | Send window must be between 1 and 24 hours. | Validation error |

---

## Fallback Time

| String ID | String | Notes |
|-----------|--------|-------|
| `sto.fallback.label` | Fallback send time | Field label |
| `sto.fallback.helper` | Used for contacts without enough history for a prediction. | Helper text below field |
| `sto.fallback.placeholder` | Same as campaign start time | Placeholder when no custom time is set |

---

## Tooltips

| String ID | String | Trigger element |
|-----------|--------|-----------------|
| `sto.tooltip.what_is_sto` | Send-Time Optimization schedules each email at the moment your contact is most likely to open it, based on their past engagement. | "?" icon next to section header |
| `sto.tooltip.window` | A longer window gives the algorithm more flexibility but delays delivery for some contacts. | "?" icon next to send window field |
| `sto.tooltip.lift` | Estimated lift is a directional indicator based on historical baseline comparisons. Actual results may vary. | "?" icon next to lift metric in reports |
| `sto.tooltip.fallback` | Contacts with fewer than 5 prior interactions will receive your email at this time instead. | "?" icon next to fallback time field |

---

## Eligibility & Upgrade Prompts

| String ID | String | Context |
|-----------|--------|---------|
| `sto.upsell.plan` | Send-Time Optimization is available on [Plan Name] and above. [Upgrade] | Shown when feature is locked by plan |
| `sto.upsell.data` | Your account needs at least 30 days of engagement data to use Send-Time Optimization. | Shown when account is too new |
| `sto.unavailable.campaign_type` | Send-Time Optimization isn't available for triggered or transactional emails. | Shown in unsupported campaign types |

---

## Delivery Preview

| String ID | String | Notes |
|-----------|--------|-------|
| `sto.preview.title` | Estimated delivery spread | Chart section header |
| `sto.preview.optimized` | {n} contacts will receive a personalized send time | `{n}` = estimated optimized count |
| `sto.preview.fallback` | {n} contacts will use the fallback time | `{n}` = estimated fallback count |
| `sto.preview.empty` | Schedule your campaign to see the estimated delivery spread. | Empty state before campaign is scheduled |

---

## Reporting Panel

| String ID | String | Notes |
|-----------|--------|-------|
| `sto.report.panel_title` | Send-Time Optimization Performance | Panel heading |
| `sto.report.optimized_sends` | Optimized sends | Metric label |
| `sto.report.fallback_sends` | Fallback sends | Metric label |
| `sto.report.lift` | Estimated lift | Metric label |
| `sto.report.lift_value` | +{n}% opens | `{n}` = lift percentage |
| `sto.report.empty` | STO report data will appear here once your campaign has finished sending. | Empty state before send completes |
| `sto.report.insufficient_data` | Not enough data to calculate lift for this campaign. | Shown when lift cannot be computed |

---

## Confirmation & Status Messages

| String ID | String | Context |
|-----------|--------|---------|
| `sto.status.scheduled` | Send-Time Optimization is active for this campaign. | Confirmation shown after scheduling |
| `sto.status.sending` | Send-Time Optimization is in progress. Delivery will complete by {time}. | Shown while campaign is sending; `{time}` = end of window |
| `sto.status.complete` | Send-Time Optimization is complete. | Shown after all sends are delivered |
| `sto.status.disabled_after_start` | STO settings cannot be changed once sending has begun. | Read-only notice after delivery starts |
