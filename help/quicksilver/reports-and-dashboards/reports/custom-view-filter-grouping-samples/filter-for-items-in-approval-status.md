---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: display only items in an approval status'
description: You can display only items in a certain status which is currently in Pending Approval. This works the same for any other object with an approval status.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
---
# Filter: display only items in an approval status

<!--Audited: 10/2024-->

You can display only items in a certain status which is currently in Pending Approval. This works the same for any other object with an approval status.

You can place the following objects in an approval status:

* Tasks
* Issues 
* Projects

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

## Display only items in approval status

1. Go to a list of projects.
1. From the **Filter** drop-down menu, select **New filter**.
1. Choose to filter by **Project: Status**, then select the status you want to filter by from the list. 

   For example, in a project report, add **Status Equal Planning**, if you want to display only projects which are in a status of **Planning - Pending Approval**.
1. Click **Text mode**.
1. Modify the `status` line by adding **:A** to the 3-letter key of the status:  
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. Click **Apply** > **Save as new**.

   The list displays only projects that are in a status of Planning - Pending Approval.
