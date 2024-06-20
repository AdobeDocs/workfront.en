---
content-type: api
navigation-topic: api-navigation-topic
title: Specify an API Version in your integrations
description: Specify an API Version in your integrations
author: Becky
feature: Workfront API
role: Developer
exl-id: 2971749d-1d34-42a4-9eda-411aa8c3a2ab
---
# Specify an API version in your integrations

All Adobe Workfront URIs should reference a specific version of the API after the "attask/api" portion of the URI. The following example calls Version 15.0:

`attask/api/v15.0/<objectName>/<objectId>`

 Please ensure all your integrations call currently-supported Workfront APIs.

## Release and Deprecation Schedule of Workfront APIs

New versions of the API are released regularly, usually twice a year. Each version is supported for three years after its release date, with an additional year in a deprecated state where the version is available but not supported.

For more information on the release cadence and deprecation schedule of Workfront APIs, see [API versioning and support schedule](../../wf-api/api/api-version-support-schedule.md).

>[!IMPORTANT]
>
>* The default version of the API is set to the most recent version. Any API call without the version specified will use the default version. Each time Workfront releases a new version of the API, the default version will be updated to the latest version. **Therefore, after a new version of the Workfront API is released, any API calls that use the default version should be checked to make sure that the functionality is still supported.**
>
>* If your organization is currently using the Default API, your Workfront administrator has received an Announcement Center message with further instructions regarding the Default API. 
>
>To see the most recent version of the API,  see [API versioning and support schedule](../../wf-api/api/api-version-support-schedule.md). 


## Determining the API Version You Are Using

You can determine the version of the API you are using by checking the URI of an HTTP request sent to the Workfront API. The following example shows a Workfront request URI that specifies Version 15 of the API:

`https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5` 

If a URI does not specify a version, then it is using the Default Version of the API, as shown in the following example:

`https://<domainname>.my.workfront.com/attask/api/proj/4c7c08b20000002de5ca1ebc19edf2d5`

>[!IMPORTANT]
>
> Integrations that do not specify a version of the API in the URI are automatically routed to the Default Version of the API. 

## Updating Integrations to Use Supported API Versions

As you build or maintain Workfront integrations you should include a method for dynamically updating the API version and other properties subject to change (such as your API key).

To make updating integrations more efficient, you should consider the following suggestions for recording integration values:

* Store values subject to future changes in a properties file you keep updated
* Create a web service to manage properties in real time
* Store property values in a data store that your application can read

Designing your Workfront integrations with this in mind alleviates the need for extensive development work when those values inevitably change.
