---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'View: Multi-row Project View'
description: Learn about the multi-row project view in reports.
author: Nolan
feature: Reports and Dashboards
exl-id: 3c6028c0-2c9f-4f86-aa6c-bf089844bac8
---
# View: multi-row project View

<!--Audited: 11/2024-->

In this project view you can:

* Display project information in a multi-row format.  
  The view uses the `sharecol=true` tag to combine multiple fields under the same column header. To learn more about this tag, see [View: merge information from multiple columns in one shared column](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).

* Use a place holder column that holds an HTML line break tag (`<br>`) to force the Description to display below the project name, for example.
* Display the Project Owner in parentheses after the Project Name.
* Display the Project Name as a link to the project.

![](assets/project-multi-row-stacked-view-350x219.png)

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

## Build a multi-row project View

1. Go to a list of projects.
1. From the **View** drop-down menu, click **New View**.
1. Remove all the columns in the view, except for one.
1. Select the remaining column and click **Switch to Text Mode**, then **Edit Text Mode**.
1. Remove the text in the **Edit Text Mode**, then copy and paste the text mode below inside the column: 

    ```
    column.0.linkedname=direct
    column.0.link.valueformat=val
    column.0.link.linkproperty.0.name=ID
    column.0.link.linkproperty.0.valuefield=ID
    column.0.link.linkproperty.0.valueformat=int
    column.0.link.valuefield=objCode
    column.0.link.lookup=link.view
    column.0.sharecol=true
    column.0.descriptionkey=name
    column.0.width=150
    column.0.querysort=name
    column.0.valuefield=name
    column.0.name=Project Name / Manager / Description
    column.0.shortview=false
    column.0.stretch=100
    column.0.textmode=true
    column.0.listsort=string(name)
    column.0.valueformat=HTML
    column.1.valueexpression=CONCAT(" (",{owner}.{name},")")
    column.1.listsort=nested(owner).string(name)
    column.1.width=1
    column.1.linkedname=direct
    column.1.querysort=owner:name
    column.1.textmode=true
    column.1.shortview=false
    column.1.stretch=0
    column.1.valueformat=HTML
    column.1.sharecol=true
    column.2.width=1
    column.2.value=
    column.2.shortview=false
    column.2.sharecol=true
    column.2.stretch=0
    column.2.textmode=true
    column.2.valueformat=HTML
    column.3.styledef.style=font-color:#ccc;
    column.3.descriptionkey=description
    column.3.linkedname=direct
    column.3.valuefield=description
    column.3.listsort=string(description)
    column.3.querysort=description
    column.3.namekey=description.abbr
    column.3.textmode=true
    column.3.sharecol=true
    column.3.stretch=0
    column.3.shortview=false
    column.3.valueformat=HTML
    column.3.width=1
    column.4.shortview=false
    column.4.value=
    column.4.sharecol=true
    column.4.width=1
    column.4.textmode=true
    column.4.valueformat=HTML\
    column.4.stretch=0
    column.5.name=Planned Dates / Duration
    column.5.width=150
    column.5.querysort=plannedStartDate
    column.5.sharecol=true
    column.5.stretch=0
    column.5.textmode=true
    column.5.shortview=false
    column.5.linkedname=direct
    column.5.listsort=atDateAsAtDate(plannedStartDate)
    column.5.valuefield=plannedStartDate
    column.5.valueformat=atDate
    column.6.sharecol=true
    column.6.stretch=0
    column.6.width=1
    column.6.textmode=true
    column.6.value=-
    column.6.valueformat=HTML
    column.6.shortview=false
    column.7.namekey=plannedcompletiondate.abbr
    column.7.width=1
    column.7.sharecol=true
    column.7.shortview=false
    column.7.stretch=0
    column.7.listsort=atDateAsAtDate(plannedCompletionDate)
    column.7.linkedname=direct
    column.7.descriptionkey=plannedcompletiondate
    column.7.textmode=true
    column.7.querysort=plannedCompletionDate
    column.7.valueformat=atDate
    column.7.valuefield=plannedCompletionDate
    column.8.value=
    column.8.width=1
    column.8.textmode=true
    column.8.sharecol=true
    column.8.valueformat=HTML
    column.8.stretch=0
    column.9.textmode=true
    column.9.listsort=intAsInt(durationMinutes)
    column.9.stretch=0
    column.9.valuefield=durationFieldLong
    column.9.descriptionkey=duration
    column.9.viewalias=duration
    column.9.querysort=durationMinutes
    column.9.sharecol=true
    column.9.width=100
    column.9.shortview=false
    column.9.namekey=duration.abbr
    column.9.linkedname=direct
    column.9.valueformat=compound
    column.10.textmode=true
    column.10.stretch=0
    ```


1. Click **Done** > **Save View**.
