---
product-area: projects
navigation-topic: plan-a-project
title: View project Planned Hours in the Role Allocation panel
description: You can view role allocation for all job roles assigned to work items in a project in the Role Allocation panel of the project.
author: Alina
feature: Work Management
exl-id: 76f70cb6-f707-4a73-bc81-e755e2d0a33d
---
# View project Planned Hours in the Role Allocation panel

You can view role allocation for all job roles assigned to work items in a project in the Role Allocation panel of the project.

>[!NOTE]
>
>This article refers to viewing the job roles associated with tasks and issues on a project and their allocated Planned Hours in the Role Allocation panel of a project. For information about reconciling Planned Hours with initiatives hours using the Role Allocation Panel when using the Adobe Workfront Scenario Planner, see the following:
>
>* [Show role allocation for projects and initiatives in the task list](../../../scenario-planner/show-role-allocation-task-list-nwe.md) 
>* [Show role allocation for projects and initiatives in the Workload Balancer](../../../scenario-planner/show-role-allocation-workload-balancer.md) 
>
>  You must have a Scenario Planner license in order to see initiative hours in the Role Allocation panel.&nbsp;For information about the Scenario Planner, see [Get started with the Scenario Planner](../../../scenario-planner/get-started-with-scenario-planning.md) . 
>

## Access requirements

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Light or higher</p> 
   Or
   <p>Legacy license: Review or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

You must have the following:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

You must have the following:

* Tasks or issues assigned to job roles or to users associated with a job role.

  >[!TIP]
  >
  >If the tasks or issues are unassigned, assigned to teams, or are assigned to users with no job role, the Planned Hours of the project is zero in the Role Allocation panel.

* Tasks and issues with a Duration higher than zero.

## View project Planned Hours in the Role Allocation panel

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Projects**.
1. Click the name of a project to access it.&nbsp;This opens the Project page. 
1. Click one of the following in the left panel:

   * **Tasks** 
   * **Workload Balancer**

1. Click the **Show role allocation** icon ![](assets/show-role-allocation-icon.png).

   The Role Allocation panel displays.

   ![](assets/role-allocation-panel-planned-hours-only-350x316.png)

1. Review the following information in the **Role Allocation** panel:

   |Field | Description|
   |---|---|
   | **Job Role** |Job roles assigned to tasks and issues on the project. These can be job roles assigned directly to tasks and issues or job roles associated with users assigned to tasks and issues on the project.  |
   | **Planned Hours** |The total number of Planned Hours from tasks and issues assigned to job roles or users associated with a job role on the project.  |

