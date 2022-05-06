---
filename: about-mapping-files
content-type: overview
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: About mapping files in Adobe Workfront Fusion
description: Some modules have the capability to process files. These modules can either return an output file to be sent for further processing or require a file to be passed to them for processing. Before these modules can work together to process files, they have to be mapped to each other.
---

# About mapping files in Adobe Workfront Fusion

Some modules have the capability to process files. These modules can either return an output file to be sent for further processing or require a file to be passed to them for processing. Before these modules can work together to process files, they have to be mapped to each other.

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
   <td> <p>Workfront Fusion for Work Automation and Integration </p>  </td> 
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

## Mapping Files

Modules that have the ability to work with files require two pieces of information:

* File name
* File content (data)

When you map a file, you choose the modules in your scenario from which you want to obtain the data. The file name and file content are then automatically mapped as they are.

``` ```**Example: **`````` This example shows how to download documents from Adobe Workfront to Google Drive. The Workfront trigger Watch Record returns detailed information about each document, including its name and ID.

The next module, Download Document, downloads the actual data so that it can be uploaded to Google Drive.

To map this information to Google Drive so that it can be uploaded, you need to specify the source file from which the information will be mapped. If you select the Workfront - Download Document option under the source file, Workfront Fusion maps the file name and file content so that the document from Workfront is uploaded to the specified Google folder.

![](assets/wf-download-document-350x605.png)

However, if you wanted to rename the file, but keep the data as it is, you could use the Map option to map the file name and file content separately. You would enter the full file name, including the extension. Text formats and binary formats, such as photos, videos, and PDF, are supported.

![](assets/use-the-map-option-350x358.png)

