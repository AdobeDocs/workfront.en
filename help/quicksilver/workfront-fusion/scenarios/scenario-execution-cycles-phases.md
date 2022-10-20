---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Scenario execution, cycles, and phases in [!DNL Adobe Workfront] Fusion
description: This article describes events that occur while an [!DNL Adobe Workfront Fusion] scenario is running, such as initialization, operations, commits, and rollbacks.
author: Becky
feature: Workfront Fusion
exl-id: 5403f476-226d-4268-affc-8e06b1117684
---
# Scenario execution, cycles, and phases in [!DNL Adobe Workfront] Fusion

Adobe Workfront Fusion is a transactional system, similar to relational databases. Each scenario execution starts with the initialization phase, continues with at least one cycle composed of the operation and commit/rollback phases, and ends with the finalization phase:

>[!INFO]
>
>**Example**
>
>Initialization
>
>Cycle #1
>
>Operation (reading or writing)
>
>Commit or rollback
>
>Cycle #2
>
>Operation (reading or writing)
>
>Commit or rollback
>
>...
>
>Cycle #N
>
>Operation (reading or writing)
>
>Commit or rollback
>
>Finalization

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
  <td> <p>Workfront Fusion for Work Automation and Integration </p><p>Workfront Fusion for Work Automation </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Initialization

During the initialization phase, all necessary connections (connection to a database, email service, and so on) are created. They are also checked if each module is capable of performing their intended operations.

## Cycles

Each cycle represents an undividable unit of work composed of a series of operations. It is possible to set the maximum number of cycles in the [!UICONTROL scenario settings] panel. The default number is 1.

For more information, see [The scenario settings panel in Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Operation

During the operation phase reading and/or writing operation is performed:

* The reading operation consists of obtaining data from a service that is then processed by other modules according to a predefined scenario. For example, the [!UICONTROL Dropbox] >[!UICONTROL Watch files] module returns new bundles (files) created since the last scenario execution.
* The writing operation consists of sending data to a given service for further processing. For example, the [!UICONTROL Dropbox] >[!UICONTROL Upload a file] module uploads a file to a Dropbox folder.

## Commit

If the operation phase is successful for all modules, the commit phase begins during which all operations performed by the modules are committed. This means that [!DNL Workfront Fusion] sends information to all the services involved in the operation phase about its success.

## Rollback

If an error occurs during the operation or commit phase on any module, the phase is aborted and the rollback phase is started, making all operations during the given cycle void. Some modules do not support rollback and operations performed by these modules cannot be taken back. For more information see the [ACID modules](#acid-modules) section.

## Finalization

During the finalization phase, open connections (for example, FTP connections, database connections, and so on) are closed and the scenario is completed.

## ACID modules {#acid-modules}

All [!DNL Workfront] Fusion modules that support rollback (also known as transactionality) are marked with the ACID tag.

![](assets/acid-modules-350x189.png)

Modules not marked with this tag cannot be reverted back to their initial state when errors occur in other modules. A typical example of a non-ACID module is the [!UICONTROL Email] >[!UICONTROL Send an Email] action. After the email is sent you cannot undo the sending.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Examples</h2>
<h3>Transfer of bundles between databases</h3>
<p>The following example shows how to connect three ACID modules. The aim of the below scenario is to get new rows from a MySQL database, insert (transfer) them into a MSSQL database and then insert the IDs of the rows from the MSSQL database into a PostgreSQL database.</p>
<p> <img src="assets/transfer-bundles-betw-dbs-350x142.jpg" style="width: 350;height: 142;"> </p>
<p>When the scenario starts, the initialization phase is performed first. Workfront Fusion verifies connections to the MySQL, MSSQL and PostgreSQL databases one at a time. It everything goes well and the connections are successful, Workfront Fusion moves on to the operation phase. If an error occurs, the finalization phase starts instead of the operation phase and the scenario is terminated.</p>
<p>Next comes the operation phase. A preset procedure selects (reads) the table rows (bundles) from MySQL. Those rows are then passed to the next module that writes them to a selected table in the MSSQL database. If everything is in order, the last PostgresSQL procedure is called to insert the row IDs returned by the preceding module into the table.</p>
<p>If the operation phase is completed successfully, the commit phase begins. Workfront Fusion calls the SQL COMMIT command for each database and the write operations are committed.</p>
<p>However, if the operation or commit phase fails due to an error (for example, connection failure), Workfront Fusion calls rollback. During the rollback phase, Workfront Fusion goes through all modules one after another and executes the SQL <code>ROLLBACK</code> command for each module to revert each database back to its initial state.</p>
<p>Finally, during the finalization phase, each module closes its connection to the database.</p>
</div>
-->
