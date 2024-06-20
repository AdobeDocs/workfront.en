---
product-area: agile-and-teams
navigation-topic: get-started-with-agile-in-workfront
title: Create an agile team
description: Adobe Workfront enables agile teams to complete work in an incremental, organized way.
author: Lisa
feature: Agile
exl-id: 3afd16db-7829-4c9c-a981-461990c9dbc8
---
# Create an agile team

<!--Audited: 01/2024-->

[!DNL Adobe Workfront] enables agile teams to complete work in an incremental, organized way.

Any user in the organization can see the agile team and view all agile components for the team, including the backlog, iterations, story board, and individual stories. However, only members of the team with [!UICONTROL Edit] access to work can make changes to work assigned to the team.

[!DNL Workfront] supports the following agile methodologies:

* **[!UICONTROL Scrum]**: Teams have a backlog of work that needs to be done. When the team is ready to work on a specific chunk of work, the work is moved from the backlog to an iteration. For more detailed information about managing a Scrum team, see [Scrum in an agile team](../../agile/use-scrum-in-an-agile-team/scrum-in-an-agile-team.md).

* **[!UICONTROL Kanban]:** Teams move work in the Kanban view across predetermined statuses. Default statuses are: backlog, in-process, and done. For more detailed information about managing a Kanban team, see [Kanban in an agile team](../../agile/use-kanban-in-an-agile-team/using-kanban-in-an-agile-team.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

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
   <td> <p>New: Standard</p>
   Current: 
   <ul><li><p>[!UICONTROL Plan] to create a new agile team</p></li> 
   <li><p>[!UICONTROL Work] or higher to convert a team to an agile team</p></li></ul> </td> 
  </tr> 
 </tbody> 
</table>

To find out what plan or license type you have, contact your [!DNL Workfront] administrator.

+++

## Decide on an agile methodology

You can use either a Scrum or Kanban agile methodology for your agile team. Each methodology provides various benefits. The way your agile team works determines the agile methodology you choose to use.

Both Scrum and Kanban agile methodologies in [!DNL Workfront] allow you to move stories across a story board to indicate a status change and progress of the story.

Scrum and Kanban agile methodologies in [!DNL Workfront] differ in the following ways:

### Benefits of using Kanban in [!DNL Workfront]

The [!DNL Kanban] agile methodology in [!DNL Workfront] enables you to more easily move stories across an agile story board while limiting the amount of work in progress. There are no start and end dates when using the [!DNL Kanban] agile methodology.

The following functionality supports this methodology:

* Display the backlog on the [!DNL Kanban] agile story board.\
   For more information, see [Add the backlog to the [!UICONTROL Kanban] board](../../agile/use-kanban-in-an-agile-team/view-the-backlog-on-the-kanban-board.md).

* Configure items on the backlog to be automatically added to the [!UICONTROL Kanban] agile story board when other items are moved to a status that equates with Complete.\
   For more information, see the section [Configure stories to be automatically added from the backlog](../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5) in the article [Configure Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).

* Configure a Work In Progress (WIP) limit to be displayed on the [!UICONTROL Kanban] agile story board.\
   For more information, see [Manage the work in progress (WIP) limit on the Kanban board](../../agile/use-kanban-in-an-agile-team/work-in-progress-limit-on-the-kanban-board.md).

### Benefits of using Scrum in [!DNL Workfront]

The Scrum agile methodology in [!DNL Workfront] enables you to add a set of stories to an agile iteration and create a story board for that iteration. The iteration is based on the start and end dates that you define.

The following functionality supports this methodology:

* Include issues on the [!UICONTROL Scrum] story board
* Include issues on the backlog of an agile team
* Subtasks can be displayed on the [!UICONTROL Scrum] story board
* View a burndown chart to see progress against stories during the iteration\
   For more information, see [Agile burndown chart overview](../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

## Create an agile team

{{step1-to-team}}

1. Click the **[!UICONTROL Switch Teams]** icon ![Switch team icon](assets/switch-team-icon.png), then click **[!UICONTROL Create new team]**.

   ![Select Create new team.](assets/create-new-team-350x198.png)

   The New Team box displays.

1. Specify the following information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Team Name]</strong> </td> 
      <td>Type a name for the new agile team.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL This is an Agile Team]</strong> </td> 
      <td>Select this option to configure this new team to be an agile team.</td> 
     </tr> 

      <tr> 
      <td role="rowheader"><strong>[!UICONTROL Is Active]</strong> </td> 
      <td>Select this option to activate this team. Inactive teams are not visible to other users to assign to work. </td> 
     </tr> 


     <tr data-mc-conditions="QuicksilverOrClassic.Quicksilver"> 
      <td role="rowheader"><strong>[!UICONTROL Group]</strong> </td> 
      <td> <p>Begin typing the name of a group to add to the team, then select the name when it appears in the drop-down list.</p> <p><b>NOTE</b></p> <p> When a team is assigned to a group or subgroup, any group administrators of that group or subgroup can manage the team without being a member of the team. Group administrators can go to the [!UICONTROL Teams] area from the [!UICONTROL Main Menu] and click the [!UICONTROL Switch Teams] arrow <img src="assets/switch-team-icon.png" alt="Switch team icon"> to list all of the teams that are assigned to the groups that they manage.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Team Members]</strong> </td> 
      <td>Begin typing the name of a user to be on the team, then select the name when it appears in the drop-down list.<br>Repeat this process to add multiple users to the team.<br>Because users can be on more than one team, they can be on both agile and non-agile teams.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Description]</strong> </td> 
      <td><p>Type a description for the team.</p> <p>The description displays on the top right of the [!UICONTROL Teams] area when the team is selected.</p>
      <p>If the description is long, you can click it to display the full description in a pop-up. If you have access to edit the [!UICONTROL team settings], you can also edit the description directly in the pop-up.</p></td>
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Create]**.

   For information on configuring an Agile team, see the following articles:

   * [Configure [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Configure [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## Convert an existing team into an agile team

You can convert an existing team to be an agile team:

1. Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of [!DNL Adobe Workfront], then click **[!UICONTROL Teams]**.
1. Click the **[!UICONTROL Switch team]** icon ![Switch team icon](assets/switch-team-icon.png), then either select a new team from the drop-down menu or search for a team in the search bar.

1. Select the team that you want to convert to an agile team.
1. Click the **[!UICONTROL More]** menu, then select **[!UICONTROL Edit]**.\
   Only team members with either a [!UICONTROL Plan] or [!UICONTROL Work] license see this option.\
   ![](assets/edit-team-settings-350x205.png)

1. In the **[!UICONTROL Agile]** section, select **[!UICONTROL This is an Agile Team]**.

1. In the **[!UICONTROL Methodology]** section, select whether the team will be using a **[!UICONTROL Scrum]** or **[!UICONTROL Kanban]** agile methodology.

1. Click **Save Changes.**

   The team is saved as an Agile team. You can configure the new team as a Scrum or a Kanban team when you edit the team. 

   For more information, see the following articles:

   * [Configure [!UICONTROL Kanban]](../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
   * [Configure [!UICONTROL Scrum]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)
