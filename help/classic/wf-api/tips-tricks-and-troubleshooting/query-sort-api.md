---
filename: query-sort-api
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Sorting query results in the API
description: You can sort your results by any field if you append the following to your API call - EDIT ME.
---

# Sorting query results in the API

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

You can sort your results by any field if you append the following to your API call:

```
&entryDate_Sort=asc
```

For example, if you want to sort by task Planned Start Date, remove&nbsp;

```
entryDate
```

and replace it with&nbsp;

```
plannedCompletionDate
```

.

This works for most fields in Adobe Workfront.
