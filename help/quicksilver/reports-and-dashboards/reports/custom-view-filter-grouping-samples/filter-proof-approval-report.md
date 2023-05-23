---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Filter: Proof Approval report to omit previous proof versions'
description: On a Proof Approval report, you can use the Is Current Document Version filter to include only the current versions of proofs waiting for your approval.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
---
# Filter:&nbsp;Proof Approval report to omit previous proof versions

On a Proof Approval report, you can use the&nbsp;**Is Current Document Version** filter to include only the current versions of proofs waiting for your approval.

This is useful, for example, if you have been asked to approve proofs that have multiple versions. When you run the Proof Approval report with the Is Current Document Version filter, the report lists only the current version of each proof awaiting your approval, omitting earlier versions that you no longer need to work on.&nbsp;

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Request to modify a filter </p>
   <p>Plan to modify a report</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Reports, Dashboards, Calendars to modify a report</p> <p>Edit access to Filters, Views, Groupings to modify a filter</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Filter Proof Approval report to omit previous proof versions

1. If you already have a Proof Approval report, open it.

   Or

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   To create your own Proof Approval report, click the Main Menu ![](assets/main-menu-icon.png), then click **Reports** ![](assets/reports-in-main-menu.png). Click&nbsp;**New Report**. In the list that appears, scroll to and click **Proof Approval**. Click **Save + Close**, type a **Report Name** (optional), then click **Save Report**.

1. Click **Report Actions > Edit**.
1. Click **Filters**, then click **Add a Filter Rule**.

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. Click **Proof Approval**.
1. In the list that appears, click **Is Current Document Version**.
1. Click **Save + Close** in the lower-left corner of Adobe Workfront, then click **Save Report** in the box that appears.
