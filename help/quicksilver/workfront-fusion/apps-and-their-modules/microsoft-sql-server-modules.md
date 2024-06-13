---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Microsoft SQL Server modules
description: You can use [!DNL Adobe Workfront Fusion] to connect to Microsoft SQL Server.
author: Becky
feature: Workfront Fusion
exl-id: d79cf00d-a81e-4d88-ac4a-f80b7b5a92b3
---
# [!DNL Microsoft SQL Server] modules

You can use [!DNL Adobe Workfront Fusion] to connect to [!UICONTROL Microsoft SQL Server].

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



## Connecting the [!DNL Microsoft SQL Server] service to [!DNL Workfront Fusion]

For instructions about connecting your [!DNL Microsoft SQL Server] account to [!UICONTROL Workfront Fusion], see [Create a connection to [!UICONTROL Adobe Workfront Fusion] - Basic instructions](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Some Microsoft apps use the same connection, which is tied to individual user permissions. Therefore, when creating a connection, the permissions consent screen displays any permissions that were previously granted to this user's connection, in addition to any new permissions needed for the current application. 
>
>For example, if a user has "Read table" permissions granted via the Excel connector and then creates a connection in the Outlook connector to read emails, the permissions consent screen will show both the already granted "Read table" permission and the newly required "Write email" permission.

## Using [!DNL Microsoft SQL Server] modules

You can execute your custom logic directly on your database server through stored procedures. [!DNL Adobe Workfront Fusion] loads interface of input/output parameters and recordset dynamically so each parameter or value can be mapped individually. Before you start configuring your scenario, make sure the account you're using to connect to your database has read access to `INFORMATION_SCHEMA.ROUTINES` and `INFORMATION_SCHEMA.PARAMETERS` views.

When [!DNL Fusion] establishes the connection to the [!DNL SQL server] destination, the [!DNL Fusion] user identifies the Host (the domain name or IP address where the server is hosted) and the port. [!DNL Fusion] can connect to any available host and port.

For information about specific IP addresses used by [!DNL Workfront Fusion], see [IP Addresses for accessing [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)

To learn more about creating a stored procedure, see the [!DNL Microsoft SQL Server] documentation.

>[!NOTE]
>
>[!DNL Workfront Fusion] doesn't support multiple recordsets. Only the first one is processed.

## Troubleshooting error [!UICONTROL ER_LOCK_WAIT_TIMEOUT: Lock wait timeout exceeded; try restarting transaction]

This error occurs when you modify the same data using multiple modules. It is caused by SQL transactions.

When any SQL module is executed, it starts a transaction. The transaction is finished after the scenario is fully executed.

If another module tries to access the same data, it has to wait until the previous transaction is finished. Since the first transaction will be finished after the scenario is finished, the second transaction can never begin.

### Solution:

Turn on Auto-commit. Auto-commit finishes (commits) every transaction immediately after the module execution is done.

1. Click the [!UICONTROL Scenario settings] icon ![](assets/scenario-settings-icon.png)at the bottom of the screen.
1. Click the **[!UICONTROL Auto commit]** checkbox.
1. Click **[!UICONTROL OK]** to save the scenario settings.
