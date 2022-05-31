---
title: MariaDB modules
description: MariaDB modules
draft: Probably
---
# MariaDB modules

In an Adobe Workfront Fusion scenario, you can automate workflows that use MariaDB, as well as connect it to to multiple third-party applications and services.

If you need instructions on creating a scenario, see [Create a scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in Adobe Workfront Fusion](../../workfront-fusion/modules/modules.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto"> 
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

## Prerequisites

To use MariaDB modules, you must have a MariaDB account.

## Connect MariaDB to Workfront Fusion {#connect-mariadb-to-workfront-fusion}

You can create a connection to your MariaDB account directly from inside a MariaDB module.

1. In any MariaDB module, click **Add** next to the Connection field.
1. Configure the following fields:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Connection name</p> </td> 
      <td> <p>Enter a name for the new connection.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Host</td> 
      <td> <p>Enter the IP address or host name of your database instance. This host must be accessible from outside your network.</p> <p>Example: <code>mariadb.hwoh2j5h.us-east-1.rds.amazon.com</code></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Port</td> 
      <td>The default port is 3306. If you are using a non-standard port, set this number to your port. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Database Name</td> 
      <td>Enter the name of the database you want to interact with.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Username</td> 
      <td>Enter your username.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Password</td> 
      <td>Enter your password.</td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Continue** to create the connection and go back to the module.

## MariaDB Modules and their fields

When you configure MariaDB modules, Workfront Fusion displays the fields listed below. Along with these, additional MariaDB fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Execute a query (advanced)

This action module retrieves information from your database, based on a query you supply.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions about connecting your MariaDB account to Workfront Fusion, see <a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">Connect MariaDB to Workfront Fusion</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query</td> 
   <td> <p>Enter the SQL query that you want the module to use to retrieve data.</p> <p>Important: Variables used in the query are not sanitized. Make sure you sanitize variables properly to prevent SQL injection.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Select rows from a table (advanced)

This module reads record from your database.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td>For instructions about connecting your MariaDB account to Workfront Fusion, see <a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">Connect MariaDB to Workfront Fusion</a> in this article.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Table</td> 
   <td> <p>Select the table that contains the records you want to read.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Filter</td> 
   <td> <p>Set up the filter by which you want to select rows</p> 
    <ul> 
     <li> <p>Select the field that you want to search by</p> </li> 
     <li> <p>Select the operator that you want to use for your search</p> </li> 
     <li> <p>Enter or map the value that you want to search for.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sort </td> 
   <td> <p>For each level that you want your results sorted by, click <strong>Add item</strong>, then select the field that you want to sort the results by and whether you want to sort ascending or descending</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

