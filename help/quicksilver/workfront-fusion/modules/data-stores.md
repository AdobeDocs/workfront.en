---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Data Stores in [!DNL Adobe Workfront Fusion]
description: A data store, similar to a database or a simple table, can store data from scenarios, making it possible to transfer data between individual scenarios or scenario runs. You can use a data store to store new data from various systems during synchronization.
author: Becky
feature: Workfront Fusion
exl-id: 2a665a71-b819-4861-b119-f5c28b87e9c5
---
# Data Stores in [!DNL Adobe Workfront Fusion]

A data store, similar to a database or a simple table, can store data from scenarios, making it possible to transfer data between individual scenarios or scenario runs. You can use a data store to store new data from various systems during synchronization.

The data store modules enable you to take the following actions on records in your [!DNL Adobe Workfront Fusion] data store:

* Add
* Replace
* Update
* Retrieve
* Delete
* Search
* Count

For information on using data store modules, see [[!UICONTROL Data store] modules](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

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

## Create a data store in [!DNL Workfront Fusion]

* [Set up the data store](#set-up-the-data-store)
* [Set up the data structure](#set-up-the-data-structure)

### Set up the data store

Before you can use a data store in a module, you must create the data store in [!DNL Workfront Fusion].

>[!NOTE]
>
>Your organization has a limited number of available data stores. If you attempt to create more data stores than you have available, [!DNL Workfront] returns a [!UICONTROL Maximum stores reached] error.
>
>For more information, see [Maximum stores reached error](#maximum-stores-reached-error) in this article.

1. Log in to your [!DNL Workfront Fusion] account.
1. Click **[!UICONTROL Data stores]** in the left navigation panel.
1. Click **[!UICONTROL Add data store]** in the upper-right corner of the screen.
1. Enter settings for the new data store.

   A bolded title on a field in a [!DNL Workfront Fusion] module indicates a required setting.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Data store name] </td> 
      <td> <p>Enter a name for the data store. </p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Data Structure]</p> </td> 
      <td> <p>A data structure is a list of the columns for a table. This list indicates the column name and data type.</p> <p>Do one of the following:</p> 
       <ul> 
        <li style="font-weight: bold;">Select a data structure that has been already created</li> 
        <li> <p style="font-weight: bold;">Add a new data structure</p> <p>Click <strong>[!UICONTROL Add]</strong> to create a new data structure.</p> <p>For more information, see the <a href="#set-up-the-data-structure" class="MCXref xref">Set up the data structure</a> section in this article.</p> </li> 
        <li style="font-weight: bold;"> <p>Leave the field empty</p> <p style="font-weight: normal;">If you don't select or add a data structure, the database will only contain the primary key. Such a database type is useful if you want to save keys only and are interested in knowing only whether or not a specific key exists in the database.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Data storage size in MB]</p> </td> 
      <td> <p>Allocate the size for the data store from your total internal data storage.</p> <p> The default value is 10 MB. If you have less than 10 MB of unallocated Data Store space from your 500 MB allotment, the default size is the amount of unallocated storage.  <p>Note: The reserved amount can be changed at any time.</p>  </td> 
     </tr> 
    </tbody> 
   </table>

### Set up the data structure 

1. When creating or editing a data store, click **[!UICONTROL Add]**.
1. In the **[!UICONTROL Add data structure]** box that displays, configure the following fields:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Data structure name]</td> 
      <td> <p> Enter a name for the new data structure.</p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Specification]</p> </td> 
      <td> <p>Do one of the following to set up your data store's columns.</p> 
       <ul> 
        <li> <p>Click <strong>[!UICONTROL Add item]</strong> to specify the properties of one column manually.</p> <p>Enter the <strong>[!UICONTROL Name]</strong> and <strong>[!UICONTROL Type]</strong> for the data store column and define corresponding properties.</p> </li> 
        <li> <p>Click <strong>[!UICONTROL Generator]</strong> to determine the columns from the sample data you provide.</p> 
         <div class="example" data-mc-autonum="<b>Example: </b>">
          <span class="autonumber"><span><b>Example: </b></span></span> 
          <p>For example, the following JSON sample data creates three columns: name, age, and phone number. Phone number is a collection of mobile and landline phone numbers.</p> 
          <p><code>&lbrace;</code> </p> 
          <p><code>"name":"John",</code> </p> 
          <p><code>"age":30,</code> </p> 
          <p><code>"phone number": &lbrace;</code> </p> 
          <p><code>"mobile":"987654321",</code> </p> 
          <p><code>"landline":"123456789"</code> </p> 
          <p><code>&rbrace;</code> </p> 
          <p><code>&rbrace;</code> </p> 
          <p>The empty columns in the data store view:</p> 
          <p> <img src="assets/empty-columns-350x132.png" style="width: 350;height: 132;"> </p> 
          <p>You can then add values to the data store manually or by using the [!DNL Workfront Fusion] data store modules.</p> 
         </div> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Strict] </td> 
      <td> <p>Enable this option to ensure that the payload matches the data structures. Payloads that contain extra items not specified in the data structure are rejected.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Edit an existing data store

You can edit the properties and contents of an existing Data Store in the [!UICONTROL Data Store] area of [!DNL Workfront Fusion].

* [Edit the properties of a data store](#edit-the-properties-of-a-data-store)
* [Edit the contents of a data store](#edit-the-contents-of-a-data-store)

### Edit the properties of a data store 

The properties of a data store include the data structure that the data store uses, as well as the data store's size.

1. Click **[!UICONTROL Data Store]** ![](assets/data-store-icon.png) in the left navigation panel to open the [!UICONTROL Data Store] area.
1. Click **[!UICONTROL Edit]** ![](assets/data-store-edit.png) next to the data store that you want to edit.
1. (Optional) If you want to change the data structure used by this data store to another existing data structure, select it from the **[!UICONTROL Data structure]** drop-down.

   Or

   (Optional) If you want to change the data structure used by this data store to an entirely new data structure, see [Set up the data structure](#set-up-the-data-structure) in this article.

1. (Optional) Change the size of the data store by entering the new size into the **[!UICONTROL Data storage size in MB]** field.
1. Click **[!UICONTROL Save]**.

### Edit the contents of a data store 

1. Click the **[!UICONTROL Data Store]** icon ![](assets/data-store-icon.png) in the left navigation panel to open the [!UICONTROL Data Store] area.
1. Click **[!UICONTROL Browse]**  next to the data store that you want to edit.
1. (Optional) Reorder columns by dragging them to the desired location.
1. (Optional) [!UICONTROL Edit] a single cell by clicking the **[!UICONTROL Edit]** icon in that cell, then entering the desired value.
1. (Optional) Add a new item to the data store by clicking **[!UICONTROL Add]**, then entering the information for the new item.
1. Click **[!UICONTROL Save]**.

## Troubleshooting

* [Restoring lost data from a data store](#restoring-lost-data-from-a-data-store)
* [Out of space error](#out-of-space-error)
* [Maximum stores reached error](#maximum-stores-reached-error)

### Restoring lost data from a data store 

There is currently no tool which can automate restoring lost data.

#### Workaround

1. Examine all execution logs of scenarios where items were inserted to the data store.

   For more information on examining execution logs, see [View a scenario's execution history in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-scenario-execution-history.md).

1. Copy the data.
1. Insert the data into your data store again.

   For information on inserting data into a data store, see [Edit the contents of a data store](#edit-the-contents-of-a-data-store) in this article.

### [!UICONTROL Out of space] error

An [!UICONTROL Out of Space] error occurs because your previously created data stores have already been assigned your allocated data store storage.

#### Workaround

1. Edit any of your existing data stores to use less space. This frees up space for your new data store.

   For more information, see [Edit the properties of a data store](#edit-the-properties-of-a-data-store) in this article.

>[!NOTE]
>
>We recommend that you do not assign all of your space to a single data store unless you are certain you will not require more data stores.

### [!UICONTROL Maximum stores reached] error 

A [!UICONTROL Maximum stores reached] error occurs because your organization has used all of its available data stores. An organization has a number of available data stores equal to twice the number of available scenarios. Therefore, the total number of available data stores depends on the plan you have purchased.

For example, if your organization has purchased a plan with 15 scenarios, the organization can have up to 30 data stores.

#### Workaround

To reduce the number of existing data stores, consider doing one of the following:

* Combine existing data stores
* Delete unused data stores
