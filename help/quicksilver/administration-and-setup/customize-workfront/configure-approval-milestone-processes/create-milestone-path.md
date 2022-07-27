---
title: Create a milestone path
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Create a milestone path
author: Alina, Caroline
feature: System Setup and Administration
role: Admin
exl-id: c1e2f374-576c-4f1c-b502-281e8ee9e7df
---
# Create a milestone path

<!--
NOTE: DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

As an Adobe Workfront administrator, you can create milestone paths which can then be applied to any project in the system. The changes you make to milestone paths in this area affect the entire Workfront system.

## Access requirements

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator.</p> <p><b>NOTE</b>: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Milestones and milestone paths

You can associate the key tasks in a project with predefined milestones. This function can provide managers and other stakeholders with a high-level overview as to how a project is progressing.

The sum of all the predefined milestones is called a milestone path. 

The first step in building a milestone path is identifying what the milestone steps are and establishing the milestones. Because you can associate a milestone path to multiple projects, the milestone steps must be general phases or stages of any project.

For more information on how you can associate a milestone path with a project and a milestone with a task, see [Associate milestones with tasks](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

## Create a milestone path

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. Click **Processes** > **Milestone Paths**.
1. Click **New Milestone Path.**
1. Specify the following information in the **Basic Info** area:

   | Milestone Path Name |Enter a name for the milestone path. |
   |---|---|
   | Description |Enter a description to define the milestone path. |
   | **Is Active** |Select this checkbox if you want the milestone path to be active. Other users can find this path and attach it to projects when creating or editing projects. Inactive milestone paths cannot be attached to projects. This is enabled by default. |
   | Groups |Select the groups listed to allow users in these groups to see and apply this milestone path to their projects. The home group of the user entering the milestone path is selected by default. |

   {style="table-layout:auto"}

1. Specify the following information in the **Milestones** area:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td>Type descriptive names for each milestone.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Description</strong> </td> 
      <td>Type a description for the milestone.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Color</td> 
      <td> <p>Choose a color to associate with your milestone. </p> <p>If you do not choose a color, the system chooses the last color used in a milestone path. We recommend that you choose a unique color for each milestone. The color is used for visual and reporting purposes.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Add Milestone** and continue to add milestones as needed until the path is completed. 
1. Click **Create Milestone Path** to save your changes.

   Your milestone path is ready to be associated with a project.

   For more information on how to associate milestone paths to projects and milestones to tasks, see [Associate milestones with tasks](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).
