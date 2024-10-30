---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Create an Agile story in an Iteration
description: This article describes how to create a new agile story when you are already in the iteration.
author: Lisa
feature: Agile
exl-id: 9712e065-5fbf-4deb-a39f-36e0e918ed12
---
# Create an agile story in an iteration

This article describes how to create a new agile story when you are already in the iteration. For information about creating an agile story from a task, issue, or other area of [!DNL Adobe Workfront], see [Add stories to an existing iteration](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td> <p>New: [!UICONTROL Standard]</p> 
   or
   <p>Current: [!UICONTROL Work] or higher</p> </td> 
  </tr>
   <tr> 
   <td role="rowheader">Object permissions</td> 
   <td>[!UICONTROL Manage] access to the project the story is on </td> 
  </tr>
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Create an agile story in an iteration

1. Go to the agile iteration where you want to create the story:

   {{step1-to-team}}

   1. (Optional) Click the **[!UICONTROL Switch team]** icon ![Switch team icon](assets/switch-team-icon.png), then either select a new Scrum team from the drop-down menu or search for a team in the search bar.

   1. In the left panel, select **[!UICONTROL Iterations]**.
   1. Click the name of the specific iteration where you want to create a story.
   1. In the left panel, select **[!UICONTROL Stories]**.

1. &nbsp;Click **[!UICONTROL New Story]**.
1. Specify the following information:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Story Name]</strong></td>
      <td>Type a name for the story.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Description]</strong></td>
      <td>Type a description for the story.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Ready]</strong></td>
      <td>Select this option if the story is ready to be added to an iteration. When this option is selected, it indicates to users which stories in the backlog are ready to be added to an iteration.<br>A story can be added to an iteration whether or not it is marked <strong>[!UICONTROL Ready].</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimate] (points)</strong></td>
      <td>Specify the estimate for the story. If your agile team is configured to estimate stories in points, then by default 1 point equals 8 hours. Estimates are added as [!UICONTROL Planned Hours] on the story.<br>For example, if you estimate a story as 3 points, the default behavior is to add 24 Planned Hours to the story.<br>If a story contains subtasks, remember that the combined estimates for all subtasks determines the estimate of the parent story. For more information, see <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/add-a-subtask-to-an-existing-story-scrum.md" class="MCXref xref">Add a subtask to an existing story on the [!UICONTROL Scrum] board</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Project]</strong></td>
      <td>Begin typing the name of the project that this story will be associated with.<br>By default, the story color is displayed as the same color as other stories from this project.<br>The status of the project must be set to [!UICONTROL Current]. If the status of the project is anything but [!UICONTROL Current], it is not displayed in the drop-down menu.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Task]</strong></td>
      <td>After you choose a parent project, you have the option to choose a parent task. When you select a parent task, the story is created as a subtask of the parent task on the project that you selected.<br>Begin typing the name of the parent task for the story, then click it when it appears in the drop-down list.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom Forms]</strong></td>
      <td>Select any custom forms to add to the story.</td>
     </tr>
    </tbody>
   </table>

1. Click **[!UICONTROL Save Story]**.
