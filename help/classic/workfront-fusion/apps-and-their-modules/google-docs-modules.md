---
filename: google-docs-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Google Docs modules
description: The Adobe Workfront Fusion Google Docs modules enable you to monitor, create, edit and retrieve documents in your Google Docs and Google Shared Drive (for G Suite users).
---

# Google Docs modules

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

The Adobe Workfront Fusion Google Docs modules enable you to monitor, create, edit and retrieve documents in your Google Docs and Google Shared Drive (for G Suite users).

In order to use Google Docswith Adobe Workfront Fusion, it is necessary to have a Google account. If you don't have a Google account yet, you can create one at the Google Account help page.

If you need instructions on creating a scenario, see [Create a scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in Adobe Workfront Fusion](../../workfront-fusion/modules/modules.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan, Work</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion license**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Access level configurations*</td> 
    <td> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your organization.</p>
     --> <!--
      <p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must be a Workfront Fusion administrator for your team.</p>
     --> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisites

To use Google Doc modules, you must have a Google account.

## Google Doc modules and their fields

When you configure Google Docs modules, Workfront Fusion displays the fields listed below. Along with these, additional Google Docs fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Document

* [Watch Documents](#watch-documents) 
* [List Documents](#list-documents) 
* [Get Content of a Document](#get-content-of-a-document) 
* [Create a Document](#create-a-document) 
* [Create a Document From a Template](#create-a-document-from-a-template) 
* [Insert a Paragraph to a Document](#insert-a-paragraph-to-a-document) 
* [Insert an Image to a Document](#insert-an-image-to-a-document) 
* [Replace an Image with a New Image](#replace-an-image-with-a-new-image) 
* [Replace an Image with a New Image](#replace-an-image-with-a-new-image) 
* [Download a Document](#download-a-document) 
* [Delete a Document](#delete-a-document)

#### Watch Documents {#watch-documents}

This trigger module returns document details when a new document is created or modified in the selected folder.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Google account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Watch Documents</td> 
   <td> <p style="color: #000000;">Select whether you want to watch created (By Created Date) or modified (By Modified Date) documents.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Choose a Drive</td> 
   <td> <p>Select the type of drive you want to monitor.</p> 
    <ul> 
     <li> <p><strong>My Drive</strong> </p> <p>Select the folder you want to watch for created or modified documents.</p> </li> 
     <li> <p><strong>Shared With Me</strong> </p> <p>Select the folder you want to watch for created or modified documents.</p> </li> 
     <li> <p><strong>Google Shared Drive</strong> (available for G Suite users only)</p> <p>Select whether you want to Use Domain Admin Access. Selecting Yes issues the request as a domain administrator, and all shared drived in which the requester is an administrator are returned.</p> <p>Select the shared drive you want to watch.</p> <p>Note: If you have selected the Google Shared Drive option in this field and you are not a G Suite user, the error <code>[400] Invalid Value</code> is returned.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit </td> 
   <td> <p>Set the maximum number of documents Workfront Fusion returns in one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### List Documents {#list-documents}

This action module retrieves a list of documents from the selected folder.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Google account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Choose a Drive</td> 
   <td> <p>Select the type of drive you want to list documents from.</p> 
    <ul> 
     <li> <p><strong>My Drive</strong> </p> <p>Select the folder you want to list documents from.</p> </li> 
     <li> <p><strong>Shared With Me</strong> </p> <p>Select the folder you want to list documents from.</p> </li> 
     <li> <p><strong>Google Shared Drive</strong> (available for G Suite users only)</p> <p>Select whether you want to Use Domain Admin Access. Selecting Yes issues the request as a domain administrator, and all shared drived in which the requester is an administrator are returned.</p> <p>Select the shared drive you want to list documents from.</p> <p>Note: If you have selected the Google Shared Drive option in this field and you are not a G Suite user, the error <code>[400] Invalid Value</code> is returned.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Limit </td> 
   <td> <p>Set the maximum number of documents Workfront Fusion returns in one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Get Content of a Document {#get-content-of-a-document}

This action module retrieves a specified document.

You may need to extend your permissions.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Google account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Get Content of a Document</td> 
   <td> <p>Select whether you want to map the document ID of the document or select the document from the drop-down menu manually.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Choose a Drive</td> 
   <td> <p>Select the type of drive that contains the document you want to retrieve.</p> 
    <ul> 
     <li> <p><strong>My Drive</strong> </p> <p>Select the folder that contains the document you want to retrieve.</p> </li> 
     <li> <p><strong>Shared With Me</strong> </p> <p>Select the folder that contains the document you want to retrieve.</p> </li> 
     <li> <p><strong>Google Shared Drive</strong> (available for G Suite users only)</p> <p>Select whether you want to Use Domain Admin Access. Selecting Yes issues the request as a domain administrator, and all shared drived in which the requester is an administrator are returned.</p> <p>Select the shared drive that contains the document you want to retrieve.</p> <p>Note: If you have selected the Google Shared Drive option in this field and you are not a G Suite user, the error <code>[400] Invalid Value</code> is returned.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Filter</p> </td> 
   <td> <p>Select the object you want to be returned in the module's output.</p> 
    <ul> 
     <li>Image (default)</li> 
     <li>Drawing</li> 
     <li>Chart</li> 
    </ul> <p>Note:  <p>For further mapping of these objects, please use the Inline Objects Array value in this module's output (instead of inlineObjects).</p> <p>The Inline Objects Array objects are sorted in the same order they appear in the document. It will make any further processing easier.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### Create a Document {#create-a-document}

This action module allows you to create a new document in the selected folder.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Google account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Name </td> 
   <td> <p>Enter the name of the document.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Content</td> 
   <td> <p>Enter the content of the document. HTML is supported.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Choose a Drive</td> 
   <td> <p>Select the type of drive where you want to create a document.</p> 
    <ul> 
     <li> <p><strong>My Drive</strong> </p> <p>Select the folder where you want to create a document.</p> </li> 
     <li> <p><strong>Shared With Me</strong> </p> <p>Select the folder where you want to create a document.</p> </li> 
     <li> <p><strong>Google Shared Drive</strong> (available for G Suite users only)</p> <p>Select whether you want to Use Domain Admin Access. Selecting Yes issues the request as a domain administrator, and all shared drived in which the requester is an administrator are returned.</p> <p>Select the shared drive where you want to create a document.</p> <p>Note: If you have selected the Google Shared Drive option in this field and you are not a G Suite user, the error <code>[400] Invalid Value</code> is returned.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Insert a Header</td> 
   <td> <p> Enable this option to insert the header to the document, then enter or map the text of the header.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Insert a Footer </td> 
   <td> <p>Enable this option to insert the footer to the document, then enter or map the text of the header.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Create a Document From a Template {#create-a-document-from-a-template}

This action module creates a copy of an existing template document and replaces any tags. This module also allows users to replace images with new images by URL.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Google account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Create a Document from a Template</p> </td> 
   <td> 
    <ul> 
     <li><strong>By Mapping</strong> <br>Select this option to map the document template.</li> 
     <li><strong>By Dropdown</strong> <br>Select this option to choose the document template from the drop-down menu.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Choose a Drive</td> 
   <td> <p>Select the type of drive where your template is located. This option is available if you selected By Dropdown in the previous field.</p> 
    <ul> 
     <li> <p><strong>My Drive</strong> </p> <p>Select the folder where your template is located.</p> </li> 
     <li> <p><strong>Shared With Me</strong> </p> <p>Select the folder where your template is located.</p> </li> 
     <li> <p><strong>Google Shared Drive</strong> (available for G Suite users only)</p> <p>Select whether you want to Use Domain Admin Access. Selecting Yes issues the request as a domain administrator, and all shared drived in which the requester is an administrator are returned.</p> <p>Select the shared drive where your template is located.</p> <p>Note: If you have selected the Google Shared Drive option in this field and you are not a G Suite user, the error <code>[400] Invalid Value</code> is returned.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Values</p> </td> 
   <td> <p>Enter the values that will be entered instead of the variables to the new document.</p> 
    <ul> 
     <li><strong>Tags</strong> <br>Enter the tags that are contained in the document template. Do not use <code>{{}}</code>. Example: use <code>name </code>instead of <code>{{name}}</code>.</li> 
     <li><strong>Replaced Value</strong><![CDATA[	]]><br>Enter the value of the tag.</li> 
    </ul> <p>For example the<code> {{name}}</code> variable in the source document will be displayed as the name field here, where the value can be inserted, such as <code>John</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Images Replacement</p> </td> 
   <td> <p>Enter the link to the Image Object ID and Image URL that will replace the current image.</p> <p>Note:  You can retrieve the image IDs by using Get a Document module, where the IDs are contained in the array Inline Object Array.</p> <p>We recommend that you add ALT text to images in your Google document. </p> <p>To add an ALT Text to the Google Docs image:</p> 
    <ol> 
     <li value="1">Right click on the image.</li> 
     <li value="2">Select the ALT text option.</li> 
     <li value="3">Enter the ALT text in the Title field and click OK.</li> 
    </ol> <p>After the ALT text is added to the image, the ALT text is displayed in the field name in parentheses.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Title </td> 
   <td> <p>Enter the name for the new document.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Choose a Drive</td> 
   <td> <p>Select the type of drive where your template is located. This option is available if you selected By Dropdown in the previous field.</p> 
    <ul> 
     <li> <p><strong>My Drive</strong> </p> <p>Select the folder where you want the document to be created.</p> </li> 
     <li> <p><strong>Shared With Me</strong> </p> <p>Select the folder where you want the document to be created.</p> </li> 
     <li> <p><strong>Google Shared Drive</strong> (available for G Suite users only)</p> <p>Select whether you want to Use Domain Admin Access. Selecting Yes issues the request as a domain administrator, and all shared drived in which the requester is an administrator are returned.</p> <p>Select the shared drive where you want the document to be created.</p> <p>Note: If you have selected the Google Shared Drive option in this field and you are not a G Suite user, the error <code>[400] Invalid Value</code> is returned.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### Insert a Paragraph to a Document {#insert-a-paragraph-to-a-document}

This action module appends or inserts a new paragraph to an existing document.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Google account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Select a Document</p> </td> 
   <td> 
    <ul> 
     <li><strong>By Mapping</strong> <br>Select this option to map the document.</li> 
     <li><strong>By Dropdown</strong> <br> Select this option to choose the document from the drop-down menu.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Choose a Drive</td> 
   <td> <p>Select the type of drive where the document you want to add a paragraph to is located. This option is available if you selected By Dropdown in the previous field.</p> 
    <ul> 
     <li> <p><strong>My Drive</strong> </p> <p>Select the folder where the document you want to add a paragraph to is located, then select the document.</p> </li> 
     <li> <p><strong>Shared With Me</strong> </p> <p>Select the folder where the document you want to add a paragraph to is located, then select the document.</p> </li> 
     <li> <p><strong>Google Shared Drive</strong> (available for G Suite users only)</p> <p>Select whether you want to Use Domain Admin Access. Selecting Yes issues the request as a domain administrator, and all shared drived in which the requester is an administrator are returned.</p> <p>Select the shared drive where the document you want to add a paragraph to is located, then select the document.</p> <p>Note: If you have selected the Google Shared Drive option in this field and you are not a G Suite user, the error <code>[400] Invalid Value</code> is returned.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Insert a Paragraph</p> </td> 
   <td> <p>Select how you want the new text to be inserted in the document.</p> 
    <ul> 
     <li> <p><strong>By specification of location</strong> </p> 
      <ul> 
       <li> <p><strong>By index</strong> </p> 
        <ul> 
         <li> <p><strong>Index</strong> </p> <p>Enter the Index number where you would like to insert your text. You can use the Get a Document module retrieve Index number.</p> <p>To display all characters (including hidden) in the document, you can use the Show add-on. You can find the add-on under Add-ons &gt; Get add-ons. Search for Show and install the Show add-on.</p> </li> 
         <li> <p><strong>Inserted text</strong> </p> <p>Enter the text you want to insert to the document.</p> </li> 
        </ul> </li> 
       <li> <p><strong>By segment ID</strong> </p> <p>Select the header and footer you want to insert the text content to and enter the text you want to insert to the corresponding fields.</p> <p>If the header or footer already contains text, the new text will be added before the existing text.</p> </li> 
      </ul> </li> 
     <li> <p><strong>By appending to the body of the document</strong> </p> <p>Appends entered text at the end of the document's body content.</p> <p>The style of the new paragraph will be copied from the paragraph at the current insertion index, including lists and bullets.</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>By appending to the end of segment (Header and Footer)</strong> </p> <p>Select the header and footer you want to insert the text content to and enter the text you want to insert to the corresponding fields.</p> <p>If the header or footer already contain text, the new text will be added after the existing text.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Appended Text</td> 
   <td>Enter or map the text you want to append to the document</td> 
  </tr> 
 </tbody> 
</table>

#### Insert an Image to a Document {#insert-an-image-to-a-document}

This action module inserts an image from the URL to the document.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Google account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Select a Document</p> </td> 
   <td> 
    <ul> 
     <li><strong>By Mapping</strong> <br>Select this option to map the document template.</li> 
     <li><strong>By Dropdown</strong> <br> Select this option to choose the document from the drop-down menu.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Choose a Drive</td> 
   <td> <p>Select the type of drive where the document you want to add an image to is located. This option is available if you selected By Dropdown in the previous field.</p> 
    <ul> 
     <li> <p><strong>My Drive</strong> </p> <p>Select the folder where the document you want to add an image to is located, then select the document.</p> </li> 
     <li> <p><strong>Shared With Me</strong> </p> <p>Select the folder where the document you want to add an image to is located, then select the document.</p> </li> 
     <li> <p><strong>Google Shared Drive</strong> (available for G Suite users only)</p> <p>Select whether you want to Use Domain Admin Access. Selecting Yes issues the request as a domain administrator, and all shared drived in which the requester is an administrator are returned.</p> <p>Select the shared drive where the document you want to add an image to is located, then select the document.</p> <p>Note: If you have selected the Google Shared Drive option in this field and you are not a G Suite user, the error <code>[400] Invalid Value</code> is returned.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Insert an Image</p> </td> 
   <td> <p>Select how you want the new image to be inserted in the document.</p> 
    <ul> 
     <li> <p><strong>By specification of location</strong> </p> 
      <ul> 
       <li> <p><strong>By index</strong> </p> 
        <ul> 
         <li> <p><strong>Index</strong> </p> <p>Enter the Index number where you would like to insert your image. You can use the Get a Document module retrieve Index number.</p> <p>To display all characters (including hidden) in the document, you can use the Show add-on. You can find the add-on under Add-ons &gt; Get add-ons. Search for Show and install the Show add-on.</p> </li> 
         <li> <p><strong>Image URL</strong> </p> <p>Enter the URL of the image you want to insert to the document.</p> <p>The maximum image size is 50 MB. Must not exceed 25 megapixels. Only PNG, JPEG or GIF format is supported.</p> </li> 
        </ul> </li> 
       <li> <p><strong>By segment ID</strong> </p> <p>Select the header and footer you want to insert the image to and enter the image URL to the corresponding fields.</p> <p>The maximum image size is 50 MB. The image must not exceed 25 megapixels. Only PNG, JPEG, or GIF format is supported.</p> </li> 
      </ul> </li> 
     <li> <p><strong>By appending to the body of the document</strong> </p> <p>Appends a specific image at the end of the document's body content.</p> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>By appending to the end of segment (Header and Footer)</strong> </p> <p>Select the header and footer you want to insert an image to and enter the image URL you want to insert to the corresponding fields.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Height Magnitude in Points/Width Magnitude in Points</p> </td> 
   <td> <p>Define the size of the inserted image. The aspect ratio will be kept.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Replace an Image with a New Image {#replace-an-image-with-a-new-image}

This action module replaces an existing image. The aspect ratio of the original image will be maintained.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Google account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Select a Document</p> </td> 
   <td> 
    <ul> 
     <li><strong>By Mapping</strong> <br>Select this option to map the document template.</li> 
     <li><strong>By Dropdown</strong> <br> Select this option to choose the document from the drop-down menu.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Choose a Drive</td> 
   <td> <p>Select the type of drive where the document you want to replace an image is located. This option is available if you selected By Dropdown in the previous field.</p> 
    <ul> 
     <li> <p><strong>My Drive</strong> </p> <p>Select the folder where the document you want to replace an image is located, then select the document.</p> </li> 
     <li> <p><strong>Shared With Me</strong> </p> <p>Select the folder where the document you want to replace an image is located, then select the document.</p> </li> 
     <li> <p><strong>Google Shared Drive</strong> (available for G Suite users only)</p> <p>Select whether you want to Use Domain Admin Access. Selecting Yes issues the request as a domain administrator, and all shared drived in which the requester is an administrator are returned.</p> <p>Select the shared drive where the document you want to replace an image is located, then select the document.</p> <p>Note: If you have selected the Google Shared Drive option in this field and you are not a G Suite user, the error <code>[400] Invalid Value</code> is returned.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Image URL</p> </td> 
   <td> <p>Enter or map the URL of the new image that will replace the existing image.</p> <p>Images are listed in the order they appear in the document. For example, <code>Body: Image No. 1</code> is the first image in the document.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Replace Text in a Document

This action module replaces text in a document.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Google account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Select a Document</p> </td> 
   <td> 
    <ul> 
     <li><strong>By Mapping</strong> <br>Select this option to map the document template.</li> 
     <li><strong>By Dropdown</strong> <br> Select this option to choose the document from the drop-down menu.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Choose a Drive</td> 
   <td> <p>Select the type of drive where the document you want to add text to is located. This option is available if you selected By Dropdown in the previous field.</p> 
    <ul> 
     <li> <p><strong>My Drive</strong> </p> <p>Select the folder where the document you want to add text to is located, then select the document.</p> </li> 
     <li> <p><strong>Shared With Me</strong> </p> <p>Select the folder where the document you want to add text to is located, then select the document.</p> </li> 
     <li> <p><strong>Google Shared Drive</strong> (available for G Suite users only)</p> <p>Select whether you want to Use Domain Admin Access. Selecting Yes issues the request as a domain administrator, and all shared drived in which the requester is an administrator are returned.</p> <p>Select the shared drive where the document you want to add text to is located, then select the document.</p> <p>Note: If you have selected the Google Shared Drive option in this field and you are not a G Suite user, the error <code>[400] Invalid Value</code> is returned.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Replace a Text</p> </td> 
   <td> <p>Add each text that you want to replace.</p> 
    <ul> 
     <li> <p><strong>Old text to be replaced</strong> </p> <p>Enter the text you want to replace.</p> </li> 
     <li> <p><strong>New text to be inserted</strong> </p> <p>Enter the new text.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### Download a Document {#download-a-document}

This action module converts and downloads the selected document.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Google account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Choose a Drive</td> 
   <td> <p>Select the type of drive where the document you want to download is located. This option is available if you selected By Dropdown in the previous field.</p> 
    <ul> 
     <li> <p><strong>My Drive</strong> </p> <p>Select the folder where the document you want to download is located, then select the document.</p> </li> 
     <li> <p><strong>Shared With Me</strong> </p> <p>Select the folder where the document you want to download is located, then select the document.</p> </li> 
     <li> <p><strong>Google Shared Drive</strong> (available for G Suite users only)</p> <p>Select whether you want to Use Domain Admin Access. Selecting Yes issues the request as a domain administrator, and all shared drived in which the requester is an administrator are returned.</p> <p>Select the shared drive where the document you want to download is located, then select the document.</p> <p>Note: If you have selected the Google Shared Drive option in this field and you are not a G Suite user, the error <code>[400] Invalid Value</code> is returned.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Type </p> </td> 
   <td> <p>Select the target file format of the downloaded document.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Delete a Document {#delete-a-document}

This action module deletes a document.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Google account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Choose a Drive</td> 
   <td> <p>Select the type of drive where the document you want to delete is located. This option is available if you selected By Dropdown in the previous field.</p> 
    <ul> 
     <li> <p><strong>My Drive</strong> </p> <p>Select the folder where the document you want to delete is located, then select the document.</p> </li> 
     <li> <p><strong>Shared With Me</strong> </p> <p>Select the folder where the document you want to delete is located, then select the document.</p> </li> 
     <li> <p><strong>Google Shared Drive</strong> (available for G Suite users only)</p> <p>Select whether you want to Use Domain Admin Access. Selecting Yes issues the request as a domain administrator, and all shared drived in which the requester is an administrator are returned.</p> <p>Select the shared drive where the document you want to delete is located, then select the document.</p> <p>Note: If you have selected the Google Shared Drive option in this field and you are not a G Suite user, the error <code>[400] Invalid Value</code> is returned.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Shared Drive</td> 
   <td> <p>Select the drive that contains the document you want to download, then select a document. This option is available if you have selected Google Shared Drive in the Choose a Drive field.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Document ID</td> 
   <td> <p> Select or map the document you want to replace one or more images in.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Other

* [Make an API Call](#make-an-api-call) 
* [Make All Links in a Document Clickable](#make-all-links-in-a-document-clickable)

#### Make an API Call {#make-an-api-call}

This action module allows you to perform a custom API call.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection </td> 
   <td> <p>For instructions about connecting your Google account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Enter a path relative to <code>https://docs.googleapis.com/</code>. Example: <code>/v1/documents/{presentationID}</code>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Method</td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP request methods in Adobe Workfront Fusion</a>.</p> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Headers</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.For example, <code>{"Content-type":"application/json"}</code>. Workfront Fusion adds the authorization headers for you.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Query String</td> 
   <td> <p> Enter the request query string.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Body</td> 
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

GET

![](assets/api-call-example.png)

Details of the retrieved document can be found in the module's Output under Bundle > Body.

![](assets/api-output.png)

#### Make All Links in a Document Clickable {#make-all-links-in-a-document-clickable}

This action module finds all links in the document and makes them clickable.

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection</td> 
   <td> <p>For instructions about connecting your Google account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Make All Links in a Document</p> </td> 
   <td> 
    <ul> 
     <li><strong>By Mapping</strong> <br>Select this option to map the document template.</li> 
     <li><strong>By Dropdown</strong> <br> Select this option to choose the document from the drop-down menu.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Choose a Drive</td> 
   <td> <p>Select the type of drive where the document you want to make links clickable in is located. This option is available if you selected By Dropdown in the previous field.</p> 
    <ul> 
     <li> <p><strong>My Drive</strong> </p> <p>Select the folder where the document you want to make links clickable in is located, then select the document.</p> </li> 
     <li> <p><strong>Shared With Me</strong> </p> <p>Select the folder where the document you want to make links clickable in is located, then select the document.</p> </li> 
     <li> <p><strong>Google Shared Drive</strong> (available for G Suite users only)</p> <p>Select whether you want to Use Domain Admin Access. Selecting Yes issues the request as a domain administrator, and all shared drived in which the requester is an administrator are returned.</p> <p>Select the shared drive where the document you want to make links clickable in is located, then select the document.</p> <p>Note: If you have selected the Google Shared Drive option in this field and you are not a G Suite user, the error <code>[400] Invalid Value</code> is returned.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Shared Drive</td> 
   <td> <p>Select the drive that contains the document you want to update links in, then select a document. This option is available if you have selected Google Shared Drive in the Choose a Drive field.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Document ID</td> 
   <td> <p> Select or map the document you want to update the links in.</p> </td> 
  </tr> 
 </tbody> 
</table>

