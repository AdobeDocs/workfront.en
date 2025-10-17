---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: Create Personal Tasks
description: Personal tasks are ad hoc work requests that you send to a user, to yourself, or to-do items that you create for yourself in your Home area. Workfront saves ad hoc work requests and to do items as personal tasks.
author: Becky
feature: Get Started with Workfront
exl-id: b40d6b10-19c7-4e11-a74f-a8af3ebafb65
---
# Create personal tasks

<!--Audited: 10/2024-->

Personal tasks are ad hoc work requests that you send to a user or send to or add for yourself. 

Adobe Workfront saves ad hoc work requests and to do items as personal tasks on a user's personal project that is Wprfront automatically creates for each user. 

The following are characteristics of a user's personal project: 

* All users in Workfront have a personal project called "< User's full name>'s Tasks". For example, "John Smith's Tasks". 
* The personal project of each user does not display in searches and it is hidden. 
* A personal project cannot be deleted, even if users have been deactivated.
* The Status of a personal project is always Current. Personal projects cannot be completed or canceled. 
* All personal tasks are stored in a user's personal project.
* You can move personal tasks to another project, if needed.

You can create personal tasks in the following ways:

* Create a to-do item in your Home area

    For information, see [Create work items and projects from the Home area](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md). 

* Create and send a personal work request to another user from the user profile page
* Create and send a personal work request to yourself from your user profile page

This article describes how you can create a personal work request for a user or for yourself from the user profile page. 

Regardless how you add a personal task, you can find them in the same areas of Workfront. For more information, see the section [Locate personal task](#locate-personal-tasks) in this article. 

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront package</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license</strong></td> 
   <td> 
   <p>Standard<p>
   <p>Plan</p>
   <p>This is the license needed to send requests to other users. All users can create a work request for themselves.</p> 
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations</strong></td> 
   <td> <p>Edit access to Users to create a work request for them. View access to create a personal work request for yourself. </p>
   </td> 
  </tr> 
 
 </tbody> 
</table>

For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> 
   <p>New: Standard to send requests to other users. All users can create a work request for themselves.</p> 
   <p>Current: Plan to send requests to other users. All users can create a work request for themselves.</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations</strong></td> 
   <td> <p>Edit access to Users to create a work request for them. View access to create a personal work request for yourself. </p>
   </td> 
  </tr> 
 
 </tbody> 
</table>-->


## Create a personal work request

1. Go to your user's profile page, or go to another user's profile page that you have access to view.

    >[!TIP]
    >
    >Your Workfront administrator might prevent you from seeing certain users when they configure your access level. 

1. Click the **More menu** ![](assets/more-menu.png) to the right of the user's name in the header.
1. Click **Send work request**. 
    The **Send user a work request** box displays.

    ![](assets/personal-task-box.png)
1. Update the following information: 

    * **Task Name**: This is the name of the ad hoc work request or the personal task. 
    * **Description**: Add a description for the task. 
    * **Assign to**: The name of the user that you selected displays by default. You can add more users or teams.
    * **Due date**: This is the date by which you'd like this task to be completed. By default, this is today's date. You cannot select a date in the past
    * **Time**: This is the time by which you'd like this task to be completed. By default, this is the current time. 

1. Click **Send Request** to save the work request.

    The work request is saved as a personal task in Workfront and it is added to the user's To-dos widget in their Home area. If you send the work request to yourself, it displays in your To-dos widget in Home. 


## Locate personal tasks

You can locate personal tasks in the following areas:

* The To-dos widget in the Home area of the user the personal request was sent to. 

    For information, see [Create work items and projects from the Home area](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md). 

* A personal task report or list. You can build and apply a personal task filter to a task report or list to display only personal tasks and exclude project tasks. 

    For information, see [Filter: personal tasks](/help/quicksilver/reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-personal-tasks.md).
