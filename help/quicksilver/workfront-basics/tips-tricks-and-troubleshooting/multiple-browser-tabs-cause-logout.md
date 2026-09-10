---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Multiple browser tabs cause Workfront to log out
description: When a user has multiple browser tabs open, Workfront may automatically log out.
feature: Get Started with Workfront
author: Becky
exl-id: 1cc8bf6c-0eda-41ef-8efd-bba3a5f33b08
TQID: https://experienceleague.adobe.com/Zof7zbTOm-w1vyBTchiXJv2QrNYbOxw9O4DYIjYQ6Ss
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
---
# Multiple browser tabs cause Workfront to log out

## Problem

When a user has multiple browser tabs open, and clicks into a tab that has been inactive for some time, the tab session has expired. The user cannot see the page they had open, and instead sees the following message:

```
Tab session expired
This tab session has been halted due to inactivity. Refresh the tab to continue where you left off.
```

## Reason

This behavior is due to Policy-Based Authentication (PBA), a security measure configured by your organization. When a tab has been inactive for more than the time limit set in your organization's PBA configuration, the tab session expires.

## Solution

The solution depends on whether you have been active in another tab that is logged into Workfront.

* If you have an active Workfront tab open, reload the expired tab. It will return to the page you had open before it expired.

* If you do not have an active Workfront tab open, log into Workfront again.
