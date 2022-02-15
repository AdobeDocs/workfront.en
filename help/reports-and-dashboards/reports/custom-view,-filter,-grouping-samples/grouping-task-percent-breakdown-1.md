---
filename: grouping-task-percent-breakdown-1
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
---




# Grouping: task percent breakdown 1 {#grouping-task-percent-breakdown}

In this custom project grouping, you can display projects grouped by a range of their percent complete values. The breakdowns show percent complete value of 25 percent point increments: 0-25%, 25-50%, etc.&nbsp;


The following grouping organizes tasks by the percent complete value into one of six groupings:



* 0%
* 1-25%
* 26-50%
* 51-75%
* 76-99%
* 100%


![task_25__breakdown_grouping.png](assets/task-25--breakdown-grouping.png)




To apply this grouping:



1. Go to a list of tasks.
1. From the **Grouping**&nbsp;drop-down menu, select **New Grouping**.

1. Click** Switch to Text Mode**.
1. Remove the text&nbsp;in the **Group your Report** area.
1.  Replace&nbsp;the text with the following code:
   `<pre>group.0.linkedname=direct<br>group.0.name=Percent Breakdown<br>group.0.notime=false<br>group.0.valueexpression=IF({percentComplete}=0,"0 %",IF({percentComplete}<=26,"0-25 %",IF({percentComplete}<=51,"25-50 %",IF({percentComplete}<=76,"50-75 %",IF({percentComplete}<100,"75-99 %","100 %")))))<br>group.0.valueformat=string</pre>` 

1. Click **Save Grouping**.


