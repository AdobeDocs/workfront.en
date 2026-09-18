---
content-type: api
navigation-topic: api-navigation-topic
title: Deprecation of API-Internal
description: Deprecation of API-Internal
author: Becky
feature: Workfront API
role: Developer
exl-id: 45b42fe8-7ce3-441d-8fbc-b8db7f9b254e
TQID: https://experienceleague.adobe.com/LGyk8MIATMQj6JHqKmjkeL2pXW-b6xtxo2heMd4h0y4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
---
# Deprecation of API-Internal

API-Internal is a version of the Adobe Workfront API that is unsupported due to its design and purpose. Although it contains the most recent updates to the Workfront API, it is subject to change without notice and therefore should be used with caution in production integrations. Workfront strongly recommends updating all API-Internal integrations to a versioned API.

To learn more about supported versions of the Workfront API, see [API versioning and support schedule](../../wf-api/api/api-version-support-schedule.md).

**Using API-Unsupported**

If your integrations require functionality that is not available in a versioned API, Workfront recommends using API-Unsupported. Similar to API-Internal, API-Unsupported is not supported. API-Unsupported also includes the most recent changes to the Workfront API and is subject to change without notice. Workfront encourages you to use API-Unsupported in your test environment where you can explore new functionality and ensure the API is free of bugs.

**Determining the API Version You are Using**

You can determine the version of the API your integrations use by using REST to construct a URI that sends a call over HTTPS to Workfront and then returns a JSON response.

The following example shows a URI that calls API-Internal: 

```
https://<domainname>.my.workfront.com/attask/api/api-internal/proj/4c70…
```

The following example shows URI that calls API-Unsupported: 

```
https://<domainname>.my.workfront.com/attask/api-unsupported/proj/4c70...
```

>[!NOTE]
>
>API-Unsupported calls omit the `/api` section of the URL.

The following example shows a URI that calls Version 15.0 of the API: 

```
https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c70…
```
