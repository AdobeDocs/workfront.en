---
product-area: projects
navigation-topic: manage-issues
title: Move issues
description: You can move issues between projects and tasks.
author: Alina
feature: Work Management
exl-id: 8ab9be3e-0412-43d9-ad1e-75c43613fa82
---
# Move issues

You can move issues between the following objects:

* From a project to another project
* From a task to another task in the same project or in another project
* From a task to the project or to another project
* From a project to a task in the same project or a task in another project

## Access requirements

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
   <td> <p>Request or higher</p> <p>Review or higher license to move issues in the Issues section of a project.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p>View or higher access to Projects and Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to issues in your Access Level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Grant access to issues</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the issue</p> <p>Contribute permissions to the item where you are moving the issue with the ability to Add Issues.</p> <p> For information about granting permissions to issues, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Share an issue </a></p> <p>For information on requesting additional permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Considerations about moving issues

Consider the following when moving issues that contain documents or are associated with a request queue:

* **When an issue is associated with a requests queue:** When you move an issue to another object and the issue is associated with a request queue, the moved issue is no longer associated with the original queue the first issue originated from.
* **When a document is attached to the issue:** When you move an issue to another object and the issue has a document attached to it, the document, its versions and proofs also move to the new issue. Any approvals associated with the document do not move.
* **When an issue is linked to a document or a folder:** When you move an issue which has documents or folders linked to a a third party service like Google Drive, the links to the documents move with the issue. 

## Move issues in a list

You can move one or multiple issues from a list of issues or from an issue report.

1. Go to the project that contains the issue or issues that you want to move.

   Or

   Go to an issue report. 

1. If you selected to go to a project, click **Issues** in the left panel. 
1. Select the issue or issues that you want to move and click the **More menu** at the top of the issue list, then click **Move to**.

   ![](assets/copy-and-move-to-links-for-issue-in-a-list-nwe-350x119.png)

1. Continue with moving the issue, as described in the section [Move a single issue](#move-a-single-issue) starting with Step 2. 

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: ensure step stays accurate)
   </MadCap:conditionalText>
   -->

## Move a single issue {#move-a-single-issue}

You can move one issue when viewing it.

### Move a single issue in the Preview environment

1. Go to an issue that you want to copy, click the **More** menu ![](assets/more-icon.png)to the right of the issue name, then select **Move** to.

   ![](assets/nwe-move-at-issue-level-highlighted-350x579.png)

   The **Move Issue** box displays.

   ![](assets/move-issue-box-nwe-350x280.png)

1. In the **Select Destination Project** section, specify the name of the project where you want to move the issues. The name of the current project displays by default.

   >[!TIP]
   >
   >Only 100 projects display in the list.

1. (Conditional) Click **request access** if you do not have access to move issues to the project. 
1. (Conditional) Continue to move the issue on the selected destination project without requesting access if you have access to add issues to one of the tasks on the destination project.

   ![](assets/move-issue-request-access-from-project-nwe-350x118.png)

   >[!TIP]
   >
   >Similar messages display if the project selected is in pending approval, completed, or dead, when the Workfront administrator prevents adding issues to these projects. For more information, see [Configure system-wide project preferences](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (Optional) In the **Options** section, deselect any of the items listed in the table below to remove them from the moved issue. All options are selected by default.

   >[!IMPORTANT]
   >
   >Deselecting items in the Options list results in loss of data. Information from the existing issue will be removed and cannot be recovered.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Select all</td> 
      <td>Deselect this option to remove all information from the issue when moving it to its new location. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Assignments</td> 
      <td>Removes users, job roles, or teams that are assigned to the issue.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progress</td> 
      <td>Removes the percent complete, if any, of the issue. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>Documents</p></td> 
      <td> <p><span style="line-height: 1.5;">Removes everything in the documents tab, including document versions, linked documents, and folders.</span> <br> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permissions</td> 
      <td>Removes the entities that the issue is shared with. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Updates</td> 
      <td>Removes comments from the Updates section of the issue.</td> 
     </tr> 
    </tbody> 
   </table>


    <!--drafted for dropped documents patch: add this to the Documents cell when it comes to Prev and Prod: 
   <b>NOTE</b>
   If you opt to not have the documents moved with the issue, the documents will be deleted and placed in the Recycle Bin for 30 days. An administrator can restore them and they will be restored on the moved issue. If the issue is deleted after it's moved, the restored documents will be placed in the Documents area of the user page of the administrator who restores them. 
   -->

1. (Optional) In the **Select Task** section, select the task where you want to move the issue. 
1. Click **Move issue** or **Move issues**, if you selected multiple issues in a list.

   The moved issues are added to the specified project.
