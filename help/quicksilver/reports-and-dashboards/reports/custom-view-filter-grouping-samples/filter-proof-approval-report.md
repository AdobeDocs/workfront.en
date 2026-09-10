---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: "Filter: Proof Approval Report to Omit Previous Proof Versions"
description: On a Proof Approval report, you can use the Is Current Document Version filter to include only the current versions of proofs waiting for your approval.
author: Courtney
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/0K5-65eWGsnej09HOH7yZKBDgANUPN1JThyGnkwt1kM
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Filter: Proof Approval report to omit previous proof versions

<!--Audited: 10/2024-->

On a Proof Approval report, you can use the **Is Current Document Version** filter to include only the current versions of proofs waiting for your approval.

This is useful, for example, if you have been asked to approve proofs that have multiple versions. When you run the Proof Approval report with the Is Current Document Version filter, the report lists only the current version of each proof awaiting your approval, omitting earlier versions that you no longer need to work on.

## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>Contributor or Request to modify a filter </p>
   <p>Standard or Plan to modify a report</p>
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Reports, Dashboards, Calendars to modify a report</p> <p>Edit access to Filters, Views, Groupings to modify a filter</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p>  </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filter Proof Approval report to omit previous proof versions

You can create a filter for a Proof Approval report. 

1. If you already have a Proof Approval report, open it.

   Or

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   To create your own Proof Approval report, click the **Main Menu** icon ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner, or the **Main Menu** icon ![Main Menu lines](assets/lines-main-menu.png) in the upper-left corner, if available, then click **Reports** ![Reports icon](assets/reports-in-main-menu.png).
   
1. Click **New Report**. The list of object types displays.
1. Click **Proof Approval** in the list. 
   The report builder opens. 
1. Click **Filters**, then click **Add a Filter Rule**.

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. Click inside the **Set Filter Rules for your Report** box, then select **Proof Approval** from the list. 
1. Click **Is Current Document Version** in the list under the **Proof Approval** object.
1. Choose Equal for your filter modifier, then select True. 
1. Click **Save + Close** in the lower-left corner of Adobe Workfront, then click **Apply** in the box that appears.

   The Proof Approval report displays only proofs associated with the current versions of any document, if any proof approvals match this filtering criteria. 
