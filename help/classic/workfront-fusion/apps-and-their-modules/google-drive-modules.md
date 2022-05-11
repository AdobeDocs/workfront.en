---
filename: google-drive-modules
content-type: reference
product: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Google Drive modules
description: The Adobe Workfront Fusion Google Drive modules enable you to monitor, search, create, update, delete, and manage your files, folder, or shared drives in your Google Drive.
---

# Google Drive modules

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

The Adobe Workfront Fusion Google Drive modules enable you to monitor, search, create, update, delete, and manage your files, folder, or shared drives in your Google Drive.

In a Adobe Workfront Fusion scenario, you can connect your Google Drive account to multiple third-party applications and services.

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

&nbsp;

## Connecting Google Drive to Workfront Fusion {#connecting-google-drive-to-workfront-fusion}

If you are @gmail.com or @googlemail.com user you need to create an OAuth client on the [Google Cloud Platform](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) in order to obtain Client ID and Client Secret.

For step-by-step instructions on how to create the OAuth client (and obtain Client ID and Client Secret), see [Connect Adobe Workfront Fusion to Google Services using a custom OAuth client](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

For instructions about connecting your Google Drive account to Workfront Fusion, see [Create a connection to Adobe Workfront Fusion - Basic instructions](../../workfront-fusion/connections/connect-to-fusion-general.md)

## Google Drive modules and their fields

When you configure Google Drive modules, Workfront Fusion displays the fields listed below. Along with these, additional Google Drive fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<ul>
<li> <p><a href="#files-folders" class="MCXref xref">Files/Folders</a> </p> </li>
<li> <p><a href="#google-shared-drive" class="MCXref xref">Google Shared Drive</a> </p> </li>
<li> <p><a href="#other" class="MCXref xref">Other</a> </p> </li>
</ul>
<p><strong>Files/Folders</strong></p>
<ul>
<li> <p><a href="#watch-files-in-folder" class="MCXref xref">Watch Files In Folder</a> </p> </li>
<li> <p><a href="#watch-all-files" class="MCXref xref">Watch All Files</a> </p> </li>
<li> <p><a href="#watch-folders" class="MCXref xref">Watch Folders</a> </p> </li>
<li> <p><a href="#search-for-files-folders" class="MCXref xref">Search for Files/Folders</a> </p> </li>
<li> <p><a href="#download-a-file" class="MCXref xref">Download a file</a> </p> </li>
<li> <p><a href="#create-a-file-from-text" class="MCXref xref">Create a File from Text</a> </p> </li>
<li> <p><a href="#create-a-folder" class="MCXref xref">Create a Folder</a> </p> </li>
<li> <p><a href="#upload-a-file" class="MCXref xref">Upload a File</a> </p> </li>
<li> <p><a href="#update-a-file" class="MCXref xref">Update a File</a> </p> </li>
<li> <p><a href="#move-a-file-folder-to-trash" class="MCXref xref">Move a File/Folder to Trash</a> </p> </li>
<li> <p><a href="#delete-a-file-folder" class="MCXref xref">Delete a File/Folder</a> </p> </li>
<li> <p><a href="#copy-a-file" class="MCXref xref">Copy a File</a> </p> </li>
<li> <p><a href="#move-a-file-folder" class="MCXref xref">Move a File/Folder</a> </p> </li>
<li> <p><a href="#get-a-share-link" class="MCXref xref">Get a share link</a> </p> </li>
</ul>
<h4 id="watch-files-in-folder"><a name="Watch"></a>Watch Files In Folder</h4>
<p>This trigger module retrieves file details when a file is added or modified in the specified folder.</p>
<table cellspacing="15">
<col>
<col>
<tbody>
<tr>
<td>Connection </td>
<td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td>
</tr>
<tr>
<td>Watch Files</td>
<td> <p>Select which files you want to watch.</p>
<ul>
<li> <p><strong>By Created Time</strong> </p> <p>The module watches for new files<br></p> </li>
<li> <p><strong>By Modified Time</strong> </p> <p>The module watches for modified files.</p> </li>
</ul> </td>
</tr>
<tr>
<td>Choose a Drive</td>
<td> <p>Select what type of drive you want to monitor.</p>
<ul>
<li>My Drive</li>
<li>Shared With Me</li>
<li>Google Shared Drive (available for G Suite users only)</li>
</ul> <p>If you have selected the Google Shared Drive option in this field and you are not a G Suite user, the error <code>[400] Invalid Value</code> is returned.</p> </td>
</tr>
<tr>
<td>Select the Folder to be Watched</td>
<td>Select the folder on your drive that you want to watch for files.</td>
</tr>
<tr data-mc-conditions="">
<td>File Types to Watch</td>
<td> <p>Select the type of file that you want to watch.</p>
<ul>
<li> <p>Google Docs</p> </li>
<li> <p>Google Spreadsheets</p> </li>
<li> <p>Google Slides</p> </li>
<li> <p>Google Drawings</p> </li>
</ul> </td>
</tr>
<tr data-mc-conditions="">
<td>Limit</td>
<td>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</td>
</tr>
</tbody>
</table>
<h4 id="watch-all-files"><a name="Watch2"></a>Watch All Files</h4>
<p>This trigger module retrieves file details when a file in your Google Drive is added or modified.</p>
<table cellspacing="15">
<col>
<col>
<tbody>
<tr>
<td>Connection </td>
<td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td>
</tr>
<tr>
<td>Watch Files</td>
<td> <p>Select which files you want to watch.</p>
<ul>
<li> <p>By Created Time</p> <p>The module watches for new files<br></p> </li>
<li> <p>By Modified Time</p> <p>The module watches for modified files.</p> </li>
</ul> </td>
</tr>
<tr>
<td>Choose a Drive</td>
<td> <p>Select what type of drive you want to monitor.</p>
<ul>
<li>My Drive</li>
<li>Shared With Me</li>
<li>Google Shared Drive (available for G Suite users only)</li>
</ul> <p>If you have selected the Google Shared Drive option in this field and you are not a G Suite user, the error <code>[400] Invalid Value</code> is returned.</p> </td>
</tr>
<tr>
<td>File Types to Watch</td>
<td> <p>Select the type of file that you want to watch.</p>
<ul>
<li> <p>Google Docs</p> </li>
<li> <p>Google Spreadsheets</p> </li>
<li> <p>Google Slides</p> </li>
<li> <p>Google Drawings</p> </li>
</ul> </td>
</tr>
<tr>
<td>Limit</td>
<td>Set the maximum number of results that Workfront Fusion will download during one cycle (the number of repetitions per scenario run).</td>
</tr>
</tbody>
</table>
<h4 id="watch-folders"><a name="Watch5"></a>Watch Folders</h4>
<p>This trigger module starts a scenario when a folder is created or modified.</p>
<table cellspacing="15">
<col>
<col>
<tbody>
<tr>
<td>Connection </td>
<td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td>
</tr>
<tr>
<td>Watch Files</td>
<td> <p>Select which files you want to watch.</p>
<ul>
<li> <p><strong>By Created Time</strong> </p> <p>The module watches for new files<br></p> </li>
<li> <p><strong>By Modified Time</strong> </p> <p>The module watches for modified files.</p> </li>
</ul> </td>
</tr>
<tr>
<td>Choose a Drive</td>
<td> <p>Select what type of drive you want to monitor.</p>
<ul>
<li>My Drive</li>
<li>Shared With Me</li>
<li>Google Shared Drive (available for G Suite users only)</li>
</ul> <p>If you have selected the Google Shared Drive option in this field and you are not a G Suite user, the error <code>[400] Invalid Value</code> is returned.</p> </td>
</tr>
<tr>
<td>Choose a folder</td>
<td> <p>Select the folder that you want to watch for new or modified subfolders.</p> </td>
</tr>
<tr>
<td>Limit</td>
<td>Set the maximum number of results that Workfront Fusion will download during one cycle (the number of repetitions per scenario run).</td>
</tr>
</tbody>
</table>
<h4 id="search-for-files-folders"><a name="Search3"></a>Search for Files/Folders</h4>
<p>This search module searches for files or folders based on search criteria.</p>
<table cellspacing="15">
<col>
<col>
<tbody>
<tr>
<td>Connection </td>
<td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td>
</tr>
<tr>
<td>Select the Method</td>
<td> <p>Choose how you want to determine which folder the module searches.</p>
<ul>
<li> <p><strong>Enter manually</strong> </p> <p>Enter or map the IDs of the folder and shared drive that you want to search</p> </li>
<li> <p><strong>Select from a list</strong> </p> <p>Choose the drive that contains the folder you want to search, then choose the folder.</p> </li>
</ul> </td>
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
<td>Limit</td>
<td>Set the maximum number of files or folders Workfront Fusion will return during one execution cycle.</td>
</tr>
</tbody>
</table>
<h4 id="download-a-file"><a name="Download"></a>Download a file</h4>
<p>This action module downloads a file from your Google Drive.</p>
<table cellspacing="15">
<col>
<col>
<tbody>
<tr>
<td>Connection </td>
<td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td>
</tr>
<tr>
<td>Enter a File ID</td>
<td> <p>Choose how the module will select the file you want to download.</p>
<ul>
<li> <p><strong>Enter manually</strong> </p> <p>Enter or map the ID of the file you want to download</p> </li>
<li> <p><strong>Select from the list</strong> </p> <p>Choose the drive that contains the folder where the file is located, then choose the folder.</p> </li>
</ul> </td>
</tr>
<tr>
<td>Convert Google Documents Files to Format</td>
<td>Select the file format that you want to convert Google Documents to.</td>
</tr>
<tr>
<td>Convert Google Spreadsheets Files to Format</td>
<td>Select the file format that you want to convert Google Spreadsheets to.</td>
</tr>
<tr>
<td>Convert Google Slides Files to Format</td>
<td>Select the file format that you want to convert Google Documents to.</td>
</tr>
<tr>
<td>Convert Google Drawings Files to Format</td>
<td>Select the file format that you want to convert Google Documents to.</td>
</tr>
</tbody>
</table>
<h4 id="create-a-file-from-text"><a name="Create2"></a>Create a File from Text</h4>
<p>This action module creates a file from plain text.</p>
<table cellspacing="15">
<col>
<col>
<tbody>
<tr>
<td>Connection </td>
<td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td>
</tr>
<tr>
<td>Choose a Drive</td>
<td> <p>Select the type of drive where you want to create the file.</p>
<ul>
<li>My Drive</li>
<li>Shared With Me</li>
<li>Google Shared Drive (available for G Suite users only)</li>
</ul> <p>If you have selected the Google Shared Drive option in this field and you are not a G Suite user, the error <code>[400] Invalid Value</code> is returned.</p> </td>
</tr>
<tr>
<td>New Text File Location</td>
<td> <p> Select the folder where you want to create the file.</p> </td>
</tr>
<tr>
<td>File Name</td>
<td> <p>Enter or map a name for the new file.</p> </td>
</tr>
<tr>
<td>File Content</td>
<td>Enter or map the content (body) of the file.</td>
</tr>
<tr>
<td>Convert the File to Google Docs Document</td>
<td>Enable this option to set the file's <strong>mimeType</strong> to <strong>application/vnd.google-apps.document</strong> instead of <strong>text/plain</strong>.</td>
</tr>
</tbody>
</table>
<h4 id="create-a-folder"><a name="Create3"></a>Create a Folder</h4>
<p>This action module creates a folder in the specified location.</p>
<table cellspacing="15">
<col>
<col>
<tbody>
<tr>
<td>Connection </td>
<td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td>
</tr>
<tr>
<td>New Drive Location</td>
<td> <p>Select the type of drive where you want to create the folder.</p>
<ul>
<li>My Drive</li>
<li>Shared With Me</li>
<li>Google Shared Drive (available for G Suite users only)</li>
</ul> <p>If you have selected the Google Shared Drive option in this field and you are not a G Suite user, the error<code> [400] Invalid Value</code> is returned.</p> </td>
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
<td> <p>Select this option if you want to share the folder with anyone with the Share link. Otherwise, the share link is for the owner only.</p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>If you have chosen to share the folder, select the role to assign to the access rule. </p>
<ul>
<li><strong>Free Busy Reader</strong>: The user can read free/busy information. </li>
<li><strong>Owner</strong>: The user can read and modify events and can access control lists. </li>
<li><strong>Reader</strong>: The user can read events that are not private. </li>
<li><strong>Writer</strong>: The user can read and modify events.</li>
</ul> </td>
</tr>
<tr>
<td>Type</td>
<td> <p>If you have chosen to share the folder, select the type of scope. </p>
<ul>
<li><strong>Default</strong>: The public scope. This is the default value. </li>
<li><strong>User</strong>: Limits the scope to a single user. Enter or map the user's email address.</li>
<li><strong>Group</strong>: Limits the scope to a group. Enter or map the group's email address.</li>
<li><strong>Domain</strong>: Limits the scope to a domain. Enter or map the domain.</li>
</ul> <note type="note">
The permissions granted to the Default, or the public, scope apply to any user, authenticated or not.
</note> </td>
</tr>
</tbody>
</table>
<h4 id="upload-a-file"><a name="Upload2"></a>Upload a File</h4>
<p>This action module uploads a file to your Google Drive.</p>
<table cellspacing="15">
<col>
<col>
<tbody>
<tr>
<td>Connection </td>
<td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td>
</tr>
<tr>
<td>Enter a Folder ID</td>
<td> <p>Choose how the module will select were to put the file you want to upload.</p>
<ul>
<li> <p><strong>Enter manually</strong> </p> <p>Enter or map the ID of the file you want to download</p> </li>
<li> <p><strong>Select from the list</strong> </p> <p>Choose the drive that contains the folder where you want the file to be located, then choose the folder.</p> <p>If you have selected the Google Shared Drive option and you are not a G Suite user, the error <code>[400] Invalid Value </code>is returned.</p> </li>
</ul> </td>
</tr>
<tr>
<td>New File Name</td>
<td>Enter a title for the new file.</td>
</tr>
<tr>
<td>Source file</td>
<td>Select a source file from a previous module, or map the source file's name and data.</td>
</tr>
<tr>
<td>Convert a file</td>
<td>Enable this option to allow the module to convert files to the corresponding Google format, then select the format you want to convert the file to.</td>
</tr>
</tbody>
</table>
<h4 id="update-a-file"><a name="Update2"></a>Update a File</h4>
<p>This action module updates a file's metadata or content.</p>
<table cellspacing="15">
<col>
<col>
<tbody>
<tr>
<td>Connection </td>
<td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td>
</tr>
<tr>
<td>Enter a File ID</td>
<td> <p>Choose how the module will select the file you want to update.</p>
<ul>
<li> <p><strong>Enter manually</strong> </p> <p>Enter or map the ID of the file you want to download</p> </li>
<li> <p><strong>Select from the list</strong> </p> <p>Choose the drive that contains the folder where the file is located, then choose the folder.</p> <p>If you have selected the Google Shared Drive option and you are not a G Suite user, the error<code> [400] Invalid Value</code> is returned.</p> </li>
</ul> </td>
</tr>
<tr>
<td>New Updated File Name</td>
<td>Enter or map a name for the updated file. This overwrites the current file name.</td>
</tr>
<tr>
<td>File Description</td>
<td>Enter or map a description for the new file.</td>
</tr>
<tr>
<td>Change a file content</td>
<td>Enable this option. to replace the content of the file.</td>
</tr>
<tr>
<td>Source file</td>
<td>Select a source file from a previous module, or map the source file's name and data.</td>
</tr>
</tbody>
</table>
<h4 id="move-a-file-folder-to-trash"><a name="Move2"></a>Move a File/Folder to Trash</h4>
<p>This action module moves a file or folder to the trash.</p>
<table cellspacing="15">
<col>
<col>
<tbody>
<tr>
<td>Connection </td>
<td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td>
</tr>
<tr>
<td>Enter a File/Folder ID</td>
<td> <p>Choose how the module will select the file or folder you want to move to the trash.</p>
<ul>
<li> <p><strong>Enter manually</strong> </p> <p>Select whether you want to move a file or a folder, then enter or map the ID of the file you want to move to the trash.</p> </li>
<li> <p><strong>Select from the list</strong> </p> <p>Choose the drive that contains the folder where the file is located, then choose the folder.</p> <p>If you have selected the Google Shared Drive option and you are not a G Suite user, the error <code>[400] Invalid Value</code> is returned.</p> </li>
</ul> </td>
</tr>
</tbody>
</table>
<h4 id="delete-a-file-folder"><a name="Delete2"></a>Delete a File/Folder</h4>
<p>This action module permanently deletes a file or folder.</p>
<table cellspacing="15">
<col>
<col>
<tbody>
<tr>
<td>Connection </td>
<td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td>
</tr>
<tr>
<td>Enter a File/Folder ID</td>
<td> <p>Choose how the module will select the file or folder you want to delete.</p>
<ul>
<li> <p><strong>Enter manually</strong> </p> <p>Select whether you want to delete a file or a folder, then enter or map the ID of the file you want to delete.</p> </li>
<li> <p><strong>Select from the list</strong> </p> <p>Choose the drive and folder that contain the file you want to delete, then choose the file.</p> <p>If you have selected the Google Shared Drive option and you are not a G Suite user, the error <code>[400] Invalid Value</code> is returned.</p> </li>
</ul> </td>
</tr>
</tbody>
</table>
<h4 id="copy-a-file"><a name="Copy2"></a>Copy a File</h4>
<p>This action module copies a file to the new location on Google Drive.</p>
<table cellspacing="15">
<col>
<col>
<tbody>
<tr>
<td>Connection </td>
<td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td>
</tr>
<tr>
<td>Enter a File/Folder ID</td>
<td> <p>Choose how the module will select the file or folder you want to copy.</p>
<ul>
<li> <p><strong>Enter manually</strong> </p> <p>Enter or map the ID of the original file you want to copy, then enter or map the location of the new file.</p> </li>
<li> <p><strong>Select from the list</strong> </p> <p>Choose the drive where the orgiginal file is located, then select the original file. </p> <p>Choose the drive that you want to copy the file to, then choose a new folder location for the copied file.</p> <p>If you have selected the Google Shared Drive option and you are not a G Suite user, the error<code> [400] Invalid Value</code> is returned.</p> </li>
</ul> </td>
</tr>
<tr>
<td>Copied File Name</td>
<td>Enter a title for the new file. Leave this field blank if you do not want to change the original file name.</td>
</tr>
</tbody>
</table>
<h4 id="move-a-file-folder"><a name="Move3"></a>Move a File/Folder</h4>
<p>This action module moves a file or folder to a different location on Google Drive.</p>
<table cellspacing="15">
<col>
<col>
<tbody>
<tr>
<td>Connection </td>
<td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td>
</tr>
<tr>
<td>Choose a Drive</td>
<td> <p>Select the type of drive that contains the file or folder you want to move.</p>
<ul>
<li>My Drive</li>
<li>Shared With Me</li>
<li>Google Shared Drive (available for G Suite users only)</li>
</ul> <p>If you have selected the Google Shared Drive option in this field and you are not a G Suite user, the error <code>[400] Invalid Value</code> is returned.</p> </td>
</tr>
<tr>
<td>Select File/Folder</td>
<td>Select whether you want to move a file or a folder.</td>
</tr>
<tr>
<td>New Drive Location</td>
<td> <p>Select the type of drive that you want to move the file or folder to.</p>
<ul>
<li>My Drive</li>
<li>Shared With Me</li>
<li>Google Shared Drive (available for G Suite users only)</li>
</ul> <p>If you have selected the Google Shared Drive option in this field and you are not a G Suite user, the error <code>[400] Invalid Value</code> is returned.</p> </td>
</tr>
<tr>
<td>New Folder Location</td>
<td>Select the folder that you want to move the file or folder to.</td>
</tr>
</tbody>
</table>
<h4 id="get-a-share-link"><a name="Get3"></a>Get a share link</h4>
<p>This action module retrieves the share link for a file in Google Drive.</p>
<table cellspacing="15">
<col>
<col>
<tbody>
<tr>
<td>Connection </td>
<td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td>
</tr>
<tr>
<td>Choose a Drive</td>
<td> <p>Select the type of drive that contains the file or folder you want to move.</p>
<ul>
<li>My Drive</li>
<li>Shared With Me</li>
<li>Google Shared Drive (available for G Suite users only)</li>
</ul> <p>If you have selected the Google Shared Drive option in this field and you are not a G Suite user, the error <code>[400] Invalid Value</code> is returned.</p> </td>
</tr>
<tr>
<td>Select</td>
<td>Select whether you want to share a link to a file or a folder</td>
</tr>
<tr>
<td>File ID / Folder ID</td>
<td>Enter or map the ID&nbsp;of the file or folder that you want to share.</td>
</tr>
<tr>
<td>Role</td>
<td> <p>Select the role to define what users can do with a file or folder.</p>
<ul>
<li><strong>Free Busy Reader</strong>: The user can read free/busy information. </li>
<li><strong>Owner</strong>: The user can read and modify events and can access control lists. </li>
<li><strong>Reader</strong>: The user can read events that are not private. </li>
<li><strong>Writer</strong>: The user can read and modify events.</li>
</ul> </td>
</tr>
<tr>
<td>Type</td>
<td> <p>If you have chosen to share the folder, select the type of scope. </p>
<ul>
<li><strong>Default</strong>: The public scope. This is the default value. </li>
<li><strong>User</strong>: Limits the scope to a single user. Enter or map the user's email address.</li>
<li><strong>Group</strong>: Limits the scope to a group. Enter or map the group's email address.</li>
<li><strong>Domain</strong>: Limits the scope to a domain. Enter or map the domain.</li>
</ul> <note type="note">
The permissions granted to the Default, or the public, scope apply to any user, authenticated or not.
</note> </td>
</tr>
<tr>
<td>Email address / Organization Domain</td>
<td>Enter the email address or organization domain you want to restrict the access to the file or folder to.</td>
</tr>
<tr>
<td>Send notification email</td>
<td>If you have selected User or Group in the Type field, enable this option to send a notification email with the share link. Enter the text of the email in the <strong>Email Message</strong> field.</td>
</tr>
<tr>
<td>Expiration Time</td>
<td> <p>If you have selected User or Group in the Type field, set a time that the share link will expire. </p> <p>For a list of supported date and time formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">Type coercion in Adobe Workfront Fusion</a>.</p> </td>
</tr>
<tr>
<td>Allow File Discovery</td>
<td>If you have selected Domain or Anyone in the Type field, enable this option to allow the file to be discovered through search.</td>
</tr>
</tbody>
</table>
<p><strong>Google Shared Drive</strong></p> <note type="note">
Google Shared Drive modules are for G Suite users only.
</note>
<ul>
<li> <p><a href="#watch-shared-drives" class="MCXref xref">Watch shared drives</a> </p> </li>
<li> <p><a href="#search-for-shared-drives" class="MCXref xref">Search for Shared Drives</a> </p> </li>
<li> <p><a href="#create-a-shared-drive" class="MCXref xref">Create a Shared Drive</a> </p> </li>
<li> <p><a href="#get-a-shared-drive" class="MCXref xref">Get a Shared Drive</a> </p> </li>
<li> <p><a href="#update-a-shared-drive" class="MCXref xref">Update a shared Drive</a> </p> </li>
<li> <p><a href="#delete-a-shared-drive" class="MCXref xref">Delete a Shared Drive</a> </p> </li>
</ul>
<h4 id="watch-shared-drives"><a name="Watch6"></a>Watch shared drives</h4>
<p>This trigger module starts a scenario when a shared drive is created.</p> <note type="important">
The G Suite administrator privilege is required in order to use this module.
</note>
<table cellspacing="15">
<col>
<col>
<tbody>
<tr>
<td>Connection </td>
<td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td>
</tr>
<tr>
<td>Search</td>
<td> <p>Select whether you want to filter returned drives by custom search query or query filter.</p> </td>
</tr>
<tr>
<td>Query filter</td>
<td>Set the filter to filter returned shared drives by name, organizer count, or member count. You can also use AND and OR operators to combine the filter.</td>
</tr>
<tr>
<td>Query</td>
<td> <p>Enter your custom search query.</p> <p>For example:<code>name contains 'Workfront Fusion' and memberCount >= 20</code></p> <p>For more info, see <a href="https://developers.google.com/drive/api/v3/search-shareddrives">Search for shared drives</a> in the Google Drive documentation.</p> </td>
</tr>
<tr>
<td>Limit</td>
<td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td>
</tr>
</tbody>
</table>
<h4 id="search-for-shared-drives"><a name="Search4"></a>Search for Shared Drives</h4>
<p>This search module searches for the Google shared drive</p> <note type="important">
The G Suite administrator privilege is required in order to use this module.
</note>
<table cellspacing="15">
<col>
<col>
<tbody>
<tr>
<td>Connection </td>
<td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td>
</tr>
<tr>
<td>Search</td>
<td> <p>Select whether you want to filter returned drives by custom search query or query filter.</p> </td>
</tr>
<tr>
<td>Query filter</td>
<td>Set the filter to filter returned shared drives by name, organizer count, or member count. You can also use AND and OR operators to combine the filter.</td>
</tr>
<tr>
<td>Query</td>
<td> <p>Enter your custom search query.</p> <p>For example:<code>name contains 'Workfront Fusion' and memberCount >= 20</code></p> <p>For more info, see <a href="https://developers.google.com/drive/api/v3/search-shareddrives">Search for shared drives</a> in the Google Drive documentation.</p> </td>
</tr>
<tr>
<td>Limit</td>
<td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td>
</tr>
</tbody>
</table>
<h4 id="create-a-shared-drive"><a name="Create4"></a>Create a Shared Drive</h4>
<p>This action module creates a new shared drive</p> <note type="important">
The G Suite administrator privilege is required in order to use this module.
</note>
<table cellspacing="15">
<col>
<col>
<tbody>
<tr>
<td>Connection </td>
<td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td>
</tr>
<tr>
<td>New Shared Drive's Name</td>
<td> <p>Enter or map a name for the new shared drive.</p> </td>
</tr>
</tbody>
</table>
<h4 id="get-a-shared-drive"><a name="Get4"></a>Get a Shared Drive</h4>
<p>This action module retrieves shared drive details</p> <note type="important">
The G Suite administrator privilege is required in order to use this module.
</note>
<table cellspacing="15">
<col>
<col>
<tbody>
<tr>
<td>Connection </td>
<td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td>
</tr>
<tr>
<td>Shared Drive ID</td>
<td> <p>Enter or map the ID of the shared drive you want to retrieve details about.</p> </td>
</tr>
</tbody>
</table>
<h4 id="update-a-shared-drive"><a name="Update3"></a>Update a shared Drive</h4>
<p>This action module updates an existing drive's name or restrictions.</p> <note type="important">
The G Suite administrator privilege is required in order to use this module.
</note>
<table cellspacing="15">
<col>
<col>
<tbody>
<tr>
<td>Connection </td>
<td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td>
</tr>
<tr>
<td>Shared Drive ID</td>
<td> <p>Enter or map the ID of the shared drive you want to retrieve details about.</p> </td>
</tr>
<tr>
<td>Name</td>
<td> <p>Enter or map a new name for the shared drive.</p> </td>
</tr>
<tr>
<td>Restrictions</td>
<td>
<ul>
<li> <p><strong>Admin Managed Restrictions</strong> </p> <p>Select whether administrative privileges on this shared drive are required to modify restrictions.</p> </li>
<li> <p><strong>Copy Requires Writer Permission</strong> </p> <p>Select whether the options to copy, print, or download files inside this shared drive, should be disabled for readers and commenters. When this restriction is enabled, it will override the similarly named field to true for any file inside this shared drive.</p> </li>
<li> <p><strong>Domain Users Only</strong> </p> <p>Select whether access to this shared drive and items inside this shared drive is restricted to users of the domain to which this shared drive belongs. This restriction may be overridden by other sharing policies controlled outside of this shared drive.</p> </li>
<li> <p><strong>Drive Members Only</strong> </p> <p>Select whether access to items inside this shared drive is restricted to its members.</p> </li>
</ul> </td>
</tr>
</tbody>
</table>
<h4 id="delete-a-shared-drive"><a name="Delete3"></a>Delete a Shared Drive</h4>
<p>This action module deletes a shared drive. The shared drive cannot contain any content.</p> <note type="important">
The G Suite administrator privilege is required in order to use this module.
</note>
<table cellspacing="15">
<col>
<col>
<tbody>
<tr>
<td>Connection </td>
<td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td>
</tr>
<tr>
<td>Shared Drive ID</td>
<td> <p>Enter or map the ID of the shared drive you want to delete.</p> </td>
</tr>
</tbody>
</table>
<p><strong>Other</strong></p>
<ul>
<li> <p><a href="#watch-comments" class="MCXref xref">Watch Comments</a> </p> </li>
<li> <p><a href="#get-a-folder-id-for-a-path" class="MCXref xref">Get a Folder ID for a Path</a> </p> </li>
<li> <p><a href="#make-an-api-call" class="MCXref xref">Make an API&nbsp;Call</a> </p> </li>
</ul>
<h4 id="watch-comments"><a name="Watch7"></a>Watch Comments</h4>
<p>This trigger module starts a scenario when a comment is added or modified on the selected file.</p>
<table cellspacing="15">
<col>
<col>
<tbody>
<tr>
<td>Connection </td>
<td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td>
</tr>
<tr>
<td>Watch Comments</td>
<td> <p>Select which comments you want to watch.</p>
<ul>
<li> <p><strong>By Created Time</strong> </p> <p>The module watches for new files<br></p> </li>
<li> <p><strong>By Modified Time</strong> </p> <p>The module watches for modified files.</p> </li>
</ul> </td>
</tr>
<tr>
<td>Choose a Drive</td>
<td> <p>Select what type of drive you want to monitor.</p>
<ul>
<li>My Drive</li>
<li>Shared With Me</li>
<li>Google Shared Drive (available for G Suite users only)</li>
</ul> <p>If you have selected the Google Shared Drive option in this field and you are not a G Suite user, the error <code>[400] Invalid Value</code> is returned.</p> </td>
</tr>
<tr>
<td>File ID</td>
<td>Navigate to the file you want to watch for comments.</td>
</tr>
<tr>
<td>Limit</td>
<td>Enter or map the maximum number of comments you want the module to return during each scenario execution cycle.</td>
</tr>
</tbody>
</table>
<h4 id="get-a-folder-id-for-a-path"><a name="Get5"></a>Get a Folder ID for a Path</h4>
<p>This action module retrieves the Folder ID for a given path.</p>
<table cellspacing="15">
<col>
<col>
<tbody>
<tr>
<td>Connection </td>
<td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td>
</tr>
<tr>
<td>Folder Path</td>
<td> <p>Enter or map the path to the folder you want to retrieve the ID&nbsp;for. Example: <code>abc/xyz</code></p> </td>
</tr>
</tbody>
</table>
<h4 id="make-an-api-call"><a name="Make"></a>Make an API&nbsp;Call</h4>
<p>This action module allows you to perform a custom API call.</p>
<table cellspacing="0">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Connection</td>
<td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to Adobe Workfront Fusion - Basic instructions</a></p> </td>
</tr>
<tr>
<td role="rowheader"> <p>URL</p> </td>
<td>Enter a path relative to <code>https://www.googleapis.com/drive</code>. Example: <code>/v3/files</code></td>
</tr>
<tr>
<td role="rowheader"> <p>Method</p> </td>
<td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods in Adobe Workfront Fusion</a>.</p> </td>
</tr>
<tr>
<td role="rowheader">Headers</td>
<td> <p>Add the headers of the request in the form of a standard JSON object.For example, <code>{"Content-type":"application/json"}</code>. Workfront Fusion adds the authorization headers for you.</p> </td>
</tr>
<tr>
<td role="rowheader">Query String</td>
<td> <p> Add the query for the API call in the form of a standard JSON object.</p> </td>
</tr>
<tr>
<td role="rowheader">Body</td>
<td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <note type="note">
<p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p>
<div class="example" data-mc-autonum="<b>Example: </b>">
<p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p>
</div>
</note> </td>
</tr>
</tbody>
</table>
</div>
-->

* [Triggers](#triggers) 
* [Actions](#actions)

### Triggers {#triggers}

* [Watch Files In Folder](#watch-files-in-folder) 
* [Watch All Files](#watch-all-files) 
* [Watch shared files](#watch-shared-files) 
* [Watch Comments](#watch-comments)

#### Watch Files In Folder

Retrieves file details when a file is added or modified in the specified folder.

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Connection </td>
   --> 
   <td> <p>For instructions about connecting your Google Drive account to Workfront Fusion, see <a href="#connecting-google-drive-to-workfront-fusion" class="MCXref xref">Connecting Google Drive to Workfront Fusion</a></p> </td> 
  </tr> 
  <tr> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the folder to be watched</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the folder on your drive that you want to watch the files in.</td>
   --> 
  </tr> 
  <tr> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">What files to watch</td>
   --> 
   <td> <p>Select which type of files you want to watch.</p> 
    <ul> 
     <li>All</li> 
     <li>Google Documents</li> 
     <li>Google Spreadsheets</li> 
     <li>Google Slides</li> 
     <li>Google Drawings</li> 
    </ul> </td> 
  </tr> 
  <tr> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Convert Google Documents files to format</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the file format that you want to convert Google Documents to.</td>
   --> 
  </tr> 
  <tr> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Convert Google Spreadsheets files to format</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the file format that you want to convert Google Spreadsheets to.</td>
   --> 
  </tr> 
  <tr> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Convert Google Slides files to format</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the file format that you want to convert Google Documents to.</td>
   --> 
  </tr> 
  <tr> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Convert Google Drawings files to format</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the file format that you want to convert Google Documents to.</td>
   --> 
  </tr> 
  <tr> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Watch</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select whether you want to watch new files and all changes, or only new files.</td>
   --> 
  </tr> 
  <tr> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Maximum number of downloaded files</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Set the maximum number of results that Workfront Fusion will download during one cycle (the number of repetitions per scenario run).</td>
   --> 
  </tr> 
 </tbody> 
</table>

#### Watch All Files

Retrieves file details when a file in your Google Drive is added or modified.

<table cellspacing="15"> 
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

<table cellspacing="15"> 
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

<table cellspacing="15"> 
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

<table cellspacing="15"> 
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

<table cellspacing="15"> 
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

<table cellspacing="15"> 
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

<table cellspacing="15"> 
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

<table cellspacing="15"> 
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

<table cellspacing="15"> 
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

<table cellspacing="15"> 
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

<table cellspacing="15"> 
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

<table cellspacing="15"> 
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

* **Field** - Attribute of the file that is being searched, for example, the attribute 

  ```
  name
  ```

  of the file.

* **Operator** - Test that is performed on the data to provide a match, for example, 

  ```
  contains
  ```

  .

* **Value** - The content of the attribute that is tested, for example, the name of the file 

  ```
  My cool document
  ```

  .

Combine clauses with the conjunctions 

```
and
```

or 

```
or
```

, and negate the query with 

```
not
```

.

* [Fields](#fields) 
* [Value types](#value-types) 
* [Operators](#operators) 
* [Examples](#examples)

### Fields {#fields}

<table cellspacing="15"> 
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

* The 

  ```
  contains
  ```

  operator only performs prefix matching for a 

  ```
  title
  ```

  .

  For example, the title "HelloWorld" matches for 

  ```
  title contains 'Hello'
  ```

  but not for 

  ```
  title contains 'World'
  ```

  .

* The 

  ```
  contains
  ```

  operator only performs matching on entire string tokens for 

  ```
  fullText
  ```

  .

  For example, if the full text of a doc contains the string "HelloWorld" only the query 

  ```
  fullText contains 'HelloWorld'
  ```

  returns a result. Queries such as fullText contains 'Hello' would not return results in this scenario.

* The 

  ```
  contains
  ```

  operator matches on an exact alphanumeric phrase if it is surrounded by double quotes.

  For example, if the 

  ```
  fullText
  ```

  of a doc contains the string "Hello there world", then the query 

  ```
  fullText contains '"Hello there"'
  ```

  returns a result, but the query 

  ```
  fullText contains '"Hello world"'
  ```

  does not.

  Furthermore, because the search is alphanumeric, if the 

  ```
  fullText
  ```

  of a doc contains the string "Hello_world", then the query 

  ```
  fullText contains '"Hello world"'
  ```

  returns a result.

* Fields of 

  ```
  type
  ```

  date are currently not comparable to each other, only to constant dates.

### Value types {#value-types}

<table cellspacing="15"> 
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

<table cellspacing="15"> 
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
<pre>modifiedDate > '2012-06-04T12:00:00' and (mimeType contains 'image/' or mimeType contains 'video/')</pre>This search returns all files with an image or video MIME type that their last modification was after June 4, 2012. Because 

```
and
```

and 

```
or
```

operators are evaluated from left to right, without parentheses, the above example would return only images modified after June 4, 2012, but would return all videos, even those before June 4, 2012.

### Examples {#examples}

All examples on this page show the unencoded ```<q>q</q>``` parameter, where 

```
title = 'hello'
```

is encoded as

```
title+%3d+%27hello%27
```

. Client libraries handle this encoding automatically.

Search for files with the name "hello"
<pre>title = 'hello'</pre>Search for folders using the folder-specific MIME type
<pre>mimeType = 'application/vnd.google-apps.folder'</pre>Search for files that are not folders
<pre>mimeType != 'application/vnd.google-apps.folder'</pre>Search for files with a name containing the words "hello" and "goodbye"
<pre>title contains 'hello' and name contains 'goodbye'</pre>Search for files with a name that does not contain the word "hello"
<pre>not title contains 'hello'</pre>Search for files containing the word "hello" in the content
<pre>fullText contains 'hello'</pre>Search for files not containing the word "hello" in the content
<pre>not fullText contains 'hello'</pre>Search for files containing the exact phrase "hello world" in the content
<pre>fullText contains '"hello world"'fullText contains '"hello_world"'</pre>Search for files with a query containing the "\" character (e.g., "\authors")
<pre>fullText contains '\\authors'</pre>Search for files writeable by the user "test@example.org"
<pre>'test@example.org' in writers</pre>Search for the ID 

```
1234567
```

in the 

```
parents
```

collection. This finds all files and folders located directly in the folder whose ID is 

```
1234567
```

.
<pre>'1234567' in parents</pre>Search for the alias ID 

```
appDataFolder
```

in the 

```
parents
```

collection. This finds all files and folders located directly under the [Application Data folder](https://developers.google.com/drive/api/v2/appdata).
<pre>'appDataFolder' in parents</pre>Search for files writeable by the users "test@example.org" and "test2@example.org"
<pre>'test@example.org' in writers and 'test2@example.org' in writers</pre>Search for files containing the text "important" which are in the trash
<pre>fullText contains 'important' and trashed = true</pre>Search for files modified after June 4th 2012
<pre>modifiedDate > '2012-06-04T12:00:00' // default time zone is UTC</pre><pre>modifiedDate > '2012-06-04T12:00:00-08:00'</pre>Search for files shared with the authorized user with "hello" in the name
<pre>sharedWithMe and title contains 'hello'</pre>Search for files with a [custom file property](https://developers.google.com/drive/api/v2/properties) named 

```
additionalID
```

with the value 

```
8e8aceg2af2ge72e78
```

.
<pre>properties has { key='additionalID' and value='8e8aceg2af2ge72e78' and visibility='PRIVATE' }</pre>Source of this guide is [Google Drive documentation](https://developers.google.com/drive/api/v2/search-shareddrives).
