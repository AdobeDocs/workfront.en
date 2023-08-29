---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Google Docs modules
description: The Adobe Workfront Fusion [!DNL Google Docs] modules enable you to monitor, create, edit and retrieve documents in your [!DNL Google Docs] and [!DNL Google Docs] (for [!DNL G Suite] users).
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: fbe7d628-d833-43ce-83b8-8e4e6a812fd1
---
# [!DNL Google Docs] modules

The [!DNL Adobe Workfront Fusion] [!DNL Google Docs] modules enable you to monitor, create, edit and retrieve documents in your [!DNL Google Docs] and [!DNL Google Docs] (for [!DNL G Suite] users).

In order to use [!DNL Google Docs] with [!DNL Adobe Workfront Fusion], it is necessary to have a [!DNL Google] account. If you don't have a [!DNL Google] account yet, you can create one at the [!DNL Google] Account help page.

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

To use [!DNL Google Docs] modules, you must have a Google account.

## [!DNL Google Docs] modules and their fields

When you configure [!DNL Google Docs] modules, [!UICONTROL Workfront Fusion] displays the fields listed below. Along with these, additional [!DNL Google Docs] fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Document

* [[!UICONTROL Watch Documents]](#watch-documents) 
* [[!UICONTROL List Documents]](#list-documents) 
* [[!UICONTROL Get Content of a Document]](#get-content-of-a-document) 
* [[!UICONTROL Create a Document]](#create-a-document) 
* [[!UICONTROL Create a Document From a Template]](#create-a-document-from-a-template) 
* [[!UICONTROL Insert a Paragraph to a Document]](#insert-a-paragraph-to-a-document) 
* [[!UICONTROL Insert an Image to a Document]](#insert-an-image-to-a-document) 
* [[!UICONTROL Replace an Image with a New Image]](#replace-an-image-with-a-new-image) 
* [[!UICONTROL Replace Text in a Document]](#replace-text-in-a-document) 
* [[!UICONTROL Download a Document]](#download-a-document) 
* [[!UICONTROL Delete a Document]](#delete-a-document)

#### [!UICONTROL Watch Documents]

This trigger module returns document details when a new document is created or modified in the selected folder.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Google] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to [!DNL Workfront Fusion]</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch Documents]</td> 
   <td> <p style="color: #000000;">Select whether you want to watch created ([!UICONTROL By Created Date]) or modified ([!UICONTROL By Modified Date]) documents.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose a Drive]</td> 
   <td> <p>Select the type of drive you want to monitor.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Select the folder you want to watch for created or modified documents.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>Select the folder you want to watch for created or modified documents.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Shared Drive]</strong> (available for [!DNL G Suite] users only)</p> <p>Select whether you want to [!UICONTROL Use Domain Admin Access]. Selecting [!UICONTROL Yes] issues the request as a domain administrator, and all shared drives in which the requester is an administrator are returned.</p> <p>Select the shared drive you want to watch.</p> <p>Note: If you have selected the [!DNL Google Shared Drive] option in this field and you are not a [!DNL G Suite] user, the error <code>[400] Invalid Value</code> is returned.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Set the maximum number of documents Workfront Fusion returns in one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL List Documents]

This action module retrieves a list of documents from the selected folder.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Google] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to [!DNL Workfront Fusion]</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose a Drive]</td> 
   <td> <p>Select the type of drive you want to list documents from.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Select the folder you want to list documents from.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>Select the folder you want to list documents from.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Shared Drive]</strong> (available for [!DNL G Suite] users only)</p> <p>Select whether you want to [!UICONTROL Use Domain Admin Access]. Selecting [!UICONTROL Yes] issues the request as a domain administrator, and all shared drives in which the requester is an administrator are returned.</p> <p>Select the shared drive you want to list documents from.</p> <p>Note: If you have selected the [!DNL Google Docs] option in this field and you are not a [!DNL G Suite] user, the error <code>[400] Invalid Value</code> is returned.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Set the maximum number of documents [!DNL Workfront Fusion] returns in one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get Content of a Document]

This action module retrieves a specified document.

You may need to extend your permissions.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Google] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to [!DNL Workfront Fusion]</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Get Content of a Document]</td> 
   <td> <p>Select whether you want to map the document ID of the document or select the document from the drop-down menu manually.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose a Drive]</td> 
   <td> <p>Select the type of drive that contains the document you want to retrieve.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Select the folder that contains the document you want to retrieve.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>Select the folder that contains the document you want to retrieve.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Shared Drive]</strong> (available for [!DNL G Suite] users only)</p> <p>Select whether you want to [!UICONTROL Use Domain Admin Access]. Selecting [!UICONTROL Yes] issues the request as a domain administrator, and all shared drives in which the requester is an administrator are returned.</p> <p>Select the shared drive that contains the document you want to retrieve.</p> <p>Note: If you have selected the [!DNL Google Docs] option in this field and you are not a [!DNL G Suite] user, the error <code>[400] Invalid Value</code> is returned.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Filter]</p> </td> 
   <td> <p>Select the object you want to be returned in the module's output.</p> 
    <ul> 
     <li>[!UICONTROL Image] (default)</li> 
     <li>[!UICONTROL Drawing]</li> 
     <li>[!UICONTROL Chart]</li> 
    </ul> <p>Note:  <p>For further mapping of these objects, please use the [!UICONTROL Inline Objects Array] value in this module's output (instead of [!UICONTROL inlineObjects]).</p> <p>The [!UICONTROL Inline Objects Array] objects are sorted in the same order they appear in the document. It will make any further processing easier.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create a Document]

This action module allows you to create a new document in the selected folder.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Google] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to [!DNL Workfront Fusion]</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Enter the name of the document.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content]</td> 
   <td> <p>Enter the content of the document. HTML is supported.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose a Drive]</td> 
   <td> <p>Select the type of drive where you want to create a document.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Select the folder where you want to create a document.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>Select the folder where you want to create a document.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Shared Drive]</strong> (available for [!DNL G Suite] users only)</p> <p>Select whether you want to [!UICONTROL Use Domain Admin Access]. Selecting [!UICONTROL Yes] issues the request as a domain administrator, and all shared drives in which the requester is an administrator are returned.</p> <p>Select the shared drive where you want to create a document.</p> <p>Note: If you have selected the [!DNL Google Docs] option in this field and you are not a [!DNL G Suite] user, the error <code>[400] Invalid Value</code> is returned.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Insert a Header]</td> 
   <td> <p> Enable this option to insert the header to the document, then enter or map the text of the header.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Insert a Footer] </td> 
   <td> <p>Enable this option to insert the footer to the document, then enter or map the text of the header.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create a Document From a Template]

This action module creates a copy of an existing template document and replaces any tags. This module also allows users to replace images with new images by URL.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Google] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to [!DNL Workfront Fusion]</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Create a Document from a Template]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>Select this option to map the document template.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br>Select this option to choose the document template from the drop-down menu.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose a Drive]</td> 
   <td> <p>Select the type of drive where your template is located. This option is available if you selected [!UICONTROL By Dropdown] in the previous field.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Select the folder where your template is located.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>Select the folder where your template is located.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Shared Drive]</strong> (available for [!DNL G Suite] users only)</p> <p>Select whether you want to [!UICONTROL Use Domain Admin Access]. Selecting [!UICONTROL Yes] issues the request as a domain administrator, and all shared drives in which the requester is an administrator are returned.</p> <p>Select the shared drive where your template is located.</p> <p>Note: If you have selected the [!DNL Google Docs] option in this field and you are not a [!DNL G Suite] user, the error <code>[400] Invalid Value</code> is returned.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Values]</p> </td> 
   <td> <p>Enter the values that will be entered instead of the variables to the new document.</p> 
    <ul> 
     <li><strong>[!UICONTROL Tags]</strong> <br>Enter the tags that are contained in the document template. Do not use <code>&#123;&#123;&#125;&#125;</code>. Example: use <code>name</code> instead of <code>&#123;&#123;name&#125;&#125;</code>.</li> 
     <li><strong>[!UICONTROL Replaced Value]</strong><br>Enter the value of the tag.</li> 
    </ul> <p>For example the<code> &#123;&#123;name&#125;&#125;</code> variable in the source document will be displayed as the name field here, where the value can be inserted, such as <code>John</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Images Replacement]</p> </td> 
   <td> <p>Enter the link to the [!UICONTROL Image Object ID] and [!UICONTROL Image URL] that will replace the current image.</p> <p>Note:  You can retrieve the image IDs by using [!UICONTROL Get a Document] module, where the IDs are contained in the array [!UICONTROL Inline Object Array].</p> <p>We recommend that you add ALT text to images in your [!DNL Google] document. </p> <p>To add an ALT Text to the [!DNL Google Docs] image:</p> 
    <ol> 
     <li value="1">Right click on the image.</li> 
     <li value="2">Select the [!UICONTROL ALT text] option.</li> 
     <li value="3">Enter the [!UICONTROL ALT text] in the [!UICONTROL Title] field and click [!UICONTROL OK].</li> 
    </ol> <p>After the ALT text is added to the image, the ALT text is displayed in the field name in parentheses.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title] </td> 
   <td> <p>Enter the name for the new document.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose a Drive]</td> 
   <td> <p>Select the type of drive where your template is located. This option is available if you selected [!UICONTROL By Dropdown] in the previous field.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Select the folder where you want the document to be created.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>Select the folder where you want the document to be created.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Shared Drive]</strong> (available for [!DNL G Suite] users only)</p> <p>Select whether you want to [!UICONTROL Use Domain Admin Access]. Selecting [!UICONTROL Yes] issues the request as a domain administrator, and all shared drives in which the requester is an administrator are returned.</p> <p>Select the shared drive where you want the document to be created.</p> <p>Note: If you have selected the [!DNL Google Docs] option in this field and you are not a [!DNL G Suite] user, the error <code>[400] Invalid Value</code> is returned.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Insert a Paragraph to a Document]

This action module appends or inserts a new paragraph to an existing document.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Google] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to [!DNL Workfront Fusion]</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Select a Document]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>Select this option to map the document.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br> Select this option to choose the document from the drop-down menu.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose a Drive]</td> 
   <td> <p>Select the type of drive where the document you want to add a paragraph to is located. This option is available if you selected [!UICONTROL By Dropdown] in the previous field.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Select the folder where the document you want to add a paragraph to is located, then select the document.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>Select the folder where the document you want to add a paragraph to is located, then select the document.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Shared Drive]</strong> (available for [!DNL G Suite] users only)</p> <p>Select whether you want to [!UICONTROL Use Domain Admin Access]. Selecting [!UICONTROL Yes] issues the request as a domain administrator, and all shared drives in which the requester is an administrator are returned.</p> <p>Select the shared drive where the document you want to add a paragraph to is located, then select the document.</p> <p>Note: If you have selected the [!DNL Google Docs] option in this field and you are not a [!DNL G Suite] user, the error <code>[400] Invalid Value</code> is returned.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Insert a Paragraph]</p> </td> 
   <td> <p>Select how you want the new text to be inserted in the document.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL By specification of location]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL By index]</strong> </p> 
        <ul> 
         <li> <p><strong>[!UICONTROL Index]</strong> </p> <p>Enter the Index number where you would like to insert your text. You can use the [!UICONTROL Get a Document] module retrieve Index number.</p> <p>To display all characters (including hidden) in the document, you can use the [!UICONTROL Show] add-on. You can find the add-on under [!UICONTROL Add-ons] &gt; [!UICONTROL Get add-ons]. Search for [!UICONTROL Show] and install the [!UICONTROL Show] add-on.</p> </li> 
         <li> <p><strong>[!UICONTROL Inserted text]</strong> </p> <p>Enter the text you want to insert to the document.</p> </li> 
        </ul> </li> 
       <li> <p><strong>[!UICONTROL By segment ID]</strong> </p> <p>Select the header and footer you want to insert the text content to and enter the text you want to insert to the corresponding fields.</p> <p>If the header or footer already contains text, the new text will be added before the existing text.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL By appending to the body of the document]</strong> </p> <p>Appends entered text at the end of the document's body content.</p> <p>The style of the new paragraph will be copied from the paragraph at the current insertion index, including lists and bullets.</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL By appending to the end of segment (Header and Footer)]</strong> </p> <p>Select the header and footer you want to insert the text content to and enter the text you want to insert to the corresponding fields.</p> <p>If the header or footer already contain text, the new text will be added after the existing text.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Appended Text]</td> 
   <td>Enter or map the text you want to append to the document</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Insert an Image to a Document]

This action module inserts an image from the URL to the document.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Google] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to [!DNL Workfront Fusion]</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Select a Document]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>Select this option to map the document template.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br> Select this option to choose the document from the drop-down menu.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose a Drive]</td> 
   <td> <p>Select the type of drive where the document you want to add an image to is located. This option is available if you selected [!UICONTROL By Dropdown] in the previous field.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Select the folder where the document you want to add an image to is located, then select the document.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>Select the folder where the document you want to add an image to is located, then select the document.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Shared Drive]</strong> (available for [!DNL G Suite] users only)</p> <p>Select whether you want to [!UICONTROL Use Domain Admin Access]. Selecting [!UICONTROL Yes] issues the request as a domain administrator, and all shared drives in which the requester is an administrator are returned.</p> <p>Select the shared drive where the document you want to add an image to is located, then select the document.</p> <p>Note: If you have selected the [!DNL Google Docs] option in this field and you are not a [!DNL G Suite] user, the error <code>[400] Invalid Value</code> is returned.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Insert an Image]</p> </td> 
   <td> <p>Select how you want the new image to be inserted in the document.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL By specification of location]</strong> </p> 
      <ul> 
       <li> <p><strong>[!UICONTROL By index]</strong> </p> 
        <ul> 
         <li> <p><strong>[!UICONTROL Index]</strong> </p> <p>Enter the Index number where you would like to insert your image. You can use the [!UICONTROL Get a Document] module retrieve [!UICONTROL Index number].</p> <p>To display all characters (including hidden) in the document, you can use the [!UICONTROL Show] add-on. You can find the add-on under [!UICONTROL Add-ons] &gt; [!UICONTROL Get add-ons]. Search for [!UICONTROL Show] and install the [!UICONTROL Show] add-on.</p> </li> 
         <li> <p><strong>[!UICONTROL Image URL]</strong> </p> <p>Enter the URL of the image you want to insert to the document.</p> <p>The maximum image size is 50 MB. Must not exceed 25 megapixels. Only PNG, JPEG or GIF format is supported.</p> </li> 
        </ul> </li> 
       <li> <p><strong>[!UICONTROL By segment ID]</strong> </p> <p>Select the header and footer you want to insert the image to and enter the image URL to the corresponding fields.</p> <p>The maximum image size is 50 MB. The image must not exceed 25 megapixels. Only PNG, JPEG, or GIF format is supported.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL By appending to the body of the document]</strong> </p> <p>Appends a specific image at the end of the document's body content.</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL By appending to the end of segment (Header and Footer)]</strong> </p> <p>Select the header and footer you want to insert an image to and enter the image URL you want to insert to the corresponding fields.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Height Magnitude in Points/Width Magnitude in Points]</p> </td> 
   <td> <p>Define the size of the inserted image. The aspect ratio will be kept.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Replace an Image with a New Image]

This action module replaces an existing image. The aspect ratio of the original image will be maintained.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Google] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to [!DNL Workfront Fusion]</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Select a Document]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>Select this option to map the document template.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br> Select this option to choose the document from the drop-down menu.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose a Drive]</td> 
   <td> <p>Select the type of drive where the document you want to replace an image is located. This option is available if you selected [!UICONTROL By Dropdown] in the previous field.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Select the folder where the document you want to replace an image is located, then select the document.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>Select the folder where the document you want to replace an image is located, then select the document.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Shared Drive]</strong> (available for [!DNL G Suite] users only)</p> <p>Select whether you want to [!UICONTROL Use Domain Admin Access]. Selecting [!UICONTROL Yes] issues the request as a domain administrator, and all shared drives in which the requester is an administrator are returned.</p> <p>Select the shared drive where the document you want to replace an image is located, then select the document.</p> <p>Note: If you have selected the [!DNL Google Docs] option in this field and you are not a [!DNL G Suite] user, the error <code>[400] Invalid Value</code> is returned.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Image URL]</p> </td> 
   <td> <p>Enter or map the URL of the new image that will replace the existing image.</p> <p>Images are listed in the order they appear in the document. For example, <code>Body: Image No. 1</code> is the first image in the document.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Replace Text in a Document]

This action module replaces text in a document.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Google] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to [!DNL Workfront Fusion]</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Select a Document]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>Select this option to map the document template.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br> Select this option to choose the document from the drop-down menu.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose a Drive]</td> 
   <td> <p>Select the type of drive where the document you want to add text to is located. This option is available if you selected [!UICONTROL By Dropdown] in the previous field.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Select the folder where the document you want to add text to is located, then select the document.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>Select the folder where the document you want to add text to is located, then select the document.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Shared Drive]</strong> (available for [!DNL G Suite] users only)</p> <p>Select whether you want to [!UICONTROL Use Domain Admin Access]. Selecting [!UICONTROL Yes] issues the request as a domain administrator, and all shared drives in which the requester is an administrator are returned.</p> <p>Select the shared drive where the document you want to add text to is located, then select the document.</p> <p>Note: If you have selected the [!DNL Google Docs] option in this field and you are not a [!DNL G Suite] user, the error <code>[400] Invalid Value</code> is returned.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Replace a Text]</p> </td> 
   <td> <p>Add each text that you want to replace.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Old text to be replaced]</strong> </p> <p>Enter the text you want to replace.</p> </li> 
     <li> <p><strong>[!UICONTROL New text to be inserted]</strong> </p> <p>Enter the new text.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Download a Document]

This action module converts and downloads the selected document.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Google] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to [!DNL Workfront Fusion]</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose a Drive]</td> 
   <td> <p>Select the type of drive where the document you want to download is located.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Select the folder where the document you want to download is located, then select the document.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>Select the folder where the document you want to download is located, then select the document.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Shared Drive]</strong> (available for [!DNL G Suite] users only)</p> <p>Select whether you want to [!UICONTROL Use Domain Admin Access]. Selecting [!UICONTROL Yes] issues the request as a domain administrator, and all shared drives in which the requester is an administrator are returned.</p> <p>Select the shared drive where the document you want to download is located, then select the document.</p> <p>Note: If you have selected the [!DNL Google Docs] option in this field and you are not a [!DNL G Suite] user, the error <code>[400] Invalid Value</code> is returned.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Type] </p> </td> 
   <td> <p>Select the target file format of the downloaded document.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a Document]

This action module deletes a document.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Google] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to [!DNL Workfront Fusion]</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose a Drive]</td> 
   <td> <p>Select the type of drive where the document you want to delete is located.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Select the folder where the document you want to delete is located, then select the document.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>Select the folder where the document you want to delete is located, then select the document.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Shared Drive]</strong> (available for [!DNL G Suite] users only)</p> <p>Select whether you want to [!UICONTROL Use Domain Admin Access]. Selecting [!UICONTROL Yes] issues the request as a domain administrator, and all shared drives in which the requester is an administrator are returned.</p> <p>Select the shared drive where the document you want to delete is located, then select the document.</p> <p>Note: If you have selected the [!DNL Google Docs] option in this field and you are not a [!DNL G Suite] user, the error <code>[400] Invalid Value</code> is returned.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Shared Drive]</td> 
   <td> <p>Select the drive that contains the document you want to download, then select a document. This option is available if you have selected [!DNL Google Docs] in the [!UICONTROL Choose a Drive] field.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Document ID]</td> 
   <td> <p> Select or map the document you want to replace one or more images in.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Other

* [[!UICONTROL Make an API Call]](#make-an-api-call) 
* [[!UICONTROL Make All Links in a Document Clickable]](#make-all-links-in-a-document-clickable)

#### [!UICONTROL Make an API Call]

This action module allows you to perform a custom API call.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Google] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to [!DNL Workfront Fusion]</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Enter a path relative to <code>https://docs.googleapis.com/</code>. Example: <code>/v1/documents/{presentationID}</code>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP request methods in [!DNL Adobe Workfront Fusion]</a>.</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.For example, <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] adds the authorization headers for you.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> Enter the request query string.</p> </td> 
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

**Example:** The following API call retrieves the details for the specified document in your Google Docs:

**URL:**

/v1/documents/1ujkf-GDgB0TQSYPrxbCSK4Uso54tHVMqHZEVZZxB6aY

**Method:**

[!UICONTROL GET]

![](assets/api-call-example.png)

Details of the retrieved document can be found in the module's Output under [!UICONTROL Bundle] > [!UICONTROL Body].

![](assets/api-output.png)

#### [!UICONTROL Make All Links in a Document Clickable] 

This action module finds all links in the document and makes them clickable.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>For instructions about connecting your [!DNL Google] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to [!DNL Workfront Fusion]</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Make All Links in a Document]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL By Mapping]</strong> <br>Select this option to map the document template.</li> 
     <li><strong>[!UICONTROL By Dropdown]</strong> <br> Select this option to choose the document from the drop-down menu.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose a Drive]</td> 
   <td> <p>Select the type of drive where the document you want to make links clickable in is located. This option is available if you selected [!UICONTROL By Dropdown] in the previous field.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL My Drive]</strong> </p> <p>Select the folder where the document you want to make links clickable in is located, then select the document.</p> </li> 
     <li> <p><strong>[!UICONTROL Shared With Me]</strong> </p> <p>Select the folder where the document you want to make links clickable in is located, then select the document.</p> </li> 
     <li> <p><strong>[!UICONTROL [!DNL Google] Shared Drive]</strong> (available for [!DNL G Suite] users only)</p> <p>Select whether you want to [!UICONTROL Use Domain Admin Access]. Selecting [!UICONTROL Yes] issues the request as a domain administrator, and all shared drives in which the requester is an administrator are returned.</p> <p>Select the shared drive where the document you want to make links clickable in is located, then select the document.</p> <p>Note: If you have selected the [!DNL Google Docs] option in this field and you are not a [!DNL G Suite] user, the error <code>[400] Invalid Value</code> is returned.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Shared Drive]</td> 
   <td> <p>Select the drive that contains the document you want to update links in, then select a document. This option is available if you have selected [!DNL Google Docs] in the [!UICONTROL Choose a Drive field].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Document ID]</td> 
   <td> <p> Select or map the document you want to update the links in.</p> </td> 
  </tr> 
 </tbody> 
</table>
