---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Scenario execution, cycles, and phases in [!DNL Adobe Workfront Fusion]
description: This article describes events that occur while an [!DNL Adobe Workfront Fusion] scenario is running, such as initialization, operations, commits, and rollbacks.
author: Becky
feature: Workfront Fusion
exl-id: 5403f476-226d-4268-affc-8e06b1117684
---
# Scenario execution, cycles, and phases in [!DNL Adobe Workfront Fusion]

[!DNL Adobe Workfront Fusion] is a transactional system, similar to relational databases. Each scenario execution starts with the initialization phase, continues with at least one cycle composed of the operation and commit/rollback phases, and ends with the finalization phase:

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
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] license**</td> 
  <td>
   <p>Current license requirement: No [!DNL Workfront Fusion] license requirement.</p>
   <p>Or</p>
   <p>Legacy license requirement: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration],  [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

## Initialization

During the initialization phase, all necessary connections (connection to a database, email service, and so on) are created. They are also checked if each module is capable of performing their intended operations.

## Cycles

Each cycle represents an undividable unit of work composed of a series of operations. It is possible to set the maximum number of cycles in the [!UICONTROL scenario settings] panel. The default number is 1.

For more information, see [The scenario settings panel in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## Operation

During the operation phase reading and/or writing operation is performed:

* The reading operation consists of obtaining data from a service that is then processed by other modules according to a predefined scenario. For example, the [!UICONTROL Dropbox] >[!UICONTROL Watch files] module returns new bundles (files) created since the last scenario execution.
* The writing operation consists of sending data to a given service for further processing. For example, the [!DNL Dropbox] >[!UICONTROL Upload a file] module uploads a file to a [!DNL Dropbox] folder.

## Commit

If the operation phase is successful for all modules, the commit phase begins during which all operations performed by the modules are committed. This means that [!DNL Workfront Fusion] sends information to all the services involved in the operation phase about its success.

## Rollback

If an error occurs during the operation or commit phase on any module, the phase is aborted and the rollback phase is started, making all operations during the given cycle void. Some modules do not support rollback and operations performed by these modules cannot be taken back. For more information see the [ACID modules](#acid-modules) section.

## Finalization

During the finalization phase, open connections (for example, FTP connections, database connections, and so on) are closed and the scenario is completed.

## ACID modules

All [!DNL Workfront Fusion] modules that support rollback (also known as transactionality) are marked with the ACID tag.

![](assets/acid-modules-350x189.png)

Modules not marked with this tag cannot be reverted back to their initial state when errors occur in other modules. A typical example of a non-ACID module is the [!UICONTROL Email] >[!UICONTROL Send an Email] action. After the email is sent you cannot undo the sending.
