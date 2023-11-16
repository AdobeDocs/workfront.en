---
content-type: api
navigation-topic: wf-api
title: Get users available time API
description: Get users available time API
author: Becky
feature: Workfront API
role: Developer
exl-id: fa37920a-c08b-4af3-9896-7e4044834860
---
# Users available time API

**URI: attask/api/v15.0/user/getUsersAvailableTime**

The users available time endpoint retrieves data on the user's available time. This allows integrations for aggregation of data according to user attributes and time intervals. 

## Example request

`curl -XPUT /attask/api/v15.0/user/getUsersAvailableTime`

## Request parameters

* **userIDs**: array of strings. Required. Example: `"61a9cc0500002f9fdaa7a6f824f557e1"`.
 
* **fromDate**: datetime. string. Required. Example:  `"2022-07-10T00:00:00"`.

* **toDate**: datetime. string. Required. Example `"2022-07-20T23:59:59"`.

## Example response:

```
{
    "data": {
        "result": {
            "PAVL": {
                "61a9cc0500002f9fdaa7a6f824f557e1": [
                    0.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    0.0,
                    0.0,
                    480.0,
                    480.0,
                    480.0
                ]
            },
            "AVL": {
                "61a9cc0500002f9fdaa7a6f824f557e1": [
                    0.0,
                    480.0,
                    480.0,
                    480.0,
                    480.0,
                    0.0,
                    480.0,
                    0.0,
                    480.0,
                    480.0,
                    480.0
                ]
            }
        }
    }
}

```

## Response parameters

* **AVL**: Actual available hours. Array of numbers. 
* **PAVL**: Pure available hours for scheduling that does not include non-working days or user time off. String.
