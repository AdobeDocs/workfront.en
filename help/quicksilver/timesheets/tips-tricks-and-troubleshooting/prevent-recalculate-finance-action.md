---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Prevent the Recalculate Finances action from affecting historic hours when rates change
description: You need to update the hourly cost for a user or job role (due to a raise or another circumstance), but you do not want this change to affect hours that have previously been logged on projects or you want it to affect only a portion of historical hours.
author: Lisa
feature: Timesheets
exl-id: 29d3124b-cf7a-4a47-95c4-cd5379489810
---
# Prevent the Recalculate Finances action from affecting historic hours when rates change

## Problem

You need to update the hourly cost for a user or job role (due to a raise or another circumstance), but you do not want this change to affect hours that have previously been logged on projects or you want it to affect only a portion of historical hours.

## Solution

Add the hours that you do not want changed to a Billing Record on the project and set the status of the billing record to Billed.&nbsp; This locks in the old rate and will be ignored by the Recalculate Finances action.&nbsp; Any hours that don't belong to a Billed billing record are calculated at the new rate. For more information, see [Recalculate project finances](../../manage-work/projects/project-finances/recalculate-project-finances.md).
