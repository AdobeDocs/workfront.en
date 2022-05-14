---
filename: azure-dev-ops
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Azure DevOps modules
description: In an Adobe Workfront Fusion scenario, you can automate workflows that use Azure DevOps, as well as connect it to to multiple third-party applications and services.
---

# Azure DevOps modules

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

In an Adobe Workfront Fusion scenario, you can automate workflows that use Azure DevOps, as well as connect it to to multiple third-party applications and services.

If you need instructions on creating a scenario, see [Create a scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in Adobe Workfront Fusion](../../workfront-fusion/modules/modules.md).

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

## Prerequisites

To use Azure DevOps modules, you must have an Azure DevOps account.

## Connect Azure DevOps to Workfront Fusion {#connect-azure-devops-to-workfront-fusion}

1. Add an Azure DevOps module to your scenario.
1. Click **Add** next to the Connection field.
1. In the Connection Type field, select **Azure DevOps**.

   >[!IMPORTANT]
   >
   >The Azure DevOps (Request All Scopes) connection type will be deprecated in the near future. Therefore, we do not recommend using it.

1. Fill out the following fields:

   | Connection name |Enter a name for the connection that you are creating. |
   |---|---|
   | Organization |Enter the name of the organization under which you created your Azure DevOps application. |

1. Click **Continue** to finish setting up the connection and continue creating your scenario.

## Azure DevOps modules and their fields

When you configure Azure DevOps modules, Workfront Fusion displays the fields listed below. Along with these, additional Azure DevOps fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers) 
* [Actions](#actions) 
* [Searches](#searches)

### Triggers {#triggers}

#### Watch for work items

This instant trigger module executes a scenario when a record is added, updated, or deleted in Azure DevOps.

The module The module returns any standard fields associated with the record, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Webhook</td> 
   <td> <p>Select or add a webhook for the module.</p> <p>For more information on webhooks in trigger modules, see <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Instant triggers (webhooks) in Adobe Workfront Fusion</a>.</p> <p>For information on how to create a webhook, see <a href="../../workfront-fusion/apps-and-their-modules/webhooks-updated.md" class="MCXref xref">Webhooks</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions {#actions}

* [Custom API Call](#custom-api-call) 
* [Read record](#read-record) 
* [Create a record](#create-a-record) 
* [Update a work item](#update-a-work-item) 
* [Upload an attachment](#upload-an-attachment) 
* [Download an attachment](#download-an-attachment) 
* [Link work items](#link-work-items)

#### Custom API Call {#custom-api-call}

This action module lets you make a custom authenticated call to the Azure DevOps API. This way, you can create a data flow automation that can't be accomplished by the other Azure DevOps modules.

When you are configuring this module, the following fields display.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Azure DevOps account to Workfront Fusion, see <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect Azure DevOps to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Base URL</td> 
   <td> <p>Select or map the base URL that you use to connect to your Azure DevOps account</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Relative URL</td> 
   <td> <p>Enter the relative URL that you want to connect to for this API call.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><code>{organization}/_apis[/{area}]/{resource}</code> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">API Version</td> 
   <td>Select or map the version of the Azure DevOps API that you want to connect to for this API call. If no version is selected, Workfront Fusion connects to Azure DevOps API version 5.1.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Method</td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query String</td> 
   <td> <p>Add the query for the API call in the form of a standard JSON object.</p> <p>For example: <code>{“name”:“something-urgent”}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Body</td> 
   <td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### Read record {#read-record}

This action module reads data from a single record in Azure DevOps.

You specify the ID of the record.

The module returns the ID of the record and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Azure DevOps account to Workfront Fusion, see <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect Azure DevOps to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record type</td> 
   <td> <p>Select whether you want to read a project or a work item</p> 
    <ul> 
     <li> <p><strong>Project</strong>:Select the project that you want to read..</p> </li> 
     <li> <p><strong>Work item</strong>:Select the project that contains the work item you want to read, then select the work item type.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Outputs</td> 
   <td>Select the information you want included in the output bundle for this module. Available fields depend on the work item type.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID</td> 
   <td>Enter or map the ID of the record you want to read.</td> 
  </tr> 
 </tbody> 
</table>

#### Create a record {#create-a-record}

This action module creates a new project or work item.

The module outputs the object ID for the newly created work item, or the URL and status code of a newly created project.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Azure DevOps account to Workfront Fusion, see <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect Azure DevOps to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record type</td> 
   <td> <p>Select whether you want to create a work item or a project.</p> 
    <ul> 
     <li> <p><strong>Project</strong> </p> <p>Fill in the following fields:</p> 
      <ul> 
       <li> <p><strong>Name</strong>:Enter or map a name for the new project.</p> </li> 
       <li> <p><strong>Description</strong>:Enter or map a description for the new project. </p> </li> 
       <li> <p><strong>Visibility</strong>:Select whether you want your project to be public or private. Users must be signed into your organization and must have been granted access to the project in order to interact with a private project. Public projects are visible to users who are not signed in to your organization.</p> </li> 
       <li> <p><strong>Version control</strong>:Select whether you want the project to use Git or Team Foundation Version Control (TFCV) for version control.</p> </li> 
       <li> <p><strong>Work item process</strong>:Select the work process that you want to use for the project. Options are Basic, Scrum, Capability Maturity Model Integration (CMMI), and Agile.</p> <p>For more information on Azure DevOps processes, see <a href="https://docs.microsoft.com/en-us/azure/devops/boards/work-items/guidance/choose-process?view=azure-devops&amp;tabs=basic-process">Choose a Process</a> in the Azure DevOps Documentation.</p> </li> 
      </ul> </li> 
     <li> <p><strong>Work item</strong> </p> <p>Fill in the following fields:</p> 
      <ul> 
       <li> <p><strong>Project</strong>:Select the project where you want to create the work item.</p> </li> 
       <li> <p><strong>Work item type</strong>:Select the type of work item you want to create.</p> </li> 
       <li> <p><strong>Other fields</strong>:In these fields, enter the value that you want the work item to have for a given property. Available fields depend on the work item type.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### Update a work item {#update-a-work-item}

This action module updates an existing work item using its ID.

The module returns the ID of the updated work item.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Azure DevOps account to Workfront Fusion, see <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect Azure DevOps to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Project</td> 
   <td>Select the project that contains the work item you want to update.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Work Item Type</td> 
   <td> <p>Select the type of work item that you want to update.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Other Fields</td> 
   <td>In each of these fields, enter the value that you want the work item to have for a given property. Available fields depend on the work item type.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Work item ID</td> 
   <td>Enter or map the ID of the work item that you want to update.</td> 
  </tr> 
 </tbody> 
</table>

#### Upload an attachment {#upload-an-attachment}

This action module uploads a file and attaches it to a work item.

The module returns the attachment ID and a download URL for the attachment.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Azure DevOps account to Workfront Fusion, see <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect Azure DevOps to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Project </td> 
   <td> <p>Select the project where you want to upload an attachment.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Work item ID</td> 
   <td> <p>Enter or map the ID of the work item where you want to upload an attachment.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Comment</td> 
   <td>Enter the text of a comment that you want to add to the uploaded attachment.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Source file </td> 
   <td>Select a source file from a previous module, or enter or map the source file's name and content.</td> 
  </tr> 
 </tbody> 
</table>

#### Download an attachment {#download-an-attachment}

This action module downloads an attachment.

The module returns the file content of the attachment.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Azure DevOps account to Workfront Fusion, see <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect Azure DevOps to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Attachment URL</td> 
   <td> <p>Enter or map the URL of the attachment that you want to download.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Link work items  {#link-work-items}

This action module links two work items and defines the relationship between them.

The module returns the ID of the main work item and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Azure DevOps account to Workfront Fusion, see <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect Azure DevOps to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Work item ID</td> 
   <td>Enter or map the ID&nbsp;of the main work item item that you want to link another work item to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Linked work item ID</td> 
   <td>Enter or map the ID of the work item that you want to link to the main work item.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Link Type</td> 
   <td> <p>Define the relationship between the work items that you want to link.</p> <p>For more information, see <a href="https://docs.microsoft.com/en-us/azure/devops/boards/queries/link-type-reference?view=azure-devops">Link Type Reference</a> in the Azure DevOps Documentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Comment</td> 
   <td>Enter or map the text of a comment. This is useful for explaining the reasoning or intention of the link.</td> 
  </tr> 
 </tbody> 
</table>

### Searches {#searches}

#### List work items

This action module retrieves all work items of a specific type in an Azure DevOps project.

The module returns the ID of the main work item and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Azure DevOps account to Workfront Fusion, see <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Connect Azure DevOps to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Project</td> 
   <td>Select the project that you want to retrieve work items from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Work item type</td> 
   <td> <p>Select the type of work item that you want to retrieve.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Outputs</td> 
   <td>Select the properties that you want to appear in the module's output. The available fields depend on the type of work item you want to retrieve. You must select at least one property.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td>Enter or map the maximum number of work items that Workfront Fusion returns during one execution cycle.</td> 
  </tr> 
 </tbody> 
</table>

