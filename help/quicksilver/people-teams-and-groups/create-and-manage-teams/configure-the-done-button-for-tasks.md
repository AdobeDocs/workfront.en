---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Configure the Done Button for Tasks
description: The Done button can automatically set the status of a task or an issue. By default, Adobe Workfront marks a task as Completed when an assignee clicks Done on their work item.
author: Lisa
feature: People Teams and Groups
exl-id: 55cc5562-13d5-4089-8937-f33d0cde3cac
---
# Configure the [!UICONTROL Done] button for tasks

The [!UICONTROL Done] button can automatically set the status of a task or an issue. By default, [!UICONTROL Adobe Workfront] marks a task as [!UICONTROL Completed] when an assignee clicks Done on their work item.

## Overview

Users with certain permissions can configure the [!UICONTROL Done] button to reflect certain statuses in the system. There are two different ways the [!UICONTROL Done] button works for tasks in [!UICONTROL Workfront]:

* If the user has an assigned Home Team, a [!DNL Workfront] administrator or a user with a [!UICONTROL Plan] license can configure the [!UICONTROL Done] button to reflect certain statuses for team members. See [Configure the [!UICONTROL Done] button for a Team](#configure-the-uicontrol-done-button-for-a-team) in this article.
* If the user does not have a [!UICONTROL Home Team], but they have [!UICONTROL Other Teams] in their profile, Workfront searches for the setting of the [!UICONTROL Done] button on any of the teams associated with the user. The selection is random and the status associated with any of the teams is used for the task. 
* If the user does not have a Home Team assigned, the [!UICONTROL Done] button for tasks is tied to a complete status. There are no configuration options available in this scenario. The [!UICONTROL Done] button automatically defaults to this status.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront plan</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>
   <p>New: Standard</p>
   <p>or</p>
   <p>Current: Plan</p></td>
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configure the [!UICONTROL Done] button for a Team 

You can change which status is applied to the work item with the [!UICONTROL Done] button. You can also set multiple statuses and allow the user to choose which status is appropriate.

{{step1-to-team}}

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
   >  For example, associating the [!UICONTROL Done] button with [!UICONTROL In Progress] causes the work item to display as [!UICONTROL Done] for the user who changes the status from [!UICONTROL New] to [!UICONTROL In progress]. 
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
   Any team settings, including the statuses associated with the [!UICONTROL Done] button are now visible to these users.
