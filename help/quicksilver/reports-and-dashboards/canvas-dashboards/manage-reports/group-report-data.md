---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Group report data in a Canvas Dashboard
description: Organize report results into groups. Grouping works differently depending on the report type.
author: Courtney
feature: Reports and Dashboards
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
# Group report data in a Canvas Dashboard

>[!IMPORTANT]
>
>The Canvas Dashboards feature is currently only available for users participating in the beta stage. Parts of the feature may not be complete or work as intended during this stage. Please submit any feedback regarding your experience by following the instructions in the [Provide feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) section in the Canvas Dashboards beta overview article.<br>
>If you have feedback regarding a possible bug or technical issue, please submit a ticket to Workfront Support. For more information, see [Contact Customer Support](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Please note that this beta is not available on the following cloud providers:
>
>* Bring Your Own Key for Amazon Web Services
>* Azure
>* Google Cloud Platform 

Grouping organizes your report results so related records appear together. How grouping works depends on the report type, so this article has a separate section for each.

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
<p>Standard</p> 
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

You must have a report on a dashboard, or be building one, before you can group its data. For more information, see [Create a Canvas Dashboard](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

## Group rows in a table report

In a table report, grouping organizes the rows of the report itself.

1. In the **Configure** dialog box, click the **Group Settings** icon in the left panel.

1. Click **Add grouping**, then select the field you want to group by. The grouping appears in the preview on the right.

1. (Optional) Repeat to add more groupings.

## Configure drilldown groupings in chart and KPI reports

In chart and KPI reports, you don't group the main visualization. Instead, you configure how the drilldown table is grouped when a viewer drills into a value.

1. In the **Configure** dialog box, click the **Drilldown Group Settings** icon in the left panel.

1. Click **Add grouping**, then select the field you want to group the drilldown table by.

## Configure segments in a pivot table report

Pivot table reports don't use groupings. Instead, you define up to two segments, which are the categories the pivot's metrics are grouped and totaled by.

1. In the **Configure** dialog box, click the **Segments** icon in the left panel.

1. Click **Add segment**, then select the field you want. The segment appears as a column in the preview.

1. (Optional) Repeat to add a second segment. You can add a maximum of two segments.

## View grouped data on a dashboard

Report viewers can expand, collapse, and sort grouped data. For more information, see [View reports with grouped data](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md#view-reports-with-grouped-data) in [Use Canvas Dashboards](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md).
