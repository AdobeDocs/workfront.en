---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: Display Reports Scheduled for Delivery'
description: This report filter displays all reports scheduled to be delivered automatically in Adobe Workfront. It is best used with the standard view.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7b937384-80c9-4bc7-94be-5573cf86b35b
---
# Filter: display reports scheduled for delivery

<!--Audited: 10/2024-->

This report filter displays all reports scheduled to be delivered automatically in Adobe Workfront. It is best used with the standard view.

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

## Report delivery filter

To apply this filter:

1. Go to a list of reports.

1. From the **Filter** drop-down menu, select **New Filter**.

1. Click**Switch to Text Mode**.

1. In the **Set Filter Rules for your Report** area, copy and paste the following code:

    ```
    scheduledReportID=0
    scheduledReportID_Mod=notnull
    ```

1. Click **Save Filter**.
