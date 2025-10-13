---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: display your current projects pending approval'
description: The following project filter displays projects in the Current - Pending Approval status, where the logged-in user is either the Project Sponsor or the Portfolio Manager.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 32045aec-acc5-44d2-bad5-7759dc797414
---
# Filter: display your current projects pending approval

<!--Audited: 10/2024-->

The following project filter displays projects in the Current - Pending Approval status,&nbsp;where the logged-in user is either the Project Sponsor or the Portfolio Manager.

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

## Filter current projects pending approval

To apply this filter:

1. Go to a list of projects.
1. From the **Filter** drop-down menu, select **New filter**.

1. Click **Text mode**.
1. In the area displayed, copy and paste the following code:  
   <pre>status=CUR:A<br>sponsorID=$$USER.ID<br>OR:a:status=CUR:A<br>OR:a:portfolio:ownerID=$$USER.ID</pre>

1. Click **Apply** > **Save as new**.
