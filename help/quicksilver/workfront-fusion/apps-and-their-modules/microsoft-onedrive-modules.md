---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: connector
navigation-topic: apps-and-their-modules
title: Microsoft OneDrive modules
description: In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use OneDrive, as well as connect it to multiple third-party applications and services.
author: Becky
feature: Workfront Fusion
exl-id: 13a25c6c-bdf1-467d-bd90-ebd763c59235
---
# [!DNL Microsoft OneDrive] modules

In an [!DNL Adobe Workfront Fusion] scenario, you can automate workflows that use [!DNL OneDrive], as well as connect it to multiple third-party applications and services.

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

To use [!DNL OneDrive] modules, you must have a [!DNL Microsoft OneDrive] account.




## Connecting the [!DNL OneDrive] service to [!DNL Workfront Fusion]

For instructions about connecting your [!DNL OneDrive] account to [!UICONTROL Workfront Fusion], see [Create a connection to [!UICONTROL Adobe Workfront Fusion] - Basic instructions](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Some Microsoft apps use the same connection, which is tied to individual user permissions. Therefore, when creating a connection, the permissions consent screen displays any permissions that were previously granted to this user's connection, in addition to any new permissions needed for the current application. 
>
>For example, if a user has "Read table" permissions granted via the Excel connector and then creates a connection in the Outlook connector to read emails, the permissions consent screen will show both the already granted "Read table" permission and the newly required "Write email" permission.

## [!DNL Microsoft OneDrive] modules and their fields

When you configure [!DNL OneDrive] modules, [!DNL Workfront Fusion] displays the fields listed below. Along with these, additional [!DNL OneDrive] fields might display, depending on factors such as your access level in the app or service. A bolded title in a module indicates a required field.

If you see the map button above a field or function, you can use it to set variables and functions for that field. For more information, see [Map information from one module to another in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [File/Folder](#filefolder)
* [Other](#other)

### File/Folder

* [[!UICONTROL Watch Files/Folders]](#watch-filesfolders)
* [[!UICONTROL Search Files/Folders]](#search-filesfolders)
* [[!UICONTROL Get a file]](#get-a-file)
* [[!UICONTROL Download a file]](#download-a-file)
* [[!UICONTROL Upload a file]](#upload-a-file)
* [[!UICONTROL Create a Folder]](#create-a-folder)
* [[!UICONTROL Get a Share Link]](#get-a-share-link)
* [[!UICONTROL Move a File/Folder]](#move-a-filefolder)
* [[!UICONTROL Copy a File]](#copy-a-file)
* [[!UICONTROL Delete a File/Folder]](#delete-a-filefolder)

#### [!UICONTROL Watch Files/Folders]

This trigger module starts a scenario when a file or folder is created or updated.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions about connecting your [!DNL OneDrive] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watch Files/Folders]</td> 
   <td> <p>Select how you want to watch files or folders:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL By Created Time]</b> </p> <p>Watch for new files or folders.</p> </li> 
     <li> <p><b>[!UICONTROL By Updated Time]</b> </p> <p>Watch for updated existing files or folders.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose your [!DNL OneDrive] location]</td> 
   <td> <p>Select the location you want to watch:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Select whether to enable the module to enter a drive ID.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>Enter the ID of the drive that you want the module to watch.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> <p>Navigate to the folder that you want the module to watch. You can also enter a query to filter the returned results.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Shared With Me]</b> </p> <p>The module watches files that have been shared with the owner of the drive.</p> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Select the SharePoint Site that you want the module to watch. Available Sites are Sites followed by the signed-in user.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Select the group whose drive you want the module to watch.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose an Item Type]</td> 
   <td> <p>Select whether you want to watch files, folders, or both.</p> <p>Note: You cannot watch for folders in a [!UICONTROL Shared With Me] drive.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

 

#### [!UICONTROL Search Files/Folders]

This search module returns files and folders based on criteria you set.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions about connecting your [!DNL OneDrive] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose your [!DNL OneDrive] location]</td> 
   <td> <p>Select the location you want to search:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Select whether to enable the module to enter a drive ID.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>Enter the ID of the drive that you want the module to search.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> <p>Navigate to the folder that you want the module to search. You can also enter a query to filter the returned results.</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Shared With Me]</b> </p> <p>The module searches files that have been shared with the owner of the drive.</p> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Select the [!DNL SharePoint] Site that you want the module to search. Available Sites are Sites followed by the signed-in user.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Select the group whose drive you want the module to search.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose an Item Type]</td> 
   <td> <p>Select whether you want to search for files, folders, or both.</p> <p>Note: You cannot search for folders in a [!UICONTROL Shared With Me] drive.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get a file]

This action module gets the metadata of a specified file.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions about connecting your [!DNL OneDrive] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter (File ID &amp; File Path)]</td> 
   <td>Select whether you want to identify the file by File ID or by the File Path.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a File ID] / [!UICONTROL File Path]</td> 
   <td> <p>Select how you want to enter the File ID or File Path:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Enter Manually]</b> </p> <p>Select this option if you want to enter the ID or path directly, or map it from a previous module.</p> </li> 
     <li> <p><b>[!UICONTROL Select from a list]</b> </p> <p>Select this option if you want to select from a list of available files or paths. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose your [!DNL OneDrive] location]</td> 
   <td> <p>Select the location you want to search:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Select whether to enable the module to enter a drive ID.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>Enter the ID of the drive that contains the file you want to get.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Select the SharePoint Site that contains the file you want to get. Available Sites are Sites followed by the signed-in user.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Select the group whose drive contains the file you want to get.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Select or map the drive that contains the file you want to get. This field is not available if you selected [!UICONTROL No] in the [!UICONTROL Enable to Enter a Drive ID] field.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</td> 
   <td> <p>If you selected [!UICONTROL Enter Manually], enter or map the file ID or path of the file you want to get.</p> <p>If you selected [!UICONTROL Select from the list], select the file that you want to get.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Download a file]

This action module downloads the specified file.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions about connecting your [!DNL OneDrive] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter (File ID &amp; File Path)]</td> 
   <td>Select whether you want to identify the file by File ID or by the File Path.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Enter a File ID / File Path</td> 
   <td> <p>Select how you want to enter the File ID or File Path:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Enter Manually]</b> </p> <p>Select this option if you want to enter the ID or path directly, or map it from a previous module.</p> </li> 
     <li> <p><b>[!UICONTROL Select from a list]</b> </p> <p>Select this option if you want to select from a list of available files or paths. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose your [!DNL OneDrive] location]</td> 
   <td> <p>Select the location you want to that contains the file you want to download:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Select whether to enable the module to enter a drive ID.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>Enter the ID of the drive that contains the file you want to download.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Select the SharePoint Site that contains the file you want to download. Available Sites are Sites followed by the signed-in user.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Select the group whose drive contains the file you want to download.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Select or map the drive that contains the file you want to download. This field is not available if you selected [!UICONTROL No] in the [!UICONTROL Enable to Enter a Drive ID] field.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</td>
   <td> <p>If you selected [!UICONTROL Enter Manually], enter or map the file ID or path of the file you want to download.</p> <p>If you selected [!UICONTROL Select from the list], select the file that you want to download.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Convert to PDF]</td> 
   <td> <p>Enable this option to convert the file to a PDF file. You can convert from the following file types:</p> 
    <table style="table-layout:auto"> 
     <col> 
     <col> 
     <col> 
     <tbody> 
      <tr> 
       <td> 
        <ul> 
         <li> <p> <p>CSV</p> </p> </li> 
         <li> <p> <p>DOC</p> </p> </li> 
         <li> <p> <p>DOCX</p> </p> </li> 
         <li> <p> <p>ODP</p> </p> </li> 
         <li> <p> <p>ODS</p> </p> </li> 
         <li> <p> <p>ODT</p> </p> </li> 
        </ul> </td> 
       <td> 
        <ul> 
         <li> <p> <p>POT</p> </p> </li> 
         <li> <p> <p>POTM</p> </p> </li> 
         <li> <p> <p>POTX</p> </p> </li> 
         <li> <p> <p>PPS</p> </p> </li> 
         <li> <p> <p>PPSX</p> </p> </li> 
         <li> <p> <p>PPSXM</p> </p> </li> 
        </ul> </td> 
       <td> 
        <ul> 
         <li> <p>PPT</p> </li> 
         <li> <p>PPTM</p> </li> 
         <li> <p>PPTX</p> </li> 
         <li> <p>RTF</p> </li> 
         <li> <p>XLS</p> </li> 
         <li> <p>XLSX</p> </li> 
        </ul> </td> 
      </tr> 
     </tbody> 
    </table> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Upload a file]

This action module uploads a file to the specified folder.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions about connecting your [!DNL OneDrive] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Enter (Folder Location ID &amp; Path)</td> 
   <td>Select whether you want to identify the target folder by ID or by a path.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose your [!DNL OneDrive] location]</td> 
   <td> <p>Select the location where you want to upload a file:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Select whether to enable the module to enter a drive ID.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>Select the drive that contains the file you want to get.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Select the [!DNL SharePoint] Site that contains the folder where you want to upload a file. Available Sites are Sites followed by the signed-in user.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Select the group whose drive contains the folder where you want to upload a file.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Select the drive that contains the folder where you want to upload a file. This field is not available if you selected [!UICONTROL No] in the [!UICONTROL Enable to Enter a Drive ID] field.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>Select a source file from a previous module, or map the source file's name and data.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL If the File with the Same Name Exists]</td> 
   <td>Select how to proceed if a file with the same name already exists.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td>Add a description to the uploaded file.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create a Folder]

This action module creates a new folder in the specified drive.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions about connecting your [!DNL OneDrive] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose your [!DNL OneDrive] location]</td> 
   <td> <p>Select the location where you want to create a folder:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Select whether to enable the module to enter a drive ID.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>Select the drive where you want to create a folder.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Select the [!DNL SharePoint] Site where you want to create a folder. Available Sites are Sites followed by the signed-in user.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Select the group that owns the drivewhere you want to create a folder.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Select the drive that where you want to create a folder. This field is not available if you selected [!UICONTROL No] in the [!UICONTROL Enable to Enter a Drive ID] field.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>If you want the new folder to be a subfolder, navigate to the folder that you want it to be a subfolder in.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL New Folder Name]</td> 
   <td> <p>Enter or map a name for the new folder.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL If the Folder with the Same Name Exists]</td> 
   <td>Select how to proceed if a file with the same name already exists.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get a Share Link]

This action module returns a share link for the specified file.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions about connecting your [!DNL OneDrive] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter (File ID &amp; File Path)]</td> 
   <td>Select whether you want to identify the file by File ID or by the File Path.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a File ID] / [!UICONTROL File Path]</td> 
   <td> <p>Select how you want to enter the File ID or File Path:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Enter Manually]</b> </p> <p>Select this option if you want to enter the ID or path directly, or map it from a previous module.</p> </li> 
     <li> <p><b>[!UICONTROL Select from a list]</b> </p> <p>Select this option if you want to select from a list of available files or paths. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose your [!DNL OneDrive] location]</td> 
   <td> <p>Select the location you want to retrieve a share link for:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Select whether to enable the module to enter a drive ID.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>Enter the ID of the drive that contains the file you want to retrieve a share link for.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Select the SharePoint Site that contains the file you want to retrieve a share link for. Available Sites are Sites followed by the signed-in user.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Select the group whose drive contains the file you want to retrieve a share link for.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Select or map the drive that contains the file you want to retrieve a share link for. This field is not available if you selected [!UICONTROL No] in the [!UICONTROL Enable to Enter a Drive ID] field.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</td> 
   <td> <p>If you selected [!UICONTROL Enter Manually], enter or map the file ID or path of the file you want to retrieve a share link for.</p> <p>If you selected [!UICONTROL Select] from the list, select the file that you want to retrieve a share link for.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Permission Type]</td> 
   <td> <p>Select whether you want people with the link to be able to read and write to the file, or to read only.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scope]</td> 
   <td>Select whether you want the file to be available to anyone with the link, or only to members of your organization who have the link.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Move a File/Folder]

This action module moves a file or folder to a new folder location

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions about connecting your [!DNL OneDrive] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter (File ID &amp; File Path)]</td> 
   <td>Select whether you want to identify the file by File ID or by the File Path.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a File ID / File Path]</td> 
   <td> <p>Select how you want to enter the File ID or File Path:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Enter Manually]</b> </p> <p>Select this option if you want to enter the ID or path directly, or map it from a previous module.</p> </li> 
     <li> <p><b>[!UICONTROL Select from a list]</b> </p> <p>Select this option if you want to select from a list of available files or paths. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose your [!DNL OneDrive] location]</td> 
   <td> <p>Select the location that contains the file or folder that you want to move:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Select whether to enable the module to enter a drive ID.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>Enter the ID of the drive that contains the file or folder that you want to move.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Select the [!DNL SharePoint] Site that contains the file or folder that you want to move. Available Sites are Sites followed by the signed-in user.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Select the group whose drive contains the file or folder that you want to move.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Select or map the drive that contains the file or folder that you want to move. This field is not available if you selected [!UICONTROL No] in the [!UICONTROL Enable to Enter a Drive ID] field.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Select [!UICONTROL File/Folder]</td> 
   <td>Select whether you want to move a file or a folder.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</p> <p role="rowheader">[!UICONTROL Folder] / [!UICONTROL Folder ID] / [!UICONTROL Folder Path]</p> </td> 
   <td> <p>If you selected [!UICONTROL Enter Manually], enter or map the ID or path of the file or folder that you want to move.</p> <p>If you selected [!UICONTROL Select] from the list, select the file or folder that you want to move.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a New Folder Location]</td> 
   <td> <p>Select how you want to enter the location that you want to move the file or folder to:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Enter Manually]</b> </p> <p>Select this option if you want to enter the ID or path directly, or map it from a previous module.</p> </li> 
     <li> <p><b>[!UICONTROL Select from a list]</b> </p> <p>Select this option if you want to select from a list of available files or paths. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose your [!DNL OneDrive] location]</td> 
   <td> <p>Select the location where you want to move the file or folder:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Select whether to enable the module to enter a drive ID.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>Enter the ID of the drive where you want to move the file or folder.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Select the [!DNL SharePoint] Site where you want to move the file or folder. Available Sites are Sites followed by the signed-in user.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Select the group to whose drive you want to move the file or folder.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Select or map the drive that contains the folder that you want to move the file or folder to. This field is not available if you selected [!UICONTROL No] in the [!UICONTROL Enable to Enter a Drive ID] field.</p> <p>If you leave this blank, the file or folder can only be moved within the same [!DNL OneDrive].</p> <p>You can move files and folders from [!UICONTROL My Drive] to a [!UICONTROL Site's Drive] or a [!UICONTROL Group's Drive]. </p> <p>You can move files from a [!UICONTROL Site's Drive] only to the same drive in the same Site.</p> <p>You can move files from a [!UICONTROL Group's Drive] only to the same drive in the same Group.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>Enter or map the folder where you want to move the file or folder.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Copy a File]

This action module copies a file into a new folder location

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions about connecting your [!DNL OneDrive] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter (File ID &amp; File Path)]</td> 
   <td>Select whether you want to identify the file by File ID or by the File Path.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a File ID] / [!UICONTROL File Path]</td> 
   <td> <p>Select how you want to enter the File ID or File Path:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Enter Manually]</b> </p> <p>Select this option if you want to enter the ID or path directly, or map it from a previous module.</p> </li> 
     <li> <p><b>[!UICONTROL Select from a list]</b> </p> <p>Select this option if you want to select from a list of available files or paths. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose your [!DNL OneDrive] location]</td> 
   <td> <p>Select the location that contains the file that you want to copy:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Select whether to enable the module to enter a drive ID.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>Enter the ID of the drive that contains the file or folder that you want to copy.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Select the SharePoint Site that contains the file that you want to move. Available Sites are Sites followed by the signed-in user.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Select the group whose drive contains the file that you want to copy.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Select or map the drive that contains the file that you want to copy. This field is not available if you selected [!UICONTROL No] in the [!UICONTROL Enable to Enter a Drive ID] field.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</p> </td> 
   <td> <p>If you selected [!UICONTROL Enter Manually], enter or map the ID or path of the file that you want to copy.</p> <p>If you selected [!UICONTROL Select] from the list, select the file that you want to copy.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a New Folder Location]</td> 
   <td> <p>Select how you want to enter the location that you want to copy the file or to:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Enter Manually]</b> </p> <p>Select this option if you want to enter the ID or path directly, or map it from a previous module.</p> </li> 
     <li> <p><b>[!UICONTROL Select from a list]</b> </p> <p>Select this option if you want to select from a list of available folder. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL New OneDrive location]</td> 
   <td> <p>Select the location where you want to copy the filer. This option is available if you chose to select the new folder location from a list.</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Select whether to enable the module to enter a drive ID.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>Enter the ID of the drive where you want to copy the file.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Select the [!DNL SharePoint] Site where you want to copy the file. Available Sites are Sites followed by the signed-in user.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Select the group to whose drive you want to copy the file.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Select or map the drive that contains the folder that you want to copy the file to. This field is not available if you selected [!UICONTROL No] in the [!UICONTROL Enable to Enter a Drive ID] field.</p> <p>If you leave this blank, the file or folder can only be copied within the same [!UICONTROL OneDrive].</p> <p>You can copy files and folders from [!UICONTROL My Drive] to a [!UICONTROL Site's Drive] or a [!UICONTROL Group's Drive]. </p> <p>You can copy files from a [!UICONTROL Site's Drive] only to the same drive in the same Site.</p> <p>You can copy files from a [!UICONTROL Group's Drive] only to the same drive in the same Group.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>Enter or map the folder where you want to move the copy or folder.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL New Copied File Name]</td> 
   <td> <p>Enter or map a name for the new copy of the file. You can leave this blank if you do not want to change the original file name.</p> <p>The name must include the file extension. Example:<code> file.txt</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a File/Folder]

This action module deletes the selected file.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions about connecting your [!DNL OneDrive] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter (File/Folder ID &amp; Path)]</td> 
   <td>Select whether you want to identify the file by File ID or by the File Path.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a File/Folder ID /Enter a File/Folder Path]</td> 
   <td> <p>Select how you want to enter the File ID or File Path:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL Enter Manually]</b> </p> <p>Select this option if you want to enter the ID or path directly, or map it from a previous module.</p> </li> 
     <li> <p><b>[!UICONTROL Select from a list]</b> </p> <p>Select this option if you want to select from a list of available files or paths. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Choose your [!DNL OneDrive] location]</td> 
   <td> <p>Select the location you want to search:</p> 
    <ul> 
     <li> <p><b>[!UICONTROL My Drive]</b> </p> <p>Select whether to enable the module to enter a drive ID.</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Yes]</b> </p> <p>Enter the ID of the drive that contains the file or folder you want to delete.</p> </li> 
       <li> <p><b>[!UICONTROL No]</b> </p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL Site's Drive]</b> </p> <p>Select the [!DNL SharePoint] Site that contains the file or folder you want to delete. Available Sites are Sites followed by the signed-in user.</p> </li> 
     <li> <p><b>[!UICONTROL Group's Drive]</b> </p> <p>Select the group whose drive contains the file or folder you want to delete.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Drive ID]</td> 
   <td> <p>Select or map the drive that contains the file or folder you want to delete. This field is not available if you selected [!UICONTROL No] in the [!UICONTROL Enable to Enter a Drive ID] field.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Select [!UICONTROL File/Folder]</td> 
   <td>Select whether you want to delete a file or a folder.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File] / [!UICONTROL File ID] / [!UICONTROL File Path]</td>
   <td> <p>If you selected [!UICONTROL Enter Manually], enter or map the file ID or path of the file you want to delete.</p> <p>If you selected [!UICONTROL Select] from the list, select the file that you want to delete.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Other

#### [!UICONTROL Make an API Call]

This module performs a custom API call.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>For instructions about connecting your [!DNL OneDrive] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Enter a path relative to <code>https://graph.microsoft.com</code>. Example:<code> /v1.0/me/drive/root/children</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   td> <p>Select the HTTP request method you need to configure the API call. For more information, see <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP request methods in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Add the headers of the request in the form of a standard JSON object.</p> <p>For example, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion adds the authorization headers for you.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Add the query for the API call in the form of a standard JSON object.</p> <p>For example: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Add the body content for the API call in the form of a standard JSON object.</p> <p>Note:  <p>When using conditional statements such as <code>if</code> in your JSON, put the quotation marks outside of the conditional statement.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

 

## If you are unable to upload or update a file

There are several possible issues when uploading or updating a file fails:

* The uploaded file is too big and exceeds the maximum file size limit for your [!DNL OneDrive] plan or you have used all of your [!DNL OneDrive] account's storage quota. To get more storage space, delete existing files from [!DNL OneDrive] or upgrade your [!DNL OneDrive] account.
* OneDrive does not allow to upload two files with the same name to one single folder. If the target folder contains a file with the same name as the file being uploaded, the scenario run terminates with an error. The solution is to simply rename the file being uploaded. If your aim is to update a file, use the [!UICONTROL Update a file] action.
* The previously selected folder, to which the file is being uploaded, no longer exists. The scenario stops and you will need to select the target folder again.
