---
product-area: projects;user-management
navigation-topic: manage-projects
title: Remove users from projects
description: Remove users from projects
author: Alina
feature: Work Management
exl-id: 3a75c78d-faed-41cd-a0a4-59504bb981af
---
# Remove users from projects

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This also links here - some information is duplicated between these 2 articles, so update both:&nbsp;https://support.workfront.com/hc/en-us/articles/217301267-Understanding-the-Project-Team-and-Projects-I-m-On-) </p>
-->

You can remove users from a project when they are no longer involved in completing work on the project. Removing users from projects has implications on task and issue assignments, as well as on project roles.

The users associated with a project are listed in the People area of a project. They represent the Project Team.&nbsp;For more information about the Project Team, see [Project Team overview](../../../manage-work/projects/planning-a-project/project-team-overview.md).

You can assign work to the users on the project in the People area of a project.

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
   <td> <p>Edit access to Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## How removing a user affects existing tasks, issues, and projects&nbsp;

When a user is removed from a project, any tasks or issues assigned to them might be affected, depending on whether the task or issue was in an Active or Complete state when the user was removed:

* **If the item is in an Active state when the user is removed:** The item is re-assigned to a Job Role if a Job Role was already assigned. If the item&nbsp;did not have a Job Role assigned, you must manually re-assign the item. An item in an Active state is any item that has not completed yet.
* **If the item is in a Complete state when the user is removed:** The name of the removed user remains on&nbsp;the item.
* If the user removed is also the creator of a project, the project is not removed from their **Projects I'm On** list in the Projects area. The project is removed from the lists for all other users that filter for that project by the Entered By field.

## Remove users from a project and Project Team

When you remove a user from the project, the user is also removed from the project team. Likewise, when you remove a user from the project team, the user is also removed from the project.

You can remove users from a project from the People sectionof the project.

* [Remove users from a project from the People area](#remove-users-from-a-project-from-the-people-area)

### Remove users from a project from the People area {#remove-users-from-a-project-from-the-people-area}

1. Go to the project where you want to remove the users.
1. Click **People** in the left panel,&nbsp;then select the users you want to remove. This might be located under the **Show More** area.   

1. Click the **Remove** icon  ![Remove item](assets/remove-icon---x-in-circle.png) at the top of the list of users.

1. Click&nbsp;**Yes, Remove Selected Users** to confirm removal.
