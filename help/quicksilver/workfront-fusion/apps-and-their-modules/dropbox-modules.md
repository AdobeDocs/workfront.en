---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Dropbox modules
description: In a [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use Dropbox, as well as connect it to multiple third-party applications and services.This allows you to automate activities such as monitoring, searching, retrieving, listing, creating, and editing files and folders in your Dropbox.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: a35631d7-40ac-4e7f-9a37-ad3879c0b6a2
---
# [!DNL Dropbox] modules

In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use [!UICONTROL Dropbox] or [!DNL Dropbox Business], as well as connect it to multiple third-party applications and services.This allows you to automate activities such as monitoring, searching, retrieving, listing, creating, and editing files and folders in your [!UICONTROL Dropbox].

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

* To use [!DNL Dropbox] modules, you must have a [!DNL Dropbox] account.

>[!IMPORTANT]
>
>Dropbox must approve applications with more than 50 users. 
>
>For more information, search for "Production approval" in the Dropbox developer guide.


## Create a connection to [!DNL Dropbox]

To create a connection for your [!DNL Dropbox] modules:

1. Click **[!UICONTROL Add]** next to the Connection box.
    
1. Fill in the following fields:
    
    <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
        <td role="rowheader">[!UICONTROL Connection name]</td>
        <td>
          <p>Enter a name for this connection.</p>
        </td>
        <tr>
        <td role="rowheader">[!UICONTROL Environment]</td>
        <td>Select whether this connection is for a production or non-production environment.</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Type]</td>
        <td>Select whether you are connecting to a service account or a personal account.</td>
        </tr>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>Enter your [!UICONTROL Dropbox] [!UICONTROL Client ID]. </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>Enter your [!DNL Dropbox] [!UICONTROL Client Secret]. </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Account Type]</td>
        <td>Select whether you are connecting to a personal Dropbox account or a business (Dropbox Business) account.</td>
        </tr>
      </tbody>
    </table>
    
1. Click **[!UICONTROL Continue]** to save the connection and return to the module.## [!DNL Dropbox] modules and their fields

## [!DNL Dropbox] modules and their fields

When you configure [!DNL Dropbox] modules, [!DNL Workfront Fusion] displays the fields listed below. Along with these, additional [!DNL Dropbox] fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Trigger modules](#trigger-modules)
* [Modules for getting [!DNL Dropbox] files and folders](#modules-for-getting-dropbox-files-and-folders)
* [Modules for creating and editing [!DNL Dropbox] files and folders](#modules-for-creating-and-editing-dropbox-files-and-folders)
* [Other modules](#other-modules)

### Trigger modules 

#### [!UICONTROL Watch Files]

This Trigger type module returns file details when the file in a specified folder is modified.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Dropbox] account to [!DNL Workfront Fusion], see <a href="#create-a-connection-to-dropbox" class="MCXref xref">Create a connection to [!DNL Dropbox]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Select the folder you want to watch for changes.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Watch also subfolders]</td> 
   <td> <p> Enable this option to also monitor subfolders in the selected folder for modified files.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit] </td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Modules for getting [!DNL Dropbox] files and folders 

* [[!UICONTROL Search Files/Folders]](#search-filesfolders)
* [[!UICONTROL Download a File]](#download-a-file)
* [[!UICONTROL Get a Folder Metadata]](#get-a-folder-metadata)
* [[!UICONTROL List All Files/Subfolders in a Folder]](#list-all-filessubfolders-in-a-folder)
* [[!UICONTROL List File Revisions]](#list-file-revisions)

#### [!UICONTROL Search Files/Folders] 

This search module looks for records in an object in [!DNL Dropbox] that match the search query you specify.

You can map this information in subsequent modules in the scenario.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Dropbox] account to [!DNL Workfront Fusion], see <a href="#create-a-connection-to-dropbox" class="MCXref xref">Create a connection to [!DNL Dropbox]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search] </td> 
   <td> <p>Enter the search term.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Select the folder you want to search. This module searches the entire [!DNL Dropbox] if you do not select a folder.</p> </td> 
  </tr> 
  <tr> 
   <td>File Status</td> 
   <td> <p> Select the file status to restrict the search to the selected file status.</p> </td> 
  </tr> 
  <tr> 
   <td>File Categories</td> 
   <td> <p> Select the file categories to restrict the search to the selected categories.</p> </td> 
  </tr> 
  <tr> 
   <td>File extensions</td> 
   <td> <p> Choose the file extensions you want to search for.</p> </td> 
  </tr> 
  <tr> 
   <td>Limit </td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Download a File]

This action module downloads a file from a folder.

You specify the file and its location.

The module returns the ID of the file and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

>[!NOTE]
>
>This module is useful for providing files to subsequent modules.

When you are configuring this module, the following fields display.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Dropbox] account to [!DNL Workfront Fusion], see <a href="#create-a-connection-to-dropbox" class="MCXref xref">Create a connection to [!DNL Dropbox]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Way of selecting files</td> 
   <td> <p> Select whether you want to map the file path or select the file manually.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>File Path / File</p> </td> 
   <td> <p style="font-weight: bold;">File Path</p> <p>Enter or map the target path to the file.</p> <p style="font-weight: bold;">File</p> <p>Select the file from the menu.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get a Folder Metadata]

This action module retrieves shared folder details.

You specify the ID of the folder.

The module returns the ID of the folder and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Dropbox] account to [!DNL Workfront Fusion], see <a href="#create-a-connection-to-dropbox" class="MCXref xref">Create a connection to [!DNL Dropbox]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Shared Folder ID</td> 
   <td> <p> Enter or map the ID of the folder you want to retrieve details about.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL List All Files/Subfolders in a Folder] 

This action module lists files or folders in a particular folder.

You specify the ID of the folder.

The module returns the IDs of the files or foldes and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Dropbox] account to [!DNL Workfront Fusion], see <a href="#create-a-connection-to-dropbox" class="MCXref xref">Create a connection to [!DNL Dropbox]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>List </td> 
   <td> <p>Select whether you want to retrieve files or folders.</p> </td> 
  </tr> 
  <tr> 
   <td>Show Only Downloadable Files</td> 
   <td> <p> Enable this option to return only downloadable files. Some types of files, such as Google Docs, are not downloadable.</p> </td> 
  </tr> 
  <tr> 
   <td>Folder </td> 
   <td> <p>Enter or map the folder you want to retrieve files or folders from.</p> </td> 
  </tr> 
  <tr> 
   <td>Limit </td> 
   <td> <p>Enter or map the maximum number of records you want the module to list during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL List File Revisions]

This action module retrieves all file revisions (a version history) of a particular file.\
You specify the ID of the file.

The module returns any standard fields associated with the record, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Dropbox] account to [!DNL Workfront Fusion], see <a href="#create-a-connection-to-dropbox" class="MCXref xref">Create a connection to [!DNL Dropbox]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Way of selecting files</td> 
   <td> <p> Select whether you want to map the file path or select the file manually.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>File Path / File</p> </td> 
   <td> <p style="font-weight: bold;">File Path</p> <p>Enter or map the target path to the file.</p> <p style="font-weight: bold;">File</p> <p>Select the file from the menu.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Limit</p> </td> 
   <td> <p>Enter or map the maximum number of records you want the module to list during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Modules for creating and editing [!DNL Dropbox] files and folders 

* [[!UICONTROL Upload] a File](#upload-a-file)
* [[!UICONTROL Create a Folder]](#create-a-folder)
* [[!UICONTROL Create/Overwrite a Text File]](#createoverwrite-a-text-file)
* [[!UICONTROL Create/Update a Share Link]](#createupdate-a-share-link)
* [[!UICONTROL Restore a File]](#restore-a-file)
* [[!UICONTROL Move a File/Folder]](#move-a-filefolder)
* [[!UICONTROL Rename a File/Folder]](#rename-a-filefolder)
* [[!UICONTROL Delete a File/Folder]](#delete-a-filefolder)

#### [!UICONTROL Upload a File]

This action module uploads a file to a folder.

You specify information such as the location for the file, the file you want to upload, and an optional new name for the file.

The module returns the ID of the  file and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Dropbox] account to [!DNL Workfront Fusion], see <a href="#create-a-connection-to-dropbox" class="MCXref xref">Create a connection to [!DNL Dropbox]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder]</td> 
   <td> <p> Select the folder of your [!DNL Dropbox] you want to upload the file to.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Source File]</p> </td> 
   <td> <p>Enter or map the file you want to add to the [!DNL Dropbox] folder selected above.</p> <p style="font-weight: bold;">[!UICONTROL File name]</p> <p>Enter or map the file name, including the file extension.</p> <p style="font-weight: bold;">[!UICONTROL File data]</p> <p>Enter or map the file data (from previous module such as [!UICONTROL Google Drive] >[!UICONTROL Get a File)].</p> <p>Note: The maximum size of the uploaded file is 150 MB.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Overwrite an existing file]</td> 
   <td> <p> Enable this option to replace the existing file with the new file. If this option is left disabled, the uploaded file is renamed.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create a Folder]

This action module creates a new folder.

You specify the path and a name for the folder.

The module returns the ID of the  folder and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Dropbox] account to [!DNL Workfront Fusion], see <a href="#create-a-connection-to-dropbox" class="MCXref xref">Create a connection to [!DNL Dropbox]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder Name] </td> 
   <td> <p>Enter the name for the new folder.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Folder]</p> </td> 
   <td> <p>Enter or map the path where you want to create a new folder.</p> <p>Note:   <p>If you are using a [!DNL Dropbox Business] account (with team spaces), you must remove the slash <code>/</code>, or do not click <strong>[!UICONTROL Click here] to choose folder</strong> to create a team folder in the root.</p> <p>If the slash is not removed an error <code>[409] path/malformed_path/..</code> is returned.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Auto rename]</td> 
   <td> <p> Enable this option to rename the new folder, if a folder with the same name already exists in the target location.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create/Overwrite a Text File]

This action module creates a DOC file or overwrites the content of an existing one.

You specify the source file and the folder.

The module returns the ID of the  folder and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Dropbox] account to [!DNL Workfront Fusion], see <a href="#create-a-connection-to-dropbox" class="MCXref xref">Create a connection to [!DNL Dropbox]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Select to]</td> 
   <td> <p> Select whether you want to create or overwrite a DOC file.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>Select the target location where you want to create a file.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Source File]</p> </td> 
   <td> <p>Enter or map the file you want to add to the [!DNL Dropbox] folder.</p> <p style="font-weight: bold;">File name</p> <p>Enter the file name for the new DOC file (without an extension).</p> <p style="font-weight: bold;">File Content</p> <p>Enter the text content of the DOC file.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create/Update a Share Link]

This action module creates a public link to a file.

You specify the file and information about the link.

The module returns the ID of the link and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Dropbox] account to [!DNL Workfront Fusion], see <a href="#create-a-connection-to-dropbox" class="MCXref xref">Create a connection to [!DNL Dropbox]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Way of selecting files]</td> 
   <td> <p> Select whether you want to map or enter the file path, or select the file manually.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL File Path / File]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL File Path]</p> <p>Enter or map the target path to the file.</p> <p style="font-weight: bold;">[!UICONTROL File]</p> <p>Select the file from the menu.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Requested Visibility]</p> </td> 
   <td> <p>Select whether the link is public, for team, or password restricted.</p> <p>Note: [!UICONTROL Team only] and [!UICONTROL Access with password] options are only available to users who have [!DNL Dropbox Pro] or higher version.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Link's Expiration Date]</td> 
   <td> <p> Enter the date and time when the link will expire and will be no longer accessible. If this field is left empty, the link will not expire. For a list of supported date and time formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">Type coercion in [!DNL Adobe Workfront Fusion]</a>.</p> <p>Note: [!UICONTROL Team only] and [!UICONTROL Access with password] options are only available to users who have [!UICONTROL Dropbox Pro] or higher versions.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Link's Access Level]</p> </td> 
   <td> <p>Set the permission for the link recipient.</p> <p><strong>[!UICONTROL Viewer]</strong> Users who use the link can view and comment on the content.</p> <p><strong>[!UICONTROL Editor]</strong> Users who use the link can edit, view, and comment on the content.</p> <p><strong>[!UICONTROL Max]</strong> Users who use the link receive the maximum access level you can set the link to.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Restore a File] 

This action module restores a previous version of a file.

You specify the file and the number of the revision you want.

The module returns the ID of the  version and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Dropbox] account to [!DNL Workfront Fusion], see <a href="#create-a-connection-to-dropbox" class="MCXref xref">Create a connection to [!DNL Dropbox]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Way of selecting files]</td> 
   <td> <p> Select whether you want to map or enter the file path, or select the file manually.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL File Path] / [!UICONTROL File]</p> </td> 
   <td> <p><strong>[!UICONTROL File Path]</strong> </p> <p>Enter or map the target path to the file.</p> <p><strong>[!UICONTROL File]</strong> </p> <p>Select the file from the menu.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Revision]</p> </td> 
   <td> <p>Enter or map the revision number of the revision you want to restore.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Move a File/Folder]

This action module moves a file or folder to a different location.

You specify the file or folder and how and where you ant to move it.

The module returns the ID of the  file or folder and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Dropbox] account to [!DNL Workfront Fusion], see <a href="#create-a-connection-to-dropbox" class="MCXref xref">Create a connection to [!DNL Dropbox]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Way of selecting files] </td> 
   <td> <p>Select whether you want to map or enter the file path, or select the file manually.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL File/Folder Path] / [!UICONTROL File/Folder]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL File/Folder Path]</p> <p>Enter or map the target path to the file or folder.</p> <p style="font-weight: bold;">[!UICONTROL File/Folder]</p> <p>Select the file or folder from the menu.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL To Folder]</p> </td> 
   <td> <p>Enter or map the target location for the file or folder.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL New Name]</p> </td> 
   <td> <p>Enter the new name for the file or folder in the new location.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Auto Rename]</p> </td> 
   <td> <p>Enable this option to ensure that if a file or folder with the same name exists, the module renames the new file or folder by adding ([!UICONTROL NUMBER]) after the file or folder name. Otherwise the file or folder in the target location is overwritten.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Allow ownership transfer]</p> </td> 
   <td> <p>Enable this option to allow moves by owner, even if it would result in an ownership transfer for the content being moved.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Rename a File/Folder] 

This action module renames a file or folder.

You specify the file or folder and the new name.

The module returns the ID of the  file or folder and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Dropbox] account to [!DNL Workfront Fusion], see <a href="#create-a-connection-to-dropbox" class="MCXref xref">Create a connection to [!DNL Dropbox]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>Way of selecting files</td> 
   <td> <p> Select whether you want to map or enter the file path, or select the file manually.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>File/Folder Path / File/Folder</p> </td> 
   <td> <p style="font-weight: bold;">File/Folder Path</p> <p>Enter or map the target path to the file or folder.</p> <p style="font-weight: bold;">File/Folder</p> <p>Select the file or folder from the menu.</p> </td> 
  </tr> 
  <tr> 
   <td>Rename </td> 
   <td> <p>Enter the [!UICONTROL target name] for the file, including the file extension.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a File/Folder]

This action module deletes a file or folder.

You specify the file or folder.

The module returns the ID of the  record and any associated fields, along with any custom fields and values that the connection accesses. You can map this information in subsequent modules in the scenario.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Dropbox] account to [!DNL Workfront Fusion], see <a href="#create-a-connection-to-dropbox" class="MCXref xref">Create a connection to [!DNL Dropbox]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Way of selecting files]</td> 
   <td> <p> Select whether you want to map or enter the file path, or select the file manually.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL File Path] / [!UICONTROL File]</p> </td> 
   <td> <p style="font-weight: bold;">[!UICONTROL File Path]</p> <p>Enter or map the target path to the file.</p> <p style="font-weight: bold;">[!UICONTROL File]</p> <p>Select the file from the menu.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Other modules

#### [!UICONTROL Make an API Call]

This action module lets you make a custom authenticated call to the [!DNL Dropbox] API. This way, you can create a data flow automation that can't be accomplished by the other [!DNL Dropbox] modules.

When you are configuring this module, the following fields display.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Dropbox] account to [!DNL Workfront Fusion], see <a href="#create-a-connection-to-dropbox" class="MCXref xref">Create a connection to [!DNL Dropbox]</a> in this article.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>Enter a path relative to Enter a path relative to <code>https://api.dropboxapi.com</code>. For example, <code>/2/files/list_folder</code></p> <p>Note: For the list of available endpoints, see the <a href="https://www.dropbox.com/developers/documentation/http/documentation">Dropbox API v2 Documentation</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Headers] </td> 
   <td> <p>Enter the desired request headers. [!DNL Workfront Fusion] adds authorization headers automatically.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Query String]</td> 
   <td> <p> Enter the request query string.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Body] </td> 
   <td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:   <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Example:** The following API call returns the first 10 files from the [!DNL /Text files] folder in your [!DNL Dropbox] account:
>
>URL: `/2/files/list_folder`
>
>Body:
> 
>`{`
>
>`"path": "/Text files",`
>
>`"limit": 10,`
>
>`"recursive": false,`
>
>`"include_deleted": false`
>
>`}`
>
>Matches of the search can be found in the module's Output under [!UICONTROL Bundle] > [!UICONTROL Body] > entries.
>
>In our example, 10 tickets were returned:

## Common problems

* [Unable to upload or update a file](#unable-to-upload-or-update-a-file)
* [Image referenced via a shared link does not render](#image-referenced-via-a-shared-link-does-not-render)

### Unable to upload or update a file 

There are several situations when uploading or updating a file fails:

* The uploaded file is too big and exceeds the maximum file size allowed for your [!DNL Dropbox] plan, or you have used all of your [!DNL Dropbox] account's storage quota. You must delete existing files from your [!DNL Dropbox] account or upgrade your plan.
* The previously selected folder, to which the file is being uploaded to, no longer exists. The scenario stops and you must select the target folder again.

### Image referenced via a shared link does not render

The URL returned by the [!UICONTROL Dropbox] >[!UICONTROL Create a shared link] does not link directly to an image, but to a [!DNL Dropbox] page. To force the image to download, replace the trailing `?dl=0` with `?dl=1`. To force the image to render (for example, in a Web browser or in Facebook Messenger), append `&raw=1` to the URL.

If you need to get the direct or raw link of your image for your website or for other [!DNL Workfront Fusion] modules, you must modify the initial shared URL in the following way:

Original URL:

`https://www.dropbox.com/s/ia8qtvs20f3a5ux/Screen%20Shot%202018-10-15%20at%204.21.11%20PM.png?dl=0`

1. Replace `www` with `dl`.
1. Remove `?dl=0`.

Final URL:

`https://dl.dropbox.com/s/ia8qtvs20f3a5ux/Screen%20Shot%202018-10-15%20at%204.21.11%20PM.png`

To automatically modify the URL, you can use the `replace()` function twice:

* Replace www with dl

   ![](assets/www-to-dl-350x32.png)

* And to remove ?dl=0

   ![](assets/remove-dl0-350x33.png)

To do it in one step, combine these functions:

![](assets/replace-both-350x47.png)

You can also copy it and paste it into the field. Replace `1.url` with the URL.

```
{{replace(replace(1.url; "?dl=0"; ""); "www"; "dl")}}
```
