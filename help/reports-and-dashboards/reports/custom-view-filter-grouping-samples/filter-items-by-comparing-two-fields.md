---
filename: filter-items-by-comparing-two-fields
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: Filter: eliminate items in a list by comparing two fields
description: You can filter items out of a list by comparing two of their fields. For example, you can display only tasks where the Actual Completion Date of the task is greater than the Planned Completion Date.
---

# Filter: eliminate items in a list by comparing two fields

You can filter items out of a list by comparing two of their fields. For example, you can display only tasks where the Actual Completion Date of the task is greater than the Planned Completion Date.

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

## Filter items by comparing two fields

<ol> 
 <li value="1">Go to a list of tasks. </li> 
 <li value="2">From the <span class="bold">Filter</span> drop-down menu, select <span class="bold">New Filter</span>.</li> 
 <li value="3"> <p>Click <span class="bold">Add Filter Rule</span> and add <span class="bold">Actual Completion Date</span> ><span class="bold">Greater Than</span>&nbsp;> <span class="bold">Select a date</span>. </p> <note type="tip">
   Choose the filter modifier you want to use for the selected field, if available.
  </note> </li> 
 <li value="4">Click <span class="bold"> Switch to Text Mode</span>.</li> 
 <li value="5"> <p>In the <span class="bold">Set Filter Rules for your Report</span> area, add the following code: </p> <p><code>actualCompletionDate=FIELD:plannedCompletionDate<br>actualCompletionDate_Mod=gt</code> </p> </li> 
 <li value="6">Click <span class="bold">Done</span>, then <span class="bold">Save Filter</span>.</li> 
</ol>

