---
product-area: projects
navigation-topic: manage-projects
title: Select the Project Update Type
description: By selecting an Update Type for a project, you can control how frequently the changes you make to the timeline of the project are saved on the parent tasks or the project.
author: Alina
feature: Work Management
exl-id: ffdfffec-d217-4daa-9849-cb0c794992c0
---
# Select the project Update Type

By selecting an Update Type for a project, you can control how frequently the changes you make to the timeline of the project are saved on the parent tasks or the project.

When the project timeline is updated, it is recalculated based on changes made to the project, its tasks, or changes made to another project that the timeline is dependent on.

For example, the following changes to the tasks on the project trigger an update to the timeline &nbsp;of the project:

* Update the dates of tasks
* Change predecessor relationships of tasks
* Change parent-child relationships, adding or removing assignments in addition to changing the task constraint or duration type.

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
   <td><p>Standard</p> 
   <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a project</p> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Update a project's Update&nbsp;Type

When the tasks update, their parent objects (parent tasks or the project) update at the time indicated by the Update Type.&nbsp; To specify an Update Type for your project:

1. Go to the project whose Update Type you want to specify.
1. Click the More menu ![More icon](assets/more-icon.png) next to the name of the project, then click **Edit** .

1. Click  **Project** **Settings**.

   ![](assets/update-type-field-on-project-edit-box-nwe-350x378.png)

1. In the **Update Type** field, select whether you want Workfront to calculate the timeline of the project automatically daily, when there is a change, or if you want the project manager to calculate it manually.

   Select from the options in the list below.&nbsp;

   >[!IMPORTANT]
   >
   >If the timeline of a project is longer than 15 years, Workfront does not calculate the timeline automatically or on change. The Update Type of a project longer than 15 years is always Manual.

   * **Automatic and On Change:**&nbsp;This is the default setting. The project timeline is updated each time a change occurs&nbsp;in the project or in another project that the timeline is dependent on. The project timeline is also updated each night.&nbsp;   
     This is the recommended setting as it ensures that the project timeline is always up to date.

     When you update a task or the project and trigger a timeline recalculation, all available dates are immediately displayed, allowing you to continue working. On projects with more than 100 tasks, dates that require longer calculations are dimmed.

     ![](assets/dates-dimmed-when-insline-editing-350x146.png)

     This indicates that the recalculation is not yet finished, and the dates are subject to change. 
   
   * **Change Only:**&nbsp;The project timeline is updated each time a change occurs in the project or in another project that the timeline is dependent on; scheduled updates do not occur.   
     You might want to select this option if you are concerned about system performance and if&nbsp;changes rarely occur in the project or in other projects that the timeline is dependent on.
   
   * **Automatic Only:**&nbsp;The project timeline is updated each night; it is not updated immediately after changes are made.  
     You might want to select this option if you are concerned about system performance and if many changes occur each day in the project or in other projects that the timeline is dependent on.

     >[!NOTE]
     >
     >A project does not automatically recalculate each night if it is in Planning status. It only recalculates on change.

   * **Manual Only:**&nbsp;The project timeline is updated only&nbsp;when you select the option to **Recalculate Timelines**, as described in the section "Manual Recalculation" in&nbsp;the article [Recalculate project timelines](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).  
     You might want to select this option if you are making many changes to the project at one time, and you want the timeline recalculation to occur after all of the changes have been made (rather than after each individual change).

1. Click **Save**.
