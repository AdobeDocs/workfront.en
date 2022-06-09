---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Duplicates returned during a large paginated search
description: When performing a large paginated search in the API for an object, the customer is receiving duplicate entries and missing records.
feature: Workfront API
---

# Duplicates returned during a large paginated search

## Problem

When performing a large paginated search in the API for an object, the customer is receiving duplicate entries and missing records.

## Solution

When the order is not formally defined, we rely on the order of the rows returned by the Oracle database, which doesn't guarantee any deterministic ordering. For instance, two consecutive calls with the same query might return rows in a different order. Similarly, when doing paging, the rows may randomly get assigned to different "pages," leading to duplicates. The simplest solution can be adding sorting by ID, something like 

```
&ID_Sort=asc
```

.
