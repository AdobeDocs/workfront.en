---
content-type: api
navigation-topic: api-navigation-topic
title: Update integrations that use default API versioning
description: Update integrations that use default API versioning
author: John
feature: Workfront API
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
---
# Update integrations that use default API versioning

<!-- This article is going to need a complete revamp or to be removed-->

We release new versions of the Adobe Workfront API on a biannual basis. Each version is supported for three years after its release, with an additional year in a deprecated state where the version is available but not supported.

Integrations that do not specify a version of the API in the URI are automatically routed to Default, which has been deprecated. In order for your Workfront integrations to be valid, you must specify a supported API version in your Workfront API requests.

To learn about specifying a version in your API requests, see [Specify an API Version in your integrations](../../wf-api/api/specify-api-version-integrations.md).

## Understanding the Default Version of the API

The original intent of the "default API", or Default, was to map it to the latest version of the Workfront API. This would allow customers with basic integrations that called Default to never have to update their API requests. 

In 2011, Workfront released Version 3.0 of the API. Default was automatically moved to Version 3.0, which broke many customer integrations that were too complex to utilize Version 3.0 without being updated. As a result, Workfront rolled back this change and left the default version at Version 2.

Unfortunately, this topic was never revisited, and now as we plan to substantially increase API functionality, we are forced to jettison older versions of our API including Default. Rather than update Default, which would undoubtedly break more integrations, we are removing the concept of a default version entirely. This is to encourage our customers to use stable versions of our APIs and to maintain their integrations on a cycle of, at most, three years.  

## Deprecating Default

In an effort to improve the Workfront API, we are in the process of removing older API versions that have exceeded our support window of three years. One of these versions is Version 2, to which Default is mapped. This version was released in 2010, and much of the logic supported in the Attask/Workfront application at that time either no longer exists or has substantially changed.

We deprecated Default in July 2017, and we will no longer designate a specific version of the API to be the default version. Instead, all Workfront API requests must specify a specific API version.

>[!IMPORTANT]
>
> By July 1, 2018 all of your Workfront integrations that use Default must be updated to call a specific supported API version. After that date, all of your Workfront API requests used by integrations that do not specify a version will fail.

To learn about the Workfront deprecation cadence, see [API versioning and support schedule](../../wf-api/api/api-version-support-schedule.md).

## Updating Your Integrations to Supported API Versions

If your Workfront API requests do not specify a version, then they are using Default. You must update your API requests to specify a supported version of the API, preferably to the latest supported API.

For example, the following Workfront API request does not specify an API version:

`https://davidwhite.my.workfront.com/attask/api/project/metadata`

When this request is made, you receive a response with JSON encoded text that specifies data from your Workfront instance. Because no API version is specified in this URI, the call goes to Default. 

To turn a Default API request into a versioned API request, simply call a supported API version. For example, the following URI requests Version 9:

`https://davidwhite.my.workfront.com/attask/api/`**v15.0**`/project/metadata`

When updating your Workfront API requests, you can specify any supported version of our API. To learn more about referencing a specific API, see [Specify an API Version in your integrations](../../wf-api/api/specify-api-version-integrations.md).

To ensure the maximum support window, you should call the latest version (Version 9). You can find a list of supported APIs in [API versioning and support schedule](../../wf-api/api/api-version-support-schedule.md).

It is imperative that you update the integrations you have that use Default. If you currently have integrations that do not specify a version, you might receive notification from your Workfront salesperson, customer success manager, or support representative, or an announcement center message.

As soon as possible, please ensure your integrations are updated to call a supported version of our API. 
