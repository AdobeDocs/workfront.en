---
filename: iteration-completion-status-overview
content-type: overview
product-area: agile-and-teams
navigation-topic: burndown
---



# Iteration completion status overview {#iteration-completion-status-overview}

The completion information described in this section is&nbsp;displayed above the burndown&nbsp;chart.


Completion percentage on&nbsp;an iteration: 


![](assets/burndown-percentcomplete-350x47.png)




This information&nbsp;indicates the completion status of&nbsp;the iteration for the day that is currently selected in the burndown chart. By default, the completion status is displayed based on the current day's date.


The following information is available:



*  `Percent Complete:`&nbsp;Overall progress of the iteration . 


  Percent Complete adjusts based on the percent complete of each story or task within the iteration , including&nbsp;stories or tasks that are only partially complete.


  The color of the Percent Complete status bar displays as red or green to&nbsp;match&nbsp;the color of the actual burndown rate. It is&nbsp;shown in red&nbsp;when the burndown rate is less than the ideal (more points or hours remaining per day than the ideal burndown calculation), and it is shown in&nbsp;green&nbsp;when the burndown&nbsp;rate is equal to or better than the ideal (equal or fewer points remaining per&nbsp;day than the ideal burndown calculation).

* `Completed Stories:`&nbsp;(Available only in iterations) The number of stories marked Complete. This is shown in relation to the total number of stories in the iteration. For example, "3 of 6" indicates that 3 of the 6 stories in the iteration have been marked Complete.
*  `Completed Points / Hours:`&nbsp;(Available only in iterations) The number of points or hours marked Complete. Shown in relation to the total number of points or hours in the iteration. For example, "5 of 11" indicates that 5 of the 11 stories in the iteration have been marked Complete. This number is directly related to the Percent Complete calculation, and&nbsp;is updated at the same time Percent Complete is updated.


  Points and hours&nbsp;are associated with stories. When a story is marked Complete, the points or hours associated with that story are marked Complete.&nbsp;


  By default, points are used. You can change this by modifying the settings for your team, as described in [Create an agile team](create-an-agile-team.md).

*  `Points / Hours Per Day:`&nbsp;(Available only in iterations) The average number of points or hours marked Complete each day since the beginning of the iteration through the current day.


  This is calculated by the total points or hours complete, divided by the total number of days through the current day. (Partial days are recorded as a whole day.)


  This information can be useful when planning a future iteration.

*  `Estimated Completion:` The estimated date&nbsp;that the iteration will be completed, based on the current rate in the Points / Hours Per Day (for iterations). 


  When the Estimated Completion date is later than the end date defined for the iteration , the number of working days remaining is&nbsp;displayed as&nbsp;red in parenthesis next to the Estimated Completion date.


  When the Estimated Completion date is&nbsp;earlier than the planned end date of the iteration , the number of working days remaining is&nbsp;displayed in green.&nbsp;(The end date for the iteration is specified when the iteration is planned, as described in [Create an iteration](create-an-iteration.md); the end date for the project is the Planned Completion Date, or it is the current date if the Planned Completion Date is in the past. The Planned Completion Date for the project is calculated based on the duration of tasks in the&nbsp;project.) When planning the iteration, if you set the iteration end date for a non-working day and the iteration is tracking to finish on time, the Estimated Completion date is set for the last working day prior to the iteration end date that you set (because work is not scheduled to be burned down on non-working days).


  For example, "(+9 days)"&nbsp;indicates that the Estimated Completion date is 9 working days later than the iteration's planned end date.


  For more information, see [Iteration completion status overview](#understanding-how-days-off-affect-the-burndown-chart).



