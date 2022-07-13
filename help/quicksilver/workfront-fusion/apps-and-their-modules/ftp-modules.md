---
filename: ftp-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: FTP modules
description: FTP modules let you monitor file changes in a selected folder, upload new files to the desired folder, and modify or delete existing files that are already in a folder.
---

# FTP modules

FTP modules let you monitor file changes in a selected folder, upload new files to the desired folder, and modify or delete existing files that are already in a folder.

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

In order to use [Fusion App] with Workfront Fusion, you must have an FTP account.

## Create a connection in an FTP module {#create-a-connection}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection name</td> 
   <td> <p> Enter the name for your FTP connection.</p> </td> 
  </tr> 
  <tr> 
   <td>Host </td> 
   <td> <p>Enter the FTP server hostname. E.g. <code>myftp123.server.com</code></p> </td> 
  </tr> 
  <tr> 
   <td>Port </td> 
   <td> <p>Enter the FTP server port number. E.g. <code>21</code></p> </td> 
  </tr> 
  <tr> 
   <td>User name </td> 
   <td> <p>Enter your FTP account user name.</p> </td> 
  </tr> 
  <tr> 
   <td>Password </td> 
   <td> <p>Enter your FTP account password.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Use a secure connection (TLS)</p> </td> 
   <td> <p>Select whether you want to use a secure connection.</p> <p style="font-weight: bold;">No</p> <p>The connection is not secured.</p> <p style="font-weight: bold;">Explicit encryption or Implicit encryption</p> <p>The connection is secured using SSL.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Reject unauthorized certificates</p> </td> 
   <td> <p>Enable this option to verify the FTP server certificate. If the verification fails, the connection will not be created. To pass the verification, the certificate must meet one of the following criteria:</p> 
    <ul> 
     <li>be signed by a Root <a href="https://en.wikipedia.org/wiki/Certificate_authority">Certificate Authority</a></li> 
     <li>be signed by an Intermediate Certificate Authority (see e.g. <a href="https://knowledge.digicert.com/solution/SO16297.html">How certificate chains work</a> for further explanation). In this case all the Intermediate Certificates should be installed on the FTP server.</li> 
     <li>be a Self-Signed Certificate supplied in the Self-signed certificate field (see below)</li> </ul>
     
   If this option is disabled, the FTP server certificate is not verified. We strongly advise against disabling the option as it renders the connection insecure and poses a serious security risk.</td> 
  </tr> 
  <tr> 
   <td> <p>Self-signed certificate</p> </td> 
   <td> <p>Click the <b>Extract</b> button to open the upload dialog.</p> <p>Upload the certificate to use the TLS with your self-signed certificate. Workfront Fusion does not retain or store any data you provide, such as files and passwords. File and password are used only to extract the certificate.</p> </td> 
  </tr> 
 </tbody> 
</table>

## FTP modules and their fields

* [Triggers](#triggers) 
* [Actions](#actions) 

### Triggers {#triggers}

#### Watch files

Watch files is the only trigger module for FTP. It monitors the file content of the selected folder. The trigger is executed when a new file is inserted into the specified folder.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions on establishing a connection to the FTP account, see <a href="#create-a-connection" class="MCXref xref">Create a connection in an FTP module</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Folder</p> </td> 
   <td> <p>Select the folder you want to watch.</p> <p><b>Note:</b> Only one folder per scenario is allowed. Subfolders are ignored.</p> <p><b>Tip:</b> To keep track of multiple folders, create an independent scenario for each of them.</p> </td> 
  </tr> 
  <tr> 
   <td>Maximum number of returned files </td> 
   <td> <p>Set the maximum number of results that Workfront Fusion will work with during one cycle. If the value is set too high, the connection may be interrupted on the side of the given third-party service (timeout). Workfront Fusion has no influence on this. We recommend that you set a lower value and either define a higher value for the maximum number of cycles or run the scenario more frequently.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Actions {#actions}

* [Change permissions](#change-permissions)
* [Create a folder](#create-a-folder)
* [Delete a file](#delete-a-file) 
* [Delete a folder](#delete-a-folder) 
* [Get a file](#get-a-file)
* [List of files in a folder](#list-of-files-in-a-folder) 
* [Move a file or folder](#move-a-file-or-folder)
* [Upload a file](#upload-a-file) 

#### Change permissions {#change-permissions}

This action module changes permission settings of a file or folder.

<table style="width: 100%;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" />
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" />
   <tbody>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Connection</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">For instructions on establishing a connection to the FTP account, see <a href="#Create" class="MCXref_0">Create a connection in an FTP module</a> in this article.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Change permission settings of</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">
               <p>Select whether you want to change settings for a file or folder.</p>
            </td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">File path</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">Enter or map the file path to the folder or file.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-MediumGray" role="rowheader">Permissions</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-MediumGray">
               <p>Set the desired file or folder permissions. Use the chmod parameters. For example: <code>777 </code>or <code>-rwxrwxrwx</code>.</p>
               <p>Permissions must match the pattern <code> /(.?([r-][w-][x-]){3})|[0-7]{3,4}/</code>.</p>
            </td>
         </tr>
   </tbody>
</table>

#### Create a folder

This action module creates a new folder.

<table style="width: 100%;" class="TableStyle-TableStyle-List-options-in-steps" cellspacing="0">
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1" />
   <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2" />
   <tbody>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-LightGray" role="rowheader">Connection</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">For instructions on establishing a connection to the FTP account, see <a href="#Create" class="MCXref_0">Create a connection in an FTP module</a> in this article.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-MediumGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyE-Column1-MediumGray" role="rowheader">Folder path</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-MediumGray">Enter or map the file path to the new folder.</td>
         </tr>
         <tr class="TableStyle-TableStyle-List-options-in-steps-Body-LightGray">
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">New folder name</td>
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">
               <p>Enter or map a name for the new folder.</p>
            </td>
         </tr>
   </tbody>
</table>
 
#### Delete a file {#delete-a-file}

Deletes a file from the specified folder.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
            <td class="TableStyle-TableStyle-List-options-in-steps-BodyD-Column2-LightGray">For instructions on establishing a connection to the FTP account, see <a href="#Create" class="MCXref_0">Create a connection in an FTP module</a> in this article.</td>
  </tr> 
  <tr> 
   <td>Folder </td> 
   <td> <p>Select the FTP folder you want to delete a file from.</p> </td> 
  </tr> 
  <tr> 
   <td>File name</td> 
   <td> <p> Enter the filename, including file name extension. Example: <code>image.png</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### Delete a folder

This action module permanently deletes the specified folder.

<table style="width: 100%;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15">
   <col style="width: 301px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <tbody>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Connection</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">For instructions on establishing a connection to the FTP account, see <a href="#Create" class="MCXref_0">Create a connection in an FTP module</a> in this article.</td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-MediumGray" style="font-weight: bold;">Folder</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-MediumGray">
               <p>Select the FTP folder you want to delete a file from.</p>
            </td>
         </tr>
   </tbody>
</table>

#### Get a file {#get-a-file}

Retrieves a file from the FTP server which can be further processed, e.g. uploaded to the Dropbox.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions on establishing a connection to the FTP account, see <a href="#creating-the-ftp-connection" class="MCXref xref">Creating the FTP Connection</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>File path</td> 
   <td> <p> Enter the path of the file you want to get.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### List of files in a folder {#list-of-files-in-a-folder}

Retrieves file and/or folder information.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td> <p>For instructions on establishing a connection to the FTP account, see <a href="#creating-the-ftp-connection" class="MCXref xref">Creating the FTP Connection</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Folder </td> 
   <td> <p>Select the FTP folder you want to search in.</p> </td> 
  </tr> 
  <tr> 
   <td>Show </td> 
   <td> <p>Select whether you want to retrieve information about files or folders, or both.</p> </td> 
  </tr> 
  <tr> 
   <td>Search </td> 
   <td> <p>Enter the search term. If no search term is entered all files and folders from the specified folder will be retrieved.</p> </td> 
  </tr> 
  <tr> 
   <td>Maximum number of returned files</td> 
   <td> <p> Set the maximum number of retrieved files by this module.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Move a file or folder

This action module moves a file or folder to a different location.

<table style="width: 100%;" class="TableStyle-TableStyle-HeaderRow" cellspacing="15">
   <col style="width: 301px;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <col style="width: 50%;" class="TableStyle-TableStyle-HeaderRow-Column-Column1" />
   <tbody>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-LightGray" style="font-weight: bold;">Connection</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-LightGray">For instructions on establishing a connection to the FTP account, see <a href="#Create" class="MCXref_0">Create a connection in an FTP module</a> in this article.</td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-MediumGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyE-Column1-MediumGray" style="font-weight: bold;">Old file path</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyD-Column1-MediumGray">
               <p>Enter the path that you want to move the file from. Example: <code>/folder1/document.txt</code>.</p>
            </td>
         </tr>
         <tr class="TableStyle-TableStyle-HeaderRow-Body-LightGray">
            <td class="TableStyle-TableStyle-HeaderRow-BodyB-Column1-LightGray" style="font-weight: bold;">New file path</td>
            <td class="TableStyle-TableStyle-HeaderRow-BodyA-Column1-LightGray">
               <p>Enter the path that you want to move the file to. Example: <code>/folder2/document.txt</code>.</p>
            </td>
         </tr>
   </tbody>
</table>


#### Upload a file {#upload-a-file}

Uploads a file to the FTP server.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Connection </td> 
   <td>For instructions on establishing a connection to the FTP account, see <a href="#creating-the-ftp-connection" class="MCXref xref">Creating the FTP Connection</a> in this article.</td> 
  </tr> 
  <tr> 
   <td>Folder </td> 
   <td> <p>Select the FTP folder you want to upload the file to.</p> </td> 
  </tr> 
  <tr> 
   <td>Source file </td> 
   <td> <p>Select a source file from a previous module, or map the source file's name and data.</p> </td> 
  </tr> 
  <tr> 
   <td>Append to an already existing file</td> 
   <td> <p>If this option is enabled and the file already exists on the FTP server, the contents of the file are appended to the existing file. If this option is not enabled, the content of the file will be overwritten.</p> </td> 
  </tr> 
  <tr> 
   <td>Create folders if don't exist </td> 
   <td> <p>If this option is enabled and the folder you have entered to the Folder field does not exist on the FTP server, the module creates the folder</p> </td> 
  </tr> 
 </tbody> 
</table>

## Troubleshooting {#troubleshooting}

If you are experiencing issues with the FTP app either during the connection creation or during a module's operation, try to use one of the popular FTP clients, and try to perform the same action (for example, create a connection or list files in a folder). with the FTP client. If you are experiencing the same issues also with the FTP client, the reason might be a misconfiguration of the FTP server.
