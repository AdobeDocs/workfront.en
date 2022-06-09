---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Configure the Done button for issues
description: The Done button can automatically set the status of a task or an issue. By default, Adobe Workfront marks an issue as Resolved when an assignee clicks Done on their work item.
feature: "People, Teams, and Groups"
---

# Configure the Done button for issues

The Done button can automatically set the status of a task or an issue. By default, Adobe Workfront marks an issue as Resolved when an assignee clicks Done on their work item.

## Overview

Users with certain permissions can configure the Done button to reflect certain statuses in the system. There are 3 different ways the Done button works for issues in Workfront:

* If the user has an assigned Home Team, a Workfront administrator or a user with a Plan license can configure the Done button to reflect certain statuses for team members. See [Configure the Done button for a Team](#configure-the-done-button-for-a-team) in this article.
* If the user does not have a Home Team assigned, the Done button for issues is tied to a system-generated Resolved status that has the three-letter code RLV. There are no configuration options available in this scenario. The Done button automatically defaults to this status.
* If the Resolved (RLV) status is deleted and the user marking the issue as Done has no Home Team, the default issue status is tied to whatever is set as the default for Closed for the group assigned to the project the issue belongs to. The Workfront administrator can configure a system-wide default setting for the group. See [Configure the Done button when the Resolved status has been deleted](#configure-the-done-button-when-the-resolved-status-has-been-deleted) in this article.

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan*</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations*</strong></td> 
   <td>System administrator access is required to configure the Done button when the Resolved status is deleted</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Configure the Done button for a Team {#configure-the-done-button-for-a-team}

You can change which status is applied to the work item with the Done button. You can also set multiple statuses and allow the user to choose which status is appropriate.

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Teams**.

1. Click the **Switch team** icon, then either select a new team from the drop-down menu or search for a team in the search bar.
1. Click the **More** menu, then click **Edit**.
1. Find the **Done Button** section at the bottom of the **Team Settings** page.

1. Select one status or more than one status for each work item type.

   >[!NOTE]
   >
   >Consider the following when selecting statuses for tasks or issues:
   >
   >* When you select one status for each type of work item, the task or issue status is set to that status when a user clicks Done on their item. If you set multiple statuses for each type of work item, a drop-down menu is added to the Done button and the user must pick a status to change the status on the work item.  
   >* You can associate only system-level statuses with the Done button. You cannot associate Group-specific statuses with work item statuses.
   >* When a user assigned to the item places the item in the status associated with the Done button, the item displays as Done for that user regardless of whether the status you select is a Completed or Closed status or a working status. 
   >   
   >   
   >  For example, associating the Done button with In Progress causes the work item to display as Done for the user who changes the status from New to In progress. 
   >   
   >* Issue types are customizable and they might have different names than listed below in your environment.  
   >  Following are the default tasks and issue types:
   >     
   >   * Tasks
   >   * Issue
   >   * Request
   >   * Change Order
   >   * Bug Report

   If the task or issue is assigned to multiple users, you see a "Done with my part" option in the drop-down menu, in addition to the multiple statuses chosen for your team.  

1. Click **Save Changes**.

## Associate users with a Home Team

To make the changes to the Done button functionality visible to users, you can make the team whose settings you changed the Home Team of the users.

To associate users with a Home Team:

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront.

1. Click **Users**, then select the user or users you want to associate with a Home Team.
1. Click the **More** menu, then select **Edit**.  
   ![](assets/user-settings-nwe-350x291.png)

1. In the **Organization** section, select&nbsp;the **Home Team** field. Start typing the name of the team whose settings you want to associate with the&nbsp;users. Click the name of the team when you see it in the list.

1. Click **Save Changes**.  
   The users you selected are now associated with a Home Team. 
   Any team settings, including the statuses associated with the Done button, are now visible to these users.

## Configure the Done button when the Resolved status has been deleted {#configure-the-done-button-when-the-resolved-status-has-been-deleted}

If a user does not have a Home Team and the system-wide default for Resolved (RLV) has been deleted, a Workfront administrator can configure the Closed status for the group on to the project. Workfront selects this status for a closed issue when the user clicks the Done button.

### Find the group associated with the project

When a user creates a project, their Home Group is automatically assigned to the project. Users with Manage access to the project can change this group in the Project Details section at any time. To understand what status Workfront uses for a completed issue in this case, you must understand what group is associated with the project the issue is on and what the default status for Closed this group has for issues.

To find the group associated with the project:

1. Go to a Project.
1. On the left side of the page, click **Project Details**.
1. Locate the **Project association** section, then find **Group**.  
   This is the group name you need to use to check the status in the Setup area. See the following section for instructions on how to update the default status for a specific group.

### Update the default status for a specific group

As a Workfront administrator, you can update the status for a specific group:

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).
1. In the left panel, click **Project Preferences**, then **Statuses**.

1. Click **Issues**, then type the name of the group in the **System Statuses** search box located on the right.

1. Select the group.
1. Click the **Set Default Statuses** drop-down menu, then choose a default status for Closed. Workfront uses this status for a closed issue when a user clicks the Done button.

   >[!IMPORTANT]
   >
   >This status is used only when the user has no assigned Home Team and the RLV status has been deleted.

1. Click **Save**.

