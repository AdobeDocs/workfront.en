---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: display incomplete cross-project successors'
description: This task filter returns incomplete cross-project successors.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: aea955b1-581a-4ce0-8634-863ba1083c05
---
# Filter: display incomplete cross-project successors

This task filter returns incomplete cross-project successors.

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

## Filter cross-project successors

To apply this filter:

1. Go to a list of tasks.
1. From the **Filter** drop-down menu, select **New filter**.

1. Click **Text mode**.
1. In the area displayed, paste the following code:  
   <pre>percentComplete=100<br>percentComplete_Mod=ne<br>successorsMM:projectID=FIELD:projectID<br>successorsMM:projectID_Mod=ne</pre>

1. Click **Apply** > **Save as new**.
