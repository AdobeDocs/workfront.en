---
filename: example-status-timestamp-in-calculated-field
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Calculated custom field example: display a Status timestamp in a Custom Form
description: The following calculated field displays the date when the object status is marked as In Progress (INP.) You can use the same information for calculated custom fields for issues, tasks, or projects.
---

# Calculated custom field example: display a Status timestamp in a Custom Form

The following calculated field displays the date when the object status is marked as In Progress (INP.) You can use the same information for calculated custom fields for issues, tasks, or projects.

>[!NOTE]
>
>If the status of the object changes to INP, then it changes to another status, then back to INP, `Adobe Workfront` captures only the timestamp of the first change to INP.

## Access requirements

You must have the following:

<table cellspacing="15"> 
 <caption style="text-align: left;"> 
  <p>*To find out what plan, license type, or access you have, contact your <span>Workfront administrator</span>.</p> 
 </caption> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p><span>Adobe Workfront</span> plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p><span>Adobe Workfront</span> license*</p> </td> 
   <td> <p><span>Plan</span> </p> </td> 
  </tr> 
  <tr> 
   <td><span class="bold">Access level configurations*</span> </td> 
   <td> <p>Edit access to Create Reports, Dashboards, and Calendars</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><span class="bold">Object permissions</span> </p> </td> 
   <td> <p>Manage permissions on the object where the form is attached</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.<br>For more information on permissions for dashboards, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md" class="MCXref xref">Share reports, dashboards, and calendars in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Prerequisites

To add a calculated field that displays a field's edit history to a custom form, you must first:

* Create the custom form

## Display a Status timestamp in a Custom Form

<ol> 
 <li value="1">Go to a custom form where you want to add the field.</li> 
 <li value="2">Click <span class="bold">Calculated</span> to add a calculated custom field to the form.<br></li> 
 <li value="3">Specify a <span class="bold">Label</span> for the Custom Field, for example: <i>Status Timestamp Custom Field</i>.</li> 
 <li value="4">(Optional) Click the <span class="bold">Name</span> field to update it. The Name of the field matches the Label you just entered by default. </li> 
 <li value="5">Click&nbsp;<span class="bold">Done</span>. </li> 
 <li value="6">Click <span class="bold">Save+Close</span>.</li> 
 <li value="7">Re-open the Custom Form, and click the new Status Timestamp Custom Field on the form.</li> 
 <li value="8"> In the <span class="bold">Calculation</span> field, specify the following calculation for your Custom Field:<br><pre>IF(Status='INP',IF(ISBLANK({DE:Status Timestamp Custom Field}),$$NOW,{DE:Status Timestamp Custom Field}),{DE:Status Timestamp Custom Field})</pre><note type="note">
    This calculation is identical for all objects and for all statuses. You must always use the three-letter key, and not the status name for the object status in this calculation.
   <br>For more information about the keys for Statuses, see 
   <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Create or edit a status</a>.
  </note></li> 
 <li value="9"> Click <span class="bold">Save+Close</span>.<br>You can then report on the Status Timestamp Custom Field, or use it in other calculations in reports or Custom Fields.<br></li> 
</ol>

