---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Connect [!DNL Adobe Workfront Fusion] to a web service that uses API token authorization
description: Some services do not allow integration solutions such as [!DNL Adobe Workfront Fusion] to create an app that you can easily use in your scenario.
author: Becky
feature: Workfront Fusion
exl-id: 0feb745a-1ee0-4b29-92ab-14c12a8647d4
---
# Connect [!DNL Adobe Workfront Fusion] to a web service that uses API token authorization

Some services do not allow integration solutions such as [!DNL Adobe Workfront Fusion] to create an app that you can easily use in your scenario.

There is a workaround to this situation. You can connect the desired service (app) to [!DNL Workfront Fusion] using [!DNL Workfront Fusion]'s [!UICONTROL HTTP] module.

This article explains how to connect almost any web service to [!DNL Workfront Fusion] using an API Key/API token.

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Current license requirement: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy license requirement: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Current product requirement: If you have the [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article. [!DNL Workfront Fusion] is included in the [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>Or</p>
   <p>Legacy product requirement: Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Connect to a web service that uses an API token

The procedure of connecting the service via an API token is similar for most web services.

1. Create an application on the web service's website, as explained in the section [Create a new application and obtain the API token](#create-a-new-application-and-obtain-the-api-token) in this article.
1. Obtain the API Key or API token.
1. Add [!DNL Workfront Fusion]'s [!UICONTROL HTTP] > [!UICONTROL Make a Request] module to your scenario.
1. Set up the module according to the web service's API documentation and running the scenario, as explained in the section [Set up the [!UICONTROL HTTP] module](#set-up-the-http-module) in this article.

>[!NOTE]
>
>We will use the [!DNL Pushover] notification service as an example throughout this article.

## Create a new application and obtain the API token 

>[!NOTE]
>
>There are many different ways that web services create and distribute API keys or API tokens. For instructions on obtaining an API key and token for your desired web service, go to the service's website and search for "API key" or "API token."
>
>We are including instructions for obtaining a Pushover API key only as an example of what you might find.

1. Log in to your [!DNL Pushover] account.
1. Click **[!UICONTROL Create an Application/API Token]** at the bottom of the page.
1. Fill in the Application Information and click **[!UICONTROL Create an Application]**.
1. Store the provided API token in a safe place. You will need it for the [!DNL Workfront Fusion] [!UICONTROL HTTP] >[!UICONTROL Make a Request] module to connect to the desired web service ([!DNL Pushover], in this case).

## Set up the [!UICONTROL HTTP] module 

To connect a web service to your [!DNL Workfront Fusion] scenario, you need to use the [!UICONTROL HTTP] >[!UICONTROL Make a request] module in the scenario and set up the module according to the web service's API documentation.

1. Add the [!UICONTROL HTTP] >[!UICONTROL Make a Request] module to your scenario.
1. To push a message using [!DNL Workfront Fusion], set up the HTTP module as follows.

   >[!NOTE]
   >
   >These module settings correspond to the [!DNL Pushover] web service API documentation. Settings may be different for other web services. For example, the API token may be inserted to the [!UICONTROL Header] and not to the [!UICONTROL Body] field.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL URL]</td> 
      <td> <p><code>https://api.pushover.net/1/messages.json</code> </p> <p>The URL field contains the endpoint that you can find in the web service's API documentation.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Method]</td> 
      <td> <p><code>[!DNL POST]</code> </p> <p>The used method depends on the corresponding endpoint. The Pushover endpoint for pushing messages uses the POST method.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Headers]</p> </td> 
      <td> <p>Some web services may use Headers to specify the API token authentication or other parameters. This is not the case in our example as the Pushover's endpoint for pushing messages uses Body (see below) for all request types.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Query String]</p> </td> 
      <td> <p>Some web services may use a Query String to specify other parameters. This is not the case in our example as the [!DNL Pushover] web service uses [!UICONTROL Body] (see below) for all request types.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Body Type]</p> </td> 
      <td> <p><code>Raw</code> </p> <p>This setting allows you to select the JSON content type in the [!UICONTROL Content Type] field below.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Content Type]</p> </td> 
      <td> <p><code>JSON (application/json)</code> </p> <p>JSON is the required content type by the [!UICONTROL Pushover] app. This may differ from other web services.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Request Content]</p> </td> 
      <td> <p>Enter the [!UICONTROL Body] request content in the JSON format. You can use the [!UICONTROL JSON] > [!UICONTROL Create JSON] module as explained in <a href="#json-body-mapped-using-the-json-create-json-module" class="MCXref xref">JSON Body Mapped Using the [!UICONTROL JSON] > [!UICONTROL Create JSON] module</a> in this article. Or you can enter the JSON content manually, as explained in <a href="#json-body-entered-manually" class="MCXref xref">JSON Body Entered Manually</a> in this article.</p> <p>See the web service's API documentation for the required parameters for that web service.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## JSON Body Entered Manually

Specify parameters and values in the JSON format.

>[!INFO]
>
>**Example:**
>
>```
>{"user":"12345c2ecu1hq42ypqzhswbyam34",
>
>"token":"123459evz8aepwtxydndydgyumbfx",
>
>"message":"Hello World!",
>
>"title":"The Push Notification"}
>```

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL user]</p> </td> 
   <td> <p>Your USER_KEY. This can be found in your [!DNL Pushover] dashboard.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL token] </td> 
   <td> <p>Your API token/API Key that was generated you created your [!DNL Pushover] app.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL message] </td> 
   <td> <p>The text content of the push notification that is sent to the device(s).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL title] </td> 
   <td> <p>(Optional) Your message's title. If no value is entered, your app's name is used. </p> </td> 
  </tr> 
 </tbody> 
</table>

## JSON Body Mapped Using the [!UICONTROL JSON] >[!UICONTROL Create JSON] module

The [!UICONTROL Create JSON] module makes the specifying JSON easier. It also gives you the possibility to define values dynamically.

For more information about the JSON modules, see [JSON modules](../../workfront-fusion/apps-and-their-modules/json-modules.md).

1. Enter or map the values you want to create JSON from.

   ![](assets/json-values-350x288.png)

1. Connect the [!UICONTROL JSON] > [!UICONTROL Create JSON] module to the HTTP > Make a Request module.
1. Map the JSON string from the [!UICONTROL Create JSON] module to the [!UICONTROL Request content] field in the [!UICONTROL HTTP] >[!UICONTROL Make a Request] module.

   Now when you run the scenario, the push notification is sent to the device that has been registered in your [!DNL Pushover] account.
