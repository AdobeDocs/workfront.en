---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: connections-annd-webhooks
title: Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions
description: Many [!DNL Adobe Workfront Fusion] connectors do not require custom configuration when creating a connection. This article describes the default connection creation process.
author: Becky
feature: Workfront Fusion
exl-id: 6576a515-a1a1-4613-8d04-3c9d36bb1ed9
---
# Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions

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

## Create a connection

To create a connection inside a [!DNL Workfront Fusion] module:

1. Click **[!UICONTROL Add]** next to the [!UICONTROL Connection] box to open the **[!UICONTROL Create a connection]** panel.
1. (Optional) Change the default **[!UICONTROL Connection name]**.
1. (Conditional) If the app requires advanced connection settings, such as an ID, key, or [!UICONTROL secret], enter that information.

   You might need to click **[!UICONTROL Show advanced settings]** to display the fields where you can enter this kind of information.

1. Click **[!UICONTROL Continue]**.
1. In the sign-in window that displays, enter your credentials to log in to the app if you haven't already done so.
1. (Conditional) If an **[!UICONTROL Allow]** button displays, examine the actions that the connector will be able to take, then click the button to connect the app to [!DNL Workfront Fusion].

   >[!NOTE]
   >
   >Some Microsoft apps use the same connection, which is tied to individual user permissions. Therefore, when creating a connection, the permissions consent screen displays any permissions that were previously granted to this user's connection, in addition to any new permissions needed for the current application. 
   >
   >For example, if a user has "Read table" permissions granted via the Excel connector and then creates a connection in the Outlook connector to read emails, the permissions consent screen will show both the already granted "Read table" permission and the newly required "Write email" permission.