---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Configure the Done button for issues
description: The Done button can automatically set the status of a task or an issue. By default, Adobe Workfront marks an issue as Resolved when an assignee clicks Done on their work item.
author: Lisa
feature: People Teams and Groups
exl-id: 2e72854a-2d49-4665-b307-b88f660b141e
---
# Configure the [!UICONTROL Done] button for issues

The [!UICONTROL Done] button can automatically set the status of a task or an issue. By default, [!DNL Adobe Workfront] marks an issue as [!UICONTROL Resolved] when an assignee clicks [!UICONTROL Done] on their work item.

## Overview

Users with certain permissions can configure the [!UICONTROL Done] button to reflect certain statuses in the system. There are 3 different ways the [!UICONTROL Done] button works for issues in [!DNL Workfront]:

* If the user has an assigned [!UICONTROL Home Team], a [!DNL Workfront] administrator or a user with a [!UICONTROL Plan] license can configure the [!UICONTROL Done] button to reflect certain statuses for team members. See [Configure the [!UICONTROL Done] button for a Team](#configure-the-uicontrol-done-button-for-a-team) in this article.
* If the user does not have a [!UICONTROL Home Team], but they have [!UICONTROL Other Teams] in their profile, Workfront searches for the setting of the [!UICONTROL Done] button on any of the teams associated with the user. The selection is random and the status associated with any of the teams is used for the issue. 
* If the user does not have a [!UICONTROL Home Team] assigned, the [!UICONTROL Done] button for issues is tied to a system-generated [!UICONTROL Resolved] status that has the three-letter code [!UICONTROL RLV]. There are no configuration options available in this scenario. The [!UICONTROL Done] button automatically defaults to this status.
* If the [!UICONTROL Resolved] ([!UICONTROL RLV]) status is deleted and the user marking the issue as [!UICONTROL Done] has no [!UICONTROL Home Team], the default issue status is tied to whatever is set as the default for [!UICONTROL Closed] for the group assigned to the project the issue belongs to. The Workfront administrator can configure a system-wide default setting for the group. See [Configure the [!UICONTROL Done] button when the [!UICONTROL Resolved] status has been deleted](#configure-the-uicontrol-done-button-when-the-uicontrol-resolved-status-has-been-deleted) in this article.

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations*</strong></td> 
   <td>System administrator access is required to configure the [!UICONTROL Done] button when the [!UICONTROL Resolved] status is deleted</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Configure the [!UICONTROL Done] button for a Team 

You can change which status is applied to the work item with the [!UICONTROL Done] button. You can also set multiple statuses and allow the user to choose which status is appropriate.

1. Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **[!UICONTROL Teams]**.

1. Click the **[!UICONTROL Switch team]** icon, then either select a new team from the drop-down menu or search for a team in the search bar.
1. Click the **[!UICONTROL More]** menu, then click **[!UICONTROL Edit]**.
1. Find the **[!UICONTROL Done Button]** section at the bottom of the **[!UICONTROL Team Settings]** page.

1. Select one status or more than one status for each work item type.

   >[!NOTE]
   >
   >Consider the following when selecting statuses for tasks or issues:
   >
   >* When you select one status for each type of work item, the task or issue status is set to that status when a user clicks [!UICONTROL Done] on their item. If you set multiple statuses for each type of work item, a drop-down menu is added to the [!UICONTROL Done] button and the user must pick a status to change the status on the work item.  
   >* You can associate only system-level statuses with the [!UICONTROL Done] button. You cannot associate Group-specific statuses with work item statuses.
   >* When a user assigned to the item places the item in the status associated with the [!UICONTROL Done] button, the item displays as [!UICONTROL Done] for that user regardless of whether the status you select is a [!UICONTROL Completed] or [!UICONTROL Closed] status or a working status. 
   >   
   >   
   >  For example, associating the [!UICONTROL Done] button with In Progress causes the work item to display as [!UICONTROL Done] for the user who changes the status from New to In progress. 
   >   
   >* Issue types are customizable and they might have different names than listed below in your environment.  
   >  Following are the default tasks and issue types:
   >     
   >   * [!UICONTROL Tasks]
   >   * [!UICONTROL Issue]
   >   * [!UICONTROL Request]
   >   * [!UICONTROL Change Order]
   >   * [!UICONTROL Bug Report]

   If the task or issue is assigned to multiple users, you see a "[!UICONTROL Done with my part]" option in the drop-down menu, in addition to the multiple statuses chosen for your team.  

1. Click **[!UICONTROL Save Changes]**.

## Associate users with a Home Team

To make the changes to the [!UICONTROL Done] button functionality visible to users, you can make the team whose settings you changed the Home Team of the users.

To associate users with a Home Team:

1. Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of [!DNL Adobe Workfront].

1. Click **[!UICONTROL Users]**, then select the user or users you want to associate with a Home Team.
1. Click the **[!UICONTROL More]** menu, then select **[!UICONTROL Edit]**.  
   ![](assets/user-settings-nwe-350x291.png)

1. In the **[!UICONTROL Organization]** section, select the **[!UICONTROL Home Team]** field. Start typing the name of the team whose settings you want to associate with the users. Click the name of the team when you see it in the list.

1. Click **[!UICONTROL Save Changes]**.  
   The users you selected are now associated with a Home Team. 
   Any team settings, including the statuses associated with the [!UICONTROL Done] button, are now visible to these users.

## Configure the [!UICONTROL Done] button when the [!UICONTROL Resolved] status has been deleted 

If a user does not have a Home Team and the system-wide default for [!UICONTROL Resolved] ([!UICONTROL RLV]) has been deleted, a [!DNL Workfront] administrator can configure the [!UICONTROL Closed] status for the group on to the project. [!DNL Workfront] selects this status for a closed issue when the user clicks the [!DNL Done] button.

### Find the group associated with the project

When a user creates a project, their Home Group is automatically assigned to the project. Users with [!UICONTROL Manage] access to the project can change this group in the [!UICONTROL Project Details] section at any time. To understand what status [!DNL Workfront] uses for a completed issue in this case, you must understand what group is associated with the project the issue is on and what the default status for [!UICONTROL Closed] this group has for issues.

To find the group associated with the project:

1. Go to a Project.
1. On the left side of the page, click **[!UICONTROL Project Details]**.
1. Locate the **[!UICONTROL Project association]** section, then find **[!UICONTROL Group]**.  
   This is the group name you need to use to check the status in the Setup area. See the following section for instructions on how to update the default status for a specific group.

### Update the default status for a specific group

As a [!UICONTROL Workfront] administrator, you can update the status for a specific group:

1. Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **[!UICONTROL Setup]** ![](assets/gear-icon-settings.png).
1. In the left panel, click **[!UICONTROL Project Preferences]**, then **[!UICONTROL Statuses]**.

1. Click **[!UICONTROL Issues]**, then type the name of the group in the **[!UICONTROL System Statuses]** search box located on the right.

1. Select the group.
1. Click the **[!UICONTROL Set Default Statuses]** drop-down menu, then choose a default status for [!UICONTROL Closed]. [!DNL Workfront] uses this status for a closed issue when a user clicks the [!UICONTROL Done] button.

   >[!IMPORTANT]
   >
   >This status is used only when the user has no assigned Home Team and the [!UICONTROL RLV] status has been deleted.

1. Click **[!UICONTROL Save]**.
