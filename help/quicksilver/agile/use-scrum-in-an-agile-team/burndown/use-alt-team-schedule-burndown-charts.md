---
product-area: agile-and-teams
navigation-topic: burndown
title: Use an Alternate Team Schedule for Burndown Charts
description: Schedules that are defined in [!DNL Adobe Workfront] affect the burndown chart by excluding days off (weekends and holidays) from the burndown.
author: Lisa
feature: Agile
exl-id: 72650c19-434d-463a-8924-49219604ff01
---
# Use an alternate team schedule for burndown charts

Schedules that are defined in [!DNL Adobe Workfront] affect the burndown chart by excluding days off (weekends and holidays) from the burndown.

By default, the burndown chart uses the default schedule. In addition to the default schedule, agile teams can choose to also use an alternate schedule in order to incorporate team-specific non-working days. This alternate schedule is then reflected in the burndown chart of any iteration that is assigned to the team. The alternate schedule affects only the burndown chart. (For more information about the default schedule, as well as how the [!DNL Workfront] administrator can create a team-specific schedule, see [Create a schedule](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).)

The burndown chart does not take partial days into consideration. For example, if your team works 4 hours each Friday, it's represented as a full day in the burndown chart.

For more information about using the burndown chart, see the [Agile burndown chart overview](../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md).

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
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td> <p>New: [!UICONTROL Standard]</p> 
   or
   <p>Current: [!UICONTROL Work] or higher</p> </td> 
  </tr>
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Use an alternate team schedule for burndown charts

1. Ensure that the [!DNL Workfront] administrator has already created the alternate schedule, as described in [Create a schedule](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

{{step1-to-team}}

1. (Optional) Click the **[!UICONTROL Switch team]** icon ![Switch team icon](assets/switch-team-icon.png), then either select a new Scrum team from the drop-down menu or search for a team in the search bar.

1. Select the agile team that you want to manage.
1. Click the **[!UICONTROL More]** menu, then select **[!UICONTROL Edit]**.

1. In the **[!UICONTROL Agile]** section, in the **[!UICONTROL Schedule]** area, select the new schedule from the drop-down menu.

1. Click **[!UICONTROL Save Changes]**.
