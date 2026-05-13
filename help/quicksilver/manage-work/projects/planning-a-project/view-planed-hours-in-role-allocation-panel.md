---
product-area: projects
navigation-topic: plan-a-project
title: View project Planned Hours in the Role Allocation panel
description: You can view role allocation for all job roles assigned to work items in a project in the Role Allocation panel of the project.
author: Alina, Lisa
feature: Work Management
exl-id: 76f70cb6-f707-4a73-bc81-e755e2d0a33d
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/24H2qmd3CpVLWACyKQXatbTbg434YTp-Y0J6YTJeCxI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: d3382524-5489-431b-bde9-271ab257bc37
    internal-label: Workfront Scenario Planner
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
    internal-label: Get started
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
    internal-label: Projects
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
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
>  You must have a Scenario Planner license in order to see initiative hours in the Role Allocation panel. For information about the Scenario Planner, see [Get started with the Scenario Planner](../../../scenario-planner/get-started-with-scenario-planning.md). 
>
>If your company has bought the Adobe Scenario Planner in the past, it has been grandfathered in. The Scenario Planner is not available for purchase anymore.

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Adobe Workfront Ultimate</p>
   <p>Adobe Workflow Ultimate</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>Light or higher</p>
   <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to Projects</p>
   <p>Edit access to Scenario Planner to update hours on initiatives</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on the project</p> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:

able style="table-layout:auto"> 
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
-->

## Prerequisites

You must have the following:

* Tasks or issues assigned to job roles or to users associated with a job role.

  >[!TIP]
  >
  >If the tasks or issues are unassigned, assigned to teams, or are assigned to users with no job role, the Planned Hours of the project is zero in the Role Allocation panel.

* Tasks and issues with a Duration higher than zero.

## View project Planned Hours in the Role Allocation panel

{{step1-to-projects}}

1. Click the name of a project to access it. This opens the Project page. 
1. Click one of the following in the left panel:

   * **Tasks** 
   * **Workload Balancer**

1. Click the **Show role allocation** icon ![Show role allocation icon](assets/show-role-allocation-icon.png).

   The Role Allocation panel displays.

   ![Role allocation panel with planned hours only](assets/role-allocation-panel-planned-hours-only-350x316.png)

1. Review the following information in the **Role Allocation** panel:

   |Field | Description|
   |---|---|
   | **Job Role** |Job roles assigned to tasks and issues on the project. These can be job roles assigned directly to tasks and issues or job roles associated with users assigned to tasks and issues on the project.  |
   | **Planned Hours** |The total number of Planned Hours from tasks and issues assigned to job roles or users associated with a job role on the project.  |

