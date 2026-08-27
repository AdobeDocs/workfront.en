---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Build a pivot table report in a Canvas Dashboard
description: You can add a pivot table report to a Canvas Dashboard to see aggregated totals for your data in a table format.
author: Courtney
feature: Reports and Dashboards
---
# Build a pivot table report in a Canvas Dashboard

>[!IMPORTANT]
>
>The Canvas Dashboards feature is currently only available for users participating in the beta stage. Parts of the feature may not be complete or work as intended during this stage. Please submit any feedback regarding your experience by following the instructions in the [Provide feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) section in the Canvas Dashboards beta overview article.<br>
>If you have feedback regarding a possible bug or technical issue, please submit a ticket to Workfront Support. For more information, see [Contact Customer Support](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Please note that this beta is not available on the following cloud providers:
>
>* Bring Your Own Key for Amazon Web Services
>* Azure
>* Google Cloud Platform 

You can add a pivot table report to a Canvas Dashboard to see aggregated totals for your data—such as sums, counts, and averages—in a table format. Pivot tables are useful when comparing multiple aggregated values or counts against multiple dimensions.

![Pivot table report example](assets/pivot-table-example.png)

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
</tbody> 
</table> 

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Prerequisites

You must create a dashboard before you can build a pivot table report. For more information, see [Create a Canvas Dashboard](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

## Build a pivot table report in a Canvas Dashboard

There are many configuration options available for building a pivot table report. In this section, we'll walk you through the general process of creating one.

{{step1-to-dashboards}}

1. In the left panel, click **Canvas Dashboards**, then click the name of the dashboard you want to add the report to. 

1. Click **Add report** in the upper-right corner of the page. 

1. In the **Add report** box, select **Create report**.  

1. On the left side, select **Pivot Table**. 

1. In the upper-right corner, click **Create report**. 

1. (Optional) Follow the steps below to configure the **Details** section: 

    1. Choose the **Root Entity** for the report. 
    
        >[!NOTE]
        >
        > The Root Entity sets which object your fields come from. Once selected, every field selector you use later in this report starts from that object, so you can go straight to the field you want.


    1. Enter a report **Name**.

    1. Enter a report **Description**.

    1. (Optional) In the **Run this report with the access rights of** field, begin typing the name of the user whose permissions you want the report to use, then select the user when they appear in the list. When you configure a report to run as another user, all viewers of the dashboard see the same data, regardless of their own access level. If you don't select a user, each viewer sees data based on their own permissions.

        >[!IMPORTANT]
        >
        >If the selected user is deactivated or loses access to the relevant workspaces or record types, the report may display incomplete data or fail to render. 

1. Follow the steps below to configure the **Metrics** section:

    1. In the left panel, click the **Show metrics** ![Build KPI icon](assets/build-kpi-icon.png) icon. 

    1. Click **Add metric** and then select the field you want. The field appears as a column in the preview section on the right.

        >[!NOTE]
        >
        > A metric (also called a measure) is a number field you want to add up or total. For example, you might add up all the costs, or count how many tasks there are.


    1. Enter a **Column label**. 

    1. In the **Aggregation type** drop-down, select how the data rolls up for that field. The options in this field vary depending on the type of field you selected.

    1. Repeat the above two steps for each metric you want to add. 

1. Follow the steps below to configure the **Segments** section: 

    1. In the left panel, click the **Segments** ![Drilldown group icon](assets/drilldown-group-icon.png) icon.

    1. Click **Add segment** and then select the segment you want. The field appears as a column in the preview section on the right.

        >[!NOTE]
        >
        >A segment is the category you use to group your data, like grouping tasks by status or by owner. It's how your metrics get sorted and totaled.


    1. Repeat the above two steps to add up to 2 segments.

1. Follow the steps below to configure the **Filter** section: 

    1. In the left panel, click the **Filter** ![Filter icon](assets/filter-icon.png) icon.

    1. Select **Edit filter**. 

    1. Click **Add condition** and then specify the field you want to filter by and the modifier that defines what kind of condition the field must meet.

    1. (Optional) Click **Add filter group** to add another set of filtering criteria. The default operator between the sets is AND. Click the operator to change it to OR. 

1. Follow the steps below to configure the **Drilldown Column Settings** section: 

    1. In the left panel, click the **Drilldown Columns** ![Drilldown columns icon](assets/drilldown-column.png) icon. 

    1. Click **Add column** and then select the field you want to display as a column in the drilldown table. Repeat this process for each column you want to add.  

1. Click **Save** to create the report and add it to the dashboard. 

## Build a pivot table report example

In this section, we will go over the steps to create a pivot table report that summarizes task completion data.

{{step1-to-dashboards}}

1. In the left panel, click **Canvas Dashboards**, then click the name of the dashboard you want to add the report to. 

1. Click **Add report** in the upper-right corner of the page. 

1. In the **Add report** box, select **Create report**.  

1. On the left side, select **Pivot Table**. 

1. In the upper-right corner, click **Create report**. 

1. Follow the steps below to configure the **Details** section: 

    1. Choose **Task** as the **Root Entity**.
    1. Type *Task planned vs actual hours by portfolio and project* in the **Name** field. 
    1. Type a description in the **Description** field. 

1. Follow the steps below to configure the **Metrics** section: 

    1. In the left panel, click the **Show metrics** ![Build KPI icon](assets/build-kpi-icon.png) icon.
    1. Click **Add metric**, then select **Name**. Type *Task count* in the **Column label** field. In the **Aggregation type** drop-down, select **Count**.
    1. Click **Add metric**, then select **Actual hours**. Type *Actual hours* in the **Column label** field. In the **Aggregation type** drop-down, select **Sum**.
    1. Click **Add metric**, then select **Planned Hours**. Type *Total planned hours* in the **Column label** field. In the **Aggregation type** drop-down, select **Sum**.

1. Follow the steps below to configure the **Segments** section: 

    1. In the left panel, click the **Segments** ![Drilldown group icon](assets/drilldown-group-icon.png) icon.
    1. Click **Add segment**, then select **Project** > **Portfolio** > **Name**.
    1. Click **Add segment**, then select **Project** > **Name**.

1. Follow the steps below to configure the **Filter** section: 

    1. In the left panel, click the **Filter** ![Filter icon](assets/filter-icon.png) icon.
    1. Select **Edit filter**, then **Add condition**.
    1. Click into the empty condition filter, then click **Pick a Field**.
    1. Select **Status**.
    1. Change the operator to **Equal**, then choose *in progress*.

1. Follow the steps below to configure the **Drilldown Column Settings** section: 

    1. In the left panel, click the **Drilldown Columns** ![Drilldown columns icon](assets/drilldown-column.png) icon.
    1. Click **Add column**, then select **Name**.
    1. Click **Add column**, then select **Assigned To** > **Name**.
    1. Click **Add column**, then select **Planned Completion Date**.

1. Click **Save** in the top-right corner of the screen.

## Considerations when building a pivot table report

### Reports with financial data

Users with View or Edit access to Financial Data in their access level will still see financial data in Canvas Dashboard visualizations—even if the View finance permission is removed at the task or project level.

* Users without financial data rights at the access level will not see financial data in reports.
* Users who do see financial data are limited to records they already have permission to view (projects, tasks, issues, etc.). They will not see financial values for records they cannot access.
* Report creators should exercise caution when including financial data in dashboards and be mindful of who they share dashboards with to prevent unintended access.

This is a known limit, and we plan to address it in the future.

### Utilizing the field selector

The **Sections** drop-down in the **Build pivot table** section is designed to narrow down the choices in a field selector to make an object easier to find when building a pivot table report. To start, you would select a base entity object.

* **All Sections**: All object types in Workfront and Workfront Planning.
* **Workfront Objects**: Native Workfront objects.
* **Planning Record Types**: Custom record types defined in Workfront Planning.

![Sections drop-down](assets/sections-dropdown.png)

Once the base entity object has been selected, the **Sections** drop-down then updates with applicable field type options to choose from.

* **All Sections**: Native fields, custom fields, and related objects.
* **All Fields**: Both native and custom fields (excludes relationships).
* **Custom Fields**: Customer-defined fields either on a custom form or Planning record.
* **Workfront Fields**: Native fields only.
* **Relationships**: Connected records.

![Reportable objects selection](assets/reportable-objects-selection.png)

### Referencing related objects

We limit the access to choosing children objects as segments of a pivot table. Segment options can be attributes of the record itself or other related records that do not represent a 1:many or many:many relationship.

We also limit access to referencing any parent or child attribute as a metric to reduce the potential for double-counting or double-summarizing values, leading to a misrepresentation of the actual data.
