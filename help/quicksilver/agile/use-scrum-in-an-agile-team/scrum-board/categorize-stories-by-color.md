---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Categorize stories by color on the Scrum board
description: The default color association of Scrum board stories differs depending on whether the story board is located on an iteration or on a project.
author: Lisa
feature: Agile
exl-id: 8e351505-73d1-4c8f-b369-53c965b88c95
---
# Categorize stories by color on the Scrum board

## Change the default color association of stories

The default color association of stories differs depending on whether the story board is located on an iteration or on a project:

* **Iteration**: On an iteration, story board tiles are color-coded according to the project the story is associated with. (Each project is arbitrarily assigned a color on the story board.) You can change this default behavior for each agile team. Colors for agile stories on an iteration can be tied to the project (default), story priority, owner, or free form. For more information, see [Configure how color indicators are used for stories on the agile story board](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur4) in the article [Configure Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

* **Project**: On a project, any subtasks match the color of the parent task, so that the colors of all stories in any given swimlane are the same. Colors are randomly assigned to tasks when they are created if the task does not have any subtasks or does not have a parent task. You can change this default behavior by modifying the agile view. Colors for agile stories on a project can be tied to the parent story (default), story priority, owner, or free form. For more information, see [Create or customize an Agile view](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) in [Views overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] license*</strong></td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations*</strong></td> 
   <td> <p>Worker or higher</p> <p>Note: If you still don't have access, ask your [!DNL Workfront] administrator if they set additional restrictions in your access level. For information on how a [!DNL Workfront] administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

## Change the color of stories when using free form

If the agile team settings have been configured so the [!UICONTROL Associate Card Color to] option is set to Free Form, users can manually change the color of individual story tiles. This can be useful to communicate other types of information that is important to the team or the organization:

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of [!DNL Adobe] Workfront, then click **Teams**.

1. (Optional) Click the **Switch team** icon ![Switch team icon](assets/switch-team-icon.png), then either select a new Scrum team from the drop-down menu or search for a team in the search bar.

1. In the left panel, select **[!UICONTROL Iterations]** to choose a specific iteration, or select **Current Iteration**.
1. Hover over the colored banner at the top of the story tile.

   ![](assets/agile-story-color1-nwe-350x140.png)

1. Click **[!UICONTROL Change color]**, then select the desired color.

   ![](assets/agile-story-color2-nwe-350x138.png)
