---
filename: prevent-recalculate-finance-action
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Prevent the Recalculate Finances action from affecting historic hours when rates change
description: You need to update the hourly cost for a user or job role (due to a raise or another circumstance), but you do not want this change to affect hours that have previously been logged on projects or you want it to affect only a portion of historical hours.
---

# Prevent the Recalculate Finances action from affecting historic hours when rates change

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

## Problem

You need to update the hourly cost for a user or job role (due to a raise or another circumstance), but you do not want this change to affect hours that have previously been logged on projects or you want it to affect only a portion of historical hours.

## Solution

Add the hours that you do not want changed to a Billing Record on the project and set the status of the billing record to Billed.&nbsp; This locks in the old rate and will be ignored by the Recalculate Finances action.&nbsp; Any hours that don't belong to a Billed billing record are calculated at the new rate. For more information, see [Recalculate project finances](../../manage-work/projects/project-finances/recalculate-project-finances.md). 
