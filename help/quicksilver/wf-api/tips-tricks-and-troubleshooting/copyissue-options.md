---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: Options configuration for OPTASK copyIssue
description: An explanation of the integer values expected by the copyIssue endpoint.
author: Becky
feature: Workfront API
role: Developer
exl-id: a2b8ef01-1c14-47a5-8b0a-550b17b526ff
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
