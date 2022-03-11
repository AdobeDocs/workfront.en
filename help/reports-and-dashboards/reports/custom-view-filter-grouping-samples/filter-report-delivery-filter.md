---
filename: filter-report-delivery-filter
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: Filter: report delivery filter
description: This report filter displays all reports scheduled to be delivered automatically in Adobe Workfront. It is best used with the standard view.
---

# Filter: report delivery filter

This report filter displays all reports scheduled to be delivered automatically in `Adobe Workfront`. It is best used with the standard view.

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

## Report delivery filter

To apply this filter:

1. Go to a list of reports.
1. From the `Filter` drop-down menu, select `New Filter`.

1. Click `Switch to Text Mode`.
1. In the `Set Filter Rules for your Report` area, copy and paste the following code:

   ```
   scheduledReportID=0<br>scheduledReportID_Mod=notnull
   ```

1. Click `Save Filter`.

