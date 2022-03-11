---
filename: data-stores
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Data Stores
description: A data store, similar to a database or a simple table, can store data from scenarios, making it possible to transfer data between individual scenarios or scenario runs. You can use a data store to store new data from various systems during synchronization.
---

# Data Stores

A data store, similar to a database or a simple table, can store data from scenarios, making it possible to transfer data between individual scenarios or scenario runs. You can use a data store to store new data from various systems during synchronization.

<!--
For more information on scenarios, see Create a scenario
-->

The data store modules enable you to take the following actions on records in your `Adobe Workfront Fusion` data store:

* Add
* Replace
* Update
* Retrieve
* Delete
* Search
* Count

For information on using data store modules, see [Data store modules](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p><span>Pro</span> or higher</p> </td> 
  </tr> Adobe Workfront license* Plan, Work 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront Fusion</span> license**</td> 
   <td> <p><span>Workfront Fusion for Work Automation and Integration</span> </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase <span>Adobe Workfront Fusion</span> as well as <span>Adobe Workfront</span> to use functionality described in this article.</td> 
  </tr> <!--
   Access level configurations* You must be a Workfront Fusion administrator for your organization. You must be a Workfront Fusion administrator for your team.
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

&#42;&#42;For information on `Adobe Workfront Fusion` licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Create a data store in `Workfront Fusion`

* [Set up the data store](#set) 
* [Set up the data structure](#setting)

### Set up the data store

Before you can use a data store in a module, you must create the data store in `Workfront Fusion`.

>[!NOTE]
>
>Your organization has a limited number of available data stores. If you attempt to create more data stores than you have available, Workfront returns a Maximum stores reached error.
>
>For more information, see [Maximum stores reached error](#maximum) in this article.

<ol> 
 <li value="1">Log in to your <span>Workfront Fusion</span> account.</li> 
 <li value="2">Click <span class="bold">Data stores</span> in the left navigation panel.</li> 
 <li value="3">Click <span class="bold">Add data store</span> in the upper-right corner of the screen.</li> 
 <li value="4"> <p>Enter settings for the new data store.</p> <p>A bolded title on a field in a <span>Workfront Fusion</span> module indicates a required setting.</p> 
  <table cellspacing="15"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td>Data store name </td> 
     <td> <p>Enter a name for the data store. </p> </td> 
    </tr> 
    <tr> 
     <td> <p>Data Structure</p> </td> 
     <td> <p>A data structure is a list of the columns for a table. This list indicates the column name and data type.</p> <p>Do one of the following:</p> 
      <ul> 
       <li style="font-weight: bold;">Select a data structure that has been already created</li> 
       <li> <p style="font-weight: bold;">Add a new data structure</p> <p>Click the <span class="bold">Add</span> button to create a new data structure.</p> <p>For more information, see the <a href="#setting" class="MCXref xref">Set up the data structure</a> section in this article.</p> </li> 
       <li style="font-weight: bold;"> <p>Leave the field empty</p> <p style="font-weight: normal;">If you don't select or add a data structure, the database will only contain the primary key. Such a database type is useful if you want to save keys only and are interested in knowing only whether or not a specific key exists in the database.</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td> <p>Data storage size in MB</p> </td> 
     <td> <p>Allocate the size for the data store from your total internal data storage.</p> <note type="note">
       The reserved amount can be changed at any time later on.
      </note> <!--
       The total internal data storage capacity depends on the plan you have purchased.
      --> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
</ol>

### Set up the data structure

<ol> 
 <li value="1">When creating or editing a data store, click <span class="bold">Add</span>.</li> 
 <li value="2"> <p>In the <span class="bold">Add data structure</span> box that displays, configure the following fields:</p> 
  <table cellspacing="15"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td>Data structure name</td> 
     <td> <p> Enter a name for the new data structure.</p> </td> 
    </tr> 
    <tr> 
     <td> <p>Specification</p> </td> 
     <td> <p>Do one of the following to set up your data store's columns.</p> 
      <ul> 
       <li> <p>Click <span class="bold">Add item</span> to specify the properties of one column manually.</p> <p>Enter the <span class="bold">Name </span>and <span class="bold">Type </span>for the data store column and define corresponding properties.</p> </li> 
       <li> <p>Click <span class="bold">Generator </span>to determine the columns from the sample data you provide.</p> 
        <div class="example" data-mc-autonum="<b>Example: </b>">
         <span class="autonumber"><span><b>Example: </b></span></span> 
         <p>For example, the following JSON sample data creates three columns: name, age, and phone number. Phone number is a collection of mobile and landline phone numbers.</p> 
         <p><code>{</code> </p> 
         <p><code>"name":"John",</code> </p> 
         <p><code>"age":30,</code> </p> 
         <p><code>"phone number": {</code> </p> 
         <p><code>"mobile":"987654321",</code> </p> 
         <p><code>"landline":"123456789"</code> </p> 
         <p><code>}</code> </p> 
         <p><code>}</code> </p> 
         <p>The empty columns in the data store view:</p> 
         <p> <img src="assets/empty-columns-350x132.png" style="width: 350;height: 132;"> </p> 
         <p>You can then add values to the data store manually or by using the <span>Workfront Fusion</span> data store modules.</p> 
        </div> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td>Strict </td> 
     <td> <p>Enable this option to ensure that the payload matches the data structures. Payloads that contain extra items not specified in the data structure are rejected.</p> </td> 
    </tr> 
   </tbody> 
  </table> </li> 
</ol>

## Edit an existing data store

You can edit the properties and contents of an existing Data Store in the Data Store area of `Workfront Fusion`.

* [Edit the properties of a data store](#edit) 
* [Edit the contents of a data store](#edit2)

### Edit the properties of a data store

The properties of a data store include the data structure that the data store uses, as well as the data store's size.

<ol> 
 <li value="1"> <p>Click <span class="bold">Data Store</span> <img src="assets/data-store-icon.png"> in the left navigation panel to open the Data Store area.</p> </li> 
 <li value="2"> <p>Click <span class="bold">Edit </span><img src="assets/data-store-edit.png">next to the data store that you want to edit.</p> </li> 
 <li value="3"> <p>(Optional) If you want to change the data structure used by this data store to another existing data structure, select it from the <span class="bold">Data structure</span> drop-down.</p> <p>Or</p> <p>(Optional) If you want to change the data structure used by this data store to an entirely new data structure, see <a href="#setting" class="MCXref xref">Set up the data structure</a> in this article.</p> </li> 
 <li value="4"> <p>(Optional) Change the size of the data store by entering the new size into the <span class="bold">Data storage size in MB</span> field.</p> </li> 
 <li value="5"> <p>Click <span class="bold">Save</span>.</p> </li> 
</ol>

### Edit the contents of a data store

<ol> 
 <li value="1"> <p>Click the <span class="bold">Data Store</span> icon <img src="assets/data-store-icon.png"> in the left navigation panel to open the Data Store area.</p> </li> 
 <li value="2"> <p>Click <span class="bold">Browse </span><img src="assets/browse-data-store.png"> next to the data store that you want to edit.</p> </li> 
 <li value="3"> <p>(Optional) Reorder columns by dragging them to the desired location.</p> </li> 
 <li value="4"> <p>(Optional) Edit a single cell by clicking the <span class="bold">Edit</span> icon <img src="assets/data-store-edit.png">in that cell, then entering the desired value.</p> </li> 
 <li value="5"> <p>(Optional) Add a new item to the data store by clicking <span class="bold">Add</span>, then entering the information for the new item.</p> </li> 
 <li value="6"> <p>Click <span class="bold">Save</span>.</p> </li> 
</ol>

## Troubleshooting

* [Restoring lost data from a data store](#about) 
* [Out of space error](#out) 
* [Maximum stores reached error](#maximum)

### Restoring lost data from a data store

There is currently no tool which can automate restoring lost data.

#### Workaround

1. Examine all execution logs of scenarios where items were inserted to the data store.

   For more information on examining execution logs, see [View a scenario's execution history](../../workfront-fusion/scenarios/view-scenario-execution-history.md).

1. Copy the data.
1. Insert the data into your data store again.

   For information on inserting data into a data store, see [Edit the contents of a data store](#edit2) in this article.

### Out of space error

An Out of Space error occurs because your previously created data stores have already been assigned your allocated data store storage.

#### Workaround

1. Edit any of your existing data stores to use less space. This frees up space for your new data store.

   For more information, see [Edit the properties of a data store](#edit) in this article.

>[!NOTE]
>
>We recommend that you do not assign all of your space to a single data store unless you are certain you will not require more data stores.

### Maximum stores reached error

A Maximum stored reached error occurs because your organization has used all of its available data stores. An organization has a number of available data stores equal to twice the number of available scenarios. Therefore, the total number of available data stores depends on the plan you have purchased.

For example, if your organization has purchased a plan with 15 scenarios, the organization can have up to 30 data stores.

#### Workaround

To reduce the number of existing data stores, consider doing one of the following:

* Combine existing data stores
* Delete unused data stores

