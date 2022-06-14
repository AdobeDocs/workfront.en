---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;agile-and-teams;user-management
keywords: connector
navigation-topic: apps-and-their-modules
title: Google Team Drive modules
description: The Adobe Workfront Fusion Google Team Drive modules enable you to monitor, upload, update, copy, delete, or retrieve files and create folders in your Google Shared Drive.
feature: Workfront Fusion
---

# Google Team Drive modules

The Adobe Workfront Fusion Google Team Drive modules enable you to monitor, upload, update, copy, delete, or retrieve files and create folders in your Google Shared Drive.

In order to use Google Team Drive with Adobe Workfront Fusion, it is necessary to have a G Suite account. If you do not have one, you can create a G Suite account at the [G Suite sign up site](https://gsuite.google.com/signup/businessstarter/welcome).

In an Adobe Workfront Fusion scenario, you can automate workflows that use [Fusion app], as well as connect it to multiple third-party applications and services.

If you need instructions on creating a scenario, see [Create a scenario in Adobe Workfront Fusion](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in Adobe Workfront Fusion](../../workfront-fusion/modules/modules.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto"> 
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
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisites

To use Google Team Drive modules, you must have a Google Team Drive.

## Google Team Drive modules and their fields

>[!NOTE]
>
>The module dialog fields that are displayed in **bold** (in the Workfront Fusion scenario, **not** in this documentation article) are mandatory.

When you configure Google Team Drive modules, Workfront Fusion displays the fields listed below. Along with these, additional Google Team Drive fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Triggers

#### Watch Files

Returns file details when a new file is added and/or modified in the specified folder.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your Google Team Drive account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td>Team Drive</td> 
   <td> <p> Select the shared drive you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td>Folder </td> 
   <td> <p>Select the folder within the shared drive.</p> </td> 
  </tr> 
  <tr> 
   <td>What files to watch</td> 
   <td> <p> Select the type of files you want to watch.</p> </td> 
  </tr> 
  <tr> 
   <td>Convert Google Documents files to format </td> 
   <td> <p>Select the format you want the watched Google Documents files converted to.</p> </td> 
  </tr> 
  <tr> 
   <td>Convert Google Sheets files to format </td> 
   <td> <p>Select the format you want the watched Google Sheets files converted to.</p> </td> 
  </tr> 
  <tr> 
   <td>Convert Google Slides files to format </td> 
   <td> <p>Select the format you want the watched Google Slides files converted to.</p> </td> 
  </tr> 
  <tr> 
   <td>Convert Google Drawings files to format </td> 
   <td> <p>Select the format you want the watched Google Drawings files converted to.</p> </td> 
  </tr> 
  <tr> 
   <td>Watch</td> 
   <td> <p> Select whether you want to monitor the folder for new and modified files or just for new files.</p> </td> 
  </tr> 
  <tr> 
   <td>Maximum number of downloaded files</td> 
   <td> <p> Set the maximum number of files Workfront Fusion will return during one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [Upload a File](#upload-a-file) 
* [Update a File](#update-a-file) 
* [Copy a File](#copy-a-file) 
* [Delete a File](#delete-a-file) 
* [Move a File to Trash](#move-a-file-to-trash) 
* [Get a File](#get-a-file) 
* [Get a File List](#get-a-file-list) 
* [Create a Folder](#create-a-folder)

#### Upload a File {#upload-a-file}

Uploads a file to the specified shared drive.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your Google Team Drive account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td>Team Drive </td> 
   <td> <p>Select the shared drive you want to upload a file to.</p> </td> 
  </tr> 
  <tr> 
   <td>Folder </td> 
   <td> <p>Select the folder within the shared drive.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Source File</p> </td> 
   <td> <p>Specify the file you want to upload to the shared drive.</p> <p>Map the file you want to upload from the previous module (e.g. HTTP &gt; Get a File or Dropbox &gt; Get a file), or enter the file name and file data manually.</p> </td> 
  </tr> 
  <tr> 
   <td>Title</td> 
   <td> <p> Enter the title of the file that will be displayed in the shared folder.</p> </td> 
  </tr> 
  <tr> 
   <td>Convert a File</td> 
   <td> <p> Enable this option to convert the file to the corresponding Google format in your shared folder.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Update a File {#update-a-file}

Allows you to change the file name and/or file content.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your Google Team Drive account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td>Team Drive</td> 
   <td> <p> Select the shared drive that contains the file you want to update.</p> </td> 
  </tr> 
  <tr> 
   <td>Folder </td> 
   <td> <p>Select the folder within the shared drive.</p> </td> 
  </tr> 
  <tr> 
   <td>File ID</td> 
   <td> <p> Enter (map) the ID of the file you want to update.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Source File</p> </td> 
   <td>Select a source file from a previous module, or map the source file's name and data.</td> 
  </tr> 
  <tr> 
   <td>Title </td> 
   <td> <p>Enter the new title for the updated file.</p> </td> 
  </tr> 
  <tr> 
   <td>Convert a File</td> 
   <td> <p> Enable this option to convert the file to the corresponding Google format in your shared folder.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Copy a File {#copy-a-file}

Copies a specified file to the selected folder.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your Google Team Drive account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td>Team Drive</td> 
   <td> <p> Select the shared drive that contains the file you want to copy.</p> </td> 
  </tr> 
  <tr> 
   <td>Folder </td> 
   <td> <p>Select the target folder you want to copy the file to.</p> </td> 
  </tr> 
  <tr> 
   <td>File ID</td> 
   <td> <p> Enter (map) the ID of the file you want to copy.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>The name of the copy file</p> </td> 
   <td> <p>Enter the new file name if you want it to be changed in the target location.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Delete a File {#delete-a-file}

Deletes a specified file.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your Google Team Drive account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td>File ID</td> 
   <td> <p> Enter or map the ID of the file you want to delete.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Move a File to Trash {#move-a-file-to-trash}

Moves a specified file to the trash bin.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your Google Team Drive account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td>File ID</td> 
   <td> <p> Enter or map the ID of the file you want to move to the trash bin.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Get a File {#get-a-file}

Retrieves details about the specified file.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your Google Team Drive account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td>Convert Google Documents files to format </td> 
   <td> <p>Select the format you want the watched Google Documents files converted to.</p> </td> 
  </tr> 
  <tr> 
   <td>Convert Google Sheets files to format </td> 
   <td> <p>Select the format you want the watched Google Sheets files converted to.</p> </td> 
  </tr> 
  <tr> 
   <td>Convert Google Slides files to format </td> 
   <td> <p>Select the format you want the watched Google Slides files converted to.</p> </td> 
  </tr> 
  <tr> 
   <td>Convert Google Drawings files to format </td> 
   <td> <p>Select the format you want the watched Google Drawings files converted to.</p> </td> 
  </tr> 
  <tr> 
   <td>File ID</td> 
   <td> <p> Enter or map the ID of the file you want to retrieve.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Get a File List {#get-a-file-list}

Retrieves files and/or folders details based on the search term.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your Google Team Drive account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td>Team Drive</td> 
   <td> <p> Select the shared drive you want to list files from.</p> </td> 
  </tr> 
  <tr> 
   <td>Folder </td> 
   <td> <p>Select the folder you want to list files from.</p> </td> 
  </tr> 
  <tr> 
   <td>Search </td> 
   <td> <p>Select the type of search you want to perform - see below.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Query</p> </td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>Search within file names</p> <p style="font-weight: normal;">Enter the file name (including the file extension) when the Search for exact term Search option is selected or enter the part of the name when the Search for names containing the searched term option is selected.</p> </li> 
     <li> <p style="font-weight: bold;">Fulltext search</p> <p>Enter the search term to search through the file names, descriptions and contents.</p> </li> 
     <li> <p style="font-weight: bold;">Custom search query</p> <p>Enter the Google search query term. For more details please refer to Google's <a href="https://developers.google.com/drive/api/v2/ref-search-terms">Search Query Documentation</a>. Example: <code>fullText contains '"Hello world"'</code></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Retrieve</td> 
   <td>Select whether you want to retrieve files, folder, or both.</td> 
  </tr> 
  <tr> 
   <td>Maximum number of returned results</td> 
   <td> <p> Set the maximum number of files or folders Workfront Fusion will return during one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Create a Folder {#create-a-folder}

Creates a new folder.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your Google Team Drive account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td>Team Drive</td> 
   <td> <p> Select the shared drive where you want to create a folder.</p> </td> 
  </tr> 
  <tr> 
   <td>Folder </td> 
   <td> <p>Select the folder you want to create a folder in.</p> </td> 
  </tr> 
  <tr> 
   <td>The name of the new folder</td> 
   <td> <p> Enter the name of the new folder.</p> </td> 
  </tr> 
 </tbody> 
</table>

