---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Microsoft Dynamics 365 modules
description: In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use Microsoft Dynamics 365, as well as connect it to multiple third-party applications and services.
author: Becky
feature: Workfront Fusion
exl-id: 116df088-20a7-40a8-8880-9f422dc37632
---
# [!DNL Microsoft Dynamics 365 modules]

In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use [!DNL Microsoft Dynamics 365], as well as connect it to multiple third-party applications and services.

>[!NOTE]
>
>The [!DNL Microsoft Dynamics 365] connector does not support [!DNL Dynamics Finance and Operations].

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

To use [!DNL Microsoft Dynamics] 365, you must have a [!DNL Microsoft Dynamics 365] account.

## Connect Microsoft Dynamics 365 to Workfront Fusion 

You can create a connection to your [!DNL Microsoft Dynamics 365] account directly from inside an [!DNL Microsoft Dynamics 365] module.

1. In any [!DNL Microsoft Dynamics 365] module, click **[!UICONTROL Add]** next to the [!UICONTROL Connection] field.
1. Enter a name for the connection.
1. In the **[!UICONTROL Resource]** field, enter the address of your [!DNL Dynamics 365] account, without `https://`.
1. Click **[!UICONTROL Continue]** to create the connection and go back to the module.

>[!NOTE]
>
>When registering [!DNL Workfront Fusion] in your [!DNL Microsoft Azure] portal, use the following redirect URI:
>
>* `https://app.workfrontfusion.com/oauth/cb/workfront-microsoft-dynamics2` 


## [!DNL Microsoft Dynamics 365] modules and their fields

When you configure [!DNL Microsoft Dynamics 365] modules, [!DNL Workfront Fusion] displays the fields listed below. Along with these, additional [!DNL Microsoft Dynamics 365] fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Watch Records (Scheduled)]](#watch-records-scheduled)
* [[!UICONTROL Watch Records (Real Time)]](#watch-records-real-time)
* [[!UICONTROL Create Record]](#create-record)
* [[!UICONTROL Make an API Call]](#make-an-api-call)
* [[!UICONTROL Delete Record]](#delete-record)
* [[!UICONTROL Read Records]](#read-records)
* [[!UICONTROL Update Record]](#update-record)
* [[!UICONTROL Search Records]](#search-records)

### [!UICONTROL Watch Records (Scheduled)]

This scheduled trigger module executes a scenario when a record in the object you specify is created or updated after the last scheduled run in [!DNL Dynamics 365].

The module's output indicates whether the record that it found is new or updated (if it was both added and updated in the time period, it's marked as new). You can map this information in subsequent modules in the scenario.

This happens on a regularly scheduled interval that you specify.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>For instructions about connecting your [!DNL Microsoft Dynamics 365] account to [!DNL Workfront Fusion], see <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] to [!DNL Workfront Fusion]</a> in this article. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Include]</td> 
   <td>Select whether you want the module to watch <strong>[!UICONTROL Only new records]</strong>, <strong>[!UICONTROL Updated records only]</strong>, or <strong>[!UICONTROL New records and all changes]</strong>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>Choose the [!UICONTROL Microsoft Dynamics 365] record type that you want the scenario to watch.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Max Records]</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Watch Records (Real Time)]

This instant trigger module executes a scenario when a record (object) you specify is created or updated in [!DNL Dynamics 365].

A webhook is required in this module.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Select the webhook that you want to use for this module. </p> <p>To add a new webhook:</p> 
    <ol> 
     <li value="1"> <p>Click <strong>[!UICONTROL Add]</strong> to the right of the Webhook field</p> </li> 
     <li value="2"> <p>In the <strong>[!UICONTROL Webhook]</strong> name field, type a descriptive name for the webhook.</p> </li> 
     <li value="3"> <p>In the <strong>[!UICONTROL Connection]</strong> field, select the Connection that you want to use selected</p> <p>For instructions about connecting your [!DNL Microsoft Dynamics 365] account to [!DNL Workfront Fusion], see <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] to [!DNL Workfront Fusion]</a> in this article. </p> </li> 
     <li value="4"> <p>Click <strong>[!UICONTROL Save]</strong> to save your webhook and return to the module.</p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Create Record]

This action module creates an entity, such as an appointment or task,.

You specify information about the entity that you want to create.

The module returns the ID of the new entity and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Microsoft Dynamics 365] account to [!DNL Workfront Fusion], see <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] to [!DNL Workfront Fusion]</a> in this article. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>Select the type of entity that you want the module to create.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Property fields]</td> 
   <td>In these fields, enter the value that you want the work item to have for a given property. Available fields depend on the entity type.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Make an API Call]

This action module lets you make a custom authenticated call to the [!DNL Microsoft Dynamics 365] API. This way, you can create a data flow automation that can't be accomplished by the other [!DNL Microsoft Dynamics 365] modules.

The module returns information about the status code, headers, and body. You can map this information in subsequent modules in the scenario.

To learn more, see the [!DNL Microsoft] documentation about using the [!DNL Dynamics 365 Customer Engagement Web API].

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>For instructions about connecting your [!DNL Microsoft Dynamics 365] account to [!DNL Workfront Fusion], see <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] to [!DNL Workfront Fusion]</a> in this article. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Enter a path relative to <code>&lt;Instance URL>/api/data/v9.1/</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods in [!DNL Adobe Workfront Fusion]</a>.</p> <p>For more in</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] adds the authorization headers for you.</p> </td> 
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

### [!UICONTROL Delete Record]

This action module deletes an entity.

You specify the ID of the entity.

The module returns the ID of the  entity and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>For instructions about connecting your [!DNL Microsoft Dynamics 365] account to [!DNL Workfront Fusion], see <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] to [!DNL Workfront Fusion]</a> in this article. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td> <p>Select the type of entity that you want the module to delete.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>Enter or map the unique [!DNL Microsoft Dynamics 365] ID of the record that you want the module to delete.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Read Records]

This action module reads data from a single entity in [!DNL Microsoft Dynamics 365].

You specify the ID of the entity.

The module returns the ID of the entity and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>For instructions about connecting your [!DNL Microsoft Dynamics 365] account to [!DNL Workfront Fusion], see <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] to [!DNL Workfront Fusion]</a> in this article. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>Select the type of entity that you want the module to read.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Enter or map the unique [!DNL Microsoft Dynamics 365] ID of the record that you want the module to read.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Update Record]

This action module updates an entity.

You specify the ID of the entity.

The module returns the ID of the updated record and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>For instructions about connecting your [!DNL Microsoft Dynamics 365] account to [!DNL Workfront Fusion], see <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] to [!DNL Workfront Fusion]</a> in this article. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>Select the type of entity that you want the module to update.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Property fields]</td> 
   <td>In these fields, enter the value that you want the work item to have for a given property. Available fields depend on the entity type.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Enter or map the unique [!DNL Microsoft Dynamics] 365 ID of the record that you want the module to update.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Search Records]

This search module looks for records in an object in [!DNL Microsoft Dynamics 365] that match the search query you specify. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>For instructions about connecting your [!DNL Microsoft Dynamics 365] account to [!DNL Workfront Fusion], see <a href="#connect-microsoft-dynamics-365-to-workfront-fusion" class="MCXref xref">Connect [!DNL Microsoft Dynamics 365] to [!DNL Workfront Fusion]</a> in this article. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>Select the type of entity that you want the module to update.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filters]</td> 
   <td> <p>Select the filter that you want to use for this search.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Standard Filters]</strong> </p> <p>Set up the filter by selecting a field and operator, and entering or mapping the value that you want to search for. You can use AND or OR rules to your filter.</p> </li> 
     <li> <p><strong>[!UICONTROL Query Functions]</strong> </p> <p>Enter the [!DNL Dynamics 365] web API query function that you want to use to search. </p> <p>For more information on query functions, see <a href="https://docs.microsoft.com/en-us/dynamics365/customer-engagement/web-api/queryfunctions?view=dynamics-ce-odata-9">Web API Query Function Reference</a> in the [!DNL Microsoft] documentation.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort]</td> 
   <td> <p>Specify the order in which items are returned. You can add multiple sorts.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Field]</strong> </p> <p>Specify the field by which you want to sort results.</p> </li> 
     <li> <p><strong>[!UICONTROL Direction]</strong> </p> <p>Specify the direction of the sort (ascending or descending).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Max Records]</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>Select the information you want included in the output bundle for this module.</p> </td> 
  </tr> 
 </tbody> 
</table>
