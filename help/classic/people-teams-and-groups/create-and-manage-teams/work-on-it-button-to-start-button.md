---
filename: work-on-it-button-to-start-button
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Replace the Work On It button with a Start button
description: Adobe Workfront's default configuration includes a Work On It button for tasks and issues that displays for items that you have been assigned to. When you click Work On It on items assigned to you, you signal to other users that you received the work and acknowledge that you'll work on it. However, the Work On It button doesn't update the task or issue status to signal that work has actually started.
---

# Replace the Work On It button with a Start button

Adobe Workfront's default configuration includes a Work On It button for tasks and issues that displays for items that you have been assigned to. When you click Work On It on items assigned to you, you signal to other users that you received the work and acknowledge that you'll work on it. However, the Work On It button doesn't update the task or issue status to signal that work has actually started.

You can replace the Work On It button with a Start button for a team you belong to. In this case, you click the Start button instead of Work On It, which automatically updates the status and the Actual Start Date of the work item, signaling that you started work. For information about the setting of which team might affect your changes in the Work On It button, see the section [Configure the Start button](#configur) in this article.

>[!IMPORTANT]
>
>Clicking the Start button changes the item's status and Actual Start Date. If someone else has started working on a task or issue (which changed the status to In Progress and populated the Actual Start Date), the button for the item displays as Work On It even when a team you belong to has had the button replaced with a Start button.

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
   <td> <p>Plan</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan or license type you have, contact your Workfront administrator.

## Configure the Start button

If you have a Plan license, you can configure the Start button for a team in the Edit team window. Following is how the button works after it is enabled for a team:

* `The team is assigned to a work item`: If a team is assigned to the work item, members on that team see the Start button and the statuses configured for that team.
* `The user belongs to a Home Team`: If no team is assigned to the work item but the user is assigned to a Home Team in their profile, then the user sees the Start button and the statuses configured for that team. This is the scenario we recommend if you want users to use the Start button frequently.
* `The user is assigned to a work item`: If there is no team assigned to the work item and no Home Team assigned to the user but the user is assigned to the work item, then the user sees the Start button and the combined statuses configured for that all teams they are assigned to.
* `The user isn't assigned to any teams:` If there is no team assigned to the work item and no team for the user, including the Home Team, and the item is assigned to the user, then the user seems the Work On It button.

>[!NOTE]
>
>This feature is not currently available in >
>* The Workfront mobile app
>* Workfront for Office 365
>* Workfront email notifications
>

To configure the Start button:

1. In the `Teams` drop-down menu, select a team.  
   or  
   Click `Create Team`.

1. Find the `Work On It` button section near the bottom of the Team Settings page.
1. Select the `Change the Work On It button to a Start button to automatically update the status of an item` check box.
1. Select one or more statuses for each work item type. If you select more than one status, a drop-down menu appears when you click Start where you can choose the desired status.
1. Click `Save changes`. Users now see a Start Task or a Start Issue button instead of the Work On It button when they are assigned a work item.

   >[!NOTE]
   >
   >We recommend setting the team as a user's Home Team so the start button appears on all of their assigned work items. See [Associate users with a Home Team](#associat) below.

## Associate users with a Home Team

To associate users with a Home Team:

1. In the `Organization` section, select the `Home Team` field. Start typing the name of the team whose settings you want to associate with the&nbsp;users. Click the name of the team when you see it in the list.

1. Click `Save Changes`.  
   The&nbsp;users you selected are now associated with a&nbsp;Home Team. &nbsp;  
   Any team settings, including the statuses associated with the Done button are now visible to these users.&nbsp;

