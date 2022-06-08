---
filename: google-drive-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Google Drive modules
description: The Adobe Workfront Fusion Google Drive modules enable you to monitor, search, create, update, delete, and manage your files, folder, or shared drives in your Google Drive.
---

# Google Drive modules

The Adobe Workfront Fusion Google Drive modules enable you to monitor, search, create, update, delete, and manage your files, folder, or shared drives in your Google Drive.

In a Adobe Workfront Fusion scenario, you can connect your Google Drive account to multiple third-party applications and services.

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

&nbsp;

## Connecting Google Drive to Workfront Fusion {#connecting-google-drive-to-workfront-fusion}

If you are @gmail.com or @googlemail.com user you need to create an OAuth client on the [Google Cloud Platform](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) in order to obtain Client ID and Client Secret.

For step-by-step instructions on how to create the OAuth client (and obtain Client ID and Client Secret), see [Connect Adobe Workfront Fusion to Google Services using a custom OAuth client](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

For instructions about connecting your Google Drive account to Workfront Fusion, see [Create a connection to Adobe Workfront Fusion - Basic instructions](../../workfront-fusion/connections/connect-to-fusion-general.md)

## Google Drive modules and their fields

When you configure Google Drive modules, Workfront Fusion displays the fields listed below. Along with these, additional Google Drive fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)



* [Triggers](#triggers) 
* [Actions](#actions)

### Triggers {#triggers}

* [Watch Files In Folder](#watch-files-in-folder) 
* [Watch All Files](#watch-all-files) 
* [Watch shared files](#watch-shared-files) 
* [Watch Comments](#watch-comments)

#### Watch Files In Folder

Retrieves file details when a file is added or modified in the specified folder.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td>Connection </td>
   <td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td> 
  </tr> 
  <tr>
    <td>Select the folder to be watched</td>
    <td >Select the folder on your drive that you want to watch the files in.</td>
  </tr> 
  <tr> 
    <td>What files to watch</td>
   <td> <p>Select which type of files you want to watch.</p> 
    <ul> 
     <li>All</li> 
     <li>Google Documents</li> 
     <li>Google Spreadsheets</li> 
     <li>Google Slides</li> 
     <li>Google Drawings</li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td >Convert Google Documents files to format</td>
    <td>Select the file format that you want to convert Google Documents to.</td>
  </tr> 
  <tr>
    <td>Convert Google Spreadsheets files to format</td>
    <td>Select the file format that you want to convert Google Spreadsheets to.</td>
  </tr> 
  <tr>
    <td>Convert Google Slides files to format</td>
    <td>Select the file format that you want to convert Google Documents to.</td>
  </tr> 
  <tr>
    <td>Convert Google Drawings files to format</td>
    <td>Select the file format that you want to convert Google Documents to.</td>
  </tr> 
  <tr>
    <td>Watch</td>
    <td>Select whether you want to watch new files and all changes, or only new files.</td>
  </tr> 
  <tr> 
    <td>Maximum number of downloaded files</td>
    <td>Set the maximum number of results that Workfront Fusion will download during one cycle (the number of repetitions per scenario run).</td>
  </tr> 
 </tbody> 
</table>

#### Watch All Files

Retrieves file details when a file in your Google Drive is added or modified.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td> 
  </tr> 
  <tr> 
   <td>What files to watch</td> 
   <td> <p>Select which type of files you want to watch.</p> 
    <ul> 
     <li>All</li> 
     <li>Google Documents</li> 
     <li>Google Spreadsheets</li> 
     <li>Google Slides</li> 
     <li>Google Drawings</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Convert Google Documents files to format</td> 
   <td>Select the file format that you want to convert Google Documents to.</td> 
  </tr> 
  <tr> 
   <td>Convert Google Spreadsheets files to format</td> 
   <td>Select the file format that you want to convert Google Spreadsheets to.</td> 
  </tr> 
  <tr> 
   <td>Convert Google Slides files to format</td> 
   <td>Select the file format that you want to convert Google Documents to.</td> 
  </tr> 
  <tr> 
   <td>Convert Google Drawings files to format</td> 
   <td>Select the file format that you want to convert Google Documents to.</td> 
  </tr> 
  <tr> 
   <td>Watch</td> 
   <td>Select whether you want to watch new files and all changes, or only new files.</td> 
  </tr> 
  <tr> 
   <td>Maximum number of downloaded files</td> 
   <td>Set the maximum number of results that Workfront Fusion will download during one cycle (the number of repetitions per scenario run).</td> 
  </tr> 
 </tbody> 
</table>

#### Watch shared files {#watch-shared-files}

Triggers when a new file is shared to you, or an existing shared file is updated.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td> 
  </tr> 
  <tr> 
   <td>Select the folder to be watched</td> 
   <td>Select the shared folder that you want to watch the files in.</td> 
  </tr> 
  <tr> 
   <td>What files to watch</td> 
   <td> <p>Select which type of files you want to watch.</p> 
    <ul> 
     <li>All</li> 
     <li>Google Documents</li> 
     <li>Google Spreadsheets</li> 
     <li>Google Slides</li> 
     <li>Google Drawings</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Convert Google Documents files to format</td> 
   <td>Select the file format that you want to convert Google Documents to.</td> 
  </tr> 
  <tr> 
   <td>Convert Google Spreadsheets files to format</td> 
   <td>Select the file format that you want to convert Google Spreadsheets to.</td> 
  </tr> 
  <tr> 
   <td>Convert Google Slides files to format</td> 
   <td>Select the file format that you want to convert Google Documents to.</td> 
  </tr> 
  <tr> 
   <td>Convert Google Drawings files to format</td> 
   <td>Select the file format that you want to convert Google Documents to.</td> 
  </tr> 
  <tr> 
   <td>Watch</td> 
   <td>Select whether you want to watch new files and all changes, or only new files.</td> 
  </tr> 
  <tr> 
   <td>Maximum number of downloaded files</td> 
   <td>Set the maximum number of results that Workfront Fusion will download during one cycle (the number of repetitions per scenario run).</td> 
  </tr> 
 </tbody> 
</table>

#### Watch Comments {#watch-comments}

Triggers when a comment is added or modified on the selected file.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td> 
  </tr> 
  <tr> 
   <td>File</td> 
   <td>Select the file that you want to watch for comments.</td> 
  </tr> 
  <tr> 
   <td>Watch</td> 
   <td>Select whether you want to watch for all changes or for new comments only</td> 
  </tr> 
  <tr> 
   <td>Maximum number of returned comments</td> 
   <td>Set the maximum number of comments that Workfront Fusion will return during one cycle (the number of repetitions per scenario run).</td> 
  </tr> 
 </tbody> 
</table>

### Actions {#actions}

* [Upload a File](#upload-a-file) 
* [Update a File](#update-a-file) 
* [Copy a File](#copy-a-file) 
* [Delete a File](#delete-a-file) 
* [Move a File/Folder to Trash](#move-a-file-folder-to-trash) 
* [Get a file](#get-a-file) 
* [Search for Files/Folders](#search-for-files-folders) 
* [Create a Folder](#create-a-folder) 
* [Get a share link](#get-a-share-link)

#### Upload a File {#upload-a-file}

Uploads a file to your Google Drive.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td> 
  </tr> 
  <tr> 
   <td>Destination</td> 
   <td> <p>Select the destination that you want to upload a file to.</p> 
    <ul> 
     <li>My Drive</li> 
     <li>Shared with Me</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Target folder</td> 
   <td>Select the folder that you want to upload a file to. </td> 
  </tr> 
  <tr> 
   <td>Source file</td> 
   <td>Select whether you want to use a file passed in from a previous module, or if you want to map the file manually.</td> 
  </tr> 
  <tr> 
   <td>File name</td> 
   <td>Select the file name. This option is available if you select "Map" in the source file field.</td> 
  </tr> 
  <tr> 
   <td>Data</td> 
   <td>Select the data file that you want to upload. This option is available if you select "Map" in the source file field.</td> 
  </tr> 
  <tr> 
   <td>Title</td> 
   <td>Enter a title for the new file.</td> 
  </tr> 
  <tr> 
   <td>Convert a file</td> 
   <td>Enabling this option allows the module to convert files to the corresponding Google format.</td> 
  </tr> 
 </tbody> 
</table>

#### Update a File {#update-a-file}

Updates a file's metadata or content.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td> 
  </tr> 
  <tr> 
   <td>Destination</td> 
   <td> <p>Select the destination that you want to upload a file to.</p> 
    <ul> 
     <li>My Drive</li> 
     <li>Shared with Me</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Move to a folder</td> 
   <td>If you want to move the file to a different folder, select the folder that you want to move the file into.</td> 
  </tr> 
  <tr> 
   <td>File ID</td> 
   <td>Map the ID&nbsp;of the file that you want to update.</td> 
  </tr> 
  <tr> 
   <td>Title</td> 
   <td>Enter a title for the updated file.</td> 
  </tr> 
  <tr> 
   <td>Change a file content</td> 
   <td>Select whether you want to replace the content of the file.</td> 
  </tr> 
  <tr> 
   <td>Source file</td> 
   <td>Select whether you want to use a file passed in from a previous module, or if you want to map the file manually. This field is available if you selected to change the file's content in the previous field.</td> 
  </tr> 
  <tr> 
   <td>File name</td> 
   <td>Select the file name. This option is available if you select "Map" in the source file field.</td> 
  </tr> 
  <tr> 
   <td>Data</td> 
   <td>Select the data file that you want to upload. This option is available if you select "Map" in the source file field.</td> 
  </tr> 
 </tbody> 
</table>

#### Copy a File {#copy-a-file}

Copies a file to the new location.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td> 
  </tr> 
  <tr> 
   <td>Destination</td> 
   <td> <p>Select the destination that you want to upload a file to.</p> 
    <ul> 
     <li>My Drive</li> 
     <li>Shared with Me</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Target folder</td> 
   <td>Select the folder where the file you want to copy is located/</td> 
  </tr> 
  <tr> 
   <td>File ID</td> 
   <td>Map the ID&nbsp;of the file that you want to update.</td> 
  </tr> 
  <tr> 
   <td>The name of the copy</td> 
   <td>Enter a title for the new file. Leave this field blank if you do not want to change the original file name.</td> 
  </tr> 
 </tbody> 
</table>

#### Delete a File {#delete-a-file}

Permanently deletes a file or folder.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td> 
  </tr> 
  <tr> 
   <td>File ID</td> 
   <td>Map the ID&nbsp;of the file that you want to delete.</td> 
  </tr> 
 </tbody> 
</table>

#### Move a File/Folder to Trash {#move-a-file-folder-to-trash}

Moves a file or folder to the trash.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td> 
  </tr> 
  <tr> 
   <td>File ID</td> 
   <td>Map the ID&nbsp;of the file that you want to move to the trash.</td> 
  </tr> 
 </tbody> 
</table>

#### Get a file {#get-a-file}

Retrieves the file with the ID specified.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td> 
  </tr> 
  <tr> 
   <td>Convert Google Documents files to format</td> 
   <td>Select the file format that you want to convert Google Documents to.</td> 
  </tr> 
  <tr> 
   <td>Convert Google Spreadsheets files to format</td> 
   <td>Select the file format that you want to convert Google Spreadsheets to.</td> 
  </tr> 
  <tr> 
   <td>Convert Google Slides files to format</td> 
   <td>Select the file format that you want to convert Google Documents to.</td> 
  </tr> 
  <tr> 
   <td>Convert Google Drawings files to format</td> 
   <td>Select the file format that you want to convert Google Documents to.</td> 
  </tr> 
  <tr> 
   <td>File ID</td> 
   <td>Map the ID&nbsp;of the file that you want to retrieve.</td> 
  </tr> 
 </tbody> 
</table>

#### Search for Files/Folders {#search-for-files-folders}

Searches for files or folders based on search criteria.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td> 
  </tr> 
  <tr> 
   <td>Destination</td> 
   <td> <p>Select the destination that you want to search.</p> 
    <ul> 
     <li>My Drive</li> 
     <li>Shared with Me</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>List a folder</td> 
   <td>Navigate to the folder you want to search for the files or folders.</td> 
  </tr> 
  <tr> 
   <td>Retrieve</td> 
   <td> <p> Select whether you want to search for files, folders, or both.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Search</p> </td> 
   <td> <p>Select the type of the search you want to perform.</p> 
    <ul> 
     <li> <p><strong>Search within file/folder names</strong> </p> 
      <ul> 
       <li> <p><strong>Query</strong> </p> <p>Enter a part of the file name or full file name (including the suffix) you want to search.</p> </li> 
       <li> <p><strong>Search Options</strong> </p> <p>Select whether you want to search for the exact term, or if you want to search for names containing the search term.</p> </li> 
      </ul> </li> 
     <li> <p><strong>Fulltext search</strong> </p> 
      <ul> 
       <li> <p><strong>Query</strong> </p> <p>Enter any search term you want search in your Google Drive.</p> </li> 
      </ul> </li> 
     <li> <p><strong>Enter custom search query</strong> </p> 
      <ul> 
       <li> <p><strong>Query</strong> </p> <p>Enter the custom search query. For more details, please refer to the Search for Files section of this article.</p> </li> 
       <li> <p><strong>Add the folder selected above to the query</strong> </p> <p>Searches for the folder n the parents collection. This finds all files and folders located directly in the folder selected above.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Maximum number of returned results</td> 
   <td>Set the maximum number of files or folders Workfront Fusion will return during one execution cycle.</td> 
  </tr> 
  <tr> 
   <td>Continue the execution of the route even if the module returns no results</td> 
   <td>Enable this option to ensure that the scenario is not stopped if the module returns no results.</td> 
  </tr> 
 </tbody> 
</table>

#### Create a Folder {#create-a-folder}

Creates a folder in the specified location.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td> 
  </tr> 
  <tr> 
   <td>Destination</td> 
   <td> <p>Select the destination that you want to upload a file to.</p> 
    <ul> 
     <li>My Drive</li> 
     <li>Shared with Me</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>New folder location</td> 
   <td>Navigate to the location where you want to create a new folder.</td> 
  </tr> 
  <tr> 
   <td>The name of the new folder</td> 
   <td>Enter a name for the folder that you are creating.</td> 
  </tr> 
  <tr> 
   <td>Share folder</td> 
   <td>Select this option if you want to share the folder with anyone with the Share link. Otherwise, the share link is for the owner only.</td> 
  </tr> 
 </tbody> 
</table>

#### Get a share link {#get-a-share-link}

Retrieves the share link for a file in Google Drive.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td> 
  </tr> 
  <tr> 
   <td>File ID</td> 
   <td>Map the ID&nbsp;of the file that you want to get the share link for.</td> 
  </tr> 
 </tbody> 
</table>

## Troubleshooting

### Unable to upload or update a file

There are several situations when uploading or updating a file fails:

* The uploaded file is too big and exceeds the maximum file size limit allowed for your Google Drive plan or you have exceeded your Google Drive storage limit. You can either upgrade your storage plan or delete existing files from the Google Drive service.
* The selected folder where the file was to be uploaded to no longer exists. The scenario stops and it is then necessary to select a target folder again.

## Search for files

In the module List files in a folder you can use your own query which consists of these parts:

* **Field** - Attribute of the file that is being searched, for example, the attribute `name` of the file.

* **Operator** - Test that is performed on the data to provide a match, for example, `contains`.

* **Value** - The content of the attribute that is tested, for example, the name of the file `My cool document`.

Combine clauses with the conjunctions `and` or `or`, and negate the query with `not`.

* [Fields](#fields) 
* [Value types](#value-types) 
* [Operators](#operators) 
* [Examples](#examples)

### Fields {#fields}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Field </th> 
   <th>Value Type </th> 
   <th>Operators</th> 
   <th> <p> Description</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>title</code></td> 
   <td>string</td> 
   <td><code>contains</code><sup>1</sup>, <code>=</code>, <code>!=</code></td> 
   <td> <p> Name of the file.</p> </td> 
  </tr> 
  <tr> 
   <td><code>fullText</code> </td> 
   <td>string </td> 
   <td><code>contains</code><sup>2, 3</sup> </td> 
   <td> <p> Full text of the file including name, description, content, and indexable text.</p> </td> 
  </tr> 
  <tr> 
   <td><code>mimeType</code> </td> 
   <td> string</td> 
   <td><code>contains</code>, <code>=</code>, <code>!=</code></td> 
   <td> <p> MIME type of the file.</p> </td> 
  </tr> 
  <tr> 
   <td><code>modifiedDate</code> </td> 
   <td> date<sup>4</sup></td> 
   <td><code> &lt;=</code>, <code>&lt;</code>, <code>=</code>, <code>!=</code>, <code>&gt;</code>, <code>&gt;=</code></td> 
   <td> <p> Date of the last modification to the file.</p> </td> 
  </tr> 
  <tr> 
   <td><code>lastViewedByMeDate</code> </td> 
   <td> date<sup>4</sup></td> 
   <td><code>&lt;=</code>, <code>&lt;</code>, <code>=</code>, <code>!=</code>, <code>&gt;</code>, <code>&gt;=</code></td> 
   <td> <p> Date that the user last viewed a file.</p> </td> 
  </tr> 
  <tr> 
   <td><code>trashed</code></td> 
   <td>boolean </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p> Whether the file is in the trash or not.</p> </td> 
  </tr> 
  <tr> 
   <td><code>starred</code></td> 
   <td>boolean </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p>Whether the file is starred or not.</p> </td> 
  </tr> 
  <tr> 
   <td><code>parents</code></td> 
   <td>collection </td> 
   <td><code>in </code> </td> 
   <td> <p>Whether the parents collection contains the specified ID.</p> </td> 
  </tr> 
  <tr> 
   <td><code>owners</code></td> 
   <td>collection </td> 
   <td><code>in </code> </td> 
   <td> <p>Users who own the file.</p> </td> 
  </tr> 
  <tr> 
   <td><code>writers</code></td> 
   <td>collection </td> 
   <td><code>in </code> </td> 
   <td> <p>Users who have permission to modify the file.</p> </td> 
  </tr> 
  <tr> 
   <td><code>readers </code> </td> 
   <td>collection </td> 
   <td><code>in </code> </td> 
   <td> <p>Users who have permission to read the file.</p> </td> 
  </tr> 
  <tr> 
   <td><code>sharedWithMe</code> </td> 
   <td>boolean </td> 
   <td><code>=</code>, <code>!=</code></td> 
   <td> <p> Files that are in the user's "Shared with me" collection.</p> </td> 
  </tr> 
  <tr> 
   <td><code>properties </code> </td> 
   <td>collection</td> 
   <td><code>has </code> </td> 
   <td> <p> Public custom file properties.</p> </td> 
  </tr> 
 </tbody> 
</table>

Consider the following about operators in these fields:

* The `contains` operator only performs prefix matching for a `title`.

  For example, the title "HelloWorld" matches for `title contains 'Hello'` but not for `title contains 'World'`.

* The `contains` operator only performs matching on entire string tokens for `fullText`.

  For example, if the full text of a doc contains the string "HelloWorld" only the query `fullText contains 'HelloWorld'` returns a result. Queries such as `fullText contains 'Hello'` would not return results in this scenario.

* The `contains` operator matches on an exact alphanumeric phrase if it is surrounded by double quotes.

  For example, if the `fullText` of a doc contains the string "Hello there world", then the query `fullText contains '"Hello there"'` returns a result, but the query `fullText contains '"Hello world"'` does not.

  Furthermore, because the search is alphanumeric, if the `fullText` of a doc contains the string "Hello_world", then the query `fullText contains '"Hello world"'` returns a result.

* Fields of `type` date are currently not comparable to each other, only to constant dates.

### Value types {#value-types}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Value Type</th> 
   <th> <p> Notes</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>String </td> 
   <td> <p>Surround with single quotes '. Escape single quotes in queries with <code>\'</code>, e.g.,<code> 'Valentine\'s Day'</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Boolean </td> 
   <td> <p><code>true </code>or <code>false</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Date </td> 
   <td> <p>RFC 3339 format, default timezone is UTC, e.g., <code>2012-06-04T12:00:00-08:00</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Operators {#operators}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Operator </th> 
   <th> <p>Notes</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td><code>contains</code></td> 
   <td> <p>The content of one string is present in the other.</p> </td> 
  </tr> 
  <tr> 
   <td><code>=</code> </td> 
   <td> <p> The content of a string or boolean is equal to the other.</p> </td> 
  </tr> 
  <tr> 
   <td><code>!=</code> </td> 
   <td> <p> The content of a string or boolean is not equal to the other.</p> </td> 
  </tr> 
  <tr> 
   <td><code>&lt;</code> </td> 
   <td> <p> A date is earlier than another.</p> </td> 
  </tr> 
  <tr> 
   <td><code>&lt;=</code> </td> 
   <td> <p> A date is earlier than or equal to another.</p> </td> 
  </tr> 
  <tr> 
   <td><code>&gt;</code> </td> 
   <td> <p> A date is later than another.</p> </td> 
  </tr> 
  <tr> 
   <td><code>&gt;=</code> </td> 
   <td> <p> A date is later than or equal to another.</p> </td> 
  </tr> 
  <tr> 
   <td><code>in </code> </td> 
   <td> <p>An element is contained within a collection.</p> </td> 
  </tr> 
  <tr> 
   <td><code>and </code> </td> 
   <td> <p>Return files that match both clauses.</p> </td> 
  </tr> 
  <tr> 
   <td><code>or </code> </td> 
   <td> <p>Return files that match either clause.</p> </td> 
  </tr> 
  <tr> 
   <td><code>not </code> </td> 
   <td> <p>Negates a search clause.</p> </td> 
  </tr> 
  <tr> 
   <td><code>has </code> </td> 
   <td> <p>A collection contains an element matching the parameters.</p> </td> 
  </tr> 
 </tbody> 
</table>

For compound clauses, you can use parentheses to group clauses together. For example:
`modifiedDate > '2012-06-04T12:00:00' and (mimeType contains 'image/' or mimeType contains 'video/')` This search returns all files with an image or video MIME type that their last modification was after June 4, 2012. Because `and` and `or` operators are evaluated from left to right, without parentheses, the above example would return only images modified after June 4, 2012, but would return all videos, even those before June 4, 2012.

### Examples {#examples}

All examples on this page show the unencoded `<q>q</q>` parameter, where `title = 'hello'` is encoded as `title+%3d+%27hello%27`. Client libraries handle this encoding automatically.

* Search for files with the name "hello"
  <pre>title = 'hello'</pre>
* Search for folders using the folder-specific MIME type
  <pre>mimeType = 'application/vnd.google-apps.folder'</pre>
* Search for files that are not folders
  <pre>mimeType != 'application/vnd.google-apps.folder'</pre>
* Search for files with a name containing the words "hello" and "goodbye"
  <pre>title contains 'hello' and name contains 'goodbye'</pre>
* Search for files with a name that does not contain the word "hello"
  <pre>not title contains 'hello'</pre>
* Search for files containing the word "hello" in the content
  <pre>fullText contains 'hello'</pre>
* Search for files not containing the word "hello" in the content
  <pre>not fullText contains 'hello'</pre>
* Search for files containing the exact phrase "hello world" in the content
  <pre>fullText contains '"hello world"'fullText contains '"hello_world"'</pre>
* Search for files with a query containing the "\" character (e.g., "\authors")
  <pre>fullText contains '\\authors'</pre>
* Search for files writeable by the user "test@example.org"
  <pre>'test@example.org' in writers</pre>
* Search for the ID `1234567` in the `parents` collection. This finds all files and folders located directly in the folder whose ID is `1234567`.
  <pre>'1234567' in parents</pre>
* Search for the alias ID `appDataFolder` in the `parents` collection. This finds all files and folders located directly under the [Application Data folder](https://developers.google.com/drive/api/v2/appdata).
  <pre>'appDataFolder' in parents</pre>
* Search for files writeable by the users "test@example.org" and "test2@example.org"
  <pre>'test@example.org' in writers and 'test2@example.org' in writers</pre>
* Search for files containing the text "important" which are in the trash
  <pre>fullText contains 'important' and trashed = true</pre>
* Search for files modified after June 4th 2012
  <pre>modifiedDate > '2012-06-04T12:00:00' // default time zone is UTC</pre><pre>modifiedDate > '2012-06-04T12:00:00-08:00'</pre>
* Search for files shared with the authorized user with "hello" in the name
  <pre>sharedWithMe and title contains 'hello'</pre>
* Search for files with a [custom file property](https://developers.google.com/drive/api/v2/properties) named `additionalID` with the value `8e8aceg2af2ge72e78`.
  <pre>properties has { key='additionalID' and value='8e8aceg2af2ge72e78' and visibility='PRIVATE' }</pre>
  
Source of this guide is [Google Drive documentation](https://developers.google.com/drive/api/v2/search-shareddrives).
