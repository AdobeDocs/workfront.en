---
filename: filter-report-delivery-filter
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
---




# Filter: report delivery filter {#filter-report-delivery-filter}

This report filter displays all reports scheduled to be delivered automatically in `Workfront`. It is best used with the standard View.


To apply this filter:



1. Go to a list of reports.
1. From the **Filter**&nbsp;drop-down menu, select **New Filter**.

1. Click** Switch to Text Mode**.
1. In the **Set Filter Rules for your Report** area, copy and paste the following code:  


   ```
   scheduledReportID=0<br>scheduledReportID_Mod=notnull
   ```


1. Click **Save Filter**.


&nbsp;


&nbsp;
