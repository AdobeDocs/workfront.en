---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'View: Actual Hours over Planned Hours in the same column of a task View'
description: In this task view, the actual amount of hours recorded on a task are displayed over the hours planned for each task. The Hours Variance between the Planned and the Actual Hours also displays in a separate column. 
author: Nolan
feature: Reports and Dashboards
exl-id: c1179283-dc2e-40d3-b8e0-4b1b79f83ad3
---
# View: Actual Hours over Planned Hours in the same column of a task View

In this task view, the actual amount of hours recorded on a task are displayed over the hours planned for each task. The Hours Variance between the Planned and the Actual Hours also displays in a separate column. 

![actual_vs_planned_in_task_report.png](assets/actual-vs-planned-in-task-report-350x58.png)

## Access requirements

<!--Audited: 10/2024-->

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

## View Actual Hours over Planned Hours in a task view

To apply this view:

1. Go to a list of tasks.
1. From the **View** drop-down menu, select **New View**.
1. In the**Column Preview** area, eliminate all columns except for one.
1. Click the header of the remaining column, then click **Switch to Text Mode**.
1. Mouse over the text mode area, and click **Edit Text Mode**.
1. Remove the text you find in the text mode box, and replace it with the following code:
   
   ```
   column.0.descriptionkey=name
   column.0.link.linkproperty.0.name=ID
   column.0.link.linkproperty.0.valuefield=ID
   column.0.link.linkproperty.0.valueformat=int
   column.0.link.lookup=link.view
   column.0.link.valuefield=objCode
   column.0.link.valueformat=val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.shortview=false
   column.0.stretch=100
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.viewalias=assignments
   column.1.displayname=
   column.1.linkedname=direct
   column.1.namekey=assignments
   column.1.valuefield=assignmentsListString
   column.1.valueformat=HTML
   column.1.tile.name=component.assignmentslist
   column.2.displayname=Actual/ Planned Hours
   column.2.linkedname=direct
   column.2.namekey=actualworkrequired
   column.2.querysort=actualWork
   column.2.textmode=true
   column.2.valueexpression=CONCAT({actualWorkRequired}/60,' / ',{workRequired}/60)
   column.2.valuefield=actualWorkRequired
   column.2.valueformat=compound
   column.2.viewalias=actualworkrequired
   column.3.aggregator.function=SUM
   column.3.aggregator.valueexpression=SUB({actualWork}, {workRequired})
   column.3.aggregator.valueformat=compound
   column.3.displayname=Hours Variance
   column.3.linkedname=direct
   column.3.textmode=true
   column.3.valueexpression=SUB({actualWork}, {workRequired})/60
   column.3.valueformat=customNumberAsString

   ```

1. Click **Done**, then **Save View**.
