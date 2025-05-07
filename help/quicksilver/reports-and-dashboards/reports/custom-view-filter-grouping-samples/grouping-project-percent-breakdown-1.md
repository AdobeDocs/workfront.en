---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Grouping: Project Percent Breakdown 1'
description: In this custom project grouping, you can display projects grouped by a range of their percent complete values.
author: Nolan
feature: Reports and Dashboards
exl-id: 7cdc8e56-3486-4e78-b494-b2ba9389c1f7
---
# Grouping: project percent breakdown 1

<!--Audited: 10/2024-->

In this custom project grouping, you can display projects grouped by a range of their percent complete values. The breakdowns show percent complete value of 25 percent point increments: 0-25%, 26-50%, 51-75% etc.

The following grouping organizes projects by the percent complete value into one of these groupings:

* 0%
* 1-25%
* 26-50%
* 51-75%
* 76-99%
* 100%

![percent_complete_breakdown_custom_project_grouping_25__increments.png](assets/percent-complete-breakdown-custom-350x56.png)

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

## Group by project percent breakdown

To apply this grouping:

1. Go to a list of projects.
1. From the **Grouping** drop-down menu, select **New Grouping**.

1. Click **Switch to Text Mode**.
1. Remove the text in the box, and paste the following code in the available space:

   ```
   group.0.linkedname=direct
   group.0.name=Percent Breakdown
   group.0.notime=false
   group.0.valueexpression=IF({percentComplete}=0,"0 %",IF({percentComplete}<=26,"0-25 %",IF({percentComplete}<=51,"26-50 %",IF({percentComplete}<=76,"51-75 %",IF({percentComplete}<100,"76-99 %","100 %")))))
   group.0.valueformat=string
   ```
   
1. Click **Done** > **Save Grouping**.
1. (Optional) Update the name of the grouping, then click **Save Grouping**.
