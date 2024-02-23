---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Duplicates returned during a large paginated search
description: Duplicates returned during a large paginated search
author: Becky
feature: Workfront API
role: Developer
exl-id: 0359d6ba-b219-4d11-9f6f-cec2ff9ee058
---

# Duplicates returned during a large paginated search

## Problem

When performing a large paginated search in the API for an object, the customer is receiving duplicate entries and missing records.

## Solution

When the order is not formally defined, we rely on the order of the rows returned by the Oracle database, which doesn't guarantee any deterministic ordering. For instance, two consecutive calls with the same query might return rows in a different order. Similarly, when doing paging, the rows may randomly get assigned to different "pages," leading to duplicates. The simplest solution can be adding sorting by ID:

```
&ID_Sort=asc
```

