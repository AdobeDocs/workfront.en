---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Azure DevOps modules
description: In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use [!DNL Azure DevOps], as well as connect it to multiple third-party applications and services.
author: Becky
feature: Workfront Fusion
exl-id: ecaa93c9-47bb-4fe1-87b4-d2e117cc68ae
---
# [!DNL Azure DevOps] modules

In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use [!DNL Azure DevOps], as well as connect it to multiple third-party applications and services.

If you need instructions on creating a scenario, see [Create a scenario in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

## Prerequisites

To use [!DNL Azure DevOps] modules, you must have an [!DNL Azure] DevOps account.

## Connect [!DNL Azure DevOps] to [!DNL Workfront Fusion] {#connect-azure-devops-to-workfront-fusion}

1. Add an [!DNL Azure DevOps] module to your scenario.
1. Click **[!UICONTROL Add]** next to the [!UICONTROL Connection] field.
1. In the [!UICONTROL Connection Type] field, select **[!DNL Azure DevOps]**.

   >[!IMPORTANT]
   >
   >The [!UICONTROL [!DNL Azure DevOps] (Request All Scopes)] connection type will be deprecated in the near future. Therefore, we do not recommend using it.

1. Fill out the following fields:

   <table style="table-layout:auto">
        <tr>
            <td>[!UICONTROL Connection name]</td>
            <td>Enter a name for the connection that you are creating.</td>
        </tr>
      <tr>
            <td>[!UICONTROL Organization]</td>
            <td>Enter the name of the organization under which you created your [!DNL Azure DevOps] application.</td>
        </tr>
    </table>

1. Click **[!UICONTROL Continue]** to finish setting up the connection and continue creating your scenario.

## [!UICONTROL Azure DevOps] modules and their fields

When you configure [!DNL Azure DevOps] modules, [!DNL Workfront Fusion] displays the fields listed below. Along with these, additional [!DNL Azure DevOps] fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers)
* [Actions](#actions)
* [Searches](#searches)

### Triggers 

#### [!UICONTROL Watch for work items]

This instant trigger module executes a scenario when a record is added, updated, or deleted in [!UICONTROL Azure DevOps].

The module returns any standard fields associated with the record, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Select or add a webhook for the module.</p> <p>For more information on webhooks in trigger modules, see <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Instant triggers (webhooks) in [!DNL Adobe Workfront Fusion]</a>.</p> <p>For information on how to create a webhook, see <a href="../../workfront-fusion/apps-and-their-modules/webhooks-updated.md" class="MCXref xref">Webhooks</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions 

* [Custom API Call](#custom-api-call)
* [Read record](#read-record)
* [Create a record](#create-a-record)
* [Update a work item](#update-a-work-item)
* [[!UICONTROL Upload an attachment]](#upload-an-attachment)
* [Download an attachment](#download-an-attachment)
* [Link work items]([!UICONTROL #link-work-items])

#### [!UICONTROL Custom API Call] 

This action module lets you make a custom authenticated call to the [!DNL Azure DevOps] API. This way, you can create a data flow automation that can't be accomplished by the other [!DNL Azure DevOps] modules.

When you are configuring this module, the following fields display.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Azure DevOps] account to [!DNL Workfront Fusion], see <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] to [!UICONTROL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Base URL]</td> 
   <td> <p>Select or map the base URL that you use to connect to your [!DNL Azure DevOps] account</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Relative URL]</td> 
   <td> <p>Enter the relative URL that you want to connect to for this API call.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>{organization}/_apis[/{area}]/{resource}</code> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL API Version]</td> 
   <td>Select or map the version of the [!DNL Azure DevOps] API that you want to connect to for this API call. If no version is selected, [!DNL Workfront Fusion] connects to [!DNL Azure DevOps] API version 5.1.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Add the query for the API call in the form of a standard JSON object.</p> <p>For example: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Read record]

This action module reads data from a single record in [!DNL Azure DevOps].

You specify the ID of the record.

The module returns the ID of the record and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Azure DevOps] account to [!DNL Workfront Fusion], see <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] to [!UICONTROL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td> <p>Select whether you want to read a project or a work item</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Project]</strong>: Select the project that you want to read..</p> </li> 
     <li> <p><strong>[!UICONTROL Work item]</strong>: Select the project that contains the work item you want to read, then select the work item type.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Select the information you want included in the output bundle for this module. Available fields depend on the work item type.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Enter or map the ID of the record you want to read.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create a record] 

This action module creates a new project or work item.

The module outputs the object ID for the newly created work item, or the URL and status code of a newly created project.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Azure DevOps] account to [!DNL Workfront Fusion], see <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] to [!UICONTROL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td> <p>Select whether you want to create a work item or a project.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Project]</strong> </p> <p>Fill in the following fields:</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Name]</strong>:Enter or map a name for the new project.</p> </li> 
       <li> <p><strong>[!UICONTROL Description]</strong>:Enter or map a description for the new project. </p> </li> 
       <li> <p><strong>[!UICONTROL Visibility]</strong>: Select whether you want your project to be public or private. Users must be signed into your organization and must have been granted access to the project in order to interact with a private project. Public projects are visible to users who are not signed in to your organization.</p> </li> 
       <li> <p><strong>[!UICONTROL Version control]</strong>: Select whether you want the project to use [!DNL Git] or [!UICONTROL Team Foundation Version Control (TFCV)] for version control.</p> </li> 
       <li> <p><strong>[!UICONTROL Work item process]</strong>: Select the work process that you want to use for the project. Options are [!UICONTROL Basic], [!UICONTROL Scrum], [!UICONTROL Capability Maturity Model Integration (CMMI)], and [!UICONTROL Agile].</p> <p>For more information on [!DNL Azure DevOps] processes, see <a href="https://docs.microsoft.com/en-us/azure/devops/boards/work-items/guidance/choose-process?view=azure-devops&amp;tabs=basic-process">Choose a Process</a> in the [!DNL Azure DevOps] Documentation.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Work item]</strong> </p> <p>Fill in the following fields:</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Project]</strong>: Select the project where you want to create the work item.</p> </li> 
       <li> <p><strong>[!UICONTROL Work item type]</strong>: Select the type of work item you want to create.</p> </li> 
       <li> <p><strong>[!UICONTROL Other fields]</strong>:In these fields, enter the value that you want the work item to have for a given property. Available fields depend on the work item type.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update a work item]

This action module updates an existing work item using its ID.

The module returns the ID of the updated work item.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Azure DevOps] account to [!DNL Workfront Fusion], see <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] to [!UICONTROL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project]</td> 
   <td>Select the project that contains the work item you want to update.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Work Item Type]</td> 
   <td> <p>Select the type of work item that you want to update.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Other Fields]</td> 
   <td>In each of these fields, enter the value that you want the work item to have for a given property. Available fields depend on the work item type.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Work item ID]</td> 
   <td>Enter or map the ID of the work item that you want to update.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Upload an attachment] 

This action module uploads a file and attaches it to a work item.

The module returns the attachment ID and a download URL for the attachment.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Azure DevOps] account to [!DNL Workfront Fusion], see <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] to [!UICONTROL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project] </td> 
   <td> <p>Select the project where you want to upload an attachment.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Work item ID]</td> 
   <td> <p>Enter or map the ID of the work item where you want to upload an attachment.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment]</td> 
   <td>Enter the text of a comment that you want to add to the uploaded attachment.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file] </td> 
   <td>Select a source file from a previous module, or enter or map the source file's name and content.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Download an attachment]

This action module downloads an attachment.

The module returns the file content of the attachment.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Azure DevOps] account to [!DNL Workfront Fusion], see <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] to [!UICONTROL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Attachment URL]</td> 
   <td> <p>Enter or map the URL of the attachment that you want to download.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Link work items]  

This action module links two work items and defines the relationship between them.

The module returns the ID of the main work item and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Azure DevOps] account to [!DNL Workfront Fusion], see <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] to [!UICONTROL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Work item ID]</td> 
   <td>Enter or map the ID of the main work item item that you want to link another work item to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Linked work item ID]</td> 
   <td>Enter or map the ID of the work item that you want to link to the main work item.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Link Type]</td> 
   <td> <p>Define the relationship between the work items that you want to link.</p> <p>For more information, see <a href="https://docs.microsoft.com/en-us/azure/devops/boards/queries/link-type-reference?view=azure-devops">Link Type Reference</a> in the [!UICONTROL Azure DevOps] Documentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment]</td> 
   <td>Enter or map the text of a comment. This is useful for explaining the reasoning or intention of the link.</td> 
  </tr> 
 </tbody> 
</table>

### Searches 

#### [!UICONTROL List work items]

This action module retrieves all work items of a specific type in an [!DNL Azure DevOps] project.

The module returns the ID of the main work item and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Azure DevOps] account to [!DNL Workfront Fusion], see <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect [!DNL Azure DevOps] to [!UICONTROL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project]</td> 
   <td>Select the project that you want to retrieve work items from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Work item type]</td> 
   <td> <p>Select the type of work item that you want to retrieve.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Select the properties that you want to appear in the module's output. The available fields depend on the type of work item you want to retrieve. You must select at least one property.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Enter or map the maximum number of work items that [!DNL Workfront Fusion] returns during one execution cycle.</td> 
  </tr> 
 </tbody> 
</table>
