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

*   You must have an active [!DNL Adobe Photoshop] account.

## Create a connection to [!DNL Adobe Photoshop]

To create a connection for your [!DNL Adobe Photoshop] modules:

1.  Click **[!UICONTROL Add]** next to the Connection box.
    
2.  Fill in the following fields:
    
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
    
1.  Click **[!UICONTROL Continue]** to save the connection and return to the module.
    
## [!DNL Adobe Photoshop] modules and their fields

When you configure [!DNL Adobe Photoshop] modules, [!DNL Workfront Fusion] displays the fields listed below. Along with these, additional [!DNL Adobe Photoshop] fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)


### Actions

#### Create a new Photoshop document

This action module creates a Photoshop document. You can generate renditions of the document or save it as a PSD.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Connection</td>
     <td>For instructions on creating a connection to Adobe Photoshop, see <a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >Create a connection to Adobe Photoshop</a> in this article.</td>
    </tr>
    <tr>
      <td role="rowheader">
        Templates
      </td>
      <td>
        Select the template that you want to use. To create a document without a template, select Custom.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        Height
      </td>
      <td>
        Enter or map the height of the new document, in pixels.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        Width
      </td>
      <td>
        Enter or map the width of the new document, in pixels.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        Resolution
      </td>
      <td>
        Enter the resolution of the new document, in pixels per inch. This must be an integer between 72-300.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        Depth
      </td>
      <td>
        Select the bit depth for the new document. Bit depth specifies for much color information is available foe each pixel in an image. Higher bit depth allows more available colors and more accurate color representation, but creates a larger file.
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        Layers
      </td>
      <td>
        <p>For each layer that you want to add to the document, click Add item and fill in details.</p><p>For details about fields, see </p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        Global Font
      </td>
      <td>
       The full postscript name of the font to be used as the global default for the document. This font will be used for any text layer which has a missing font and no other font has been specifically provided for that layer. If this font itself is missing, the option specified for <code>manageMissingFonts</code> from above will take effect
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        Fonts
      </td>
      <td>
For each font that you want to use in the document, click Add item and enter one of the following:<ul><li>An Adobe Creative Cloud assets path</li><li>A presignedGETURL</li></ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        Manage missing fonts
      </td>
      <td>
        Action to take if there are one or more missing fonts in the document. <ul><li><b>Fail</b> The job will not succeed and the status will be set to failed, with the details of the error provided in the details section in the status.</lo><li><b>Use default</b> The job will succeed. By default, all the missing fonts will be replaced with the font ArialMT.
      </td>
    </tr>
  </tbody>
</table>

#### Custom API Call

#### Edit text layers

#### Execute Depth Blur

#### Execute Photoshop Actions

#### Execute Product Crop

#### Get layer info

