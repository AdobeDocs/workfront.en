---
filename: azure-ad-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Azure Active Directory modules
description: In a Adobe Workfront Fusion scenario, you can connect your Azure Active Directory account to multiple third-party applications and services.
---

# Azure Active Directory modules

In a Adobe Workfront Fusion scenario, you can connect your Azure Active Directory account to multiple third-party applications and services.

If you need instructions on creating a scenario, see [Create a scenario](../../workfront-fusion/scenarios/create-a-scenario.md). For information about modules, see [Modules in Adobe Workfront Fusion](../../workfront-fusion/modules/modules.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
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

To use Azure Active Directory modules, you must have an Azure Active Directory account.

## Azure Active Directory modules and their fields

When you configure Azure Active Directory modules, Workfront Fusion displays the fields listed below. Along with these, additional Azure Active Directory fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers) 
* [Actions](#actions) 
* [Searches](#searches)

### Triggers {#triggers}

#### Watch records (scheduled)

This polling (scheduled) trigger module executes a scenario when a record in a selected object has been created

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
or updated
</MadCap:conditionalText>
-->

since the last scheduled run in Azure Active Directory. It also returns all standard fields associated with the record or records, along with any custom fields and values that the connection accesses.You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Azure Active Directory account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Filter</td> 
    <td> <p>Specify whether you want to include<!--
       <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
         New Records Only, Updated Records Only, or both
       </MadCap:conditionalText>
      --> New and Updated Records. <!--
       <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Only "New or updated records" is visible.</span>
      --></p> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">Type</td> 
   <td>Select whether you want to watch User records or Group records.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Maximum Number of Records</td> 
   <td>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</td> 
  </tr> 
 </tbody> 
</table>

### Actions {#actions}

* [Read Record](#read-record) 
* [Create Record](#create-record) 
* [Custom API Call](#custom-api-call)

#### Read Record {#read-record}

This action module reads data from a single record in Azure Active Directory.

You specify the ID of the record.

The module returns the ID of the record and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

You must have sufficient permissions to access the record in Azure Active Directory in order to retrieve this information.

When you are configuring this module, the following fields display.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Azure Active Directory account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td>Select whether you want to read a User record or a Group record.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Outputs</td> 
   <td>Select the information you want included in the output bundle for this module.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">ID</td> 
   <td>Enter or map the unique Azure Active Directory ID of the record that you want the module to read.</td> 
  </tr> 
 </tbody> 
</table>

#### Create Record {#create-record}

This action module creates a new user or group record.

You specify the type of the record you want.

The module returns the ID of the  record and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Azure Active Directory account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Record Type</td> 
   <td>Select whether you want to read a User record or a Group record.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Other Fields</td> 
   <td>Fill in these fields to set the values for the new record.</td> 
  </tr> 
 </tbody> 
</table>

#### Custom API Call {#custom-api-call}

This action module lets you make a custom authenticated call to the Azure Active Directory API. This way, you can create a data flow automation that can't be accomplished by the other Azure Active Directory modules.

When you are configuring this module, the following fields display.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Azure Active Directory account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>Enter or map a path relative to <code>https://graph.microsoft.com/{version}/{resource}?{query-parameters}</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Method</td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods</a>.</p> </td> 
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

### Searches {#searches}

* [Search Users](#search-users) 
* [Search Users/Groups Delta](#search-users-groups-delta)

#### Search Users {#search-users}

This search module looks for records in an object in Azure Active Directory that match the search query you specify. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Azure Active Directory account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Search Criteria</td> 
   <td> <p>Enter the criteria that you want to use in your search.</p> <p>For information about the parameters to use, such as "$filter, see <a href="https://docs.microsoft.com/en-us/graph/query-parameters">Use query parameters to customize responses</a> in the Microsoft API&nbsp;documentation.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Outputs</td> 
   <td>Select the information you want included in the output bundle for this module.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Maximal count of records</td> 
   <td>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</td> 
  </tr> 
 </tbody> 
</table>

#### Search Users/Groups Delta  {#search-users-groups-delta}

This search module looks for records in Azure AD that have been created, updated, or deleted.You can map this information in subsequent modules in the scenario.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Azure Active Directory account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Limit</td> 
   <td>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</td> 
  </tr> 
 </tbody> 
</table>

