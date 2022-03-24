---
filename: configure-the-done-button-for-tasks
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Configure the Done button for tasks
description: The Done button can automatically set the status of a task or an issue. By default, Adobe Workfront marks a task as Completed when an assignee clicks Done on their work item.
---

# Configure the Done button for tasks

The Done button can automatically set the status of a task or an issue. By default, Adobe Workfront&nbsp;marks a task as Completed when an assignee clicks Done on their work item.

## Overview

&nbsp;Users with certain permissions can configure the Done button to reflect certain statuses in the system. There are two different ways the Done button works for tasks in Workfront:

* If the user has an assigned Home Team, a Workfront administrator or a user with a Plan license can configure the Done button to reflect certain statuses for team members. See [Configure the Done button for a Team](#configur) in this article.
* If the user does not have a Home Team assigned, the Done button for tasks is tied to a complete status. There are no configuration options available in this scenario. The Done button automatically defaults to this status.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan or license type you have, contact your Workfront administrator.

## Configure the Done button for a Team

You can change which status is applied to the work item with the Done button. You can also set multiple statuses and allow the user to choose which status is appropriate.

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Teams**.

1. Click the **Switch team** icon, then either select a new team from the drop-down menu or search for a team in the search bar.
1. Click the **More** menu, then click **Edit**.
1. Find the **Done Button** section at the bottom of the **Team Settings** page.

1. Select one status or more than one status for each work item type.

   >[!NOTE]
   >
   >Consider the following when selecting statuses:  

   >
   >   
   >   
   >   * When you select one status for each type of work item, the task or issue status is set to that status when a user clicks Done on their&nbsp;item.&nbsp;If you set multiple statuses for each type of work item, a drop-down menu is added to the Done button and the user must pick a status to change the status on the work item.  
   >   * You can associate only system-level statuses with the Done button. You cannot associate Group-specific statuses with work item statuses.
   >   * Issue types are customizable and they might have different names than listed below in your environment.  
   >     Following&nbsp;are the default tasks and issue types:   >   
   >      
   >      
   >      * Tasks
   >      * Issue
   >      * Request
   >      * Change Order
   >      * Bug Report
   >      
   >      
   >   
   >   
   >

   If the task or issue is assigned to multiple users, you see a "Done with my part" option in the drop-down menu, in addition to the multiple statuses chosen for your team.  

1. Click **Save Changes**.

## Associate users with a Home Team

To make the changes to the Done button functionality visible to users, you can make the team whose settings you changed the Home Team of the users.&nbsp;

To associate users with a Home Team:

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront.

1. Click **Users**, then select the user or users you want to associate with a Home Team.
1. Click the **More** menu, then select **Edit**.  
   ![](assets/user-settings-nwe-350x291.png)

1. In the **Organization** section, select&nbsp;the **Home Team** field. Start typing the name of the team whose settings you want to associate with the&nbsp;users. Click the name of the team when you see it in the list.

1. Click **Save Changes**.  
   The&nbsp;users you selected are now associated with a&nbsp;Home Team. &nbsp;  
   Any team settings, including the statuses associated with the Done button are now visible to these users.&nbsp;

