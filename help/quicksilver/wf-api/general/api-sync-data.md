---
content-type: api
keywords: API,data,sync,journal,entry,object
navigation-topic: general-api
title: Use the API to sync data for programs and services
description: Use the API to sync data for programs and services
author: Becky
feature: Workfront API
role: Developer
exl-id: 1d0583fc-1573-4279-a3fa-a912d9a4213c
---

# Using the API to sync data for programs and services

These are some common ways for you to utilize the API&nbsp;to sync data for programs and services.

## Near real-time updates

Adobe Workfront uses "Event Subscriptions" (also commonly referred to as webhooks) to send near real-time updates about supported objects and actions, via the API, to your desired endpoint(s). You can expect to receive an update regarding new objects and actions within 5 seconds, but on average updates arrive in approximately 1 second. For additional information about what type of objects are supported, what types of actions are supported, technical details, and examples for how to set up event subscriptions see [Event Subscription API](../../wf-api/general/event-subs-api.md) and [Event Subscription delivery requirements](../../wf-api/general/setup-event-sub-endpoint.md).

## Batch updates

Batch updates are a way to configure your system for updates by making periodic requests to Workfront servers. There are a lot of ways to do this, but generally the process consists of having your service make a request to the Workfront API servers and searching for objects that have been created or modified since the last request call. For information about potential requests calls and helpful parameters please see the [GET Behavior](../../wf-api/general/api-basics.md#get-behavior) section from the [API basics](../../wf-api/general/api-basics.md) article.

As you are setting up your service for batch updates here are a few important things to keep in mind:

### Entry Dates

Entry dates are stored utilizing ISO 8601 formatting. This standard includes date, time, and timezone infromation.

**Example:** ISO 8601 date format

<!-- [Copy](javascript:void(0);) --> 
&nbsp;  
<pre><code>2020-05-18T17:00:00:000-0600</code></pre>&nbsp;

Both the date that an object is created and the last date that the object was modified are stored as "entryDate" and "lastUpdateDate", respectively. For in depth information about Workfront objects, their associated fields, and field names, please see the [API Explorer](../../wf-api/general/api-explorer.md). Notice that the entryDate for any given Workfront object doesn't change, where as the lastUpdatedDate changes each time the object is modified.

**Example:** GET reqeust for an issue object, utilizing the **lastUpdateDate** field. This request would return all issues updated since that specified date.

<!-- [Copy](javascript:void(0);) --> 
&nbsp;  

```
GET
https://<domain>.my.workfront.com/attask/api/v15.0/OPTASK/search?fields=ID,name,lastUpdateDate&$$LIMIT=200&lastUpdateDate=2020-05-13T18:18:37.255Z&lastUpdateDate_Mod=gte
```

### Journal Entry Object

If you are interested in obtaining changes regarding a specific field on an object then you can query the "Journal Entry" object. The Workfront Journal Entry object can be set up to log information about specific object fields any time those fields are modified, see [Configure system updates](../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md) for additional details.

When a field is setup to be logged as a part of the Journal Entry object a corresponding Journal Entry will be created every time that field is modified. Then, you can query the Journal Entry object using an API&nbsp;call similar to the following:

<!-- [Copy](javascript:void(0);) --> 

<pre><code>GET https://&#123;&#123;domain&#125;&#125;.my.workfront.com/attask/api/v15.0/JRNLE/search?fields=newTextVal,oldTextVal,newDateVal,oldDateVal,newNumberVal,oldNumberVal,entryDate,objObjCode,objID,fieldName&fieldName=name&objObjCode=OPTASK&entryDate=2020-05-13T18:18:37.255Z&entryDate_Mod=gte</code></pre>

>[!NOTE]
>
>"entryDate" is used to look at a journal entry of a change, as opposed to looking at the changed object, itself.
