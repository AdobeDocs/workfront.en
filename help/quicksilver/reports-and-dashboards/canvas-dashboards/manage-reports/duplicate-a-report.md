---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Copy and move reports in Canvas Dashboards
description: You can copy or move a report between Canvas Dashboards.
author: Courtney
feature: Reports and Dashboards
exl-id: e0f9d091-bb89-4c5b-a18d-b1e339084e67
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/5ioNl-M-KgnYE0huAbxMmLlE-qIrnwwKp-eeTRRiYLo'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: c6dd2ac5-f5bd-4e59-9101-25b156918623
    internal-label: Reports and dashboards
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Copy and move reports in Canvas Dashboards

{{highlighted-preview}}

>[!IMPORTANT]
>
>The Canvas Dashboards feature is currently only available for users participating in the beta stage. Parts of the feature may not be complete or work as intended during this stage. Please submit any feedback regarding your experience by following the instructions in the [Provide feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) section in the Canvas Dashboards beta overview article.<br>
>If you have feedback regarding a possible bug or technical issue, please submit a ticket to Workfront Support. For more information, see [Contact Customer Support](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Please note that this beta is not available on the following cloud providers:
>
>* Bring Your Own Key for Amazon Web Services
>* Azure
>* Google Cloud Platform 

You can duplicate a KPI, table, or chart report in a Canvas Dashboard after it's been created. Once duplicated, you can edit the report as needed before saving.  
 
 
## Access Requirements

+++ Expand to view access requirements for the functionality in this article. 

 <table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Any </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td> 
<p>Standard </p> 
<p>Plan</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configurations</p></td> 
   <td><p>Edit access to Reports, Dashboards, and Calendars</p>
  </td> 
  </tr>  
      <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td><p>Manage permissions for the dashboard</p>
  </td> 
  </tr>
</tbody> 
</table> 

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Prerequisites

You must add a report to a dashboard before it can be duplicated.  

For more information, see [Create a Canvas dashboard](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

## Duplicate a report in Production

{{step1-to-dashboards}}

1. In the left panel, click **Canvas Dashboards**. 
1. On the **Canvas Dashboards** page, click the **More** ![More button](assets/more-icon.png) icon in the upper-right corner of the report you want to duplicate, then select **Duplicate**. 

    ![Duplicate button](assets/duplicate-button.png)

1. (Optional) In the **Configure** box that appears, enter a new report **Name** in the **Details** tab.   

1. (Optional) Make any needed adjustments to the configurations using the tabs on the left side. 
  
    >[!NOTE]
    >
    >These tabs will vary depending on if you duplicated a KPI, table, or chart report.  For more, see [Build a KPI report in a Canvas Dashboard](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-kpi-report.md), [Build a chart report in a Canvas Dashboard](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md), and [Build a table report in a Canvas Dashboard](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-table-report.md). 
 
1. Click **Save**. The duplicated report appears on the dashboard.

<div class="preview">

## Copy or move a report in Preview

You can copy a report to the current dashboard, copy it to another dashboard, or move it to another dashboard. Copying creates a duplicate of the report at the destination; moving relocates it off its current dashboard.

>[!IMPORTANT]
>
>* To copy a report, you need Manage permissions for the destination dashboard. 
>* To move a report, you need Manage access to both the source and destination dashboards. 
>* If the report has a Run as User configured and you aren't a System Administrator or the Run as User, you can still copy or move it, but the Run as User is removed from the resulting report.


To copy or move a report:

{{step1-to-dashboards}}

1. In the left panel, click **Canvas Dashboards**.
1. Open the dashboard that contains the report.
1. Click the **More** ![More button](assets/more-icon.png) icon in the upper-right corner of the report, then select **Copy report**.

    ![Copy report option](assets/copy-report-button.png)

1. In the **Copy report** dialog box, choose one of the following options:

   <table>
   <tr>
   <td><strong>Copy</strong></td>
   <td>Click <strong>Copy</strong> at the bottom of the screen to copy the report. The current dashboard is selected by default. You need Manage access to the dashboard to copy a report.</td>
   </tr>
   <tr>
   <td><strong>Copy and move</strong></td>
   <td>Select a different destination dashboard to copy the report and move it to a new dashboard. The original report stays on the current dashboard.You need Manage access to the destination dashboard to copy and move a report. </td>
   </tr>
   <tr>
   <td><strong>Move</strong></td>
   <td>Select a different destination dashboard to move the report to. This relocates the report to the destination dashboard and removes it from the current one. You need Manage access to both the source and destination dashboards to move a report.</td>
   </tr>
   </table>

   >[!NOTE]
   >
   >If the report has a Run as User configured, and you are not a System Administrator or the user set as the Run as User, you can still copy or move the report. The Run as User is removed from the resulting report.

1. Click **Save**.

    ![copy and move](assets/copy-and-move.png)

</div>
