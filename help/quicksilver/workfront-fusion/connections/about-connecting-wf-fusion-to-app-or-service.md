---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: About connecting [!DNL Adobe Workfront Fusion] to an app or service
description: For most apps, it is necessary to create a connection, through which [!DNL Adobe Workfront Fusion] can communicate with the given third-party service according to the settings of the specific scenario.
author: Becky
feature: Workfront Fusion
exl-id: 2d5cf083-9893-45e8-8f7d-0f8f5a74eef3
---
# About connecting [!DNL Adobe Workfront Fusion] to an app or service

For most apps, it is necessary to create a connection, through which [!DNL Adobe Workfront Fusion] can communicate with the given third-party service according to the settings of the specific scenario.

For example, if you want to create a scenario that retrieves information from [!DNL Workfront], you must grant access permission for [!DNL Workfront Fusion] to access your [!DNL Workfront] account.

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td> <p>New: [!UICONTROL Standard]</p><p>Or</p><p>Current: [!UICONTROL Work] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td>
   <p>Current: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy: Any </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>New:</p> <ul><li>[!UICONTROL Select] or [!UICONTROL Prime] [!DNL Workfront] Plan: Your organization must purchase [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plan: [!DNL Workfront Fusion] is included.</li></ul>
   <p>Or</p>
   <p>Current: Your organization must purchase [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Access rights

For every connection, [!DNL Workfront Fusion] requires only those access rights that are necessary to successfully complete a given scenario. For example, if you create a scenario to list documents from [!DNL Google Docs], [!DNL Workfront Fusion] does not ask for permission to get the content of the documents.

Unfortunately, not all services allow you to limit access to specific tasks. Therefore, [!DNL Workfront Fusion] must require full access rights. For more information on how to restrict [!DNL Workfront Fusion] access to your account registered to those services, see the application-specific documentation.

## About administering connections

You can administer all connections from the [!UICONTROL Connections] area. Here you can:

* See which permissions were given to [!DNL Workfront Fusion] for each connection
* Rename connections
* Reauthorize existing connections
* Delete existing connections
* Verify that the connection to the service was established successfully

To open the [!UICONTROL Connections] area, click <b>[!UICONTROL Connections]</b> in the left navigation.

## Renew a connection

[!DNL Workfront Fusion] usually obtains access rights to a given service for an unlimited period of time. However, this is not always the case. With some services, the access permission must be renewed after a certain period of time. In these cases, [!DNL Workfront Fusion] notifies you via email shortly before its access rights expire.

To renew a connection:

1. Click the **[!UICONTROL Reauthorize]** button in the **[!UICONTROL Connections]** area.
