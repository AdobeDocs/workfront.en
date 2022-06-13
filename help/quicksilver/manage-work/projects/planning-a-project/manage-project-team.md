---
product-area: projects;agile-and-teams
navigation-topic: plan-a-project
title: Manage the Project Team
description: Manage the Project Team
feature: Work Management
---

# Manage the Project Team

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;remove the NWE way of doing this when the Scheduling tools will be removed from the app)</p>
-->

The Project&nbsp;Team consists of users who are associated with the project. They display  in the People section of the project.

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
   <td role="rowheader">&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>View or higher access to Users</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Add users to a Project Team

When you add users to the project team, they gain permissions on the project and the tasks, issues, and documents of the project. For more information, see the article [Project Team overview](../../../manage-work/projects/planning-a-project/project-team-overview.md).

You can add users to the project team in the following ways:

* [Automatically add users to a Project Team](#automatically-add-users-to-a-project-team) 
* [Manually add users to a Project Team](#manually-add-users-to-a-project-team)

### Automatically add users to a Project Team {#automatically-add-users-to-a-project-team}

The users that fulfill the following roles on the project are automatically added to the project team and appear  in the People section when the project is created:

* The creator of the project
* The project owner
* The project sponsor

Users are also automatically added to the project team when they are assigned to the following roles:

* Users assigned to tasks on the project
* Users assigned to issues on the project

### Manually add users to a Project Team {#manually-add-users-to-a-project-team}

You can manually add users to a project team by using the Team Scheduling tab.

>[!IMPORTANT]
>
>You can add to the Project Team only users that belong to the Group associated with the project.

1. Go to the project where you want to add users to the project team, then click **Scheduling** in the left panel.

   >[!TIP]
   >
   >You might need to click **Show More** to find the Scheduling section, or click Workload Balancer first, and then select **Scheduling** in the upper-right corner of the Workload Balancer.

1. Click **Add Users**.

   The Add Users to Project Team dialog box displays.

   ![add_users_dialog.png](assets/add-users-dialog-350x217.png)

1. In the **Add Users** box, begin typing the name of the user you want to add to the project team, then click the name when it appears in the drop-down list.

   Repeat this step to add multiple users to the project team.

1. Click **Add**.

   The users are now available in the project scheduling area.

For more information about using the project scheduling area, see the article [Get started with Resource Scheduling](../../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md).

## Remove users from a Project Team

When you remove users from their roles on the project, they remain part of the project team.

If you remove a user from the project team and the user is assigned to tasks or issues in the project, the user is unassigned from the tasks, and issues and the tasks and issues are returned to the Unassigned area in the scheduling timeline.

For more information about removing users from the project team, see the article [Remove users from projects](../../../manage-work/projects/manage-projects/remove-users-from-projects.md).
