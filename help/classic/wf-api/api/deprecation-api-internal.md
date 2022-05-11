---
filename: deprecation-api-internal
content-type: api
navigation-topic: api-navigation-topic
title: Deprecation of API-Internal
description: API-Internal is a version of the Adobe Workfront API that is unsupported due to its design and purpose. Although it contains the most recent updates to the Workfront API, it is subject to change without notice and therefore should be used with caution in production integrations. Workfront strongly recommends updating all API-Internal integrations to a versioned API.
---

# Deprecation of API-Internal

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

API-Internal is a version of the Adobe Workfront API that is unsupported due to its design and purpose. Although it contains the most recent updates to the Workfront API, it is subject to change without notice and therefore should be used with caution in production integrations. Workfront strongly recommends updating all API-Internal integrations to a versioned API.&nbsp;

To learn more about supported versions of the Workfront API, see [API versioning and support schedule](../../wf-api/api/api-version-support-schedule.md).

**Using API-Unsupported**

If your integrations require functionality that is not available in a versioned API, Workfront recommends using API-Unsupported. Similar to API-Internal, API-Unsupported is not supported. API-Unsupported also includes the most recent changes to the Workfront API and is subject to change without notice. Workfront encourages you to use API-Unsupported in your test environment where you can explore new functionality and ensure the API is free of bugs.

**Determining the API Version You are Using**

You can determine the version of the API your integrations use by using REST to construct a URI that sends a call over HTTPS to Workfront and then returns a JSON response.

<!--WRITER
```The following example shows a URI that calls API-Internal:``` 
<pre>https://<domainname>.my.workfront.com/attask/api/<strong>api-internal</strong><span style="font-weight: 400;">/proj/4c70…</span></pre>```The following example shows URI that calls API-Unsupported:``` 
<pre>https://<domainname>.my.workfront.com/attask/api/<strong>api-unsupported</strong><span style="font-weight: 400;">/proj/4c70...</span></pre>```The following example shows a URI that calls Version 7.0 of the API:``` 
<pre>https://<domainname>.my.workfront.com/attask/api/<strong>v7.0</strong><span style="font-weight: 400;">/proj/4c70…</span></pre>
-->
