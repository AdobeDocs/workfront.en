---
filename: filter-proof-approval-report
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Filter Proof Approval report to omit previous proof versions
description: On a Proof Approval report, you can use the Is Current Document Version filter to include only the current versions of proofs waiting for your approval.
---

# Filter Proof Approval report to omit previous *proof* versions

On a Proof Approval report, you can use the  `Is Current Document Version` filter to include only the current versions of proofs waiting for your approval.

This is useful, for example, if you have been asked to approve proofs that have multiple versions. When you run the Proof Approval report with the Is Current Document Version filter, the report lists only the current version of each proof awaiting your approval, omitting earlier versions that you no longer need to work on.&nbsp;

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

## Filter Proof Approval report to omit previous *proof* versions

<ol> 
 <li value="1"> <p>If you already have a Proof Approval report, open it.</p> <p>Or</p> <draft-comment>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">To create your own Proof Approval report, click the Main Menu <img src="assets/main-menu-icon.png">, then click <span class="bold">Reports</span> <img src="assets/reports-in-main-menu.png">. Click&nbsp;<span class="bold">New Report</span>. In the list that appears, scroll to and click <span class="bold">Proof Approval</span>. Click <span class="bold">Save + Close</span>, type a <span class="bold">Report Name</span> (optional), then click <span class="bold">Save Report</span>.</p>
  </draft-comment><p data-mc-conditions="QuicksilverOrClassic.Draft mode">To create your own Proof Approval report, click the Main Menu <img src="assets/main-menu-icon.png">, then click <span class="bold">Reports</span> <img src="assets/reports-in-main-menu.png">. Click&nbsp;<span class="bold">New Report</span>. In the list that appears, scroll to and click <span class="bold">Proof Approval</span>. Click <span class="bold">Save + Close</span>, type a <span class="bold">Report Name</span> (optional), then click <span class="bold">Save Report</span>.</p> </li> 
 <li value="2">Click <span class="bold">Report Actions >&nbsp;Edit</span>.</li> 
 <li value="3"> <draft-comment>
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
    Click 
    <span class="bold">Filters</span>, then click 
    <span class="bold">Add a Filter Rule</span>.
   </MadCap:conditionalText>
  </draft-comment><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   Click 
   <span class="bold">Filters</span>, then click 
   <span class="bold">Add a Filter Rule</span>.
  </MadCap:conditionalText> </li> 
 <li value="4"> <p>Click <span class="bold">Proof Approval</span>.</p> </li> 
 <li value="5">In the list that appears, click <span class="bold">Is Current Document Version</span>.</li> 
 <li value="6">Click <span class="bold">Save +&nbsp;Close</span> in the lower-left corner of <em>Adobe Workfront</em>, then click <span class="bold">Save Report</span> in the box that appears.</li> 
</ol>

