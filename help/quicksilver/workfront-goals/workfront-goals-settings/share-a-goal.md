---
product-previous: workfront-goals
navigation-topic: workfront-goals-settings
title: Share a goal in Workfront Goals
description: When you share a goal you give Manage permissions to a goal to someone who did not create it.
author: Alina
feature: Workfront Goals
exl-id: 747449cf-9092-4b9f-9add-db2e7d3fab48
---
# Share a goal in Adobe Workfront Goals

When you share a goal you give Manage permissions to a goal to someone who did not create it.

## Access requirements

You must have the follwoing: 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
 <p> New product requirement, one of the following: </p>
<ul>
<li>A Select or Prime Adobe Workfront plan and an additional Adobe Workfront Goals license.</li>
<li>An Ultimate Workfront plan which includes Workfront Goals by default. </li></ul>
 <p>Or</p>
 <p>Current product requirement: A Workfront plan and an additional license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Object permissions</td>
 <td>
  <div>
  <p>View or higher permissions to the goal to view it</p>
  <p>Manage permissions to the goal to edit it</p>
  <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Considerations about sharing goals

* Users can have the following permissions to a goal:

   <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <tbody> 
   <tr> 
      <td role="rowheader"><p><b>Goal permissions</b></p></td> 
      <td>
      <p><b>Description</b></p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>View</p></td> 
      <td>
      <p>Users have permissions to view the goal, but they cannot edit information for the goal, they cannot add or edit information for results, or activities, update status, or delete the goal.</p>      
      <p>By default, all users with access to Goals can view all goals in the system. Users can copy the goal, if they have Edit access to Goals in their access level.</p> </td> 
   </tr> 
   <tr> 
      <td role="rowheader"><p>Manage</p></td> 
      <td> <p>Users can edit all information for the goal, including for the results, or activities, including delete them.</p> 
      <p>Only goal creators or users who are specifically given Manage permissions to a goal can manage a goal.</p> 
      Only users with Manage permissions to a goal can share the goal with others to give them Manage permissions to the goal. </p> </td> 
   </tr> 
   </tbody> 
   </table>

* You can share the following types of goals with others:

   * A goal you created 
   * A goal created by someone else to which you were given permissions to Manage.

* If you have Manage permissions to a goal, you can change the permissions on the goal for the goal creator. By default, they have Manage permissions when they create the goal, but you can change their permissions to View.

## Share a goal

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) > **Goals** in the upper-right corner.

   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../workfront-goals-settings/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->

   The Goal List displays. 

1. Click the name of a goal in the list. The goal page opens. 

1. Click the **More icon** next to the goal name, then click **Share**.

   ![](assets/more-menu-highlighted-goal-details-panel-with-share-link-350x156.png)

   The Goal Access box displays.

   ![](assets/goal-access-sharing-box-manage-system-wide-deselected-350x400.png)

1. Do one of the following:

   * Select the **Manage system-wide** setting to give Manage permissions to everyone in the system who has Edit access to Goals in their access level. This is deselected by default for all new goals. 
   * Start typing the name of a user that you want to give Manage permissions to in the **Give Manage access to** box. Select the name when it appears in the list.

     >[!TIP]
     >
     >You can only share a goal with other users. You cannot share goals with groups, teams, or your company.

1. Click **Share**.

   The goal is shared with the users you specified. A "System-wide" label or the name of the users who have Manage permissions to the goal display in the Access to Manage field in the Goal Details panel.

## Goal permission options

The following table lists the permissions that you can grant when sharing a goal. For more information about the access users get based on their license, see [Grant access to Adobe Workfront Goals](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md). 

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p><strong>Actions</strong> </p> </th> 
   <th> <p><strong>Manage</strong> </p> </th> 
   <th> <p><strong>View</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>View goal</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>View results or activities</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td>Copy goal* </td> 
   <td>✓ </td> 
   <td>✓</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Convert results or activities into other goals*</td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>View projects added as activities** </td> 
   <td>✓</td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td>Edit goal</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Edit results or activities</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Add results or activities for the goal</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td>Associate a project as an activity to the goal**</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p>Delete goal</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Delete results or activities</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>&nbsp;</p> </td> 
  </tr> 
  <tr> 
   <td>Disconnect projects from the goal</td> 
   <td>✓</td> 
   <td>&nbsp;</td> 
  </tr> 
 </tbody> 
</table>

*You must have Edit access to Goals in your access level to be able to convert results and activities to goals.

**You must have access to View Projects and View permission to the projects added or that you want to add to the goal to view them.

For information about project access level, see [Grant access to projects](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md).

For information about project permissions, see [Share a project in Adobe Workfront](../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

&nbsp;
