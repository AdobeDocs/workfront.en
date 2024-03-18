---
product-area: projects
navigation-topic: manage-projects
title: Change the status of a project
description: You can manually update the Status of a project to any other status, if needed. You can manually update the Status of a project to a status that equates Complete only when the Completion Mode of the project is set to Manual. 
author: Alina
feature: Work Management
exl-id: 80098514-fd44-436d-836b-bd9c1b52b3a9
---
# Change the status of a project

<!--Audited: 02/2024-->

You can manually update the Status of a project to any other status, if needed.  

You can manually update the Status of a project to a status that equates Complete only when the Completion Mode of the project is set to Manual. 

Otherwise, Adobe Workfront automatically marks the project as Complete when all the tasks and issues of the project are completed and approved. 

For more information about the project's Completion Mode, see [Edit projects](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md). 

## Access requirements

You must have the following access to perform the steps in this article:

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

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator. For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

## Considerations about updating to specific statuses

* **When updating a project to Complete:** Ensure that all tasks and issues are completed on the project. You cannot select the Complete status for a project, or any other status that equates Complete when there are tasks or issues that have not been completed on the project. This includes approving any task or issue that is in a Complete-Pending Approval status.
* **When updating a project from Complete to Current:** If all the tasks and issues on the project are completed, ensure that the project's Completion Mode is set to Manual. If the project's Completion&nbsp;Mode is Automatic, the status of the project remains Complete.

## Change project status

1. Go to the project whose status you want to update.
1. In the project header, click the name of the status in the **Status** field, then select a new status.

   ![](assets/change-project-status-in-header-drop-down-nwe-350x371.png)

   Or

   Click the **More** menu ![](assets/qs-more-menu.png) next to the name of the project and click **Edit** and select a new status in the **Status** field, then click **Save**.

   The project status updates to the status you selected.
