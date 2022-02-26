---
filename: use-date-based-wildcards-generalize-reports
product-area: reporting
navigation-topic: reporting-elements
title: Use date-based wildcards to generalize reports
description: You can generalize a report by using wildcards instead of specific information when building certain reporting elements.
---

# Use date-based wildcards to generalize reports

You can generalize a report by using wildcards instead of specific information when building certain reporting elements.

For example, if you want to create a report that shows the tasks that have a specific Planned Start Date, you can use the calendar date picker in a filter to select a specific date. However, if you want to create a report that shows tasks that have the Planned Start Date within a certain timeframe from the date when the report is accessed, you can use a wildcard that indicates that when someone views the report it displays information for a timeframe relevant for the moment when they view the report.

For example in the past week, in the past year, in the next two weeks, etc. This way, you build the report once, but because you use a wildcard in the filter, it produces different results every time someone reads it because it adapts to the day when they run the report.

You can use date-based wildcards when building the following reporting elements:

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
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Filters, Views, Groupings</p> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars to edit reporting elements in a report</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report to edit reporting elements in a report</p> <p>Manage permissions to a view or filter to edit them</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Prerequisites

You must create a report before you can add wildcard variables to it.

For information on creating a report, see [Create a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Walk-through

View the following video to learn how you can generalize the information in your reports and adapt them to the date when they are run by using date-based wildcards.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Quicksilver">This video was recorded in <em>Adobe Workfront</em> Classic. However, the content also applies to the new Workfront experience.</p>
-->

This video was recorded in *Adobe Workfront* Classic. However, the content also applies to the new Workfront experience.

[ ![](assets/video-date-based-wildcards-350x198.png)](https://workfront-video.wistia.com/medias/poww2vz0r4)

## How-to steps

To insert a date-based wildcard in a report:

<ol> 
 <li value="1">Go to a report for which you want to insert a date-based wildcard.</li> 
 <li value="2">Click <span class="bold">Report Actions</span>, then <span class="bold">Edit</span>.</li> 
 <li value="3">Click the <span class="bold">Filters</span> tab.</li> 
 <li value="4">Click <span class="bold">Add a Filter Rule</span>.</li> 
 <li value="5"> <p>Start typing the name of the field that you want to filter by.<br>You must type fields that reference a date.</p> </li> 
 <li value="6"> <p>Select <span class="bold">Equal</span> in the drop-down menu for the filter variable.</p> <note type="tip">
   You must always select the 
   <span class="bold">Equal</span> filter variable when working with wildcards in 
   <em>Adobe Workfront</em>.
  </note> </li> 
 <li value="7"> <p>In the <span class="bold">Start typing name ...</span> box, type: <code>$$TODAY</code> if you want to display information about something that occurs the same day that the report is run.</p> <p>Or</p> <p>Type <code>$$NOW</code> if you want to display information about something that occurs at the same date and time that the report is run.</p> <p>This date is always different, as it changes with the date the report is actually viewed by a user. so the information in the report is different from day to day.</p> </li> 
 <li value="8"> <p>(Optional) If you want to display information that occurs within a timeframe after the date when the report is run, type<code> $$TODAY+1w</code> to display information in the following week, or <code>$$TODAY+2m</code> to display information in the next two months. You can also indicate timeframes for quarters, hours, days, or years.</p> </li> 
 <li value="9"> <p>(Optional) If you want to display information about something that occurred within a timeframe before the date when the report is run, type $$TODAY-1w to display information from the previous week, or <code>$$TODAY-2m</code> to display information from the previous two months. You can also indicate timeframes for quarters, hours, days, or years.</p> <p>For a complete list of attributes, qualifiers, and operators that you can use in date-based wildcards, see the article <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">Wildcard filter variables</a>.</p> <p> <img src="assets/video-date-based-wildcard-in-task-filter-350x81.png" style="width: 350;height: 81;"> </p> </li> 
 <li value="10">Click <span class="bold">Save + Close</span>.</li> 
</ol>

## Additional information

See also:

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p><a href="https://one.workfront.com/s/basic-report-creation-program">Basic Report Creation Program for the new Workfront experience</a> </p> </li>
  -->

* [Basic Report Creation Program for the new Workfront experience](https://one.workfront.com/s/basic-report-creation-program) 
* [Wildcard filter variables](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md) 
* [Create or edit filters in Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md) 
* [Add a prompt to a report](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md) 
* [Use conditional formatting in Views](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)

