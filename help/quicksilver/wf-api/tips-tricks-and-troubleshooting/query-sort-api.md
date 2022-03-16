---
filename: query-sort-api
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Sorting query results in the API
description: You can sort your results by any field if you append the following to your API call:
---

# Sorting query results in the API

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
