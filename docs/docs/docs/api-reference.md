# API Reference — Send-Time Optimization

## Overview

The Send-Time Optimization API allows you to enable and configure STO programmatically when creating or updating campaigns. STO settings are passed as a nested object on the campaign resource.

Base URL: `https://api.[platform].com/v1`

Authentication: Bearer token — include your API key in the `Authorization` header.

---

## Campaign Object — STO Fields

When creating or updating a campaign, include the `send_time_optimization` object to configure STO.

```json
"send_time_optimization": {
  "enabled": true,
  "window_hours": 12,
  "fallback_time": "2024-10-15T09:00:00Z"
}
