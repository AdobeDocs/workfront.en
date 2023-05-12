---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Split.io modules
description: In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use [!DNL Split.io], as well as connect it to multiple third-party applications and services.
author: Becky
feature: Workfront Fusion
exl-id: 4576a2e4-b495-430e-a9de-4e1ec7379ab8
---
# [!DNL Split.io] modules

In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use [!DNL Split.io], as well as connect it to multiple third-party applications and services.

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

To use [!DNL Split.io] modules, you must have a [!DNL Split.io] account.

## Connect [!DNL Split.io] to [!DNL Workfront Fusion]  {#connect-split-io-to-workfront-fusion}

You can create a connection to your [!DNL Split.io] account directly from inside a [!DNL Split.io] module.

1. In any [!DNL Split.io] module, click **[!UICONTROL Add]** next to the [!UICONTROL Connection] field.
1. Enter a name for the connection.
1. Enter your [!DNL Split.io] API key.

   For more information on [!DNL Split.io] API keys, see [API keys](https://help.split.io/hc/en-us/articles/360019916211-API-keys) in the [!DNL Split.io] documentation.

1. Click **[!UICONTROL Continue]** to create the connection and go back to the module.

## [!DNL Split.io] modules and their fields

When you configure [!DNL split.io] modules, [!DNL Workfront Fusion] displays the fields listed below. Along with these, additional [!DNL split.io] fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Actions](#actions)
* [Searches](#searches)

### Actions

* [[!UICONTROL Custom API Call]](#custom-api-call)
* [[!UICONTROL Get Split]](#get-split)
* [[!UICONTROL Get Split Definition in Environment]](#get-split-definition-in-environment)
* [[!UICONTROL Create Split]](#create-split)
* [[!UICONTROL Delete Split]](#delete-split)
* [[!UICONTROL Create Split Definition in Environment]](#create-split-definition-in-environment)
* [[!UICONTROL Remove Split Definition from Environment]](#remove-split-definition-from-environment)
* [[!UICONTROL Partial Update Split Definition in Environment]](#partial-update-split-definition-in-environment)
* [[!UICONTROL Associate Tags]](#associate-tags)

#### [!UICONTROL Custom API Call]

This action module lets you make a custom authenticated call to the [!DNL split.io] API. This way, you can create a data flow automation that can't be accomplished by the other [!DNL split.io] modules.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Split.io] account to [!DNL Workfront Fusion], see <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] to [!UICONTROL Workfront Fusion] </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Enter a path relative to <code>https://api.split.io/internal/api/v2/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP request methods in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion adds the authorization headers for you.</p> </td> 
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
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Enter or map the maximum number of records you want the module to work with during each scenario execution cycle.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get Split]

This action module retrieves the split.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Split.io] account to [!DNL Workfront Fusion], see <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] to [!UICONTROL Workfront Fusion] </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Select or map the workspace that contains the split you want to retrieve.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Enter or map the name of the split you want to retrieve.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get Split Definition in Environment]

This action module retrieves a specific split definition from the designated environment.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Split.io] account to [!DNL Workfront Fusion], see <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] to [!UICONTROL Workfront Fusion] </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Select or map the workspace that contains the split definition you want to retrieve.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Environment Name or ID]</td> 
   <td>Select or map the environment that contains the split definition you want to retrieve.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Enter or map the name of the split that you want to retrieve the split definition for.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create Split]

This action module creates a new split in your organization, given a traffic type.

>[!NOTE]
>
>The API does not configure the split in any environment.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Split.io] account to [!DNL Workfront Fusion], see <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] to [!UICONTROL Workfront Fusion] </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Select or map the workspace where you want to create the split.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Traffic Type ID or Name]</td> 
   <td>Select or map the traffic type that you want to use to create the split.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Enter or map a name for the split you want to create.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Description]</td> 
   <td>Enter or map a [!UICONTROL split] description for the split you want to create.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete Split]

This action module deletes a split from your organization. This automatically unconfigures the split definition from all environments.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Split.io] account to [!DNL Workfront Fusion], see <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] to [!UICONTROL Workfront Fusion] </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Select or map the workspace where you want to delete the split.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Enter or map the name of the split you want to delete.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create Split Definition in Environment]

This action module configures a split definition for a specific environment.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Split.io] account to [!DNL Workfront Fusion], see <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] to [!UICONTROL Workfront Fusion] </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Select or map the workspace where you want to create a split definition.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Environment Name or ID]</td> 
   <td>Select or map the environment where you want to create a split definition.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Enter or map the name of the split you want to create a definition for.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comments]</td> 
   <td>Enter or map any comments that you want to add to the split definition.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rules]</td> 
   <td> <p>For each targeting rule you want to add to the definition, click <b>[!UICONTROL Add item]</b>, then enter or map the rule.</p> <p>For more information on targeting rules, see <a href="https://docs.split.io/reference#create-split-definition-in-environment">Create split definition in an environment</a> in the [!DNL Split.io] documentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Default rule]</td> 
   <td> <p>Enter or map the rule that you want the split to use for the traffic that does not meet specifications for the other rules.</p> <p>For more information on targeting rules, see <a href="https://docs.split.io/reference#create-split-definition-in-environment">Create split definition in an environment</a> in the [!DNL Split.io] documentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Default treatment]</td> 
   <td> <p>Enter or map the treatment that you want the split to use if the split is killed or the customer is not included in traffic allocation.</p> <p>For more information on treatments, see <a href="https://docs.split.io/reference#create-split-definition-in-environment">Create split definition in an environment</a> in the [!DNL Split.io] documentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Treatments]</td> 
   <td> <p>For each treatment you want to add to the definition, click <b>[!UICONTROL Add item]</b>, then enter or map the treatment.</p> <p>For more information on treatments, see <a href="https://docs.split.io/reference#create-split-definition-in-environment">Create split definition in an environment</a> in the [!DNL Split.io] documentation.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remove Split Definition from Environment]

This action module unconfigures a split definition for a specific environment.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Split.io] account to [!DNL Workfront Fusion], see <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] to [!UICONTROL Workfront Fusion] </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Select or map the workspace where you want to remove a split definition.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Environment Name or ID]</td> 
   <td>Select or map the environment where you want to remove a split definition.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Enter or map the name of the split that you want to remove a definition for.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comments]</td> 
   <td>Enter or map any comments that you want to add to the split definition.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Partial Update Split Definition in Environment]

This action module updates a split definition for a specific environment.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Split.io] account to [!DNL Workfront Fusion], see <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] to [!UICONTROL Workfront Fusion] </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Select or map the workspace where you want to update a split definition.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Environment Name or ID]</td> 
   <td>Select or map the environment where you want to update a split definition.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Enter or map the name of the split you want to update a definition for.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Update content]</td> 
   <td> <p>For each attribute of the split that you want to update, click <b>[!UICONTROL Add item]</b> and enter or map the desired changes.</p> <p>For more information, see <a href="https://docs.split.io/reference#partial-update-split-definition-in-environment">Partial Update Split Definition in Environment</a> in the [!DNL Split.io] documentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comments]</td> 
   <td>Enter or map any comments that you want to add to the split definition.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Associate Tags]

This action module adds tags to the specified object.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Split.io] account to [!DNL Workfront Fusion], see <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] to [!UICONTROL Workfront Fusion] </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Select or map the workspace where you want to add a tag.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object Name]</td> 
   <td>Enter or map the name of the object you want to add tags to,</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object Type]</td> 
   <td> <p>Enter or map the type of object you want to add tags to.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tags]</td> 
   <td> <p>For each tag you want to add, click <b>[!UICONTROL Add item]</b> and enter or map the tag.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Searches

* [[!UICONTROL Get Workspaces]](#get-workspaces)
* [[!UICONTROL Get Environments]](#get-environments)
* [[!UICONTROL Get Splits]](#get-splits)
* [[!UICONTROL List Split Definitions in an Environment]](#list-split-definitions-in-an-environment)
* [[!UICONTROL Get Traffic Types]](#get-traffic-types)

#### [!UICONTROL Get Workspaces]

This search module retrieves the workspaces for an organization.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Split.io] account to [!DNL Workfront Fusion], see <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] to [!UICONTROL Workfront Fusion] </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Enter or map the maximum number of workspaces you want the module to retrieve during each scenario execution cycle.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get Environments]

This search module retrieves a list of environments.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Split.io] account to [!DNL Workfront Fusion], see <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] to [!UICONTROL Workfront Fusion] </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Select or map the workspace that contains the environments you want to list.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get Splits]

This search module retrieves a list of splits.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Split.io] account to [!DNL Workfront Fusion], see <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] to [!UICONTROL Workfront Fusion] </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Select or map the workspace that contains the splits you want to list.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Enter or map the maximum number of splits you want the module to retrieve during each scenario execution cycle.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL List Split Definitions in an Environment]

This search module retrieves a list of split definitions in a given environment.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Split.io] account to [!DNL Workfront Fusion], see <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] to [!UICONTROL Workfront Fusion] </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Select or map the workspace that contains the split definitions you want to list.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Environment Name or ID]</td> 
   <td>Select or map the environment that contains the split definitions you want to list.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Enter or map the maximum number of split definitions you want the module to retrieve during each scenario execution cycle.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get Traffic Types]

This search module retrieves a list of traffic types.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Split.io] account to [!DNL Workfront Fusion], see <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Connect [!DNL Split.io] to [!UICONTROL Workfront Fusion] </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Select or map the workspace that contains the traffic types you want to list.</td> 
  </tr> 
 </tbody> 
</table>
