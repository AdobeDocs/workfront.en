---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Multiple browser tabs cause Workfront to log out
description: When a user has multiple browser tabs open, Workfront may automatically log out.
feature: Get Started with Workfront
exl-id: 1cc8bf6c-0eda-41ef-8efd-bba3a5f33b08
---
# Multiple browser tabs cause Workfront to log out

>[!IMPORTANT]
>
>This issue is present only for organizations that have been onboarded to Adobe IMS.

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
