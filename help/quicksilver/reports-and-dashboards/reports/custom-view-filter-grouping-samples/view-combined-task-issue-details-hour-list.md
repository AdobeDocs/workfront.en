---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'View: Combined Task and Issue Details in an Hour List'
description: This hour view combines the Task and Issue Name columns, as well as the Task and Issue Planned Hours using the sharecol tag. Because an hour entry can only belong to either a task or issue, both objects cannot appear in the same column at the same time. Each line of the view populates with the information from either a Task or an Issue.
author: Nolan
feature: Reports and Dashboards
exl-id: cf1137fd-c26a-4907-afe9-2373d3434631
---
# View: combined task and issue details in an Hour list

<!--Audited:11/2024-->

This hour view combines the Task and Issue Name columns, as well as the Task and Issue Planned Hours using the `sharecol` tag. Because an hour entry can only belong to either a task or issue, both objects cannot appear in the same column at the same time. Each line of the view populates with the information from either a Task or an Issue.

To learn more about the `sharecol` tag, see [View: merge information from multiple columns in one shared column](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md). 

![custom_view_hours_with_task_and_issue_information.png](assets/custom-view-hours-with-350x48.png)

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
    <p>New:</p>
   <ul><li><p>Contributor to modify a filter </p></li>
   <li><p>Standard to modify a report</p></li> </ul>

   <p>Current:</p>
   <ul><li><p>Request to modify a filter </p></li>
   <li><p>Plan to modify a report</p></li> </ul></td> 
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

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## View combined task and issue details in an Hour list

1. Go to a list of hours.
1. From the **View** drop-down menu, click **New View**.
1. In the**Column Preview** area, eliminate all columns except for one.
1. Click the header of the remaining column, then click **Switch to Text Mode** > **Edit Text Mode**.
1. Remove the text you find in the **Edit Text Mode** box, and replace it with the following code:  

   ```
   column.1.querysort=project:name
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=project:name
   column.1.valueformat=HTML
   column.1.width=100
   column.2.description=Task or Issue
   column.2.link.linkproperty.0.name=ID
   column.2.link.linkproperty.0.valuefield=task:ID
   column.2.link.linkproperty.0.valueformat=int
   column.2.link.lookup=link.view
   column.2.link.valuefield=task:objCode
   column.2.link.valueformat=val
   column.2.linkedname=task
   column.2.listsort=nested(task).string(name)
   column.2.name=Task or Issue
   column.2.querysort=task:name
   column.2.sharecol=true
   column.2.shortview=false
   column.2.stretch=0
   column.2.valuefield=task:name
   column.2.valueformat=HTML
   column.2.width=100
   column.3.descriptionkey=optask
   column.3.link.linkproperty.0.name=ID
   column.3.link.linkproperty.0.valuefield=opTask:ID
   column.3.link.linkproperty.0.valueformat=int
   column.3.link.lookup=link.view
   column.3.link.valuefield=opTask:objCode
   column.3.link.valueformat=val
   column.3.linkedname=optask
   column.3.listsort=nested(opTask).string(name)
   column.3.namekey=opTask
   column.3.querysort=opTask:name
   column.3.shortview=false
   column.3.stretch=0
   column.3.valuefield=opTask:name
   column.3.valueformat=HTML
   column.3.width=1
   column.4.valuefield=task:work
   column.4.sharecol=true
   column.4.linkedname=task
   column.4.valueformat=doubleAsInt
   column.4.namekey=view.relatedcolumn
   column.4.querysort=task:work
   column.4.textmode=true
   column.4.namekeyargkey.0=task
   column.4.namekeyargkey.1=work
   column.4.displayname=Planned Effort
   column.5.displayname=Planned Effort
   column.5.viewalias=opTask:workrequired
   column.5.linkedname=opTask
   column.5.valuefield=opTask:workRequired
   column.5.valueformat=compound
   column.5.querysort=opTask:workRequired
   column.5.namekeyargkey.0=opTask
   column.5.namekeyargkey.1=workrequired
   column.5.namekey=view.relatedcolumn
   column.5.textmode=true
   column.6.descriptionkey=hours
   column.6.linkedname=direct
   column.6.listsort=doubleAsDouble(hours)
   column.6.namekey=hours.abbr
   column.6.querysort=hours
   column.6.shortview=false
   column.6.stretch=0
   column.6.valuefield=hours
   column.6.valueformat=doubleAsString
   column.6.width=75
   column.7.descriptionkey=entrydate
   column.7.linkedname=direct
   column.7.listsort=atDateAsAtDate(entryDate)
   column.7.namekey=entrydate.abbr
   column.7.querysort=entryDate
   column.7.shortview=false
   column.7.stretch=0
   column.7.valuefield=entryDate
   column.7.valueformat=atDate
   column.7.width=75
   column.8.descriptionkey=description
   column.8.linkedname=direct
   column.8.listsort=string(description)
   column.8.namekey=description.abbr
   column.8.querysort=description
   column.8.shortview=false
   column.8.stretch=0
   column.8.valuefield=description
   column.8.valueformat=HTML
   column.8.width=150

   ```

1. Click **Done** > **Save View**.
1. (Optional) Update the view name, then click **Save View**.
