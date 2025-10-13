---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'View: display the result of a calculation between two fields in a column'
description: You can use text mode in a column to display a calculation between two fields.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 303f8824-311a-4de0-9777-cfa11ecad1e1
---
# View: display the result of a calculation between two fields in a column

<!--Audited: 11/2024-->

You can use text mode in a column to display a calculation between two fields.

For example, if you want to find out the number of week days that elapsed between two dates, you can use text mode syntax and data expressions to calculate this difference.  
For example, you can calculate the week day difference between the Planned Completion Date and the Actual Completion Date of a task and display the result in a column.

You can use any other two dates in this calculation (Actual Start, Actual Completion, Projected Start, Projected Completion, etc).  
For more information about calculated data expressions, see [Overview of calculated data expressions](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>Contributor or Request to modify a filter </p>
   <p>Standard or Plan to modify a report</p>
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Reports, Dashboards, Calendars to modify a report</p> <p>Edit access to Filters, Views, Groupings to modify a filter</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p>  </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Display the result of a calculation between two fields in a column

To add this column to a task view:

1. Go to a list of tasks.
1. From the **View** drop-down menu, click **New View**.

1. Click **Add Column**, then **Switch to Text Mode** > **Edit Text Mode**.
1. Remove the text you find in the **Text Mode** box, and replace it with the following code:

   ```
   displayname=Week Day Difference
   textmode=true
   valueexpression=WEEKDAYDIFF({plannedCompletionDate},{actualCompletionDate})
   valueformat=HTML
   ```

1. (Optional) To aggregate the values displayed in the view in a grouping, follow the steps described in [Grouping: display the result of aggregating multiple calculated values in a grouping](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/grouping-calculation-between-two-fields-aggregated-in-grouping.md).
1. Click **Done**, then **Save View**.
