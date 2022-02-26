---
filename: understand-how-organize-reports-dashboard
content-type: overview
product-area: reporting;dashboards
navigation-topic: report-usage
title: Understand how to organize reports on a dashboard
description: You can see whether a report is added to a dashboard in Adobe Workfront. This might be useful when deciding which reports you can keep and which can be deleted from the system. If reports are on dashboards, users might still be relying on them. We recommend not deleting reports that are listed on dashboards that users are using. For more information about adding reports to dashboards, see the article Add a report to a dashboard.
---

# Understand how&nbsp;to organize reports on a dashboard

## Access dashboard information in a report list

You can see whether a report is added to a dashboard in *Adobe Workfront*. This might be useful when deciding which reports you can keep and which can be deleted from the system. If reports are on dashboards, users might still be relying on them. We recommend not deleting reports that are listed on dashboards that users are using.  
For more information about adding reports to dashboards, see the article [Add a report to a dashboard](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/add-report-dashboard.md).

You can see whether a report is added to a dashboard by doing one of the following:

* Building a view for a list of reports and including dashboard information in the columns
* Filtering a list of reports by one or several specific dashboards that you know are being actively used
* Building a report for the report object and using a view or a filter which include dashboard information

Anyone can build a view or a filter, but you must have Edit access to Reports in your access level to build a report.  
For more information about access to reports, see the article [Grant access to reports, dashboards, and calendars](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).  
For more information about building a report, see the article [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

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
   <td> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Edit access to Filters, Views, Groupings</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Display dashboard information in the View of a report list

To build a view with dashboard information for a report list:

<ol> 
 <li value="1"> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     Click the 
    <span class="bold">Main Menu</span> icon 
    <img src="assets/main-menu-icon.png"> in the upper-right corner of 
    <em>Workfront</em>, then click 
    <span class="bold">Reports</span>. 
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click the 
   <span class="bold">Main Menu</span> icon 
   <img src="assets/main-menu-icon.png"> in the upper-right corner of 
   <em>Workfront</em>, then click 
   <span class="bold">Reports</span>. 
  </MadCap:conditionalText> </li> 
 <li value="2">On the list of reports, click the <span class="bold">View</span> drop-down menu.</li> 
 <li value="3">Click <span class="bold">New View</span>.</li> 
 <li value="4">Click <span class="bold">Add Column</span>.</li> 
 <li value="5">Start typing "Dashboards" in the <span class="bold">Start typing field name</span> field.</li> 
 <li value="6">Under the <span class="bold">Report</span> object, select <span class="bold">Dashboards</span>.</li> 
 <li value="7">Click <span class="bold">Save View</span>.<br>The dashboards that a report appears on display in the Dashboards column of the report list.<br><draft-comment>
   <img src="assets/qs-dashboards-in-report-view.png" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
  </draft-comment><img src="assets/qs-dashboards-in-report-view.png" data-mc-conditions="QuicksilverOrClassic.Quicksilver"><br><br></li> 
</ol>

## Filter a report list by dashboard information

To filter a list of reports by dashboard information:

<ol> 
 <li value="1"> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
     Click the 
    <span class="bold">Main Menu</span> icon 
    <img src="assets/main-menu-icon.png"> in the upper-right corner of 
    <em>Workfront</em>, then click 
    <span class="bold">Reports</span>. 
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click the 
   <span class="bold">Main Menu</span> icon 
   <img src="assets/main-menu-icon.png"> in the upper-right corner of 
   <em>Workfront</em>, then click 
   <span class="bold">Reports</span>. 
  </MadCap:conditionalText> </li> 
 <li value="2">On the list of reports, click the <span class="bold">Filter</span> drop-down menu.</li> 
 <li value="3">Click <span class="bold">New Filter</span>, then click <span class="bold">Add a Filter Rule</span>.</li> 
 <li value="4">Start typing "Dashboards" in the <span class="bold">Start typing field name</span> field.<br></li> 
 <li value="5">Under the <span class="bold">Dashboards</span> object, select <span class="bold">Name</span>.</li> 
 <li value="6">Select <span class="bold">Equal</span> in the modifier drop-down menu, then start typing the name of the dashboard you want to filter by. You can select multiple dashboards for your filter.<br><draft-comment>
   <img src="assets/qs-dashboards-in-report-filters-350x143.png" style="width: 350;height: 143;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
  </draft-comment><img src="assets/qs-dashboards-in-report-filters-350x143.png" style="width: 350;height: 143;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"></li> 
 <li value="7">Click <span class="bold">Save + Close</span>.<br>This displays a list of reports that are listed only on the specified dashboards.<br>You can also build a report for the report object and use this filter in the report.<br></li> 
</ol>

