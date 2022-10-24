---
title: Widen modules
description: Widen modules
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: d46935bc-4f6c-4502-bd2f-3927f33241e1
---
# Widen modules

In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use [!UICONTROL Widen], as well as connect it to multiple third-party applications and services.

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
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisites

To use [!UICONTROL Widen] modules, you must have a [!UICONTROL Widen] account.

## Connect Widen to Workfront Fusion  {#connect-widen-to-workfront-fusion}

You can create a connection to your [!DNL Widen] account directly from inside a [!DNL Widen] module.

1. In any Widen module, click **[!UICONTROL Add]** next to the Connection field.
1. Select the Widen domain that you want to connect to.
1. Enter the token for your [!DNL Widen] account. For instructions on locating this token, see the [[!DNL Widen] API FAQs](https://community.widen.com/collective/s/article/API-FAQs).
1. Click **[!UICONTROL Continue]** to create the connection and go back to the module.

## Widen modules and their fields

When you configure Widen modules, [!DNL Workfront Fusion] displays the fields listed below. Along with these, additional Widen fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Trigger modules](#trigger-modules)
* [Action Modules](#action-modules)
* [Search Modules](#search-modules)

### Trigger modules {#trigger-modules}

#### Watch assets

This trigger module starts a scenario when an asset is created or updated.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Widen] account to [!DNL Workfront] Fusion, see <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect Widen to Workfront Fusion] </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Event type</td> 
   <td> <p>Select whether you want to watch new assets or updated assets.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Expand</td> 
   <td> <p>Select the properties that you want to include in the module output in addition to the asset fields.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Outputs</td> 
   <td>Select the fields that you want to include in the module output.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>Enter or map the maximum number of assets you want the module to work with during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Action Modules {#action-modules}

* [Custom API Call](#custom-api-call)
* [Read asset info](#read-asset-info)
* [Add assets to collections](#add-assets-to-collections)
* [Remove assets from collection](#remove-assets-from-collection)
* [Update asset metadata](#update-asset-metadata)
* [Download File](#download-file)
* [[!UICONTROL Upload] a file](#upload-a-file)

#### Custom API Call {#custom-api-call}

This action module lets you make a custom authenticated call to the [!DNL Widen] API. This way, you can create a data flow automation that can't be accomplished by the other [!DNL Widen] modules.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Widen] account to [!DNL Workfront] Fusion, see <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect Widen to Workfront Fusion] </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API Version</td> 
   <td>Select whether you want to use the latest version of the Widen API, or Version 1.0</td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>Enter or map the URL for your API call.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Method</td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP request methods in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Add the headers of the request in the form of a standard [!DNL JSON] object.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion 2.0 adds the authorization headers for you.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query String</td> 
   <td> <p>Add the query for the API call in the form of a standard JSON object.</p> <p>For example: <code>{“name”:“something-urgent”}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Add the body content for the API call in the form of a standard [!DNL JSON] object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### Read asset info {#read-asset-info}

This action module retrieves an individual asset by its unique ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Widen] account to [!DNL Workfront] Fusion, see <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect Widen to Workfront Fusion] </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Asset ID</td> 
   <td> <p>Enter or map the ID of the asset you want to read information for.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Expand</td> 
   <td> <p>Select the properties that you want to include in the module output in addition to the asset fields.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Outputs</td> 
   <td>Select the fields that you want to include in the module output.</td> 
  </tr> 
 </tbody> 
</table>

#### Add assets to collections {#add-assets-to-collections}

This action module adds one or more assets to collections.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Widen] account to [!DNL Workfront] Fusion, see <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect Widen to Workfront Fusion] </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Collections ID</td> 
   <td> <p>For each collection that you want to add the assets to:</p> 
    <ol> 
     <li value="1"> <p> Click <strong>Add</strong>.</p> </li> 
     <li value="2"> <p>Enter or map the Collection ID.</p> </li> 
     <li value="3"> <p>Click <strong>Add item</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Assets ID</td> 
   <td> <p>For each asset that you want to add to a collection:</p> 
    <ol> 
     <li value="1"> <p> Click <strong>Add</strong>.</p> </li> 
     <li value="2"> <p>Enter or map the Asset ID.</p> </li> 
     <li value="3"> <p>Click <strong>Add item</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>Enter or map the maximum number of assets you want the module to work with during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Remove assets from collection {#remove-assets-from-collection}

This action module removes one or more assets from collections.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Widen] account to [!DNL Workfront] Fusion, see <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect Widen to Workfront Fusion] </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Collections ID</td> 
   <td> <p>For each collection that you want to remove the assets from:</p> 
    <ol> 
     <li value="1"> <p> Click <strong>Add</strong>.</p> </li> 
     <li value="2"> <p>Enter or map the Collection ID.</p> </li> 
     <li value="3"> <p>Click <strong>Add item</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Assets ID</td> 
   <td> <p>For each asset that you want to remove from a collection:</p> 
    <ol> 
     <li value="1"> <p> Click <strong>Add</strong>.</p> </li> 
     <li value="2"> <p>Enter or map the Asset ID.</p> </li> 
     <li value="3"> <p>Click <strong>Add item</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>Enter or map the maximum number of assets you want the module to work with during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Update asset metadata {#update-asset-metadata}

This action module updates the metadata fields of an asset.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Widen] account to [!DNL Workfront] Fusion, see <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect Widen to Workfront Fusion] </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Asset ID</td> 
   <td> <p>Enter or map the ID of the asset where you want to update metadata.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Metadata type</td> 
   <td> <p>Select the [!UICONTROL metadata type] for the metadata you want to update.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Metadata</td> 
   <td>Select the metadata fields that you want to update. For each field, enter the new value for the field.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>Enter or map the maximum number of assets you want the module to work with during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Download File {#download-file}

This action module downloads an asset from your [!DNL Widen] account.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Widen] account to [!DNL Workfront] Fusion, see <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect Widen to Workfront Fusion] </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Asset ID</td> 
   <td> <p>Enter or map the ID of the asset you want to download.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Upload a file {#upload-a-file}

This action module uploads a file into your [!DNL Widen] account.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Widen] account to [!DNL Workfront] Fusion, see <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect Widen to Workfront Fusion] </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Upload Profile</td> 
   <td> <p>Select the upload profile that you want the module to use.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Upload Method</td> 
   <td> <p>Select how you want to upload the file.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL From File]</strong> </p> <p>Select or map the source file from a previous module.</p> </li> 
     <li> <p><strong>By URL</strong> </p> <p>Enter or map the URL of the file that you want to upload.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">File name</td> 
   <td>Enter or map a name for the uploaded file.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Metadata Type</td> 
   <td>Select the metadata type for the file you want to upload.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Metadata</td> 
   <td>Select the metadata fields that you want to include in the file upload. For each field, enter the [!UICONTROL value] for the field.</td> 
  </tr> 
 </tbody> 
</table>

### Search Modules {#search-modules}

* [Read collection assets](#read-collection-assets)
* [Search assets](#search-assets)

#### Read collection assets {#read-collection-assets}

This action module retrieves a list of assets within a collection.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Widen] account to [!DNL Workfront] Fusion, see <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect Widen to Workfront Fusion] </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Collection ID</td> 
   <td> <p>Enter or map the ID of the collection that contains the assets you want to read.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Start</td> 
   <td>Enter or map the number of the first item you want to list. This is a way to paginate the records.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Max</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sort By</td> 
   <td> <p>Select the property by which you want to sort the assets. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Order</td> 
   <td>Select whether you want to sort assets ascending or descending.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Outputs</td> 
   <td>Select the fields that you want to include in the module output.</td> 
  </tr> 
 </tbody> 
</table>

#### Search assets {#search-assets}

This search module retrieves a list of assets that match the specific search criteria.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Widen] account to [!DNL Workfront] Fusion, see <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect Widen to Workfront Fusion] </a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Search query</td> 
   <td> <p>Enter the criteria by which you want to search assets.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sort By</td> 
   <td> <p>Select how you want to sort the assets. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Order</td> 
   <td>Select whether you want to sort assets ascending or descending.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Include deleted</td> 
   <td>Enable this option to include deleted assets in the search.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Include archived</p> </td> 
   <td> <p>Enable this option to include archived assets in the search.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Search document text</td> 
   <td>Enable this option to include document text in your search, or false to include only assets for which the title matches the search criteria.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Offset</td> 
   <td>Enter or map the number of the first item you want to retrieve details for. This is a way to paginate the records.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Scroll</td> 
   <td>Enable this option to allow scrolling.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Expand</td> 
   <td> <p>Select the properties that you want to include in the module output in addition to the asset fields.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Outputs</td> 
   <td>Select the fields that you want to include in the module output.</td> 
  </tr> 
 </tbody> 
</table>
