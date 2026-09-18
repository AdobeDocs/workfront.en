---
product-area: projects
navigation-topic: manage-projects
title: Change the Status of a Project
description: You can manually update the Status of a project to any other status, if needed. You can manually update the Status of a project to a status that equates Complete only when the Completion Mode of the project is set to Manual.
author: Alina
feature: Work Management
exl-id: 80098514-fd44-436d-836b-bd9c1b52b3a9
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/PRLph0Euqn69SUFkRMT1N7BmJinnao-xfzMWWEE407Q
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
    internal-label: Projects
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Change the status of a project

<!--Audited: 02/2024-->

You can manually update the Status of a project to any other status, if needed.  

You can manually update the Status of a project to a status that equates Complete only when the Completion Mode of the project is set to Manual. 

Otherwise, Adobe Workfront automatically marks the project as Complete when all the tasks and issues of the project are completed and approved. 

For more information about the project's Completion Mode, see [Edit projects](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md). 

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
   <td> <p>Standard</p> 
   <p>Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project</p> </td> 
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
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>New: Standard </p> 
   Or
   <p>Current: Plan </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## Considerations about updating to specific statuses

* **When updating a project to Complete:** Ensure that all tasks and issues are completed on the project. You cannot select the Complete status for a project, or any other status that equates Complete when there are tasks or issues that have not been completed on the project. This includes approving any task or issue that is in a Complete-Pending Approval status.
* **When updating a project from Complete to Current:** If all the tasks and issues on the project are completed, ensure that the project's Completion Mode is set to Manual. If the project's Completion Mode is Automatic, the status of the project remains Complete.

## Change project status

1. Go to the project whose status you want to update.
1. In the project header, click the name of the status in the **Status** field, then select a new status.

   ![Change project status](assets/change-project-status-in-header-drop-down-nwe-350x371.png)

   Or

   Click the **More** menu ![More menu](assets/qs-more-menu.png) next to the name of the project and click **Edit** and select a new status in the **Status** field, then click **Save**.

   The project status updates to the status you selected.
