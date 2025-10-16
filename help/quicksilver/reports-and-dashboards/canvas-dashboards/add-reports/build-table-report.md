---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Build a table report in a Canvas Dashboard
description: You can add a table report to a Canvas Dashboard in order to visualize your data in a table format.
author:  Courtney and Jenny 
feature: Reports and Dashboards
exl-id: a7aa8614-6e80-4fc1-88ff-d952d87ddcbc
---
# Build a table report in a Canvas Dashboard

>[!IMPORTANT]
>
>The Canvas Dashboards feature is currently only available for users participating in the beta stage. Parts of the feature may not be complete or work as intended during this stage. Please submit any feedback regarding your experience by following the instructions in the [Provide feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) section in the Canvas Dashboards beta overview article.<br>
>If you have feedback regarding a possible bug or technical issue, please submit a ticket to Workfront Support. For more information, see [Contact Customer Support](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Please note that this beta is not available on the following cloud providers:
>
>* Bring Your Own Key for Amazon Web Services
>* Azure
>* Google Cloud Platform 

You can add a table report to a Canvas Dashboard in order to visualize your data in a table format.  

![Table report example](assets/table-example-main.png)

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
</tbody> 
</table> 

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Prerequisites

You must create a dashboard before you can build a table report. 


## Build a table report in a Canvas Dashboard

There are many configuration options available for building a table report. In this section, we'll walk you through the general process of creating one.

{{step1-to-dashboards}}

1. In the left panel, click **Canvas Dashboards**. 

1. Click **New Dashboard** in the upper-right corner.  

1. In the **Create dashboard** box, enter the dashboard's **Name** and **Description**.  

1. Click **Create**. 

1. In the **Add report** box, select **Create report**.  

1. On the left side, select **Table**. 

1. In the upper-right corner, click **Create report**. 

1. (Optional) Follow the steps below to configure the **Details** section: 
    
    1. Enter a report **Name**.

    1. Enter a report **Description**.

1. Follow the steps below to configure the **Build table** section:

    1. In the left panel, click the **Table columns** ![Build table icon](assets/drilldown-column.png) icon. 

    1. Click **Add column** and then select the field you want to display as a column in the table. The column appears in the preview section on the right.  

  

    1. Repeat the above step for each column you want to add. 

1. Follow the steps below to configure the **Filter** section: 

    1. In the left panel, click the **Filter** ![Filter icon](assets/filter-icon.png) icon.

    1. Select **Edit filter**. 

    1. Click **Add condition** and then specify the field you want to filter by and the modifier that defines what kind of condition the field must meet. The column appears in the preview section on the right.

1. (Optional) Click **Add filter group** to add another set of filtering criteria. The default operator between the sets is AND. Click the operator to change it to OR. 

1. Follow the steps below to configure the **Drilldown Group Settings** section: 

    1. In the left panel, click the **Group Settings** ![Group settings icon](assets/drilldown-group-icon.png) icon. 

    1. Click the **Add grouping** button and then select the field you want to create as a grouping. The grouping column appears in the preview section on the right. 

1. Click **Save** to create the report and add it to the dashboard. 

## Build a table report example

In this section, we will go over the steps to create a table report that displays pending document approvals. 

For more information on table report examples, see [Create a report dashboard for review and approvals](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md).

{{step1-to-dashboards}}

1. In the left panel, click **Canvas Dashboards**. 

1. Click **New Dashboard** in the upper-right corner.  

1. In the **Create dashboard** box, enter the dashboard's **Name** and **Description**.  

1. Click **Create**. 

1. In the **Add report** box, select **Create report**.  

1. On the left side, select **Table**. 

1. In the upper-right corner, click **Create report**. 

1. Follow the steps below to configure the **Details** section: 

    1. Type _Pending approvals_ in the **Name** field. 
    1. Type a description in the **Description** field. This text displays as a tooltip next to the chart name. 

1. Follow the steps below to configure the **Build table** section: 

    1. In the left panel, click the **Table columns** ![Table columns icon](assets/drilldown-column.png) icon.
    1. Click **Add column**.
    1. Scroll down and select **Document Approvals** > **Status**.
    1. Add the following columns:

    <table>
    <tr>
    <td><strong>Project name</strong></td>
    <td>Document Version > Document > Project > Name</td>
    </tr>
    <tr>
    <td><strong>Document name</strong></td>
    <td>Document Version > Document > type <em>Name</em> in the search box.</td>
    </tr>
    <tr>
    <td><strong>Document version</strong></td>
    <td>Document Version > Document > Version</td>
    </tr>
    <tr>
    <td><strong>Deadline</strong></td>
    <td>Document Approval > Approval Stage > Deadline</td>
    </tr>
    <tr>
    <td><strong>Requested by</strong></td>
    <td>Document Approval > Approval Stage > Approval Stage Participants* > Requester > type <em>Name</em> in the search box.</td>
    </tr>
    <tr>
    <td><strong>Requested date</strong></td>
    <td>Document Approval > Approval Stage > Approval Stage Participants* > Created at</td>
    </tr>
    <tr>
    <td><strong>Approver</strong></td>
    <td>Document Approval > Approval Stage > Approval Stage Participants* > Participant User > type <em>Name</em> in the search box.</td>
    </tr>
    </table>


    *Approval Stage Participants is truncated to _Approval Stage Pa.._
    

1. Follow the steps below to configure the **Filter** section: 
    1. In the left panel, click the **Filter** ![filter tab icon](assets/filter-tab.png) icon.
    1. Click **Edit Filter**, then **Add condition**.
    1. Click into the empty condition filter, then click **Pick a Field**.
    1. Select **Status**.
    1. Change the operator to **Equal**, then type _pending approval_ in the textbox.
        ![pending approval table filter example](assets/pending-approval-table-filter.png) 
    1. (Optional) Add additional filters as described in the **Optional filters** section below.
1. Click **Save** in the top-right corner of the screen.

## Considerations when building a table report

### Utilizing the field selector

The **Sections** drop-down in the **Build table** section is designed to narrow down the choices in a field selector to make an object easier to find when building a table report. To start, you would select a base entity object.

* **All Sections**: All object types in Workfront Workflow and Workfront Planning.
* **Workfront Objects**: Native Workfront Workflow objects.
* **Planning Record Types**: Custom record types defined in Workfront Planning.

![Sections drop-down](assets/sections-dropdown.png)

Once the base entity object has been selected, the **Sections** drop-down then updates with applicable field type options to choose from.

* **All Sections**: Native fields, custom fields, and related objects.
* **All Fields**: Both native and custom fields (excludes relationships).
* **Custom Fields**: Customer-defined fields either on a custom form or Planning record.
* **Workfront Fields**: Native fields only.
* **Relationships**: Connected records.

![Reportable objects selection](assets/reportable-objects-selection.png)

### Referencing children objects

Available relationships for additional columns, filter options, and grouping attributes are generally limited to objects higher in the Workfront object hierarchy or otherwise have a single selection on the report's base entity object. There are some exceptions to this, which include the following:

* Project > Tasks
* Document Approval > Document Approval Stages
* Document Approval Stages > Document Approval Stage Participants 

When utilizing any of the parent-to-child relationships listed above, you will see a row in the table for each child record connected to the parent object.  
