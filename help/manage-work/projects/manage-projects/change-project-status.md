---
filename: change-project-status
product-area: projects
navigation-topic: manage-projects
title: Change the status of a project
description: You can manually change the status of a project.
---

# Change the status of a project

You can manually change the status of a project.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Considerations about updating to specific statuses

* `When updating a project to Complete:` Ensure that all tasks and issues are completed on the project. You cannot select the Complete status for a project, or any other status that equates Complete when there are tasks or issues that have not been completed on the project. This includes approving any task or issue that is in a Complete-Pending Approval status.
* `When updating a project from Complete to Current:` If all the tasks and issues on the project are completed, ensure that the project's Completion Mode is set to Manual. If the project's Completion&nbsp;Mode is Automatic, the status of the project remains Complete.

## Change project status

1. Go to the project whose status you want to update.
1. In the project header, click the name of the status in the `Status` field, then select a new status.

   Or

   Click the More menu next to the name of the project and click Edit and select a new status in the `Status` field, then click `Save`.

   The project status updates to the status you selected.

