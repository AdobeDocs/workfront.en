---
filename: share-a-document-folder
product-area: projects
navigation-topic: grant-and-request-access-to-objects
title: Share a document folder
description: The highlighted information on this page refers to functionality available only in the new Workfront experience beta.
---

# Share a document folder

The highlighted information on this page refers to functionality available only in the new Workfront experience beta.

You can share a folder and its contents from the Documents area.

>[!NOTE]
>
>* The folder must be in the >
>  <!-->
>  <MadCap:conditionalText class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">>
>  top five levels>
>  </MadCap:conditionalText>>
>  -->
>  of a folder hierarchy on an object. >
>  <!-->
>  <span class="preview" data-mc-conditions="QuicksilverOrClassic.Draft mode">Each folder at the sixth level or below inherits its sharing configurations from the folder directly above it.</span>>
>  -->
>  For information about adding subfolders to create a folder hierarchy, see the section [Create folders and subfolders](../../documents/organizing-documents/create-documents-folder.md#creating-folders) in the article [Create document folders](../../documents/organizing-documents/create-documents-folder.md).
>
>* Smart folders can't be shared.
>* If you configure sharing options for a document folder within a template, and then someone creates a project from that template, your sharing configurations don't transfer to the document folder in the new project. 
>* If you configure sharing options for a document folder within a work item and then copy the work item, your sharing configurations don't transfer to the document folder in the new work item.
>

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
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
   <td> <p>View access to an object</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Share a folder

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Documents**.

   Or

   With a Workfront object open, click **Documents** in the left panel. 

1. Select the folder, then click the Share icon ![](assets/share-icon.png) in the toolbar.

   The folder 

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   <span class="preview">must be in the top five levels of a folder hierarchy on an object</span>, and
   </MadCap:conditionalText>
   -->

   cannot be a smart folder.

1. In the box that displays, under **Give folder access to**, start typing the name of the user, team, job role, group, or company you want to share the folder with, then press **Enter** when the name displays.
1. To adjust access for the user, team, job role, group, or company you just added, click the drop-down menu to the right of the name, then configure one of the following available options and any of its advanced settings:

   <table cellspacing="0"> 
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

## How your recipients access the contents of a folder you share with them

Currently, when you share a folder, your recipients do not see the folder in their Documents area. However, they can access its documents by running a document report.

## How inherited permissions work when you share a parent object containing a folder

When you share the parent object where a document folder resides, your recipients also get access to the folder:

* If you grant your recipients View access to the parent object, they have View access to the folder.
* If you grant your recipients Contribute or Manage access to the parent object, they have Manage access to the folder.
* If you grant one type of access (View, Contribute, or Manage) to the parent object, and another type to the folder, your recipients have the highest of those two types of access to documents within the folder

  For example, if you share the parent object with View access, and the folder with Manage access, your recipients have Manage to the documents in the folder.

  >[!NOTE]
  >
  >An attached document inherits permissions only from the object where it was attached. If you create a folder on the object and move the document into the folder, it inherits the folder's permissions. But, if you create a folder on a parent or grandparent object and move the document into that folder, it does not inherit that folder's permissions.

