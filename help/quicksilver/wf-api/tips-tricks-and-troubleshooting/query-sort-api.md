---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Sorting query results in the API
description: Sorting query results in the API
author: Becky
feature: Workfront API
role: Developer
exl-id: f001adb8-6295-4646-b9f1-78244a8c44a6
TQID: https://experienceleague.adobe.com/r7PCHEpU413ajyML7-uzWdmXN11gylNHRU2q60J35Go
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
# Sorting query results in the API

You can sort your results by any field if you append the following to your API call:

```
&entryDate_Sort=asc
```

For example, if you want to sort by task Planned Completition Date, remove `entryDate` and replace it with `plannedCompletionDate`.

```
&plannedCompletionDate_Sort=asc
```

This works for most fields in Adobe Workfront.
