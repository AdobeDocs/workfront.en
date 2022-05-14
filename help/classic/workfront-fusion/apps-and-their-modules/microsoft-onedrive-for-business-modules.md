---
filename: microsoft-onedrive-for-business-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Microsoft OneDrive for Business
description: In an Adobe Workfront Fusion scenario, you can automate workflows that use Microsoft OneDrive for Business, as well as connect it to to multiple third-party applications and services.
---

# Microsoft OneDrive for Business

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

In an Adobe Workfront Fusion scenario, you can automate workflows that use Microsoft OneDrive for Business, as well as connect it to to multiple third-party applications and services.

If you need instructions on creating a scenario, see [Create a scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in Adobe Workfront Fusion](../../workfront-fusion/modules/modules.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table> 
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

To use Microsoft OneDrive for Business with Adobe Workfront Fusion, you will need a Microsoft account.

For instructions about connecting your OneDrive for Business account to Workfront Fusion, see [Create a connection to Adobe Workfront Fusion - Basic instructions](../../workfront-fusion/connections/connect-to-fusion-general.md)

## Microsoft OneDrive for Business modules and their fields

When you configure [Fusion app] modules, Workfront Fusion displays the fields listed below. Along with these, additional [Fusion app] fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Triggers](#triggers) 
* [Actions](#actions)

### Triggers {#triggers}

* [Watch files](#watch-files) 
* [Watch folders](#watch-folders)

#### Watch files {#watch-files}

This trigger module activates when a new file is added or updated in a folder being watched.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Drive ID</p> </td> 
   <td> <p>Select the drive that you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Folder</td> 
   <td> <p> Select the folder that you want to watch. Within a scenario, you can only monitor one folder.</p> <p>Tip: To keep track of multiple folders, create an independent scenario for each of them.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>I want to watch</p> </td> 
   <td> <p>Select whether you want to watch new files and all changes, or new files only.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Maximum number of returned rows</td> 
   <td> <p> Set the maximum number of results that Workfront Fusion will work with during one cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Watch folders {#watch-folders}

This trigger module activates when a new folder is added to the folder being watched.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Connection</p> </td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Drive ID</p> </td> 
   <td> <p>Select the drive that you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Folder</td> 
   <td> <p> Select the folder that you want to watch. Within a scenario, you can only monitor one folder.</p> <p>Tip: To keep track of multiple folders, create an independent scenario for each of them.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>I want to watch</p> </td> 
   <td> <p>Select whether you want to watch new folders and all changes, or new folders only.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Maximum number of returned rows</td> 
   <td> <p> Set the maximum number of results that Workfront Fusion will work with during one cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions {#actions}

* [Upload a file](#upload-a-file) 
* [Delete a file](#delete-a-file) 
* [Get a file](#get-a-file) 
* [Create a folder](#create-a-folder) 
* [Delete a folder](#delete-a-folder) 
* [Get a sharing link](#get-a-sharing-link)

#### Upload a file {#upload-a-file}

This action module uploads a binary or text file to a specified folder

<table> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in Adobe Workfront Fusion</a>.</p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Drive ID</td> 
   <td> <p>Select the drive you want to upload a file to.</p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Folder </td> 
   <td> <p>Select the folder within the drive.</p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p>Source File</p> </td> 
   <td> <p>Select a source file from a previous module, or map the source file's name and data.</p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>If the file with the same name exists</td> 
   <td> <p> Select what you want to do if a file with the same name as the file you are trying up upload already exists.</p> 
    <ul> 
     <li>Replace the existing file</li> 
     <li>Rename the new file</li> 
     <li>End with an error</li> 
    </ul> </td> 
   <td>&nbsp;</td> 
  </tr> 
 </tbody> 
</table>

#### Delete a file {#delete-a-file}

This action module moves the specified file to the recycle bin.

<table> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in Adobe Workfront Fusion</a>.</p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Drive ID</td> 
   <td> <p>Select the drive you want to delete a file from.</p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>File ID</td> 
   <td> <p>Enter the ID of the file you want to delete. </p> </td> 
   <td>&nbsp;</td> 
  </tr> 
 </tbody> 
</table>

#### Get a file {#get-a-file}

This action module retrieves the file with the given ID.

<table> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in Adobe Workfront Fusion</a>.</p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Drive ID</td> 
   <td> <p>Select the drive you want to retrieve a file from.</p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>File ID</td> 
   <td> <p>Enter the ID of the file you want to retrieve. </p> </td> 
   <td>&nbsp;</td> 
  </tr> 
 </tbody> 
</table>

#### Create a folder {#create-a-folder}

Creates a folder inside the specified parent folder.

<table> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Connection</strong> </td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in Adobe Workfront Fusion</a>.</p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>Drive ID</strong> </td> 
   <td> <p>Select the drive where you want to create a new folder.</p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>Folder</strong> </td> 
   <td> <p>Select the folder that you want to create a new folder in.</p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>Folder name</strong> </td> 
   <td>Enter or map a name for the new folder.</td> 
   <td>&nbsp;</td> 
  </tr> 
 </tbody> 
</table>

#### Delete a folder {#delete-a-folder}

<table> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in Adobe Workfront Fusion</a>.</p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Drive ID</td> 
   <td> <p>Select the drive you want to delete a file from.</p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Folder ID</td> 
   <td> <p>Enter or map the ID of the folder you want to delete. </p> </td> 
   <td>&nbsp;</td> 
  </tr> 
 </tbody> 
</table>

#### Get a sharing link {#get-a-sharing-link}

This module retrieves a link that you can share to give access to the specified file.

<table> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your Office 365 account to Workfront Fusion, see <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Connect the module's app or web service to Workfront Fusion</a> in the article <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Create a scenario in Adobe Workfront Fusion</a>.</p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Drive ID</td> 
   <td> <p>Select the drive you want to upload a file to.</p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Enter</td> 
   <td> <p>Select whether you want to choose a file by using the File ID&nbsp;or the File path. Enter the File ID&nbsp;or path in the field that appears.</p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p>Permission type</p> </td> 
   <td> <p>Select whether you want people who receive the link to have read/write permissions or read only.</p> </td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Scope</td> 
   <td> <p> Select whether you want the file to be accessible by anyone who has the link or accessible to members of your organization only.</p> </td> 
   <td>&nbsp;</td> 
  </tr> 
 </tbody> 
</table>

