---
content-type: api
navigation-topic: api-navigation-topic
title: Update integrations that use default API versioning
description: Update integrations that use default API versioning
author: Becky
feature: Workfront API
role: Developer
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
---
# Update integrations that use default API versioning

We release new versions of the Adobe Workfront API on a biannual basis. Each version is supported for three years after its release, with an additional year in a deprecated state where the version is available but not supported.

Integrations that do not specify a version of the API in the URI are automatically routed to Default. If you want your API call to use a specific version of the API, you must specify that version in your Workfront API requests.

>[!NOTE]
>
>If your organization is currently using the Default API, your Workfront administrator has received an Announcement Center message with further instructions regarding the Default API.

To learn about specifying a version in your API requests, see [Specify an API Version in your integrations](../../wf-api/api/specify-api-version-integrations.md).

## Considerations when using the Default API

Consider the following when working with the Workfront Default API:

* The default version of the API the most recent version. Any API call without the version specified will use the default version. Each time Workfront releases a new version of the API, the default version will be updated to the latest version. **Therefore, after a new version of the Workfront API is released, any API calls that use the default version should be checked to make sure that the functionality is still supported**.
*  If your organization is currently using the prevoius deprecated Default API, your Workfront administrator has received an Announcement Center message with further instructions regarding the Default API. 

To see the most recent version of the API,  see [API versioning and support schedule](../../wf-api/api/api-version-support-schedule.md). 

## Updating Your Integrations to Supported API Versions

If your Workfront API requests do not specify a version, then they are using Default. We recommend your API requests to specify a supported version of the API, preferably to the latest supported API.

For example, the following Workfront API request does not specify an API version:

`https://davidwhite.my.workfront.com/attask/api/project/metadata`

When this request is made, you receive a response with JSON encoded text that specifies data from your Workfront instance. Because no API version is specified in this URI, the call goes to Default. 

To turn a Default API request into a versioned API request, simply call a supported API version. For example, the following URI requests Version 15:

`https://davidwhite.my.workfront.com/attask/api/`**v15.0**`/project/metadata`

When updating your Workfront API requests, you can specify any supported version of our API. To learn more about referencing a specific API, see [Specify an API Version in your integrations](../../wf-api/api/specify-api-version-integrations.md).

To ensure the maximum support window, you should call the latest version. You can find a list of supported APIs in [API versioning and support schedule](../../wf-api/api/api-version-support-schedule.md).

## History of the Default Version of the API

The original intent of the "default API", or Default, was to map it to the latest version of the Workfront API. This would allow customers with basic integrations that called Default to never have to update their API requests. 

In 2011, Workfront released Version 3.0 of the API. Default was automatically moved to Version 3.0, which broke many customer integrations that were too complex to utilize Version 3.0 without being updated. As a result, Workfront rolled back this change and left the default version at Version 2.

Since 2011, Workfront has substantially increased API functionality. Because of this, we have deprecated older versions of our API. In 2017, rather than update Default, we removed the concept of a default version entirely. This was to encourage our customers to use stable versions of our APIs and to maintain their integrations on a cycle of, at most, three years.  

Workfront is now reinstating the Default API version. The Default API is set to the most recent version of the Workfront API, and will be updated to the most recent version each time a new version is released.

