---
filename: sftp
content-type: reference
product: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: SFTP modules
description: The Adobe Workfront Fusion SFTP modules allow you to monitor file changes in a selected folder/subfolder, upload new files to the desired folder, modify, or delete existing files that are already in a folder, or change file permissions.
---

# SFTP modules

The Adobe Workfront Fusion SFTP modules allow you to monitor file changes in a selected folder/subfolder, upload new files to the desired folder, modify, or delete existing files that are already in a folder, or change file permissions.

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

In order to use SFTP with Workfront Fusion, it is necessary to have an SFTP account (such as GoDaddy web hosting).

## Connect SFTP to Workfront Fusion {#connect-sftp-to-workfront-fusion}

To connect your SFTP account to Workfront Fusion you need to enter the target Host and the SFTP credentials (user name and password or user name and key) to the module's Create a connection dialog.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Connection name</td> 
   <td> <p> Enter the name for your SFTP connection.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Host</p> </td> 
   <td> <p>Enter the host name of the SFTP server you want to connect.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Port </td> 
   <td> <p>Enter the SFTP server port. For example, 22.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Auth type</p> </td> 
   <td> <p>Select the authorization method you want to use for connecting to the SFTP server.</p> 
    <ul> 
     <li><strong>User name and password</strong>: Enter your credentials.</li> 
     <li> <p><strong>User name and key</strong>: Enter your user name and the private key/certificate</p> <p>Upload the private key to use the client-side authorization or upload your certificate (P12 or PFX file) if you want to use TLS using your self-signed certificate. If you're using the client-side certificate authorization, you can enter your CA certificate here.</p> <p>Workfront Fusion does not retain or store any data (files, passwords) you provide here. File and password are only used to extract a private key/certificate.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

After entering the connection information, click **Continue** to establish a connection.

## SFTP modules and their fields

When you configure SFTP modules, Workfront Fusion displays the fields listed below. Along with these, additional SFTP fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Triggers

#### Watch Files in a Folder

Returns files with details when a file is created or changed in a specified folder.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your SFTP account to Workfront Fusion, see <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connect SFTP to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Folder </td> 
   <td> <p>Enter or map the folder you want to watch. You can specify an absolute path such <code>/home/user/</code>. Or you can specify a relative path pointing to a specific folder of the logged in user, such as <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>Buffer Size [B]</td> 
   <td> <p> Enter the buffer size in bytes. The value defines the size of transferred chunks from the server. Some servers may cause problems or corrupt files when the value is too high.</p> </td> 
  </tr> 
  <tr> 
   <td>Maximum number of returned files</td> 
   <td> <p> Set the maximum number of files that Workfront Fusion will work with during one cycle</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Watch Subfolders in a Folder

Returns folders with details when a folder is created or changed in a specified folder.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your SFTP account to Workfront Fusion, see <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connect SFTP to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Folder </td> 
   <td> <p>Enter or map the folder you want to watch. You can specify an absolute path such <code>/home/user/</code>. Or you can specify a relative path pointing to a specific folder of the logged in user, such as <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>Maximum number of returned files</td> 
   <td> <p> Set the maximum number of folders that Workfront Fusion will return during one cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions

#### List a folder's content

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your SFTP account to Workfront Fusion, see <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connect SFTP to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Show </td> 
   <td> <p>Select whether you want to retrieve files, folders, or both.</p> </td> 
  </tr> 
  <tr> 
   <td>Folder </td> 
   <td> <p>Enter or map the folder that contains the files or folders you want to list. You can specify an absolute path such <code>/home/user/</code>. Or you can specify a relative path pointing to a specific folder of the logged in user, such as <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>Search </td> 
   <td> <p>Enter or map the search term. For example, if you want to search for files with the file extension .txt, enter <code>.txt</code>.You can also enter or map the name of the file you want to search for.</p> </td> 
  </tr> 
  <tr> 
   <td>Sort By</td> 
   <td> <p> Select whether you want to sort results by file name, size, last access date, or last modified date.</p> </td> 
  </tr> 
  <tr> 
   <td>Sort Order </td> 
   <td> <p>Select whether the result should be returned in ascending or descending order.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Continue the execution of the route even if the module returns no results</p> </td> 
   <td>Enable this option to ensure that this module does not stop the scenario if it returns no results.</td> 
  </tr> 
  <tr> 
   <td>Maximum number of returned results</td> 
   <td> <p> Set the maximum number of results that Workfront Fusion will return during one cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Get Files

This module lists files from a specified folder.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your SFTP account to Workfront Fusion, see <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connect SFTP to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Buffer Size [B]</td> 
   <td> <p> Enter the buffer size in bytes. The value defines the size of transferred chunks from the server. Some servers may cause problems or corrupt files when the value is too high.</p> </td> 
  </tr> 
  <tr> 
   <td>Folder </td> 
   <td> <p>Enter or map the folder that contains the files or folders you want to list. You can specify an absolute path such <code>/home/user/</code>. Or you can specify a relative path pointing to a specific folder of the logged in user, such as <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>Search </td> 
   <td> <p>Enter or map the search term. For example, if you want to search for files with the file extension .txt, enter <code>.txt</code>.You can also enter or map the name of the file you want to search for.</p> </td> 
  </tr> 
  <tr> 
   <td>Sort By</td> 
   <td> <p> Select whether you want to sort results by the file name, size, last access date, or last modified date.</p> </td> 
  </tr> 
  <tr> 
   <td>Sort Order</td> 
   <td> <p> Select whether the result should be returned in ascending or descending order.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Continue the execution of the route even if the module returns no results</p> </td> 
   <td>Enable this option to ensure that this module does not stop the scenario if it returns no results.</td> 
  </tr> 
  <tr> 
   <td>Maximum number of returned results</td> 
   <td> <p> Set the maximum number of files that Workfront Fusion will return during one cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Get a File

This module retrieves file details, including a file's data.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your SFTP account to Workfront Fusion, see <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connect SFTP to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Buffer Size [B]</td> 
   <td> <p> Enter the buffer size in bytes. The value defines the size of transferred chunks from the server. Some servers may cause problems or corrupt files when the value is too high.</p> </td> 
  </tr> 
  <tr> 
   <td>File Path </td> 
   <td> <p>Enter the path to the file. You can specify an absolute path such as<code>/home/user/file.txt</code>. Or you can specify a relative path pointing to a specific folder of the logged in user, such as <code>./file.txt</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Upload a File

This module allows you to upload a file to the SFTP server.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your SFTP account to Workfront Fusion, see <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connect SFTP to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Folder </td> 
   <td> <p>Specify an existing folder as the storage location for the file. You can specify an absolute path such <code>/home/user/</code>. Or you can specify a relative path pointing to a specific folder of the logged in user, such as <code>./.</code></p> </td> 
  </tr> 
  <tr> 
   <td>Source File</td> 
   <td> <p> Map the source file from a previous module, such as Dropbox &gt; Get File. You can also enter or map the file name and file data.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Permissions</p> </td> 
   <td> <p>Set the desired permissions for the file or folder. Use chmod parameters. For example: <code>777 </code>or <code>-rwxrwxrwx</code>.</p> <p>For more details about chmod, please refer to the <a href="https://ss64.com/bash/chmod.html">chmod documentation</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Rename a File

Renames a file.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your SFTP account to Workfront Fusion, see <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connect SFTP to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>File Path</td> 
   <td> <p> Enter the path to the file you want to rename. You can specify an absolute path such as<code>/home/user/file.txt</code>. Or you can specify a relative path pointing to a specific folder of the logged in user, such as <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>New file name</td> 
   <td> <p> Enter the new name for the file, including the file extension.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Move a File

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your SFTP account to Workfront Fusion, see <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connect SFTP to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>File Path</td> 
   <td> <p> Enter the path to the file you want to move. You can specify an absolute path such as<code>/home/user/file.txt</code>. Or you can specify a relative path pointing to a specific folder of the logged in user, such as <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>New Folder</td> 
   <td> <p> Enter the path to the file's new location. You can specify an absolute path such <code>/home/user/</code>. Or you can specify a relative path pointing to a specific folder of the logged in user, such as <code>./.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### Delete a File

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your SFTP account to Workfront Fusion, see <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connect SFTP to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>File Path</td> 
   <td> <p> Enter the path to the file you want to delete. You can specify an absolute path such as<code>/home/user/file.txt</code>. Or you can specify a relative path pointing to a specific folder of the logged in user, such as <code>./file.txt</code>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Update file permissions

Allows you to change permissions of the file.

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your SFTP account to Workfront Fusion, see <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connect SFTP to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>File Path</td> 
   <td> <p> Enter the path to the file you want to move. You can specify an absolute path such as<code>/home/user/file.txt</code>. Or you can specify a relative path pointing to a specific folder of the logged in user, such as <code>./file.txt</code>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Permissions</p> </td> 
   <td> <p>Set the desired file permissions. Use the chmod parameters. For example, <code>777 </code>or <code>-rwxrwxrwx</code>.</p> <p>Must match pattern /(.?([r-][w-][x-]){3})|[0-7]{3}/.</p> <p>For more details about chmod, please refer to the <a href="https://ss64.com/bash/chmod.html">chmod documentation</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Create Folder

Creates a new folder in the specified location.

>[!NOTE]
>
>If the folder already exists, the module will throw an error. To continue the flow uninterrupted, attach an error handler route to the module to catch the error and employ the Resume directive to continue the flow. For information about attaching an error handler route, see [Error handling in Adobe Workfront Fusion](../../workfront-fusion/errors/error-handling.md). For information about the error handler route, see [Directives for error handling in Adobe Workfront Fusion](../../workfront-fusion/errors/directives-for-error-handling.md).

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your SFTP account to Workfront Fusion, see <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connect SFTP to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Folder </td> 
   <td> <p>Specify an existing folder as the storage location for the new folder. You can specify an absolute path such as<code>/home/user/file.txt</code>. Or you can specify a relative path pointing to a specific folder of the logged in user, such as <code>./</code>.</p> </td> 
  </tr> 
  <tr> 
   <td>Folder Name</td> 
   <td> <p> Enter the folder name.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Permissions</p> </td> 
   <td> <p>Set the desired folder permissions. Use chmod parameters. For example, <code>777 </code>or <code>-rwxrwxrwx</code>.</p> <p>Must match pattern /(.?([r-][w-][x-]){3})|[0-7]{3}/.</p> <p>For more details about chmod, please refer to the <a href="https://ss64.com/bash/chmod.html">chmod Man Page</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Delete a Folder

<table> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions about connecting your SFTP account to Workfront Fusion, see <a href="#connect-sftp-to-workfront-fusion" class="MCXref xref">Connect SFTP to Workfront Fusion</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Folder Path</td> 
   <td> <p> Specify the path to the folder you want to delete. You can specify an absolute path such <code>/home/user/</code>. Or you can specify a relative path pointing to a specific folder of the logged in user, such as <code>./.</code></p> </td> 
  </tr> 
 </tbody> 
</table>

