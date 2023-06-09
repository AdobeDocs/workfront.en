---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: eliminate items in a list by comparing two fields'
description: You can filter items out of a list by comparing two of their fields. For example, you can display only tasks where the Actual Completion Date of the task is greater than the Planned Completion Date.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
---
# Filter: eliminate items in a list by comparing two fields

You can filter items out of a list by comparing two of their fields. For example, you can display only tasks where the Actual Completion Date of the task is greater than the Planned Completion Date.

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request to modify a filter </p>
   <p>Plan to modify a report</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Reports, Dashboards, Calendars to modify a report</p> <p>Edit access to Filters, Views, Groupings to modify a filter</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Filter items by comparing two fields

1. Go to a list of tasks. 
1. From the **Filter** drop-down menu, select **New Filter**.

1. Click **Add Filter Rule** and add **Actual Completion Date** >**Greater Than**&nbsp;> **Select a date**.

   >[!TIP]
   >
   >Choose the filter modifier you want to use for the selected field, if available.

1. Click **Switch to Text Mode**.
1. In the **Set Filter Rules for your Report** area, add the following code:

   ```
   actualCompletionDate=FIELD:plannedCompletionDate<br>actualCompletionDate_Mod=gt
   ```

1. Click **Done**, then **Save Filter**.
