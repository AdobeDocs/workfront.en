---
filename: run-deliver-report-access-rights-another-user
product-area: reporting
navigation-topic: create-and-manage-reports
title: Run and deliver a report with the access rights of another user
description: By default, users can only see the objects in a report that they have permissions to View.
---

# Run and deliver a report with the access rights of another user

By default, users can only see the objects in a report that they have permissions to View.

You can allow all users to see the same results in a report as another user, regardless of their access level or permission level on the objects inside the report.

If you run a report with the access rights of another user who has higher access (for example, the access rights of an `Adobe Workfront administrator`), all the users who have permissions to View the report can see the information in the report as the user specified in the report builder. You can set this up for both reports that users find in the `Workfront` interface, or for reports that are delivered to users as an attachment to an email.

>[!TIP]
>
>You should replace the `Run this report with the Access Rights of:` field with an active user only when you want the report to display with the access rights of that user.&nbsp;For example, a Work-license user might not have permissions to see all the items in a report built by a Plan-license user or a System Administrator, unless the report displays with the access rights of a Planner or a System Administrator.  
>If the report is shared with users with similar access as the user specified in the `Run this report with the Access Rights of:` field, you can leave this field blank.

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
   <td> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Edit access to Filters,&nbsp;Views, Groupings</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to a report (to view the delivered report)</p> <p>Manage permissions to a report (to run the report)</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Display a report with the access rights of another user

Populating the `Run this Report with the Access Rights of:` field ensures a report contains the same data, regardless of which user is accessing the report. The report displays as it would for the specified user.

The users accessing the report must have at least View permissions on the report to be able to see it. If the user listed in the `Run this Report with the Access Rights of:` field is deactivated, the report no longer displays for any other users who the report is shared with.

To run a report with the access rights of another user:

<ol> 
 <li value="1"> Click the Main Menu icon in the upper-right corner of Workfront, then click Reports. </li> 
 <li value="2">Select the report you want to display with the access rights of another user.</li> 
 <li value="3">Click <span class="bold">Report Actions</span>, then click <span class="bold">Edit</span>.</li> 
 <li value="4">Click <span class="bold">Report Settings</span>.<br></li> 
 <li value="5">In the <span class="bold">Run this report with the Access Rights of:</span> field, start typing the name of the user that you want the report to display as, then select it when you see it in the list.<br><br><note type="note">
   Users with a lower access level that are allowed to build reports do not have the ability to select a user other than themselves for the 
   <span class="bold">Run this Report with the Access Rights of:</span> field.
  </note></li> 
 <li value="6">Click <span class="bold">Done</span>.</li> 
 <li value="7">Click <span class="bold">Save + Close</span>.<br>The report now displays for all users who the report is shared with as if it was viewed by the user specified in the <span class="bold">Run this report with the Access Rights of:</span> field.</li> 
</ol>

>[!IMPORTANT]
>
>We do not recommend using a different user other than the logged-in user for the `Run this report with the Access Rights of:` field if the report contains a filter that uses a wildcard referring to the logged-in user. This can create confusion for the users looking at the report, as the report displays according to what is defined in the filter. This means that the report displays differently for each user, according to the filter, and disregards the value specified in the `Run this report with the Access Rights of:` field.  
>For more information about wildcards for user fields, see the "User-based variables" section in the [Wildcard filter variables](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Deliver a report with the access rights of another user

You can set up reports to be delivered as attachment to an email. You can set up these delivered reports to display as they display for users of a higher access level, so all users can see the same information in the delivered reports. The users who are going to see the report delivered in the email must be added to the Send to list of recipients inside the report delivery. For more information on setting up a report for delivery, see the article [Report delivery overview](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

To deliver a report with the access rights of another user:

<ol> 
 <li value="1"> Click the Main Menu icon in the upper-right corner of Workfront, then click Reports. </li> 
 <li value="2">Select the report you want to deliver with the access rights of another user.</li> 
 <li value="3">Click the name of the report to select it.</li> 
 <li value="4">Click <span class="bold">Report Actions</span>.</li> 
 <li value="5">Click <span class="bold">Send Report</span>.<br></li> 
 <li value="6">In the <span class="bold">Deliver this report with the Access Rights of:</span> field, start typing the name of the user that you want the report to display as when it is delivered in an email, then select it when you see it in the list. The default is the name of the user who is building the report.<br><note type="note">
   Users with a lower access level that are allowed to build reports do not have the ability to select a user other then themselves for the 
   <span class="bold">Deliver&nbsp;this Report with the Access Rights of:</span> field.
  </note></li> 
 <li value="7"> <p>Select the <span class="bold">Format</span> you want the report to display in the email:</p> 
  <ul> 
   <li>HTML</li> 
   <li>PDF</li> 
   <li>MS Excel</li> 
   <li>MS Excel (.xlsx)</li> 
   <li>TSV</li> 
  </ul> </li> 
 <li value="8">Click <span class="bold">Send Now</span> to send it immediately.<br>Or<br>Click <span class="bold">Make Repeating Delivery</span> to schedule a recurring delivery for the report.<br>For more information about report deliveries, see the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md" class="MCXref xref">Report delivery overview</a>.</li> 
</ol>

>[!IMPORTANT]
>
>We do not recommend using a different user other than the user who schedules the delivery for the `Deliver this report with the Access Rights of:` field, if the report contains a filter that uses a wildcard referring to the logged in user. This can create confusion for the users receiving the report, as the delivered report displays as it would for the user who is scheduling the report for delivery. In this case, the delivered report disregards the value specified in the `Deliver this report with the Access Rights of:` field.  
>For more information about wildcards for user fields, see the "User-Based Variables" section in the [Wildcard filter variables](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

