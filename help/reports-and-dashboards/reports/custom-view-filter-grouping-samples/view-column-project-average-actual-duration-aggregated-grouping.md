---
filename: view-column-project-average-actual-duration-aggregated-grouping
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: View and grouping: display project Actual Duration aggregated by the average in a Grouping
description: You can add the following column in a project report to show the Actual Duration aggregated as an average in a grouping.
---

# View and grouping: display project Actual Duration aggregated by the average in a Grouping

You can add the following column in a project report to show the Actual Duration aggregated as an average in a grouping.

![project_with_aggregate_actual_duration_in_grouping_view.png](assets/project-with-aggregate-actual-duration-in-grouping-view-350x65.png)

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><span>Adobe Workfront</span> license*</td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Edit access to Filters, Views, Groupings</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Display project Actual Duration aggregated by the average in a Grouping

To add this column to a project view:

1. (Recommended)&nbsp;For best results and to see the aggregated average value of the Actual Duration, you must have a Grouping added to your project list or report.  
   For more information about creating Groupings, see the article [Groupings overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. Go to an existing project view.
1. Expand the View drop-down menu, and select  `Customize View`.
1. Click  `Add Column`.
1. Click  `Switch to Text Mode`.
1. Mouse over the  `Show in this column` area, and click  `Click to edit text`.

1. Remove all text in the Text Mode box, and replace it with the following code:  
   <pre>aggregator.displayformat=compound <br>aggregator.function=AVG <br>aggregator.namekey=view.relatedcolumn <br>aggregator.namekeyargkey=actualduration <br>aggregator.valuefield=actualDurationMinutes <br>aggregator.valueformat=val <br>displayname=Project Actual Duration <br>durationunitfield=durationUnit.value <br>linkedname=project <br>namekey=actualduration <br>namekeyargkey=actualduration <br>querysort=actualDurationMinutes <br>textmode=true <br>valuefield=actualDurationMinutes <br>valueformat=compound#M:D <br>viewalias=actualduration</pre>

1. Click `Save View`.

