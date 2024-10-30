---
content-type: overview
product-area: agile-and-teams
navigation-topic: burndown
title: Iteration Completion Status Overview
description: The completion information described in this article is displayed above the burndown chart.
author: Lisa
feature: Agile
exl-id: cc6bebdb-f2aa-4e85-9f9f-15e7753d84cb
---
# Iteration completion status overview

The completion information described in this article is displayed above the burndown chart.

Completion percentage on an iteration:

![](assets/burndown-percentcomplete-350x47.png)

This information indicates the completion status of the iteration for the day that is currently selected in the burndown chart. By default, the completion status is displayed based on the current day's date.

The following information is available:

* **[!UICONTROL Percent Complete]:** Overall progress of the iteration

   [!UICONTROL Percent Complete] adjusts based on the percent complete of each story or task within the iteration, including stories or tasks that are only partially complete.

   The color of the [!UICONTROL Percent Complete] status bar displays as red or green to match the color of the actual burndown rate. It is shown in red when the burndown rate is less than the ideal (more points or hours remaining per day than the ideal burndown calculation), and it is shown in green when the burndown rate is equal to or better than the ideal (equal or fewer points remaining per day than the ideal burndown calculation).

* **[!UICONTROL Completed Stories]:** (Available only in iterations) The number of stories marked [!UICONTROL Complete]. This is shown in relation to the total number of stories in the iteration. For example, "3 of 6" indicates that 3 of the 6 stories in the iteration have been marked [!UICONTROL Complete].
* **[!UICONTROL Completed Points / Hours]:** (Available only in iterations) The number of points or hours marked [!UICONTROL Complete]. Shown in relation to the total number of points or hours in the iteration. For example, "5 of 11" indicates that 5 of the 11 stories in the iteration have been marked [!UICONTROL Complete]. This number is directly related to the [!UICONTROL Percent Complete] calculation, and is updated at the same time [!UICONTROL Percent Complete] is updated.

   Points and hours are associated with stories. When a story is marked [!UICONTROL Complete], the points or hours associated with that story are marked Complete.

   By default, points are used. You can change this by modifying the settings for your team, as described in [Create an agile team](../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

* **[!UICONTROL Points / Hours Per Day]:** (Available only in iterations) The average number of points or hours marked [!UICONTROL Complete] each day since the beginning of the iteration through the current day.

   This is calculated by the total points or hours complete, divided by the total number of days through the current day. (Partial days are recorded as a whole day.)

   This information can be useful when planning a future iteration.

* **[!UICONTROL Estimated Completion]:** The estimated date that the iteration will be completed, based on the current rate in the Points / Hours Per Day (for iterations).

   When the [!UICONTROL Estimated Completion] date is later than the end date defined for the iteration, the number of working days remaining is displayed as red in parenthesis next to the [!UICONTROL Estimated Completion] date.

   When the [!UICONTROL Estimated Completion] date is earlier than the planned end date of the iteration, the number of working days remaining is displayed in green. (The end date for the iteration is specified when the iteration is planned, as described in [Create an iteration](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md); the end date for the project is the [!UICONTROL Planned Completion Date], or it is the current date if the [!UICONTROL Planned Completion Date] is in the past. The [!UICONTROL Planned Completion Date] for the project is calculated based on the duration of tasks in the project.) When planning the iteration, if you set the iteration end date for a non-working day and the iteration is tracking to finish on time, the Estimated Completion date is set for the last working day prior to the iteration end date that you set (because work is not scheduled to be burned down on non-working days).

   For example, "(+9 days)" indicates that the Estimated Completion date is 9 working days later than the iteration's planned end date.

   For more information, see [Iteration completion status overview](#Understanding-How-Days-Off-Affect-the-Burndown-Chart).
