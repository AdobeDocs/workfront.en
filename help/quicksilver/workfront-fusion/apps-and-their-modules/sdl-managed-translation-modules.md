---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: connector
navigation-topic: apps-and-their-modules
title: SDL Managed Translation modules
description: In an [!DNL Adobe Workfront Fusion] scenario, you can connect your SDL Managed Translation account to multiple third-party applications and services.
author: Becky
feature: Workfront Fusion
exl-id: e1ef114f-8ce4-4210-b176-727dc4f5e561
---
# [!DNL SDL Managed Translation] modules

In an [!DNL Adobe Workfront Fusion] scenario, you can connect your [!DNL SDL Managed Translation] account to multiple third-party applications and services.

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

## SDL Managed Translation API information

The SDL Managed Translation connector uses the following:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Base URL</td> 
   <td>https://languagecloud.sdl.com</td> 
  </tr>
  <tr> 
   <td role="rowheader">API tag</td> 
   <td>v1.4.26</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL SDL Managed Translation] Modules

>[!NOTE]
>
>The operation timeout for calls to [!DNL SDL Managed Translation] is **120 seconds**.

### Files

#### [!UICONTROL Download Translated File]

This module retrieves the content of a single translated file, contained within the specified project. If the requested file is not yet in Downland status, the content of the file may not yet be fully translated. If the file is in Download status, and you have successfully retrieved it, be sure to mark the file as complete using the `Cancel or Complete File` method.

#### [!UICONTROL Upload a File]

This module allows uploads of files for translation or for inclusion in a translation project as reference material. Uploads must be submitted using multipart/form-data and can contain more than one file. You specify the `ProjectOptionId` that should be used to evaluate the uploaded file(s). This determines whether each file you upload is a possible candidate for translation or must be handled as reference material. In the case of archives (`zip `, `rar`, `7z`, `tar` files) the app examines the contents of the archive and indicates whether the archive as a whole can be translated, or whether it contains a mixture of translatable and non-translatable files.

>[!NOTE]
>
>Uploading more than one file at a time is not recommended, because it can increase the impact of any failure.

#### [!UICONTROL Add a Reference File]

This module adds a Reference File.

### Projects

#### [!UICONTROL Create a project]

This module creates the specified project.

#### Cancel or Complete a Project

This module cancels or completes the specified project. If the project is awaiting download, the project transitions through any final steps in the workflow, and eventually moves to complete. If the project is awaiting approval or vendor selection is cancelled. If the project is at any other status, the request will fail.

#### [!UICONTROL Download Project Zip]

This module gets the `zip` file of translated files for the specified project.

#### [!UICONTROL Read a Project]

This module gets the specified project.

#### [!UICONTROL Get Projects at Status]

This module gets all available projects in the specified status. This method allows the results to be paged, by specifying `$top`, `$skip`, and `$orderby` query parameters.

#### [!UICONTROL Get Projects List]

Gets a simple list of all projects, providing general information about each project. This method allows the results to be pages, by specifying `$top`, `$skip`, and `$orderby` query parameters.

#### [!UICONTROL Search Project Creation Options]

This module gets Project Creation Options.

### Other

#### [!UICONTROL Make an API Call]

This module performs an arbitrary authorized API call.
