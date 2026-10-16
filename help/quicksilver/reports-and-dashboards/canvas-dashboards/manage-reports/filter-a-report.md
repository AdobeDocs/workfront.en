---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Filter a report in a Canvas Dashboard
description: Add or edit a filter on a report to control which data displays in a Canvas Dashboard.
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
# Filter a report in a Canvas Dashboard

>[!IMPORTANT]
>
>The Canvas Dashboards feature is currently only available for users participating in the beta stage. Parts of the feature may not be complete or work as intended during this stage. Please submit any feedback regarding your experience by following the instructions in the [Provide feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) section in the Canvas Dashboards beta overview article.<br>
>If you have feedback regarding a possible bug or technical issue, please submit a ticket to Workfront Support. For more information, see [Contact Customer Support](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Please note that this beta is not available on the following cloud providers:
>
>* Bring Your Own Key for Amazon Web Services
>* Azure
>* Google Cloud Platform 

You can filter a report to control which data displays, both while you build the report and any time afterward. The filtering options and behavior are the same in either case.

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

You must have a report on a dashboard, or be building one, before you can filter it. For more information, see [Create a Canvas Dashboard](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

## Add or edit a report filter

To add or edit a filter on a report:

1. Open the report's filter panel:

   * If you're building a report, click the **Filter** icon in the left panel of the **Configure** dialog box.
   * If you're editing an existing report, click the **More** icon in the upper-right corner, select **Edit**, then click the **Filters** panel in the **Configure** dialog box.

1. Click **Edit filter**.

1. Click **Add condition**, then define the condition:

   * Click **Pick Field**, then select the field you want to filter by.
   * Select the modifier that defines what kind of condition the field must meet.
   * Type or select the value to evaluate against, if the modifier requires one.

   ![Add condition](assets/add-condition.png)

1. (Optional) Repeat the previous step to add more conditions.

1. (Optional) Click **Add filter group** to add another set of filtering criteria. The default operator between the sets is AND. Click the operator to change it to OR.

>[!NOTE]
>
>For the full list of fields, operators, wildcards, and special filtering rules, see [Report filter reference for Canvas Dashboards](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/filter-reference.md).

1. Click **Save**.
