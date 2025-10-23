---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: 'Calculated custom field example: display a Status timestamp in a Custom Form'
description: The following calculated field displays the date when the object status is marked as In Progress (INP). You can use the same information for calculated custom fields for issues, tasks, or projects.
author: Jenny
feature: Reports and Dashboards
exl-id: 55817a68-3655-4288-8cc7-48547829c46e
---
# Calculated custom field example: display a Status timestamp in a custom form

The following calculated field displays the date when the object status is marked as In Progress (INP). You can use the same information for calculated custom fields for issues, tasks, or projects.

>[!NOTE]
>
>If the status of the object changes to INP, then it changes to another status, then back to INP, Adobe Workfront captures only the timestamp of the first change to INP.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront package</p> </td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license</p> </td> 
   <td>
      <p>Standard</p>
      <p>Plan</p></td>
  </tr> 
  <tr> 
   <td><p>Access level configurations</p></td> 
   <td> <p>Edit access to Create Reports, Dashboards, and Calendars</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Object permissions</p> </td> 
   <td> <p>Manage permissions on the object where the form is attached</p></td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisite

To add a calculated field that displays a field's edit history to a custom form, you must first create the custom form.

## Display a Status time stamp in a Custom Form

1. Go to a custom form where you want to add the field.
1. Click **Calculated** to add a calculated custom field to the form.  
1. Type a **Label** for the custom field. For example, "Status Timestamp Custom Field".
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
