---
filename: split-io-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Split.io modules
description: In a Adobe Workfront Fusion scenario, you can connect your Split.io account to multiple third-party applications and services.
---

# Split.io modules

In a Adobe Workfront Fusion scenario, you can connect your Split.io account to multiple third-party applications and services.

If you need instructions on creating a scenario, see [Create a scenario](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in Adobe Workfront Fusion](../../workfront-fusion/modules/modules.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> Adobe Workfront license* Plan, Work 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion license**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr> <!--
   Access level configurations* You must be a Workfront Fusion administrator for your organization. You must be a Workfront Fusion administrator for your team.
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisites

To use Split.io modules, you must have a Split.io account.

## Connect Split.io to Workfront Fusion

You can create a connection to your Split.io account directly from inside a Split.io module.

1. In any Split.io module, click `Add`next to the Connection field.
1. Enter a name for the connection.
1. Enter your Split.io API key.

   For more information on Split.io API keys, see [API keys](https://help.split.io/hc/en-us/articles/360019916211-API-keys) in the Split.io documentation.

1. Click `Continue` to create the connection and go back to the module.

## Split.io modules and their fields

When you configure split.io modules, Workfront Fusion displays the fields listed below. Along with these, additional split.io fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Actions](#actions) 
* [Searches](#searches)

### Actions

* [Custom API Call](#custom) 
* [Get Split](#get5) 
* [Get Split Definition in Environment](#get6) 
* [Create Split](#create) 
* [Delete Split](#delete) 
* [Create Split Definition in Environment](#create2) 
* [Remove Split Definition from Environment](#remove) 
* [Partial Update Split Definition in Environment](#partial) 
* [Associate Tags](#associat)

#### Custom API Call

This action module lets you make a custom authenticated call to the split.io API. This way, you can create a data flow automation that can't be accomplished by the other split.io modules. 

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Split.io account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect Split.io to Workfront Fusion </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>Enter a path relative to <code>https://api.split.io/internal/api/v2/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Method</td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP request methods</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion adds the authorization headers for you.</p> </td> 
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
  <tr> 
   <td role="rowheader">Limit</td> 
   <td>Enter or map the maximum number of records you want the module to work with during each scenario execution cycle.</td> 
  </tr> 
 </tbody> 
</table>

#### Get Split

This action module retrieves the split.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Split.io account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect Split.io to Workfront Fusion </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workspace ID</td> 
   <td>Select or map the workspace that contains the split you want to retrieve.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Split Name</td> 
   <td> <p>Enter or map the name of the split you want to retrieve.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Get Split Definition in Environment

This action module retrieves a specific split definition from the designated environment.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Split.io account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect Split.io to Workfront Fusion </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workspace ID</td> 
   <td>Select or map the workspace that contains the split definition you want to retrieve.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Environment Name or ID</td> 
   <td>Select or map the environment that contains the split definition you want to retrieve.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Split Name</td> 
   <td> <p>Enter or map the name of the split that you want to retrieve the split definition for.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Create Split

This action module creates a new split in your organization, given a traffic type.

>[!NOTE]
>
>The API does not configure the split in any environment.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Split.io account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect Split.io to Workfront Fusion </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workspace ID</td> 
   <td>Select or map the workspace where you want to create the split.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Traffic Type ID or Name</td> 
   <td>Select or map the traffic type that you want to use to create the split.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Split Name</td> 
   <td> <p>Enter or map a name for the split you want to create.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Split Description</td> 
   <td>Enter or map a split description for the split you want to create.</td> 
  </tr> 
 </tbody> 
</table>

#### Delete Split

This action module deletes a split from your organization. This automatically unconfigures the split definition from all environments.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Split.io account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect Split.io to Workfront Fusion </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workspace ID</td> 
   <td>Select or map the workspace where you want to delete the split.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Split Name</td> 
   <td> <p>Enter or map the name of the split you want to delete.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Create Split Definition in Environment

This action module configures a split definition for a specific environment.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Split.io account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect Split.io to Workfront Fusion </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workspace ID</td> 
   <td>Select or map the workspace where you want to create a split definition.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Environment Name or ID</td> 
   <td>Select or map the environment where you want to create a split definition.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Split Name</td> 
   <td> <p>Enter or map the name of the split you want to create a definition for.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Comments</td> 
   <td>Enter or map any comments that you want to add to the split definition.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Rules</td> 
   <td> <p>For each targeting rule you want to add to the definition, click <b>Add item</b>, then enter or map the rule.</p> <p>For more information on targeting rules, see <a href="https://docs.split.io/reference#create-split-definition-in-environment">Create split definition in an environment</a> in the Split.io documentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Default rule</td> 
   <td> <p>Enter or map the rule that you want the split to use for the traffic that does not meet specifications for the other rules.</p> <p>For more information on targeting rules, see <a href="https://docs.split.io/reference#create-split-definition-in-environment">Create split definition in an environment</a> in the Split.io documentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Default treatment</td> 
   <td> <p>Enter or map the treatment that you want the split to use if the split is killed or the customer is not included in traffic allocation.</p> <p>For more information on treatments, see <a href="https://docs.split.io/reference#create-split-definition-in-environment">Create split definition in an environment</a> in the Split.io documentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Treatments</td> 
   <td> <p>For each treatment you want to add to the definition, click <b>Add item</b>, then enter or map the treatment.</p> <p>For more information on treatments, see <a href="https://docs.split.io/reference#create-split-definition-in-environment">Create split definition in an environment</a> in the Split.io documentation.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Remove Split Definition from Environment

This action module unconfigures a split definition for a specific environment.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Split.io account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect Split.io to Workfront Fusion </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workspace ID</td> 
   <td>Select or map the workspace where you want to remove a split definition.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Environment Name or ID</td> 
   <td>Select or map the environment where you want to remove a split definition.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Split Name</td> 
   <td> <p>Enter or map the name of the split that you want to remove a definition for.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Comments</td> 
   <td>Enter or map any comments that you want to add to the split definition.</td> 
  </tr> 
 </tbody> 
</table>

#### Partial Update Split Definition in Environment

This action module updates a split definition for a specific environment.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Split.io account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect Split.io to Workfront Fusion </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workspace ID</td> 
   <td>Select or map the workspace where you want to update a split definition.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Environment Name or ID</td> 
   <td>Select or map the environment where you want to update a split definition.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Split Name</td> 
   <td> <p>Enter or map the name of the split you want to update a definition for.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Update content</td> 
   <td> <p>For each attribute of the split that you want to update, click <b>Add item</b> and enter or map the desired changes.</p> <p>For more information, see <a href="https://docs.split.io/reference#partial-update-split-definition-in-environment">Partial Update Split Definition in Environment</a> in the Split.io documentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Comments</td> 
   <td>Enter or map any comments that you want to add to the split definition.</td> 
  </tr> 
 </tbody> 
</table>

#### Associate Tags

This action module adds tags to the specified object. 

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Split.io account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect Split.io to Workfront Fusion </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workspace ID</td> 
   <td>Select or map the workspace where you want to add a tag.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object Name</td> 
   <td>Enter or map the name of the object you want to add tags to,</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object Type</td> 
   <td> <p>Enter or map the type of object you want to add tags to.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tags</td> 
   <td> <p>For each tag you want to add, click <b>Add item</b> and enter or map the tag.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Searches

* [Get Workspaces](#get) 
* [Get Environments](#get2) 
* [Get Splits](#get3) 
* [List Split Definitions in an Environment](#list) 
* [Get Traffic Types](#get4)

#### Get Workspaces

This search module retrieves the workspaces for an organization.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Split.io account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect Split.io to Workfront Fusion </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td>Enter or map the maximum number of workspaces you want the module to retrieve during each scenario execution cycle.</td> 
  </tr> 
 </tbody> 
</table>

#### Get Environments

This search module retrieves a list of environments.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Split.io account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect Split.io to Workfront Fusion </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workspace ID</td> 
   <td>Select or map the workspace that contains the environments you want to list.</td> 
  </tr> 
 </tbody> 
</table>

#### Get Splits

This search module retrieves a list of splits.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Split.io account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect Split.io to Workfront Fusion </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workspace ID</td> 
   <td>Select or map the workspace that contains the splits you want to list.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td>Enter or map the maximum number of splits you want the module to retrieve during each scenario execution cycle.</td> 
  </tr> 
 </tbody> 
</table>

#### List Split Definitions in an Environment

This search module retrieves a list of split definitions in a given environment.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Split.io account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect Split.io to Workfront Fusion </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workspace ID</td> 
   <td>Select or map the workspace that contains the split definitions you want to list.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Environment Name or ID</td> 
   <td>Select or map the environment that contains the split definitions you want to list.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td>Enter or map the maximum number of split definitions you want the module to retrieve during each scenario execution cycle.</td> 
  </tr> 
 </tbody> 
</table>

#### Get Traffic Types

This search module retrieves a list of traffic types.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Split.io account to Workfront Fusion, see <a href="#connect" class="MCXref xref">Connect Split.io to Workfront Fusion </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Workspace ID</td> 
   <td>Select or map the workspace that contains the traffic types you want to list.</td> 
  </tr> 
 </tbody> 
</table>

