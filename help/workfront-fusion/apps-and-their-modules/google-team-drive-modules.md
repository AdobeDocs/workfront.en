---
filename: google-team-drive-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations;agile-and-teams;user-management
keywords: connector
navigation-topic: apps-and-their-modules
title: Google Team Drive modules
description: The Google Team Drive modules enable you to monitor, upload, update, copy, delete, or retrieve files and create folders in your Google Shared Drive.
---

# Google Team Drive modules

The Google Team Drive modules enable you to monitor, upload, update, copy, delete, or retrieve files and create folders in your Google Shared Drive.

In order to use Google Team Drive with `Adobe Workfront Fusion`, it is necessary to have a G Suite account. If you do not have one, you can create a G Suite account at the [G Suite sign up site](https://gsuite.google.com/signup/businessstarter/welcome).

In a `Adobe Workfront Fusion` scenario, you can connect your `[Fusion app]` account to multiple third-party applications and services.

If you need instructions on creating a scenario, see [Create a scenario](../../workfront-fusion/scenarios/create-a-scenario.md).

For information about modules, see [Modules in Adobe Workfront Fusion](../../workfront-fusion/modules/modules.md).

## Access requirements

You must have the following access to use the functionality in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p><span>Pro</span> or higher</p> </td> 
  </tr> Adobe Workfront license* Plan, Work 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront Fusion</span> license**</td> 
   <td> <p><span>Workfront Fusion for Work Automation and Integration</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase <span>Adobe Workfront Fusion</span> as well as <span>Adobe Workfront</span> to use functionality described in this article.</td> 
  </tr> <!--
   Access level configurations* You must be a Workfront Fusion administrator for your organization. You must be a Workfront Fusion administrator for your team.
  --> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

&#42;&#42;For information on `Adobe Workfront Fusion` licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Prerequisites

To use Google Team Drive modules, you must have a Google Team Drive.

## Google Team Drive modules and their fields

>[!NOTE]
>
>The module dialog fields that are displayed in `bold` (in the `Workfront Fusion` scenario, `not` in this documentation article) are mandatory.

When you configure `Google Team Drive` modules, `Workfront Fusion` displays the fields listed below. Along with these, additional `Google Team Drive` fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Triggers

#### Watch Files

Returns file details when a new file is added and/or modified in the specified folder.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your <span>Google Team Drive</span> account to <span>Workfront Fusion</span>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
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
   <td> <p> Set the maximum number of files <span>Workfront Fusion</span> will return during one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions

* [Upload a File](#upload) 
* [Update a File](#update) 
* [Copy a File](#copy) 
* [Delete a File](#delete) 
* [Move a File to Trash](#move) 
* [Get a File](#get) 
* [Get a File List](#get2) 
* [Create a Folder](#create)

#### Upload a File

Uploads a file to the specified shared drive.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your <span>Google Team Drive</span> account to <span>Workfront Fusion</span>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
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

#### Update a File

Allows you to change the file name and/or file content.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your <span>Google Team Drive</span> account to <span>Workfront Fusion</span>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
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

#### Copy a File

Copies a specified file to the selected folder.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your <span>Google Team Drive</span> account to <span>Workfront Fusion</span>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
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

#### Delete a File

Deletes a specified file.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your <span>Google Team Drive</span> account to <span>Workfront Fusion</span>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td>File ID</td> 
   <td> <p> Enter or map the ID of the file you want to delete.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Move a File to Trash

Moves a specified file to the trash bin.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your <span>Google Team Drive</span> account to <span>Workfront Fusion</span>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td>File ID</td> 
   <td> <p> Enter or map the ID of the file you want to move to the trash bin.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Get a File

Retrieves details about the specified file.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your <span>Google Team Drive</span> account to <span>Workfront Fusion</span>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
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

#### Get a File List

Retrieves files and/or folders details based on the search term.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your <span>Google Team Drive</span> account to <span>Workfront Fusion</span>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
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
   <td> <p> Set the maximum number of files or folders <span>Workfront Fusion</span> will return during one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Create a Folder

Creates a new folder.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your <span>Google Team Drive</span> account to <span>Workfront Fusion</span>, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Workfront Fusion - Basic instructions</a></p> </td> 
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

