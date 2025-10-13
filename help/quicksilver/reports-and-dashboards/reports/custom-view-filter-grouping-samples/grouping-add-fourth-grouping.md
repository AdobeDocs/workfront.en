---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Grouping: add a fourth grouping to a list'
description: You can have 4 groupings in a matrix report. For more information about matrix reports, see Create a matrix report.
author: Nolan
feature: Reports and Dashboards
exl-id: 1147a47b-c6e2-496e-b202-eefeb500054e
---
# Grouping: add a fourth grouping to a list

<!--Audited: 10/2024-->

You can have 4 groupings in a matrix report. For more information about matrix reports, see [Create a matrix report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

You can only have 3 groupings in a standard report through the standard interface. To add a 4th grouping in a standard report, you must use text mode.

![Four_groupings_in_a_standard_report.png](assets/four-tier-grouping-for-tasks-350x239.png)

For example, you might have a task report which is grouped by Project Name, Progress Status and Planned Completion Date, but you also want to group the report by Assigned To Name.

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

## Add a fourth grouping to a list

To add a fourth grouping:

1. Click **Switch to Text Mode**.
1. Remove the text in the **Group your Report** area.
1. Replace the text in the box displayed with the following code: 

   ```
   group.0.linkedname=project<br>group.0.namekey=view.relatedcolumn<br>group.0.namekeyargkey.0=project<br>group.0.namekeyargkey.1=name<br>group.0.valuefield=project:name<br>group.0.valueformat=string<br>group.1.enumclass=com.attask.common.constants.ProgressStatusEnum<br>group.1.enumtype=TASK<br>group.1.linkedname=direct<br>group.1.namekey=progressStatus<br>group.1.type=enum<br>group.1.valuefield=progressStatus<br>group.1.valueformat=val<br>group.2.groupdatesby=WY<br>group.2.linkedname=direct<br>group.2.namekey=plannedCompletionDate<br>group.2.notime=false<br>group.2.valuefield=plannedCompletionDate<br>group.2.valueformat=atDateAsWeekString<br><strong>group.3.valuefield=assignedTo:name</strong><br style="font-weight: bold;"><strong>group.3.valueformat=HTML</strong><br>textmode=true
   ```

1. Click **Done**, then **Save Grouping**.
1. (Optional) Update the name for the grouping, then click **Save Grouping**.
