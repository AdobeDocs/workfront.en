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
        <p>Enter or map the ID of the catalog that contains the asset.</p>
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
        <p>Enter or map the ID of the catalog that contains the asset.</p>
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

#### Generate renditions for an original file

This action module asynchronously generate renditions for an original file.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Lightroom], see <a href="#create-a-connection-to-adobe-lightroom" class="MCXref xref" >Create a connection to [!DNL Adobe Lightroom]</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Rendition Type(s) (semi-colon separated)]</td>
      <td>
        <p>Enter the rendition type for the rendition you want to create. If entering more than one type, separate them with a semicolon (;). <p>Possible types:</p><ul><li><code>fullsize</code></li><li><code>2560</code></li></ul></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Length of content in bytes]</td>
      <td>
        <p>Enter or map the length of the content in bytes.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Catalog ID]</td>
      <td>
        <p>Enter or map the ID of the catalog that contains the asset.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset ID]</td>
      <td>
        <p>Enter or map the ID of the asset that you want to create a rendition of a file for.</p>
      </td>
    </tr>
  </tbody>
</table> 

#### Get a catalog asset

This action module retrieves information about a single asset in a catalog. The catalog must be owned by the user whose credentials are represented in the connection used in this module.

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
        <p>Enter or map the ID of the catalog that contains the asset.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset ID]</td>
      <td>
        <p>Enter or map the ID of the asset that you want to retrieve information for.</p>
      </td>
    </tr>
  </tbody>
</table> 


#### Get the latest asset external XMP develop setting file

This action module retrieves the most recent asset external XMP setting file.

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
        <p>Enter or map the ID of the catalog that contains the asset.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset ID]</td>
      <td>
        <p>Enter or map the ID of the asset associated with the XMP develop setting file.</p>
      </td>
    </tr>
  </tbody>
</table> 

#### Get the latest asset rendition

This action module retrieves the latest asset rendition of the specified type.

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
        <p>Enter or map the ID of the catalog that contains the asset.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset ID]</td>
      <td>
        <p>Enter or map the ID of the asset associated with the XMP develop setting file.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Rendition type]</td>
      <td>
        <p>Select the type of rendition that you want to retrieve.</p>
      </td>
    </tr>
  </tbody>
</table> 

#### Retrieve assets

This action module retrieves assets owned by the by the user whose credentials are represented in the connection used in this module.

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
        <p>Enter or map the ID of the catalog that contains the asset.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Starting timestamp]</td>
      <td>
        <p>Enter or map a timestamp. The module returns records that have been updated after this time stamp.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Return assets captured before]</td>
      <td>
        <p>Enter a date with the format <code>YYYY-MM-DDT00:00:00</code>. The module returns results captured before this date.</p><p> This field cannot be used with the field <code>Return assets captured after</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Maximum number of returned records]</td>
      <td>
        <p>Set the maximum number of rows that [!DNL Workfront Fusion] will return during one execution cycle. This number must be less than or equal to 100.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL SHA256 Hash value of original file]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Hide assets that are inside stacks?"]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset subtype values]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Asset IDs]</td>
      <td>
        <p>Enter or map up to 100 asset IDs, separated by commas.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Types of assets to exclude]</td>
      <td>
        <p>Select if you want to exclude complete or incomplete assets. To include all assets, leave this field blank.</p>
      </td>
    <tr>
      <td role="rowheader">[!UICONTROL Group values]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Name values]</td>
      <td>
        <p></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Favorite status]</td>
      <td>
        <p></p>
      </td>
    </tr>
    </tr>
  </tbody>
</table> 

### Albums

#### Add assets to album

This action module adds one or more assets to the specified album. You can add up to 50 assets in one execution cycle.

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
        <p>Enter or map the ID of the catalog that contains the album that you want to add assets to.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Album ID]</td>
      <td>
        <p>Enter or map the ID of the album that you want to add assets to.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Assets]</td>
      <td>
        <p>For each asset that you want to add to the album, click <b>Add item</b> and enter the following.</p>
      </td>
    </tr>
  </tbody>
</table> 

Create album

Delete album

Get album

List assets of an album

Retrieve albums

Update album














