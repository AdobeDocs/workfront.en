---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Add Stories to an Existing Iteration
description: You can add stories to an iteration in many ways.
author: Lisa
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
---
# Add stories to an existing iteration

You can add stories to an iteration in any of the following ways:

* From the backlog after the iteration is created, as described in the [Move stories from the backlog to an iteration or [!UICONTROL Kanban] board](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#move-stories-from-the-backlog-to-an-iteration-or--board) section in [Manage the agile backlog](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)

* From the [!UICONTROL Details] page of the individual task or issue
* From a task or issue list
* From a report
* From a dashboard

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

## Understand how adding stories affects task dates

By default, when you add an existing task to an iteration, the task's [!UICONTROL Planned Start Date] and [!UICONTROL Planned Completion Date] are set as follows:

### Task [!UICONTROL Planned Start Date]

* The task uses the iteration's Start Date when:

   * The project does not have a [!UICONTROL Planned Start Date] set.
   * The project's [!UICONTROL Planned Start Date] is *before* or *on* the iteration's start date.

* The task uses the project's [!UICONTROL Planned Start Date] when:

   * The project's [!UICONTROL Planned Start Date] is *after* the iteration's start date.

### Task [!UICONTROL Planned Completion Date]

* The task uses the iteration's End Date when:

   * The project does not have a [!UICONTROL Planned Completion Date] set.
   * The project's [!UICONTROL Planned Start Date] is *before or on* the iteration's Start Date or the Project's [!UICONTROL Planned Completion Date] is *before or on* the iteration's End Date.

* The task uses the project's [!UICONTROL Planned Completion Date] when:

   * The project's [!UICONTROL Planned Start Date] is *after* the iteration's Start Date and the project's [!UICONTROL Planned Completion Date] is *after* the iteration's End Date.

You can configure individual Scrum teams to use the project dates by default, rather than the iteration dates. For information, see the section [Configure how dates are applied when adding work items to an iteration](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration) in the article [Configure Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Add a story to an existing iteration

You can add any task or issue to any iteration if you have Manage access to the project. Keep the following in mind when moving a task or issue to an iteration:

* If you add multiple teams, the task or issue can display only on one team's iteration. This is the iteration you choose in step 3 below.
* If the task or issue is assigned to an agile team and moved to another team's iteration, the team assignment does not change.
* If the task or issue is not assigned to a team, the task or issue is assigned to the team who owns the iteration.
* You can't add parent tasks to the iteration. If you add any child tasks, the parent task appears on the Scrum board as a swimlane.

>[!IMPORTANT]
>
>After the task moves to the iteration, you cannot update the [!UICONTROL Duration Type] or [!UICONTROL Task Constraint]. [!UICONTROL Duration Type] is set to [!UICONTROL Simple] and [!UICONTROL Task Constraint] is set to [!UICONTROL Fixed Dates] to keep the task timeline consistent with the iteration's timeline.

1. Open the task or issue you want to add to an iteration.
   Or
   Go to the project, report, or dashboard that contains the task or issue you want to add to an iteration. Then, select one or more tasks or issues.

1. Click **[!UICONTROL More]** ![](assets/more-icon.png) > **[!UICONTROL Add to Iteration]**.
   You cannot assign tasks or issues assigned to non-agile teams.

1. In the **[!UICONTROL Add To]** box, begin typing the name of the iteration, and select it when it appears in the list.

   >[!NOTE]
   >
   >You can move a story from an existing iteration to a new iteration.

1. Click **[!UICONTROL Add]**.
