---
filename: aem-assets-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: Adobe Experience Manager Assets modules
description: With the [!DNL Adobe Experience Manager Assets] connector for [!DNL Adobe Workfront Fusion], you can start a scenario based on events in your [!DNL Adobe Experience Manager Assets] account, create, upload, and update assets, and copy or move folders and assets.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 0749f230-8cab-464f-863c-9cb4870125d1
---
# [!DNL Adobe Experience Manager Assets] modules

With the [!DNL Adobe Experience Manager Assets] connector for [!DNL Adobe Workfront Fusion], you can start a scenario based on events in your [!DNL Adobe Experience Manager Assets] account, create, upload, and update assets, and copy or move folders and assets.

For an introduction to the Adobe Experience Manager Assets connector, see:

* [Adobe Experience Manager Assets](https://video.tv.adobe.com/v/3427034/){target=_blank}

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

## Prerequisites

* You must have an [!DNL Adobe Experience Manager Assets] account to use these modules.
* You must set up [!UICONTROL Server-to-server] flow in the [!DNL Adobe Developer console].

   For instructions on setting up [!UICONTROL Server-to-server] flow in the [!DNL Adobe Developer console], see [Generating Access Tokens for Server Side APIs](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).
* Your Adobe Experience Manager technical account must have write permissions.

   For instructions on adding write permissions to your Adobe Experience Manager technical account, see [Service credentials](https://experienceleague.adobe.com/en/docs/experience-manager-learn/getting-started-with-aem-headless/authentication/service-credentials) in the Adobe Experience Manager documentation.

## Connect [!DNL Adobe Experience Manager Assets] to [!DNL Workfront Fusion] {#connect-adobe-experience-manager-assets-to-workfront-fusion}

To create a connection for your [!DNL Adobe Experience Manager Assets] modules:

1. Click [!UICONTROL Add] next to the [!UICONTROL Connection] box.

2. Select the type of connection that you are creating:

   * **[!DNL AEM Assets as a Cloud Service]**

      This configuration requires information from the [!DNL Adobe Admin Console].

   * **[!DNL AEM Assets Basic] ([!DNL Adobe Managed Services])**

      This configuration requires a username and password.

3. Fill in the fields for the type of connection that you are creating.

   For [!DNL AEM Assets as a Cloud Service], see [Configure the connection for [!DNL AEM Assets as a Cloud Service]](#configure-the-connection-for-aem-assets-as-a-cloud-service).

   For [!UICONTROL AEM Assets Basic] ([!DNL Adobe Managed Services]), see [Configure the connection for [!UICONTROL AEM Assets Basic]](#configure-the-connection-for-aem-assets-basic).

4. Click **[!UICONTROL Continue]** to save the connection and return to the module.


### Configure the connection for [!DNL AEM Assets as a Cloud Service]

>[!NOTE]
>
>* The information for these fields is generated as part of setting up [!UICONTROL Server-to-server] flow on the [!DNL Adobe Developer Console]. You can find these values in the service credentials JSON file generated as part of that setup.
>
>   For instructions on setting up [!UICONTROL Server-to-server] flow on the [!UICONTROL Adobe Developer Console], see [Generating Access Tokens for Server Side APIs](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/developing/generating-access-tokens-for-server-side-apis.html#the-server-to-server-flow).
>
>* Your Adobe Experience Manager technical account must have write permissions.
>
>   For instructions on adding write permissions to your Adobe Experience Manager technical account, see [Service credentials](https://experienceleague.adobe.com/en/docs/experience-manager-learn/getting-started-with-aem-headless/authentication/service-credentials) in the Adobe Experience Manager documentation.


<table style="table-layout:auto"> 
          <col/>
          <col/>
          <tbody>
              <tr>
                  <td role="rowheader">[!UICONTROL Connection name]</td>
                  <td>
                      <p>Enter a name for this connection</p>
                  </td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Instance URL without a trailing slash]</td>
                  <td>Enter the URL for your [!DNL Adobe Experience Manager] instance. Do not include a slash <code>/</code> at the end of the URL.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Client ID]</td>
                  <td>Enter the Client ID generated in the [!UICONTROL Server-to-server] setup.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Client Secret]</td>
                  <td>Enter the Client Secret generated in the [!UICONTROL Server-to-server] setup.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Technical account ID]</td>
                  <td>Enter the ID of the technical account. This is the "[!UICONTROL id]" field in the client credentials JSON file.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Org ID]</td>
                  <td class="">Enter the ID of your organization. This is the "[!UICONTROL org]" field in the client credentials JSON file.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Meta Scopes]</td>
                  <td>Enter the Meta Scopes generated in the [!UICONTROL Server-to-server] setup.</td>
              </tr>
              <tr>
                  <td role="rowheader">[!UICONTROL Private key]</td>
                  <td>Enter the Private Key generated win the [!UICONTROL Server-to-server] setup. To extract the private key, click [!UICONTROL Extract], then enter the file to extract and the password for the file.</td>
              </tr>
          </tbody>
      </table>


### Configure the connection for [!DNL AEM Assets Basic] ([!DNL Adobe Managed Services])

<table style="table-layout:auto"> 
        <col/>
        <col />
        <tbody>
            <tr>
                <td role="rowheader">[!UICONTROL Connection name]</td>
                <td>
                    <p>Enter a name for this connection</p>
                </td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Instance URL without a trailing slash]</td>
                <td>Enter the URL for your [!DNL Adobe Experience Manager] instance. Do not include a slash <code>/</code> at the end of the URL.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Username]</td>
                <td>Enter the username for the [!DNL AEM Assets] account that this connection uses.</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Password]</td>
                <td>Enter the password for the [!DNL AEM Assets] account that this connection uses.</td>
            </tr>
        </tbody>
    </table>


## [!DNL Adobe Experience Manager Assets] modules and their fields

When you configure [!DNL Adobe Experience Manager Essentials] modules, [!DNL Workfront Fusion] displays the fields listed below. Along with these, additional [!DNL Adobe Experience Manager Essentials] fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Copy a folder or asset](#copy-a-folder-or-asset)
* [Create a record](#create-a-record)
* [Delete a folder, asset, or rendition](#delete-a-folder-asset-or-rendition)
* [Get a folder listing](#get-a-folder-listing)
* [Make a custom API call](#make-a-custom-api-call)
* [Move a folder or asset](#move-a-folder-or-asset)
* [Update a record](#update-a-record)
* [Upload an asset](#upload-an-asset)

### [!UICONTROL Copy a folder or asset]

This action module copies a folder or asset to another location in your Adobe Experience Manager Assets account.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Adobe Experience Manager Assets] account to [!DNL Workfront Fusion], see <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td> <p>Select whether you want to copy a folder or an asset.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder] / [!UICONTROL Asset selection]</td> 
   <td>Select or map the folder or asset that you want to copy.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destination path]</td> 
   <td>Select or map the path to the location for the new folder or asset.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name of copied folder] / [!UICONTROL asset]</td> 
   <td>Enter a name for the new folder or asset. The folder name that displays in [!DNL Adobe Experience Manager Assets] is the same as the original name. The name entered here appears in the URL of the new folder or asset.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copy children]</td> 
   <td>Enable this option to copy any subfolders or assets within the folder.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Overwrite]</td> 
   <td>Enable this option to overwrite any folder or asset in the destination location that has the same name as the folder or asset being copied.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Create a record]

This action module creates a folder or an asset comment.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Adobe Experience Manager Assets] account to [!DNL Workfront Fusion], see <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object type]</td> 
   <td> <p>Select whether you want to create a folder or a comment on an asset.</p> 
    <ul> 
     <li> <p>[!UICONTROL Folder]</p> <p>Fill in the following fields:</p> 
      <ul> 
       <li> <p>[!UICONTROL Name]</p> <p>Enter a name for the folder. This name will appear in the file path, so it must not include spaces or other characters. </p> </li> 
       <li> <p>[!UICONTROL Title]</p> <p>Enter a title for the folder, which can be displayed instead of the name.</p> </li> 
      </ul> </li> 
     <li> <p>[!UICONTROL Asset comment]</p> <p>Fill in the following fields:</p> 
      <ul> 
       <li> <p>[!UICONTROL Asset selection]</p> <p>Select or map the ID of the asset you want to add a comment to.</p> </li> 
       <li> <p>[!UICONTROL Comment]</p> <p>Enter the text of the comment.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Delete a folder, asset, or rendition]

This action module deletes a folder, asset, or rendition.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Adobe Experience Manager Assets] account to [!DNL Workfront Fusion], see <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td> <p>Select whether you want to delete a folder, asset, or rendition.</p> 
    <ul> 
     <li> <p>[!UICONTROL Folder]</p> <p>Select the folder to delete by selecting the folders in its path.</p> </li> 
     <li> <p>[!UICONTROL Asset] </p> <p>Select the asset by selecting the folders in its path, then the asset you want to delete.</p> </li> 
     <li> <p>[!UICONTROL Rendition]</p> <p>Select the rendition by selecting the folders in its path.</p> <p>Enter or map the name of the rendition.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Get a folder listing]

This action module retrieves a representation of an existing folder and of its child entities (folders or assets).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Adobe Experience Manager Assets] account to [!DNL Workfront Fusion], see <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>Select or map the folder that you want to retrieve. To add subfolders to the path, click the plus icon and select the subfolder.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Make a custom API call]

This action module makes a custom API call to the [!DNL Adobe Experience Manager Assets] API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Adobe Experience Manager Assets] account to [!DNL Workfront Fusion], see <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Enter a path relative to your [!DNL Adobe Experience Manager] base URL.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP request methods in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] adds authorization headers automatically.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String] </td> 
   <td> <p>Enter the request query string. For Each Key/Value pair, click <b>[!UICONTROL Add item]</b> and enter the [!UICONTROL Key] and [!UICONTROL Value].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Move a folder or asset]

This action module moves the asset or folder at the given path to a new location.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Adobe Experience Manager Assets] account to [!DNL Workfront Fusion], see <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td> <p>Select whether you want to move a folder or an asset.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder] / [!UICONTROL Asset]</td> 
   <td>Select or map the folder or asset that you want to move.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destination path]</td> 
   <td>Select or map the path to the location that you want to move the folder or asset to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name of moved folder] / [!UICONTROL asset]</td> 
   <td>Enter a new name for the moved folder or asset. The folder name that displays in [!DNL Adobe Experience Manager Assets] is the same as the original name. The name entered here appears in the URL of the moved folder or asset.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Overwrite]</td> 
   <td>Enable this option to overwrite any folder or asset in the destination location that has the same name as the folder or asset being copied.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Update a record]

This action module updates an existing record.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Adobe Experience Manager Assets] account to [!DNL Workfront Fusion], see <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td> <p>Select whether you want to delete asset metadata or an asset rendition.</p> 
    <ul> 
     <li> <p>[!UICONTROL Asset metadata]</p> 
      <ul> 
       <li> <p>Select the asset that you want to update metadata for.</p> </li> 
       <li> <p>Enter the new title of the asset.</p> </li> 
      </ul> </li> 
     <li> <p>[!UICONTROL Asset rendition]</p> 
      <ul> 
       <li> <p>Select the asset that you want to update the rendition for.</p> </li> 
       <li> <p>Select a source file from a previous module, or map the source file's name and data.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Upload an asset]

This action module uploads an asset to your [!DNL Adobe Experience Manager Assets] account.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Adobe Experience Manager Assets] account to [!DNL Workfront Fusion], see <a href="#connect-adobe-experience-manager-assets-to-workfront-fusion" class="MCXref xref">Connect [!DNL Adobe Experience Manager Assets] to [!DNL Workfront Fusion]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destination]</td> 
   <td> <p>Select the folder where you want to upload an asset.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Enter or map the source file's name and data.</td> 
  </tr> 
 </tbody> 
</table>
