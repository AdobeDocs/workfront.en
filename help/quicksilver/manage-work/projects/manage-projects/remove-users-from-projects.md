---
product-area: projects;user-management
navigation-topic: manage-projects
title: Remove users from projects
description: You can remove users from a project when they are no longer involved in completing work on the project. 
author: Alina
feature: Work Management
exl-id: 3a75c78d-faed-41cd-a0a4-59504bb981af
---
# Remove users from projects

You can remove users from a project when they are no longer involved in completing work on the project. Removing users from projects has implications on task and issue assignments, as well as on project roles. Removed users stop receiving notifications intended for the Project Team. For more information about notifications for the project teams, see [Event notification types](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

The users associated with a project are listed in the People area of a project. They represent the Project Team. For more information about the Project Team, see [Project Team overview](../../../manage-work/projects/planning-a-project/project-team-overview.md).

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*To find out what plan, license type, or access you have, contact your Workfront administrator.

## How removing a user affects existing tasks, issues, and projects

When a user is removed from a project, any tasks or issues assigned to them might be affected, depending on whether the task or issue was completed when the user was removed:

* **If the item is not completed when the user is removed:** The item is re-assigned to a job role if a job role was already assigned, or it is assigned to the job role the user was fulfilling on the item. If the item or the user did not have a job role assigned, you must manually re-assign the item. 
* **If the item is completed when the user is removed:** The name of the removed user remains on the item.
* **If the user removed is also the creator of a project:** The project is not removed from their **Projects I'm On** list in the Projects area. The project is removed from the lists for all other users that filter for that project by the Entered By field.
* **If the user is the project Owner or Sponsor:** The user remains in their roles as sponsor or owner of the project. 

## Remove users from a project and Project Team

You can remove users from a project by removing them from the Project Team. 

When users fulfill roles on a project, they become part of the Project Team. 

When you remove users from their roles on the project, they remain part of the project team. 

For information about users' roles on a project, see [Manage the Project Team](../planning-a-project/manage-project-team.md). 

To remove users from the Project Team: 

1. Go to the project where you want to remove the users.

1. Click **People** in the left panel, then select the users you want to remove. You might need to click **Show More**, then **People**.   

1. Click the **Remove** icon  ![Remove item](assets/remove-icon---x-in-circle.png) at the top of the list of users.

1. Click **Yes, Remove Selected Users** to confirm removal.

    The users are removed from the project team and from any incomplete tasks or issues that they might be assigned to. They no longer receive notifications intended for the Project Team. 
