---
filename: issue-status
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-groups
title: Configure the Done button for issues if no team is assigned
description: Clicking the Done button on an issue updates the status for the issue. By default, the Done button marks an issue as Resolved. Users with certain permissions can configure the Done button to reflect certain statuses in the system. The primary way to configure statuses for the Done button is through the Home Team. For more information, see Configure the Done button for issues.
hidefromtoc: true
---

# Configure the Done button for issues if no team is assigned

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

Clicking the Done button on an issue updates the status for the issue. By default, the Done button marks an issue as Resolved. Users with certain permissions can configure the Done button to reflect certain statuses in the system. The primary way to configure statuses for the Done button is through the Home Team. For more information, see [Configure the Done button for issues](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md).

If the user does not have a Home Team assigned, the Done button for issues is tied to a system-generated Resolved status that has the three-letter code RLV. System administrators can delete the Resolved (RLV) status if they wish, though this is not recommended.

If the Resolved (RLV) status is deleted and the user marking the issue as Done has no Home Team, the default issue status is tied to whatever is set as the default for Closed for the group assigned to the project. This article explains how to find the group associated with a project, then update that status if needed.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>System administrator</p> </td> 
  </tr> 
 </tbody> 
</table>

## Find the group associated with the project

When a user creates a project, their Home group is automatically assigned to the project. Users can change this group in the Project Details section at any time. You need to know what group is on a specific project to modify the default status for the issue Done button. To find the group associated with the project

1. Go to a project.
1. Click **Project Details** at the top of the page.
1. Locate the **Group** field.  
   This is the group name you need to use to change the status in the Setup area. See the following section for instructions on how to update the default status for a specific group.

## Update the default status for a specific group

1. Click **Setup** in the Global Navigation Bar.
1. In the left panel, click **Project Preferences**, then **Statuses**.

1. Click **Requests**, then type the name of the group in the **System Statuses** search box located on the right.

1. Select the group.
1. Click the Set Default Statuses drop-down menu, then choose the status you want the Done button to use.

   >[!IMPORTANT]
   >
   >This status is used only when they user has no assigned Home Team and the RLV status has been deleted.

1. Click **Save**.

