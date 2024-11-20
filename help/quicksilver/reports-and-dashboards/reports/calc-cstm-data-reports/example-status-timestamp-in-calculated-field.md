---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 'Calculated custom field example: display a Status timestamp in a Custom Form'
description: The following calculated field displays the date when the object status is marked as In Progress (INP.) You can use the same information for calculated custom fields for issues, tasks, or projects.
author: Nolan
feature: Reports and Dashboards
exl-id: 55817a68-3655-4288-8cc7-48547829c46e
---
# Calculated custom field example: display a Status timestamp in a custom form

The following calculated field displays the date when the object status is marked as In Progress (INP.) You can use the same information for calculated custom fields for issues, tasks, or projects.

>[!NOTE]
>
>If the status of the object changes to INP, then it changes to another status, then back to INP, Adobe Workfront captures only the timestamp of the first change to INP.

## Access requirements

You must have the following:

<table style="table-layout:auto"> 
 <caption style="text-align: left;"> 
  <p>*To find out what plan, license type, or access you have, contact your Workfront administrator.</p> 
 </caption> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Access level configurations*</strong> </td> 
   <td> <p>Edit access to Create Reports, Dashboards, and Calendars</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Object permissions</strong> </p> </td> 
   <td> <p>Manage permissions on the object where the form is attached</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.<br>For more information on permissions for dashboards, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md" class="MCXref xref">Share reports, dashboards, and calendars </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Prerequisite

To add a calculated field that displays a field's edit history to a custom form, you must first create the custom form.

## Display a Status time stamp in a Custom Form

1. Go to a custom form where you want to add the field.
1. Click **Calculated** to add a calculated custom field to the form.  
1. Type a **Label** for the custom field. For example,"Status Timestamp Custom Field".
1. Click **Save+Close**.
1. Re-open the custom form, then select the new **Status Timestamp Custom Field** on the form.
1. In the **Calculation** box, copy and paste the following calculation for your custom field:  
   
   ```
   IF({status}='INP',IF(ISBLANK({DE:Status Timestamp Custom Field}),$$NOW,{DE:Status Timestamp Custom Field}),{DE:Status Timestamp Custom Field})  
   ```

   >[!NOTE]
   >
   >This calculation is identical for all objects and for all statuses. You must always use the three-letter key, and not the status name for the object status in this calculation.
   >
   >For more information about the keys for Statuses, see [Create or edit a status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. Click **Save+Close**.  
   
   You can now report on the Status Timestamp Custom Field or use it in other calculations, in reports, or in custom fields.
