---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Adobe Photoshop modules
description: With the Adobe Photoshop modules, you can start an Adobe Workfront Fusion scenario based on events in your Adobe Photoshop account, create, read, or update agreements and other records, search for records using criteria you set, and upload documents.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
---
# [!DNL Adobe Photoshop] modules

In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use [!DNL Adobe Photoshop], as well as connect it to multiple third-party applications and services. [!DNL Adobe Photoshop] modules allow you to create, read, update, or delete records, list all records of a given type, search records based on criteria you specify, or perform a custom API call to the [!DNL Adobe Photoshop] API.


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

Before you can use the [!DNL Adobe Photoshop] connector, you must ensure that the following prerequisites are met:

* You must have an active [!DNL Adobe Photoshop] account.

## Create a connection to [!DNL Adobe Photoshop]

To create a connection for your [!DNL Adobe Photoshop] modules:

1. Click **[!UICONTROL Add]** next to the Connection box.
    
1. Fill in the following fields:
    
    <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
        <td role="rowheader">[!UICONTROL Connection name]</td>
        <td>
          <p>Enter a name for this connection.</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>Enter your [!UICONTROL Adobe] [!UICONTROL Client ID]. This can be found in the [!UICONTROL Credentials] details section of the [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Enter your [!DNL Adobe] [!UICONTROL Client Secret]. This can be found in the [!UICONTROL Credentials] details section of the [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Technical account ID]</td>
        <td>Enter your [!DNL Adobe] [!UICONTROL Technical account ID]. This can be found in the [!UICONTROL Credentials] details section of the [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Organization ID]</td>
        <td>Enter your [!DNL Adobe] [!UICONTROL Organization ID]. This can be found in the [!UICONTROL Credentials] details section of the [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Private key]</td>
        <td>
          <p>Enter the private key that was generated when your credentials were created in the [!DNL Adobe Developer Console]. </p>
          <p>To extract your private key or certificate:</p>
          <ol>
            <li value="1">
              <p>Click <b>[!UICONTROL Extract]</b>.</p>
            </li>
            <li value="2">
              <p>Select the type of file you are extracting.</p>
            </li>
            <li value="3">
              <p>Select the file that contains the private key or certificate.</p>
            </li>
            <li value="4">
              <p>Enter the password for the file.</p>
            </li>
            <li value="5">
              <p>Click <b>Save</b> to extract the file and return to th[!UICONTROL ]e connection setup.</p>
            </li>
          </ol>
        </td>
        </tr>
      </tbody>
    </table>
    
1. Click **[!UICONTROL Continue]** to save the connection and return to the module.
    
## [!DNL Adobe Photoshop] modules and their fields

When you configure [!DNL Adobe Photoshop] modules, [!DNL Workfront Fusion] displays the fields listed below. Along with these, additional [!DNL Adobe Photoshop] fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)


### Actions

* [Create a new PSD](#create-a-new-psd)
* [Edit text layers](#edit-text-layers)
* [Execute Depth Blur](#execute-depth-blur)
* [Execute Photoshop actions](#execute-photoshop-actions)
* [Execute Product Crop](#execute-product-crop)
* [Get layer info](#get-layer-info)
* [Make a custom API call](#make-a-custom-api-call)

#### Create a new PSD

#### Edit text layers

This action module edits text layers on a Photoshop file.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Photoshop], see <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Create a connection to [!DNL Adobe Photoshop]</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Input file storage]</td>
      <td>
        <p>Select the file service where the file you want to edit is stored.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Input file URL]</p>
      </td>
   <td> Enter or map the URL or path of the file that you want to edit. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Manage missing fonts]</td>
      <td>
        <p>Select the action to take if there are one or more missing fonts in the document. If the font is not provided, the module uses the default font.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Default font]  </td>
      <td>
        <p>Enter the full postscript name of the font to be used as the global default for the document. This font will be used for any text layer which has a missing font and no other font has been specifically provided for that layer. If this font is missing, the option specified in Manage missing fonts will take effect.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Layers]</td>
   <td> <p>For details about layer options, see <a href="https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/text">Edit text layer</a> in the Adobe Photoshop documentation.</p>  </td>     </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Output file storage]</td>
      <td>
        <p>Select the file service where the you want the edited file to be stored.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Output file URL]</p>
      </td>
   <td> Enter or map the URL or path of where the edited file will be stored. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Output file type]</p>
      </td>
   <td> Select the file type for the edited file. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>Select whether the newly edited file will overwrite any output file that already exists.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compression]</p>
      </td>
   <td> Select the compression level for the output file. </td> 
    </tr>
  </tbody>
</table>

#### Execute Depth Blur

This action module executes Depth Blur on the selected file.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Photoshop], see <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Create a connection to [!DNL Adobe Photoshop]</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Input file storage]</td>
      <td>
        <p>Select the file service where the file you want to edit is stored.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Input file URL]</p>
      </td>
   <td> Enter or map the URL or path of the file that you want to edit. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Output file storage]</td>
      <td>
        <p>Select the file service where the you want the edited file to be stored.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Output file URL]</p>
      </td>
   <td> Enter or map the URL or path of where the edited file will be stored. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Output file type]</p>
      </td>
   <td> Select the file type for the edited file. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Other fields]</td>
      <td>
        <p>For details about other Depth Blur options, see <a href="https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/depthBlur">Execute Depth Blur </a>in the Adobe Photoshop API documentation.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>Select whether the newly edited file will overwrite any output file that already exists.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compression]</p>
      </td>
   <td> Select the compression level for the output file. </td> 
    </tr>
  </tbody>
</table>

#### Execute Photoshop Actions

This action module executes a Photoshop action on the selected image.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Photoshop], see <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Create a connection to [!DNL Adobe Photoshop]</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Input file storage]</td>
      <td>
        <p>Select the file service where the file you want to edit is stored.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Input file URL]</p>
      </td>
   <td> Enter or map the URL or path of the file that you want to edit. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Actions file storage]</td>
      <td>
        <p>Select the file service where actions file is stored.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Actions file URL]</p>
      </td>
   <td> Enter or map the URL or path of the actions file. </td> 
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Action name]</p>
      </td>
   <td> If you only want to execute a particular action, you may specify which action to play from the ActionSet. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Font / Pattern / Brush storage]</td>
      <td>
        <p>Select the file service where the file you want to use is stored.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Font / Pattern / Brush file URL]</p>
      </td>
   <td> Enter or map the URL or path of the file that you want to use. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Output file storage]</td>
      <td>
        <p>Select the file service where the you want the edited file to be stored.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Output file URL]</p>
      </td>
   <td> Enter or map the URL or path of where the edited file will be stored. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Output file type]</p>
      </td>
   <td> Select the file type for the edited file. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>Select whether the newly edited file will overwrite any output file that already exists.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compression]</p>
      </td>
   <td> Select the compression level for the output file. </td> 
    </tr>
  </tbody>
</table>

#### Execute Product Crop

This action module executes Product Crop on the selected image.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Photoshop], see <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Create a connection to [!DNL Adobe Photoshop]</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Input file storage]</td>
      <td>
        <p>Select the file service where the file you want to crop is stored.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Input file URL]</p>
      </td>
   <td> Enter or map the URL or path of the file that you want to crop. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Unit]</p>
      </td>
   <td> Select whether you want to describe the height and width adjustment in pixels or as a percent. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Width]</p>
      </td>
   <td> Enter or map amount of width padding you want to add. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Height]</p>
      </td>
   <td> Enter or map amount of height padding you want to add. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Output file storage]</td>
      <td>
        <p>Select the file service where the you want the edited file to be stored.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Output file URL]</p>
      </td>
   <td> Enter or map the URL or path of where the edited file will be stored. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Output file type]</p>
      </td>
   <td> Select the file type for the edited file. </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>Select whether the newly edited file will overwrite any output file that already exists.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Compression]</p>
      </td>
   <td> Select the compression level for the output file. </td> 
    </tr>
  </tbody>
</table>

#### Get layer info

This action module retrieves layer information from the specified PSD file.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Photoshop], see <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Create a connection to [!DNL Adobe Photoshop]</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Input file storage]</td>
      <td>
        <p>Select the file service where the file you want to retrieve layer information from is stored.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Input file URL]</p>
      </td>
   <td> Enter or map the URL or path of the file that you want to retrieve layer information from. </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Thumbnails]</p>
      </td>
   <td> </td> 
    </tr>
  </tbody>
</table>

#### Make a custom API call

This action module makes a custom call to the Photoshop API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Photoshop], see <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Create a connection to [!DNL Adobe Photoshop]</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>Enter a path relative to <code>https://image.adobe.io/pie/psdService</code>. Example: <code>/photoshopActions</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
      </td>
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Add the headers of the request in the form of a standard JSON object.</p>
        <p>For example, <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] adds authorization headers automatically.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]  </td>
      <td>
        <p>Enter the request query string.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

