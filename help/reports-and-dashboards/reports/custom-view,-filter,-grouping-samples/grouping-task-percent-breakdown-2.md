---
filename: grouping-task-percent-breakdown-2
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
---




# Grouping: task percent breakdown 2 {#grouping-task-percent-breakdown}

In this custom task&nbsp;grouping, you can display tasks&nbsp;grouped by a range of their percent complete values. The breakdowns show percent complete value of 10&nbsp;percent point increments: 1-10%, 11-20%, etc.


The following grouping organizes projects by the percent complete value into one of these&nbsp;groupings:



* 0%
* 1-10%
* 11-20%
* 21-30%
* 31-40%
* 41-50%
* 51-60%
* 61-70%
* 71-80%
* 81-90%
* 91-99%
* 100%


![task_10__breakdown_grouping.png](assets/task-10--breakdown-grouping.png)




To apply this grouping:



1. Go to a list of tasks.
1. From the **Grouping**&nbsp;drop-down menu, select **New Grouping**.

1. Click** Switch to Text Mode**.
1. Remove the text&nbsp;in the **Group your Report** area.
1. Replace&nbsp;the text with the following code:  
   `<pre>group.0.linkedname=direct<br>group.0.name=Percent Breakdown<br>group.0.notime=false<br>group.0.valueexpression=IF({percentComplete}=0,"0 %",IF({percentComplete}<=11,"1-10 %",IF({percentComplete}<=21,"11-20 %",IF({percentComplete}<=31,"21-30 %",IF({percentComplete}<41,"31-40 %",IF({percentComplete}<51,"41-50 %",IF({percentComplete}<61,"51-60 %",IF({percentComplete}<71,"61-70 %",IF({percentComplete}<81,"71-80 %",IF({percentComplete}<91,"81-90 %",IF({percentComplete}<100,"91-99 %","100 %")))))))))))<br>textmode=true</pre>`

1. Click **Save Grouping**.


