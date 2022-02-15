---
filename: grouping-project-sponsor-hours
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
---




# Grouping: Project Sponsor for hours {#grouping-project-sponsor-for-hours}

This hour grouping organizes hours by the sponsor of the project where the hours are logged. The standard report builder interface for hour groupings does not provide a mapping to the Project Sponsor field. You must use the Text Mode interface to access this field.


![hour_report_grouped_by_sponsor.png](assets/hour-report-grouped-by-sponsor-600x66.png)




To apply this grouping:



1. Go to a list of hours.
1. From the **Grouping**&nbsp;drop-down menu, select **New Grouping**.

1. Click** Switch to Text Mode**.
1. Remove the text&nbsp;in the **Group your Report** area.
1. Replace&nbsp;the text with the following code:  
   `<pre>group.0.linkedname=project:sponsor:name<br>group.0.name=<br>group.0.valuefield=project:sponsor:name<br>group.0.valueformat=HTML<br>textmode=true</pre>`

1. Click **Save Grouping**.


