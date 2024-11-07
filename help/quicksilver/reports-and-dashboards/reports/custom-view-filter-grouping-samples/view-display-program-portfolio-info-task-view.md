---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: 'View: Display Program and Portfolio Information in a Task View'
description: This task view displays the Program and Portfolio that are associated with the project of the task. This information is not available in the report builder when building a task view. This is information is available only in text mode.
author: Nolan
feature: Reports and Dashboards
exl-id: cdd5a1e9-3cbf-4951-b803-fca544b2519a
---
# View: display Program and Portfolio information in a task view

This task view displays the Program and Portfolio that are associated with the project of the task. This information is not available in the report builder when building a task view. This is information is available only in text mode.

The view also provides links to the Project, Program, and Portfolio from a task list.

![](assets/view--program-and-portfolio-350x116.png)

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

## Display Program and Portfolio information in a task View

1. Go to a list of tasks.
1. From the **View** drop-down menu, select **New View**.

1. In the**Column Preview** area, eliminate all columns except for one.
1. Click the header of the remaining column, click **Switch to Text Mode**, then **Edit Text Mode**.
1. Remove the text you find in the **Edit Text Mode** box, and replace it with the following code:  

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
   column.1.descriptionkey=project
   column.1.link.linkproperty.0.name=ID
   column.1.link.linkproperty.0.valuefield=project:ID
   column.1.link.linkproperty.0.valueformat=int
   column.1.link.lookup=link.view
   column.1.link.valuefield=project:objCode
   column.1.link.valueformat=val
   column.1.linkedname=project
   column.1.listsort=nested(project).string(name)
   column.1.namekey=project
   column.1.querysort=project:name
   column.1.shortview=false
   column.1.stretch=0
   column.1.valuefield=project:name
   column.1.valueformat=HTML
   column.1.width=150
   column.2.descriptionkey=program
   column.2.displayname=Program
   column.2.link.linkproperty.0.name=ID
   column.2.link.linkproperty.0.valuefield=project:program:ID
   column.2.link.linkproperty.0.valueformat=int
   column.2.link.lookup=link.view
   column.2.link.valuefield=project:program:objCode
   column.2.link.valueformat=val
   column.2.linkedname=project
   column.2.listsort=nested(project:program).string(name)
   column.2.namekey=project
   column.2.querysort=project:program:name
   column.2.shortview=false
   column.2.stretch=0
   column.2.valuefield=project:program:name
   column.2.valueformat=HTML
   column.2.width=150
   column.3.descriptionkey=portfolio
   column.3.displayname=Portfolio
   column.3.link.linkproperty.0.name=ID
   column.3.link.linkproperty.0.valuefield=project:portfolio:ID
   column.3.link.linkproperty.0.valueformat=int
   column.3.link.lookup=link.view
   column.3.link.valuefield=project:portfolio:objCode
   column.3.link.valueformat=val
   column.3.linkedname=project
   column.3.listsort=nested(project:portfolio).string(name)
   column.3.namekey=project
   column.3.querysort=project:portfolio:name
   column.3.shortview=false
   column.3.stretch=0
   column.3.valuefield=project:portfolio:name
   column.3.valueformat=HTML
   column.3.width=150 
   ```

1. Click **Done** > **Save View**.
