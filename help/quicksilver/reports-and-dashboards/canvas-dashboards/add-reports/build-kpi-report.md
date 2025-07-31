---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Build a KPI report
description: A KPI report that prominently displays a single aggregated KPI can be added to a Canvas Dashboard.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: e1c68ac3-112e-4f9e-b644-f44bb0778b92
---
# Build a KPI report

>[!IMPORTANT]
>
>The Canvas Dashboards feature is currently only available for users participating in the beta stage. For more information, see [Canvas Dashboards beta information](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md).

You can build and add a KPI report to a Canvas Dashboard that visually represents your key performance indicator data as a number, which you can then use to see how your projects and teams are performing.   

![KPI report example](assets/kpi-example-main.png)

+++ Expand to view access requirements. 

 <table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan</p></td> 
   <td> 
<p>Any </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td> 
<p>Current: Plan </p> 
<p>New: Standard</p> 
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

You must create a dashboard before you can build a KPI report. 

## Build a KPI report in a Canvas Dashboard

There are many configuration options available for building a KPI report. In this section, we'll walk you through the general process of creating one. 

{{step1-to-dashboards}}

1. In the left panel, click **Canvas Dashboards**. 

1. Click **New Dashboard** in the upper-right corner.  

1. In the **Create dashboard** box, enter the dashboard's **Name** and **Description**.  

1. Click **Create**. 

1. In the **Add report** box, select **Create report**.  

1. On the left side, select **KPI**.

1. In the upper-right corner, click **Create report**.  

1. Follow the steps below to configure the **Details** section: 

    1. Enter a report **Name**. 
    1. Enter a report **Description**. 
    
        >[!NOTE]
        >
        >The description will be used as a caption below the KPI value. If you don't enter a description, a caption will be generated for you based on the aggregator and aggregation type you select in the following steps.  

1. Follow the steps below to configure the **Build KPI** section: 

    1. In the left panel, click the **Build KPI** ![Build KPI icon](assets/build-kpi-icon.png) icon.  

    1. Click **Select field** and then specify the field you want to add to the report.  

    1. In the **Aggregation type** drop-down, select how the data rolls up to produce the KPI output. The options in this field will vary depending on the type of field that was selected in the previous step. 

1. Follow the steps below to configure the **Filter** section: 

    1. In the left panel, click the **Filter** ![Filter icon](assets/filter-icon.png) icon. 

    1. Select **Edit filter**. 

    1. Click **Add condition** and then specify the field you want to filter by and the modifier that defines what kind of condition the field must meet.   

    1. (Optional) Click **Add filter group** to add another set of filtering criteria. The default operator between the sets is AND. Click the operator to change it to OR. 

1. Follow the steps below to configure the **Drilldown Column Settings** section: 

    1. In the left panel, click the **Drilldown Columns** ![Drilldown columns icon](assets/drilldown-column.png) icon. The fields from your chart automatically appear as columns in the preview section on the right.  

    1. (Optional) To update any of the existing column configurations, select the column you want to update in the **Current columns** section and then update the desired information (e.g. label, linked status, and formatting rules). 

    1. Click **Add column** and then select the field you want to display as a column in the table. Repeat this process for each column you want to add.  

1. Follow the steps below to configure the **Drilldown Group Settings** section: 

    1. In the left panel, click the **Group Settings** ![Drilldown group icon](assets/drilldown-group-icon.png) icon. 

    1. Click the **Add grouping** button and then select the field you want to create as a grouping.  

1. Click **Save** to create the report and add it to the dashboard. 


