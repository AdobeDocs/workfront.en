---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Adobe Authenticator module
description: With the Adobe Authenticator module, you can connect to any Adobe product with an API, using a single connection.
author: Becky
feature: Workfront Fusion
---
# Adobe Authenticator modules

The Adobe Authenticator module allows you to connect to any Adobe API, using a single connection. This allows you to more easily connect to Adobe products that do not yet have a dedicated Fusion connector.

The advantage over the HTTP modules is that you can create a connection, as in a dedicated app.

To see a list of available Adobe APIs, see X. You may be able to use only the APIs to which you are assigned.

## Access requirements

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] plan</td>
      <td>
        <p>New: Any</p><p>Or</p><p>Current: [!UICONTROL Pro] or higher</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] license</td>
      <td>
        <p>New: Standard</p><p>Or</p><p>Current: [!UICONTROL Plan], [!UICONTROL Work]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] license</td>
      <td>
   <p>Current Fusion license requirement: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy Fusion license requirement: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">Product</td>
      <td>
   <p>New Workfront plan: If you have the [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Adobe Workfront] Plan, your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article. [!DNL Workfront Fusion] is included in the [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>Or</p>
   <p>Current Workfront plan: Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</p>
   </td>
    </tr>
  </tbody>
</table>

## Prerequisites

* You must have access to the Adobe product that you want the module to connect to.
* You must have access to the Adobe Developer Console.
* You must have a project on the Adobe Developer Console that includes the API that you want the module to connect to. You can:

   * Create a new project with the API.

       Or
   * Add the API to an existing project.

  For information on creating or adding an API to a project on the Adobe Developer Console, see [Create a project](https://developer.adobe.com/dep/guides/dev-console/create-project/) in the Adobe documentation.

## Create a connection

An Adobe Authenticator connection connects to a single project on the Adobe Developer Console. To use the same connection for more than one Adobe API, add the APIs to the same project, and create a connection to that project.

You can create separate connections to separate projects, but you cannot use a connection to access an API that is not on the project specified in that connection.

To create a connection:

1. In any Adobe Authenticator module, click **Add** next to the Connection field.
1.

## Module

You have to make a project on developer. You can add the APIs you want to use to the project.

You have to put the entire address

