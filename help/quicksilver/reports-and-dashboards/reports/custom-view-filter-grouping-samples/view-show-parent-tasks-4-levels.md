---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'View: Show Parent Tasks up to 4 Levels Deep'
description: This task view shows the task name in the first column and (if they exist) up to 4 parent tasks in separate columns in the same list.
author: Nolan
feature: Reports and Dashboards
exl-id: 66b45d64-794d-4adc-b208-2ded0dc9c5dc
---
# View: show parent tasks up to 4 levels deep

<!--Audited: 11/2024-->

This task view shows the task name in the first column and (if they exist) up to 4 parent tasks in separate columns in the same list.

![parent_tasks_4_levels_deep.png](assets/parent-tasks-4-levels-deep-350x29.png)

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
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p> Current: 
   <ul>
   <li>Request to modify a view</li> 
   <li>Plan to modify a report</li>
   </ul>
     </p>
     <p> New: 
   <ul>
   <li>Contributor to modify a view</li> 
   <li>Standard to modify a report</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Reports, Dashboards, Calendars to modify a report</p> <p>Edit access to Filters, Views, Groupings to modify a view</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Show parent tasks up to 4 levels deep

1. Go to a list of tasks.
1. From the **View** drop-down menu, select **New View**.
1. In the **Column Preview** area, eliminate all columns except for one.
1. Click the header of the remaining column, then click **Switch to Text Mode** > **Edit Text Mode**.
1. Remove the text you find in the **Text Mode** box, and replace it with the following code:

   
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
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=150
   column.1.descriptionkey=parent
   column.1.link.linkproperty.0.name=ID
   column.1.link.linkproperty.0.valuefield=parent:ID
   column.1.link.linkproperty.0.valueformat=int
   column.1.link.lookup=link.view
   column.1.link.valuefield=parent:objCode
   column.1.link.valueformat=val
   column.1.linkedname=parent
   column.1.listsort=nested(parent).string(name)
   column.1.namekey=parent
   column.1.querysort=parent:name
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=parent:name
   column.1.valueformat=HTML
   column.1.width=150
   column.2.description=Parent Parent
   column.2.link.linkproperty.0.name=ID
   column.2.link.linkproperty.0.valuefield=parent:parent:ID
   column.2.link.linkproperty.0.valueformat=int
   column.2.link.lookup=link.view
   column.2.link.valuefield=parent:parent:objCode
   column.2.link.valueformat=val
   column.2.linkedname=parent
   column.2.listsort=nested(parent:parent).string(name)
   column.2.name=Parent Parent
   column.2.querysort=parent:parent:name
   column.2.shortview=false
   column.2.stretch=0
   column.2.valuefield=parent:parent:name
   column.2.valueformat=HTML
   column.2.width=150
   column.3.description=Parent Parent Parent
   column.3.link.linkproperty.0.name=ID
   column.3.link.linkproperty.0.valuefield=parent:parent:parent:ID
   column.3.link.linkproperty.0.valueformat=int
   column.3.link.lookup=link.view
   column.3.link.valuefield=parent:parent:parent:objCode
   column.3.link.valueformat=val
   column.3.linkedname=parent
   column.3.listsort=nested(parent:parent:parent).string(name)
   column.3.name=Parent Parent Parent
   column.3.querysort=parent:parent:parent:name
   column.3.shortview=false
   column.3.stretch=0
   column.3.valuefield=parent:parent:parent:name
   column.3.valueformat=HTML
   column.3.width=150
   column.4.description=Parent Parent Parent Parent
   column.4.link.linkproperty.0.name=ID
   column.4.link.linkproperty.0.valuefield=parent:parent:parent:parent:ID
   column.4.link.linkproperty.0.valueformat=int
   column.4.link.lookup=link.view
   column.4.link.valuefield=parent:parent:parent:parent:objCode
   column.4.link.valueformat=val
   column.4.linkedname=parent
   column.4.listsort=nested(parent:parent:parent:parent).string(name)
   column.4.name=Parent Parent Parent Parent
   column.4.querysort=parent:parent:parent:parent:name
   column.4.shortview=false
   column.4.stretch=100
   column.4.valuefield=parent:parent:parent:parent:name
   column.4.valueformat=HTML
   column.4.width=150
   ```

1. Click **Done** >  **Save View**.

   The name of the task displays in the first column, and if the task has any parents, up to 4 parents display in the remaining columns.
