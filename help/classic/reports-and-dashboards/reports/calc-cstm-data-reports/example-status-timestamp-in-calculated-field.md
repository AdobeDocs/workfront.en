---
filename: example-status-timestamp-in-calculated-field
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Calculated custom field example: display a Status timestamp in a Custom Form
description: The following calculated field displays the date when the object status is marked as In Progress (INP.) You can use the same information for calculated custom fields for issues, tasks, or projects.
---

# Calculated custom field example: display a Status timestamp in a Custom Form

>[!IMPORTANT]
>
>You're currently viewing the Adobe Workfront Classic version of this document. Adobe Workfront Classic is no longer supported. All Adobe Workfront Classic functionality, along with this documentation, will be removed in July 2022. Please transition to the the new Adobe Workfront experienceas soon as possible, and switch to the new Adobe Workfront experience version of this document.

The following calculated field displays the date when the object status is marked as In Progress (INP.) You can use the same information for calculated custom fields for issues, tasks, or projects.

>[!NOTE]
>
>If the status of the object changes to INP, then it changes to another status, then back to INP, Adobe Workfront captures only the timestamp of the first change to INP.

## Access requirements

You must have the following:

<table cellspacing="15"> 
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

## Prerequisites

To add a calculated field that displays a field's edit history to a custom form, you must first:

* Create the custom form

## Display a Status timestamp in a Custom Form

1. Go to a custom form where you want to add the field.
1. Click **Calculated** to add a calculated custom field to the form.  

1. Specify a **Label** for the Custom Field, for example: *Status Timestamp Custom Field*.

1. (Optional) Click the **Name** field to update it. The Name of the field matches the Label you just entered by default. 
1. Click&nbsp;**Done**. 
1. Click **Save+Close**.
1. Re-open the Custom Form, and click the new Status Timestamp Custom Field on the form.
1. In the **Calculation** field, specify the following calculation for your Custom Field:  
   <pre>IF(Status='INP',IF(ISBLANK({DE:Status Timestamp Custom Field}),$$NOW,{DE:Status Timestamp Custom Field}),{DE:Status Timestamp Custom Field})</pre>

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: text should wrap here.)</p>
   -->

   >[!NOTE]
   >
   >This calculation is identical for all objects and for all statuses. You must always use the three-letter key, and not the status name for the object status in this calculation.  
   >For more information about the keys for Statuses, see [Create or edit a status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

1. Click **Save+Close**.  
   You can then report on the Status Timestamp Custom Field, or use it in other calculations in reports or Custom Fields.

