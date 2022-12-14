---
product-area: agile-and-teams;projects
navigation-topic: use-kanban-in-an-agile-team
title: Use flags on stories on the Kanban board
description: On the [!DNL Kanban] board, flags provide a visual indication of when a story is ready to move to the next status. This enables Kanban teams to use a "pull" approach rather than a "push" approach when moving stories across statuses.
author: Lisa
feature: Agile
exl-id: e19a007d-737c-42d4-aa69-771d8a9e9fd8
---
# Use flags on stories on the [!UICONTROL Kanban] board

On the [!DNL Kanban] board, flags provide a visual indication of when a story is ready to move to the next status. This enables [!UICONTROL Kanban] teams to use a "pull" approach rather than a "push" approach when moving stories across statuses.

**Example:** Consider the following example of a team using a "pull" approach: Olivia, the graphic designer on the team, finishes her work and then sets the story flag as "[!UICONTROL Ready to Pull]." This flag provides a visual indication to Tony, the copywriter on the team, that the story is ready for him to move to the next status. Tony then moves the story to the next status when he is ready to begin working on it.

Consider the following when using flags on stories:

* Flags are not a status, but rather a visual indication that the story is ready to be moved to the next status by another member of the team.
* Flags do not appear on any story cards that are in the [!UICONTROL Backlog] column or in the [!UICONTROL Complete] column (or in any column where the status of the column equates with [!UICONTROL Complete]).

   For more information about story statuses, see [Use flags on stories on the Kanban board](#updating-the-status-of-stories-and-subtasks)

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>[!UICONTROL Work] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations*</strong></td> 
   <td> <p>[!UICONTROL Worker] or higher</p> <p>Note: If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

## Use flags on stories on the [!UICONTROL Kanban] board

To change a flag on a story:

1. Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of [!DNL Adobe Workfront], then click **[!UICONTROL Teams]**.

1. (Optional) Click the **[!UICONTROL Switch team]** icon ![Switch team icon](assets/switch-team-icon.png), then either select a new [!UICONTROL Kanban] team from the drop-down menu or search for a team in the search bar.

1. Go to the [!UICONTROL Kanban] board where you want to change a flag on a story.
1. Expand the story tile to view the flag.\
   The flag is set to **[!UICONTROL On Track]** for each story by default.\
   ![Kanban card](assets/agile-storycard-kanban-2021-350x308.png)

1. Click the current flag, then select from the following flag options:

   * **[!UICONTROL On Track]:** The story is in the appropriate status and no action needs to be taken at this time.\

      This is the default flag for each story on the Kanban board.\
      ![kanban_flag_ontrack.png](assets/kanban-flag-ontrack.png)

   * **[!UICONTROL Is Blocked]:** The story cannot proceed to the next status. When this flag is set on a story, the story does not count toward the WIP limit. (For more information about WIP limits, see&nbsp;the article [Configure Kanban](../../agile/get-started-with-agile-in-workfront/configure-kanban.md).\

      ![kanban_flag_blocked.png](assets/kanban-flag-blocked.png)

   * **[!UICONTROL Ready to Pull]:** The story is ready to be moved to the next status by another member of the team.\

      ![kanban_flag_ready.png](assets/kanban-flag-ready.png)
