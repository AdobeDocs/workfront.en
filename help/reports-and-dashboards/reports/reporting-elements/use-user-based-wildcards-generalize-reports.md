---
filename: use-user-based-wildcards-generalize-reports
product-area: reporting
navigation-topic: reporting-elements
title: Use user-based wildcards to generalize reports
description: You can generalize a report by using wildcards instead of specific information when building certain reporting elements. For example, if you want to create a report that shows the tasks assigned to a specific user, you can use the user's name in the Assigned To field of the filter. However, if you want to create a report that shows tasks assigned to the logged in user, regardless of who that user is, you can use a wildcard that indicates that when someone views the report it displays information pertaining only to them. This way, you build the report once but because you use a wildcard in the filter it produces different results every time someone else reads it.
---

# Use user-based wildcards to generalize reports

You can generalize a report by using wildcards instead of specific information when building certain reporting elements. For example, if you want to create a report that shows the tasks assigned to a specific user, you can use the user's name in the Assigned To field of the filter. However, if you want to create a report that shows tasks assigned to the logged in user, regardless of who that user is, you can use a wildcard that indicates that when someone views the report it displays information pertaining only to them. This way, you build the report once but because you use a wildcard in the filter it produces different results every time someone else reads it.

You can use user-based wildcards when building the following reporting elements:

* Filters
* Custom prompts
* Views when adding rules for columns

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
   <td> <p>Edit access to Filters, Views, Groupings</p> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars to edit reporting elements in a report</p> <p>Note: If you still don't have access, ask your <span>Workfront administrator</span> if they set additional restrictions in your access level. For information on how a <span>Workfront administrator</span> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report to edit reporting elements in a report</p> <p>Manage permissions to a view or filter to edit them</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your `Workfront administrator`.

## Prerequisites

You must create a report before you can add a wildcard variable to it.

For instructions on creating reports, see [Create a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Walk-through

View the following video to learn how you can generalize the information in your reports and adapt them to the user who runs the report by using user-based wildcards.
This video was recorded in Adobe Workfront Classic. However, the content also applies to the new Workfront experience. 

[ ![](assets/video-user-based-wildcards-front-350x201.png)](https://workfront-video.wistia.com/medias/jfn0iczd8m)

## How-to steps

To insert a user-based wildcard in a report:

<ol> 
 <li value="1">Go to a report for which you want to insert a user-based wildcard.</li> 
 <li value="2">Click <span class="bold">Report Actions</span>, then <span class="bold">Edit</span>.</li> 
 <li value="3">Click the <span class="bold">Filters</span> tab.</li> 
 <li value="4">Click <span class="bold">Add a Filter Rule</span>.</li> 
 <li value="5"> <p>Start typing the name of the field that you want to filter by.<br>You must type fields that reference the user object or information about users.</p> </li> 
 <li value="6"> <p>Select <span class="bold">Equal</span> in the drop-down menu for the filter variable.</p> <note type="tip">
   You must always select the 
   <span class="bold">Equal</span> filter variable when working with wildcards in 
   <span>Adobe Workfront</span>.
  </note> </li> 
 <li value="7"> <p>In the <span class="bold">Start typing name ...</span> box, type: <code>$$USER.ID</code> or <code>$$USER.name</code> if you want the report to display information about the user who logs in, based on their name. You can insert other wildcards that refer to the logged-in user's Group, Team, Company, or other information.</p> <p>For a complete list of user-based wildcards, see <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">Wildcard filter variables</a>.</p> <p> <img src="assets/user-based-wildcard-in-project-filter-350x74.png" style="width: 350;height: 74;"> </p> </li> 
 <li value="8">Click <span class="bold">Save + Close</span>.</li> 
</ol>

## Additional information

See also:

* [Wildcard filter variables](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md) 
* [Create or edit filters in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md) 
* [Filters overview in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md) 
* [Add a prompt to a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md) 
* [Use conditional formatting in Views](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)

