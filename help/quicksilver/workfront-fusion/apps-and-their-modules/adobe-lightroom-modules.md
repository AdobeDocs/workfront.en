---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Adobe Lightroom modules
description: With the Adobe Lightroom modules, you can start an Adobe Workfront Fusion scenario based on events in your Adobe Lightroom account.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
---
# [!DNL Adobe Lightroom] modules

In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use [!DNL Adobe Lightroom], as well as connect it to multiple third-party applications and services. 

If you need instructions on creating a scenario, see [Create a scenario](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
      <td>
        <p>[!UICONTROL Pro] or higher</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] license*</td>
      <td>
        <p>[!UICONTROL Plan], [!UICONTROL Work]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td>
      <td >
        <p>[!UICONTROL Workfront Fusion for Work Automation and Integration]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Product</td>
      <td>Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</td>
    </tr>
    </tr>
  </tbody>
</table>


&#42;To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

&#42;&#42;For information on [!DNL Adobe Workfront Fusion] licenses, see [!DNL [Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisites

Before you can use the [!DNL Adobe Lightroom] connector, you must ensure that the following prerequisites are met:

* You must have an active [!DNL Adobe Lightroom] account.

## Create a connection to Adobe Lightroom



## Adobe Lightroom modules and their fields

### Other

#### Health check

This action module retrieves a Lightroom server version ID, proving whether the Lightroom service is currently running.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Lightroom], see <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Create a connection to [!DNL Adobe Lightroom]</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Credentials]</td>
      <td>
        <p>If you want to supply specific credentials to ensure that a specific server is running, click Add item and enter the credentials.</p><p>Authorization headers are added automatically.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Retrieve user catalog metadata

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Lightroom], see <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Create a connection to [!DNL Adobe Lightroom]</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Credentials]</td>
      <td>
        <p>If you want to supply specific credentials to ensure that you can access the correct user account, click Add item and enter the credentials.</p><p>Authorization headers are added automatically.</p>
      </td>
    </tr>
  </tbody>
</table>

### Assets

#### Create an asset original file

This action module creates and uploads an original file for an asset.


<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Lightroom], see <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Create a connection to [!DNL Adobe Lightroom]</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Catalog ID]</td>
      <td>
        <p>Enter or map the ID of the catalog that the asset belongs to.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset ID]</td>
      <td>
        <p>Enter or map the ID of the asset that you want to create and upload a file for.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Length of content in bytes]</td>
      <td>
        <p>Enter or map the length of the content in bytes.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Byte range]</td>
      <td>
        <p>Enter or map the byte range for the request, including first and last bytes and entity length as defined in RFC 2616. Should be included only when the data is too large to be uploaded in a single call.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Content type]</td>
      <td>
        <p>Select the content type for the new file.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Create an asset

This action module creates a new asset with initial metadata and import information.


<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Lightroom], see <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Create a connection to [!DNL Adobe Lightroom]</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Catalog ID]</td>
      <td>
        <p>Enter or map the ID of the catalog where the asset will be created.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset ID]</td>
      <td>
        <p>Enter or map the ID of the new asset.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset type]</td>
      <td>
        <p>Select whether the asset is an image or a video.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Datetime user created]</td>
      <td>
        <p>Enter or map a date with the format <code>YYYY-MM-DDT00:00:00-00:00</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Datetime user updated]</td>
      <td>
        <p>Enter or map a date with the format <code>YYYY-MM-DDT00:00:00-00:00</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Date captured]</td>
      <td>
        <p>Enter or map a date with the format <code>YYYY-MM-DDT00:00:00-00:00</code>.</p>
      </td>
    </tr>
  </tbody>
</table>

#### Create an asset external XMP develop setting file

This action module supports two workflows. The first workflow is to upload the external XMP develop settings file for the asset. The second workflow is to create an external XMP develop settings file by copying from another asset's external xmp develop setting file. 

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Lightroom], see <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Create a connection to [!DNL Adobe Lightroom]</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Length of content in bytes]</td>
      <td>
        <p>Enter or map the length of the content in bytes.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Upload new or copy XMP/develop file]</td>
      <td>
        <p>Select whether you are uploading a new file, or copying a file from an existing asset.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Catalog ID]</td>
      <td>
        <p>Enter or map the ID of the catalog that the asset belongs to.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset ID]</td>
      <td>
        <p>Enter or map the ID of the asset that you want to upload or copy a file to.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Link to XMP/develop file]</td>
      <td>
        <p>Enter or map a link to the file you want to upload or copy.</p><p>This file must be JSON if copying a file, or XML if uploading a file.</p>
      </td>
    </tr>
  </tbody>
</table>

Generate renditions for an original file

Get a catalog asset

Get the latest asset external XMP develop setting file

Get the latest asset rendition

Retrieve assets

### Albums

Add assets to album

Create album

Delete album

Get album

List assets of an album

Retrieve albums

Update album














