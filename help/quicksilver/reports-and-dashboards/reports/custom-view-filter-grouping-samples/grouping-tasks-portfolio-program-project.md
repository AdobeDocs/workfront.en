---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Grouping: Tasks by Portfolio, Program, and Project'
description: Use this task grouping to group tasks by the portfolio, by program, and then by the project they are associated with.
author: Nolan
feature: Reports and Dashboards
exl-id: 8fdad6a1-54b3-4d3e-8f21-4f2efc2dc27a
---
# Grouping: tasks by portfolio, program, and project

<!--Audited: 10/2024-->

Use this task grouping to group tasks by the portfolio, by program, and then by the project they are associated with.

![Portfolio program project grouping](assets/portfolio-program-project-grouping-for-tasks-350x120.png)

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

## Group tasks by portfolio, program, and project

To apply this grouping:

1. Go to a list of tasks.
1. From the **Grouping** drop-down menu, select **New Grouping**.
1. Click **Add grouping**. 

1. Click**Switch to Text Mode**.
1. Remove the text in the **Group by** area.
1. Replace the text with the following code:

   ```
   group.0.linkedname=project
   group.0.namekey=portfolio
   group.0.notime=false
   group.0.valuefield=project:portfolio:name
   group.0.valueformat=string
   group.1.linkedname=project
   group.1.namekey=program
   group.1.notime=false
   group.1.valuefield=project:program:name
   group.1.valueformat=string
   group.2.name=Project
   group.2.valuefield=project:name
   group.2.valueformat=HTML
   textmode=true

   ```

1. Click **Done** > **Save Grouping**.
1. (Optional) Update the grouping name, then click **Save Grouping**. 

