---
filename: filter-proof-approval-report
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Filter Proof Approval report to omit previous proof versions
description: On a Proof Approval report, you can use the Is Current Document Version filter to include only the current versions of proofs waiting for your approval.
---

# Filter Proof Approval report to omit previous proof versions

On a Proof Approval report, you can use the  `Is Current Document Version` filter to include only the current versions of proofs waiting for your approval.

This is useful, for example, if you have been asked to approve proofs that have multiple versions. When you run the Proof Approval report with the Is Current Document Version filter, the report lists only the current version of each proof awaiting your approval, omitting earlier versions that you no longer need to work on.&nbsp;

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Edit access to Filters, Views, Groupings</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Filter Proof Approval report to omit previous proof versions

1. If you already have a Proof Approval report, open it.

   Or
   To create your own Proof Approval report, click Reporting. On the Reports tab, click New Report > Proof Approval. Click Save + Close, type a Report Name (optional), then click Save Report. 

   <!--
   To create your own Proof Approval report, click the Main Menu , then click Reports . Click New Report. In the list that appears, scroll to and click Proof Approval. Click Save + Close, type a Report Name (optional), then click Save Report.
   -->

1. Click `Report Actions > Edit`.
1. On the Filters tab, click Add a Filter Rule. 
1. Click `Proof Approval`.
1. In the list that appears, click `Is Current Document Version`.
1. Click `Save + Close` in the lower-left corner of Adobe Workfront, then click `Save Report` in the box that appears.

