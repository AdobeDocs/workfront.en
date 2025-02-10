---
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Share a document folder
description: You can share a folder and its contents from the Documents area.
author: Alina
feature: Get Started with Workfront
exl-id: c0d318a8-b1cf-4522-b478-acf092687658
---
# Share a document folder

You can share a folder and its contents from the Documents area.

>[!NOTE]
>
>* The folder must be in the top five levels of a folder hierarchy on an object. Each folder at the sixth level or below inherits its sharing configurations from the folder directly above it. 
>
>  For information about adding subfolders to create a folder hierarchy, see the section [Create folders and subfolders](../../documents/organizing-documents/create-documents-folder.md#creating-folders) in the article [Create document folders](../../documents/organizing-documents/create-documents-folder.md).
>
>* Smart folders can't be shared.
>* If you configure sharing options for a document folder within a template, and then someone creates a project from that template, your sharing configurations don't transfer to the document folder in the new project. 
>* If you configure sharing options for a document folder within a work item and then copy the work item, your sharing configurations don't transfer to the document folder in the new work item.
>

## Access requirements

<!--drafted for P&P
(I am putting Contributor and higher here because this is what I found in testing. Normally, Review equals Light but I found out that Contributor can also have manage rights to documents and can share them.)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Contributor or higher</p> 
   Or
   <p>Legacy license: Review or higher</p>
      </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access to Documents</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View access to an object</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View access to Documents</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View access to an object</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Share a folder

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Documents**.

   Or

   With a Workfront object open, click **Documents** in the left panel. 

1. Select the folder, then click the Share icon ![](assets/share-icon.png) in the toolbar.

   The folder must be in the top five levels of a folder hierarchy on an object, and cannot be a smart folder.

1. In the box that displays, under **Give folder access to**, start typing the name of the user, team, job role, group, or company you want to share the folder with, then press **Enter** when the name displays.
1. To adjust access for the user, team, job role, group, or company you just added, click the drop-down menu to the right of the name, then configure one of the following available options and any of its advanced settings:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">View it</td> 
      <td> <p>Ability to view the folder and its contents.</p> <p>Click <strong>Advanced Settings</strong> to specify whether you want to allow the following:</p> 
       <ul> 
        <li><strong>Download</strong>: Ability to download the folder and its contents as a ZIP file</li> 
        <li> <p><strong>Share</strong>: Ability to share the folder with others in the system</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Manage it</td> 
      <td> <p>Ability to view and edit the folder and its contents</p> <p>Click <strong>Advanced Settings</strong> to specify whether you want to allow users to do the following:</p> 
       <ul> 
        <li><strong>Delete</strong>: Delete the folder and its contents from the system</li> 
        <li><b>Download</b>: Download the folder and its contents as a ZIP file</li> 
        <li><strong>Share</strong>: Share the folder and its contents with other users in the system</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Repeat Steps 3-4 to add other names to the list and configure their options.
1. (Optional) If you want everyone in the system to be able to view the folder and its contents, click the gear icon ![](assets/gear-icon-settings-with-dn-arrow.jpg) in the upper right corner of the sharing box, then click **Make this visible system-wide.**

   If you change your mind, you can, click **Remove system-wide access** (the default option).

## How users access the contents of a folder shared with them

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Delete these 2 paragraphs when the story &nbsp;<a href="https://hub.workfront.com/task/622f8d6f000897c9a4a11bdfd9b2cf34/overview">Handle email notification content when a folder is shared</a> goes to Preview:</p>
-->

Currently, when you share a folder, your recipients don't see the folder in their Documents area. However, they can access its documents by running a document report.

For information about running a report, see the section [Report on objects](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects) in the article [Understand objects in Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md). Also see [Create a custom report](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

<!--
<div class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>Workfront sends a notification email when someone shares a document folder on an object with a user or a team. To access the folder from the email, recipients can click the folder title or the "See it in Workfront" link.</p> <note type="note">
<ul class="preview">
<li> <p>The email notification "Someone shares an object with me" or "Someone shares an object with my team" must be enabled in order for a user or team to receive a notification email about a shared folder.</p> </li>
<li> <p>When someone shares a document folder from the global Documents area, the links in the notification email take the recipient to the global Documents area. Because folders in this area are private, the shared folder is not displayed there, but the recipient can access its documents by creating a document report. </p> <p>For information about running a report, see the section <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#reporting-on-objects" class="MCXref xref">Report on objects</a> in the article <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>. Also see <a href="../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.</p> </li>
<li> <p>Currently, it is not possible to share folders with external users.</p> </li>
</ul>
</note>
</div>
-->

## Inherited permissions when you share an object containing a folder

When you share an object that has a document folder, your recipients also get access to the folder:

* If you grant your recipients View access to the parent object, they have View access to the folder.
* If you grant your recipients Contribute or Manage access to the parent object, they have Manage access to the folder.
* If you grant one type of access (View, Contribute, or Manage) to the parent object, and another type to the folder, your recipients have the highest of those two types of access to documents within the folder

  For example, if you share the parent object with View access, and the folder with Manage access, your recipients have Manage to the documents in the folder.

  >[!NOTE]
  >
  >An attached document inherits permissions only from the object where it was attached. If you create a folder on the object and move the document into the folder, it inherits the folder's permissions. But, if you create a folder on a parent or grandparent object and move the document into that folder, it does not inherit that folder's permissions.

* If the option "Never inherit document access from projects, tasks, issues, etc" is enabled in the recipient's access level, they will not inherit permissions to documents in a folder that you share with them. To give them access to a document in the folder, you must share the document.

  For information about the "Never inherit" option, see [Configure access to Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md).

  For information about sharing a document, see [Share a document](../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).
