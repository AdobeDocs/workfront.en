---
filename: microsoft-sql-server-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Microsoft SQL Server modules
description: You can use Adobe Workfront Fusion to connect to Microsoft SQL Server.
---

# Microsoft SQL Server modules

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

You can use Adobe Workfront Fusion to connect to Microsoft SQL Server.

## Access requirements

You must have the following access to use the functionality in this article:

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan, Work</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion license**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your organization.</p>
     --> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your team.</p>
     --> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Using Microsoft SQL Server modules

You can execute your custom logic directly on your database server through stored procedures. Adobe Workfront Fusion loads interface of input/output parameters and recordset dynamically so each parameter or value can be mapped individually. Before you start configuring your scenario, make sure the account you're using to connect to your database has read access to 

```
INFORMATION_SCHEMA.ROUTINES
```

and 

```
INFORMATION_SCHEMA.PARAMETERS
```

views.

When Fusion establishes the connection to the SQL server destination, the Fusion user identifies the Host (the domain name or IP address where the server is hosted) and the port. Fusion can connect to any available host and port.

For information about specific IP&nbsp;addresses used by Workfront Fusion, see [IP Addresses for accessing Adobe Workfront Fusion](../../workfront-fusion/get-started/ip-addresses-for-fusion.md)

To learn more about creating a stored procedure, see the Microsoft SQL Server documentation.

>[!NOTE]
>
>Workfront Fusion doesn't support multiple recordsets. Only the first one is processed.

## Troubleshooting error ER_LOCK_WAIT_TIMEOUT: Lock wait timeout exceeded; try restarting transaction

This error occurs when you modify the same data using multiple modules. It is caused by SQL transactions.

When any SQL module is executed, it starts a transaction. The transaction is finished after the scenario is fully executed.

If another module tries to access the same data, it has to wait until the previous transaction is finished. Since the first transaction will be finished after the scenario is finished, the second transaction can never begin.

### Solution:

Turn on Auto-commit. Auto-commit finishes (commits) every transaction immediately after the module execution is done.

1. Click the Scenario settings icon ![](assets/scenario-settings-icon.png)at the bottom of the screen.
1. Click the **Auto commit** checkbox.
1. Click **OK** to save the scenario settings.

