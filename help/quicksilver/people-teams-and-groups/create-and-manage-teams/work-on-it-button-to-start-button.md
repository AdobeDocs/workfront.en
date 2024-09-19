---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Replace the Work On It Button with a Start Button
description: Adobe Workfront's default configuration includes a Work On It button for tasks and issues that displays for items that you have been assigned to.
author: Lisa
feature: People Teams and Groups
exl-id: 9387c5ae-2835-4d8f-80ec-22fcd16c5b6e
---
# Replace the [!UICONTROL Work On It] button with a [!UICONTROL Start] button

[!DNL Adobe Workfront]'s default configuration includes a [!UICONTROL Work On It] button for tasks and issues that displays for items that you have been assigned to. When you click [!UICONTROL Work On It] on items assigned to you, you signal to other users that you received the work and acknowledge that you'll work on it. However, the [!DNL Work On It] button doesn't update the task or issue status to signal that work has actually started.

You can replace the [!DNL Work On It] button with a [!UICONTROL Start] button for a team you belong to. In this case, you click the [!UICONTROL Start] button instead of [!UICONTROL Work On It], which automatically updates the status and the [!UICONTROL Actual Start Date] of the work item, signaling that you started work. For information about the setting of which team might affect your changes in the [!UICONTROL Work On It] button, see the section [Configure the [!UICONTROL Start] button](#configure-the-uicontrol-start-button) in this article.

>[!IMPORTANT]
>
>Clicking the [!UICONTROL Start] button changes the item's status and [!UICONTROL Actual Start Date]. If someone else has started working on a task or issue (which changed the status to [!UICONTROL In Progress] and populated the [!UICONTROL Actual Start Date]), the button for the item displays as [!UICONTROL Work On It] even when a team you belong to has had the button replaced with a [!UICONTROL Start] button.

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

## Configure the [!UICONTROL Start] button 

If you have a [!UICONTROL Plan] license, you can configure the [!UICONTROL Start] button for a team in the [!UICONTROL Edit] team window. Following is how the button works after it is enabled for a team:

* **The team is assigned to a work item**: If a team is assigned to the work item, members on that team see the [!UICONTROL Start] button and the statuses configured for that team.
* **The user belongs to a Home Team**: If no team is assigned to the work item but the user is assigned to a Home Team in their profile, then the user sees the [!UICONTROL Start] button and the statuses configured for that team. This is the scenario we recommend if you want users to use the [!UICONTROL Start] button frequently.
* **The user is assigned to a work item**: If there is no team assigned to the work item and no Home Team assigned to the user but the user is assigned to the work item, then the user sees the [!UICONTROL Start] button and the combined statuses configured for that all teams they are assigned to.
* **The user isn't assigned to any teams:** If there is no team assigned to the work item and no team for the user, including the Home Team, and the item is assigned to the user, then the user seems the [!UICONTROL Work On It] button.

>[!NOTE]
>
>This feature is not currently available in
>
>* The [!DNL Workfront] mobile app
>* [!DNL Workfront for Office 365]
>* [!DNL Workfront] email notifications
>

To configure the Start button:

{{step1-to-team}}

1. In the **[!UICONTROL Teams]** drop-down menu, select a team.  
   or  
   Click **[!UICONTROL Create Team]**.

1. Click the **[!UICONTROL More]** icon ![](assets/more-icon.png), then click **[!UICONTROL Edit]**. 

1. Find the **[!UICONTROL Work On It]** button section near the bottom of the [!UICONTROL Edit Teams] page.
1. Select the **[!UICONTROL Change the Work On It button to a Start button to automatically update the status of an item]** check box.
1. Select one or more statuses for each work item type. If you select more than one status, a drop-down menu appears when you click [!UICONTROL Start] where you can choose the desired status.
1. Click **[!UICONTROL Save changes]**. Users now see a [!UICONTROL Start Task] or a [!UICONTROL Start Issue] button instead of the [!UICONTROL Work On It] button when they are assigned a work item.

   >[!NOTE]
   >
   >We recommend setting the team as a user's Home Team so the start button appears on all of their assigned work items. See [Associate users with a Home Team](#associate-users-with-a-home-team) below.

## Associate users with a Home Team 

To associate users with a Home Team:

{{step-1-to-users}}

1. Select the user or users you want to associate with a Home Team.
1. Click the **[!UICONTROL More]** menu, then select **[!UICONTROL Edit]**.  
   ![](assets/user-settings-nwe-350x291.png)

1. In the **[!UICONTROL Organization]** section, select the **[!UICONTROL Home Team]** field. Start typing the name of the team whose settings you want to associate with the users. Click the name of the team when you see it in the list.

1. Click **[!UICONTROL Save Changes]**.  
   The users you selected are now associated with a Home Team.

   Any team settings, including the statuses associated with the [!UICONTROL Done] button are now visible to these users.
   
