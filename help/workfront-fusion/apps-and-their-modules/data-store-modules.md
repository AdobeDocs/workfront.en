---
filename: data-store-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Data store modules
description: A data store, similar to a database or a simple table, can store data from scenarios, making it possible to transfer data between individual scenarios or scenario runs. You can use a data store to store new data from various systems during synchronization.
---

# Data store modules

A data store, similar to a database or a simple table, can store data from scenarios, making it possible to transfer data between individual scenarios or scenario runs. You can use a data store to store new data from various systems during synchronization.

The data store modules enable you to add, replace, update, retrieve, delete, search, or count records in your *Adobe Workfront Fusion* data store.

For information on creating, editing, and troubleshooting data stores, see [Data Stores](../../workfront-fusion/modules/data-stores.md)

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p><em>Pro</em> or higher</p> </td> 
  </tr> <draft-comment>
   <tr data-mc-conditions=""> 
    <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
    <td> <p>Plan, Work</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions=""> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p>Plan, Work</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront Fusion</em> license**</td> 
   <td> <p><em>Workfront Fusion for Work Automation and Integration</em> </p> <draft-comment>
     <p data-mc-conditions="SnippetConditions.HIDE"><em>Workfront Fusion for Work Automation</em> </p>
    </draft-comment><p data-mc-conditions="SnippetConditions.HIDE"><em>Workfront Fusion for Work Automation</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase <em>Adobe Workfront Fusion</em> as well as <em>Adobe Workfront</em> to use functionality described in this article.</td> 
  </tr> <draft-comment>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <draft-comment>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your organization.</p>
     </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your organization.</p> <draft-comment>
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your team.</p>
     </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your team.</p> </td> 
   </tr>
  </draft-comment>
  <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your organization.</p> <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a <em>Workfront Fusion</em> administrator for your team.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

&#42;&#42;For information on *Adobe Workfront Fusion* licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisites

To use Data Store modules, you must first create a data store.

For information on creating data stores, see [Data Stores](../../workfront-fusion/modules/data-stores.md)

## Data Store modules and their fields

When you configure *Data Store* modules, *Workfront Fusion* displays the fields listed below. Along with these, additional *Data Store* fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

All Data Store modules are Action type modules.

* [Add/Replace a Record](#add/repl) 
* [Update a Record](#update) 
* [Get a Record](#get) 
* [Check the Existence of a Record](#check) 
* [Delete a Record](#delete) 
* [Delete All Records](#delete2) 
* [Search Records](#search) 
* [Count Records](#count)

### Add/Replace a Record

This action module *adds or replaces a record*

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
in
<em>Data Store</em>
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <em>Data Store</em></MadCap:conditionalText>`.

You specify the data store and the record's key.

The module returns the ID of the 

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
<em>new or replaced</em>
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  <em>new or replaced</em></MadCap:conditionalText>` *record* and any associated fields, along with any custom fields and values that the connection accesses. You can map *this information* in subsequent modules in the scenario.

>[!NOTE]
>
>The module throws an error when you try to add the record which is already in the data store under the same name and the Overwrite an existing record option is disabled.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Data Store</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Data Store</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Data store</td> 
   <td> <p> Select or add the data store where you want to create a record. </p> </td> 
  </tr> 
  <tr> 
   <td>Key </td> 
   <td> <p>Enter the unique key of the record you want the module to add or replace. The key can be used later to retrieve the record. If you leave this field blank, a key is generated automatically.</p> </td> 
  </tr> 
  <tr> 
   <td>Overwrite an existing record </td> 
   <td> <p>Enable this option to overwrite the record. The record you want to overwrite must be specified in the Key field above.</p> </td> 
  </tr> 
  <tr> 
   <td>Record </td> 
   <td> <p>Enter the desired values to the record's fields.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Update a Record

This action module *updates a record*

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
in
<em>Data Store</em>
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <em>Data Store</em></MadCap:conditionalText>`.

You specify the data store and the record's key.

The module returns the ID of the 

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
<em>updated</em>
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  <em>updated</em></MadCap:conditionalText>` *record* and any associated fields, along with any custom fields and values that the connection accesses. You can map *this information* in subsequent modules in the scenario.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Data Store</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Data Store</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Data store</td> 
   <td> <p> Select or add the data store where you want to create a record. </p> </td> 
  </tr> 
  <tr> 
   <td>Key </td> 
   <td> <p>Enter the unique key of the record you want the module to update.</p> </td> 
  </tr> 
  <tr> 
   <td>Insert missing record </td> 
   <td> <p>Enable this option to create a new record if the record with the specified key doesn't already exist.</p> </td> 
  </tr> 
  <tr> 
   <td>Record</td> 
   <td> <p> Enter the desired values to the record's fields that you want to update.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Get a Record

This action module *retrieves a record*

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
in
<em>Data Store</em>
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <em>Data Store</em></MadCap:conditionalText>`.

You specify the data store and the record's key.

The module returns the ID of the *record* and any associated fields, along with any custom fields and values that the connection accesses. You can map *this information* in subsequent modules in the scenario.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Data store</td> 
   <td> <p> Select the data store you want to retrieve a record from</p> </td> 
  </tr> 
  <tr> 
   <td>Key </td> 
   <td> <p>Enter the unique key of the record you want the module to retrieve.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Check the Existence of a Record

This action module *specifies whether a particular record exists*

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
in
<em>Data Store</em>
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <em>Data Store</em></MadCap:conditionalText>`.

You specify the data store and the record's key.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The module returns the ID of the <em>record</em> and a True or False value. It also returns any associated fields, along with any custom fields and values that the connection accesses. You can map <em>this information</em> in subsequent modules in the scenario.</p>
-->

The module returns the ID of the *record* and a True or False value. It also returns any associated fields, along with any custom fields and values that the connection accesses. You can map *this information* in subsequent modules in the scenario.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Data store </td> 
   <td> <p>Select the data store you want to check for the record existence.</p> </td> 
  </tr> 
  <tr> 
   <td>Key </td> 
   <td> <p>Enter the unique key of the record you want the module to check for existence.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Delete a Record

This action module *deletes a record*

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
in
<em>Data Store</em>
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  in  <em>Data Store</em></MadCap:conditionalText>`.

You specify the data store and the record's key.

The module returns the ID of the 

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
<em>deleted</em>
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">  <em>deleted</em></MadCap:conditionalText>` *record* and any associated fields, along with any custom fields and values that the connection accesses. You can map *this information* in subsequent modules in the scenario.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Data store </td> 
   <td> <p>Select the data store you want to check for the record existence.</p> </td> 
  </tr> 
  <tr> 
   <td>Key </td> 
   <td> <p>Enter the unique key of the record you want the module to delete.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Delete All Records

This action module *deletes all records from a particular data store*.

You specify the data store.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The module returns the IDs of the deleted records and any associated fields, along with any custom fields and values that the connection accesses. You can map <em>this information</em> in subsequent modules in the scenario.</p>
-->

The module returns the IDs of the deleted records and any associated fields, along with any custom fields and values that the connection accesses. You can map *this information* in subsequent modules in the scenario.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Data store </td> 
   <td> <p>Select the data store you want to delete all records from.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Search Records

This search module looks for *records in an object* in *Data Store* that match the search query you specify.

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
The module
<em>returns all standard fields associated with the record or records, along with any custom fields and values that the connection accesses</em>.
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> The module  <em>returns all standard fields associated with the record or records, along with any custom fields and values that the connection accesses</em>.</MadCap:conditionalText>` You can map *this information* in subsequent modules in the scenario.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Data Store</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Data Store</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Data store</td> 
   <td> <p> Select the data store you want to search.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Filter</p> </td> 
   <td> <p>Set the filter for the search.</p> <draft-comment>
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the column, operator and required value (search term) for the search.</p>
    </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the column, operator and required value (search term) for the search.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Sort</p> </td> 
   <td> <p style="font-weight: normal;">For each field that you want to sort by, fill in the following fields:</p> <p style="font-weight: bold;">Key</p> <p>Select the column name you want to sort the results by.</p> <p style="font-weight: bold;">Order</p> <p>Select whether you want to sort results in the ascending or descending order.</p> </td> 
  </tr> 
  <tr> 
   <td>Limit</td> 
   <td> <p> Set the maximum number of search results <em>Workfront Fusion</em> returns during one execution cycle.</p> </td> 
  </tr> 
  <tr> 
   <td>Continue the execution of the route even if the module returns no results</td> 
   <td> <p> If enabled, the route that this module is part of continues processing even if this module returns no results..</p> </td> 
  </tr> 
 </tbody> 
</table>

### Count Records

This action module *numbers the records in a data store*.

You specify the data store.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The module returns the number of records and any associated fields, along with any custom fields and values that the connection accesses. </p>
-->

The module returns the number of records and any associated fields, along with any custom fields and values that the connection accesses.

When you are configuring this module, the following fields display

<!--
<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE">
, along with any other available
<em>Data Store</em> fields, depending on the connection and options you choose
</MadCap:conditionalText>
-->

`<MadCap:conditionalText data-mc-conditions="SnippetConditions.HIDE"> , along with any other available  <em>Data Store</em> fields, depending on the connection and options you choose</MadCap:conditionalText>`.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Data store </td> 
   <td> <p>Select the data store that contains the records you want to count.</p> </td> 
  </tr> 
 </tbody> 
</table>

