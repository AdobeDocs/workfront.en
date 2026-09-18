---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Options configuration for OPTASK copyIssue
description: An explanation of the integer values expected by the copyIssue endpoint.
author: Becky
feature: Workfront API
role: Developer
exl-id: a2b8ef01-1c14-47a5-8b0a-550b17b526ff
TQID: https://experienceleague.adobe.com/9cDJFoKl6zqpaAvqzpGqzflcbGZNrAWvEnUAFuqD-Rc
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
# Options configuration for OPTASK copyIssue


One of the properties for a copyIssue API call is a field called `options`. This field expects an integer.

To include one of the following options, enter the matching integer. To include more than one option, enter the sum of the matching integers.

| option | value* |
|---|---|
| Clear assignments | 2 |
| Clear progress | 4 |
| Clear documents | 128 |
| Clear updates | 65536 |
| Clear permissions | 524288 |
| Clear custom data | 1048576 |

*All values are powers of 2.

Examples:

* To clear progress when you copy the issue, enter an `options` value of `4`. 

* To clear both progress and documents, enter an `options` value of `132`. 

  Clear progress = 4

  Clear documents = 128

  4 + 128 = 132
