---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Duplicates returned during a large paginated search
description: Duplicates returned during a large paginated search
author: Becky
feature: Workfront API
role: Developer
exl-id: 0359d6ba-b219-4d11-9f6f-cec2ff9ee058
TQID: https://experienceleague.adobe.com/1FXTHSro-rlUVHaajM1monR2Y-sxVHN6KIviogoXqRc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
    internal-label: APIs
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
---
# Duplicates returned during a large paginated search

## Problem

When performing a large paginated search in the API for an object, the customer is receiving duplicate entries and missing records.

## Solution

When the order is not formally defined, we rely on the order of the rows returned by the Oracle database, which doesn't guarantee any deterministic ordering. For instance, two consecutive calls with the same query might return rows in a different order. Similarly, when doing paging, the rows may randomly get assigned to different "pages," leading to duplicates. The simplest solution can be adding sorting by ID:

```
&ID_Sort=asc
```

