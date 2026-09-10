---
product-area: projects
navigation-topic: task-duration
title: Update the Planned Hours and Duration of a Task with a Simple Duration Type
description: By default, Adobe Workfront calculates the Duration of a task with a Simple Duration Type based on the amount of Planned Hours. However, you can also manually edit the amount of Planned Hours and the Duration of a Simple Duration task in certain areas of Workfront.
author: Alina
feature: Work Management
exl-id: 47a9b095-2b7d-4ed0-8cb6-e6bd5e37ce9c
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/SLemiOnFj-dOnWtXjH6gNzHZdVaXfp47qB0xzVJkRck
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
    internal-label: Tasks
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
    internal-label: Projects
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Update the Planned Hours and Duration of a task with a Simple Duration Type

By default, Adobe Workfront calculates the Duration of a task with a Simple Duration Type based on the amount of Planned Hours. However, you can also manually edit the amount of Planned Hours and the Duration of a Simple Duration task in certain areas of Workfront.

You can either edit Planned Hours and Duration of a task with a Simple Duration Type inline or at the task level in the Assignments area.

For more information about editing information inline, see [Inline edit items in a list in Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

This article describes how you can update the Planned Hours and Duration for a task with a Simple Duration Type at the task level, in the Assignments area.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td><p>Standard or higher</p> 
   <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>View or higher access to Projects</p> <p>Edit access to Tasks</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage access to the task </p></td> 
  </tr> 
 </tbody> 
</table>

For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:

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
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Update the Planned Hours and Duration of a task with a Simple Duration Type

>[!IMPORTANT]
>
>After you manually update the Duration on a Simple Duration task, Workfront stops calculating it based on the Planned Hours.

To edit the Planned Hours and Duration of a task with a Simple Duration Type in the Advanced Assignments box:

1. In a task list, click the name of the task for which you want to change the duration type.
1. Do one of the following:

   * Click the **More** icon ![More icon on an object](assets/qs-more-icon-on-an-object.png) next to the name of the task, click **Edit**, then **Assignments**. 
   * Click the **Assigned to** or the name of the assignments in the Assignments area of the task header, then click **Advanced**.

1. Enter a total value for the **Planned Hours** for all the assignments, for example, 10 hours. The total number of Planned Hours is distributed equally between all the resources assigned to the task.
1. (Optional) Manually adjust the Planned Hours of each resource assigned to the task. The total number of Planned Hours for the task updates to reflect the new hours individually assigned to your resources.
1. Enter a value for the task **Duration**, for example 2 Days.

   ![Advanced assignments simple duration multiple resources](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

1. Click **Save**.
