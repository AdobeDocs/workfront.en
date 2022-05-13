---
filename: duplicates-paginated-search
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Duplicates returned during a large paginated search
description: When performing a large paginated search in the API for an object, the customer is receiving duplicate entries and missing records.
---

# Duplicates returned during a large paginated search

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

## Problem

When performing a large paginated search in the API for an object, the customer is receiving duplicate entries and missing records.

## Solution

When the order is not formally defined, we rely on the order of the rows returned by the Oracle database, which doesn't guarantee any deterministic ordering. For instance, two consecutive calls with the same query might return rows in a different order. Similarly, when doing paging, the rows may randomly get assigned to different "pages," leading to duplicates. The simplest solution can be adding sorting by ID, something like 

```
&ID_Sort=asc
```

.
