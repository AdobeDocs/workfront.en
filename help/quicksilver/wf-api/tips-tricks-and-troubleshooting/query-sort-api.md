---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Sorting query results in the API
description: Sorting query results in the API
author: Becky
feature: Workfront API
role: Developer
exl-id: f001adb8-6295-4646-b9f1-78244a8c44a6
---

# Sorting query results in the API

You can sort your results by any field if you append the following to your API call:

```
&entryDate_Sort=asc
```

For example, if you want to sort by task Planned Start Date, remove `entryDate` and replace it with `plannedCompletionDate`.

This works for most fields in Adobe Workfront.
