---
filename: chart-report-by-multi-select-custom-field
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: Chart a report by a multi-select custom field
description: You cannot chart a report by a multi-select custom field. You need to create an additional calculated field that refers to the multi-select custom field to also chart the report by the value of the multi-select custom field.
---

# Chart a report by a multi-select custom field

You cannot chart a report by a multi-select custom field. You need to create an additional calculated field that refers to the multi-select custom field to also chart the report by the value of the multi-select custom field.

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
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

Before you begin, you must create a calculated custom field that shows the values selected from the multi-select custom field.&nbsp;For information, see the [Build a calculated custom field that references a multi-select custom field](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field) section in this article.

## Chart a report by multi-select Custom Fields

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved to its own article, linked in the Note above!)</p>
-->

You cannot build a chart in a report by referencing a multi-select custom field. Instead, you can create a calculated field that records the values of the multi-select custom field on a given object and group by the calculated field.&nbsp;

* [Build a calculated custom field that references a multi-select custom field](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field) 
* [Build a chart that references a calculated custom field](#build-a-chart-that-references-a-calculated-custom-field)

### Build a calculated custom field that references a multi-select custom field {#build-a-calculated-custom-field-that-references-a-multi-select-custom-field}

To be able to build a calculated field that references a multi-select custom field, you must have the following prerequisites:

* Build the multi-select custom field in a custom form.  
  For information about building custom forms and adding custom fields to them, see the article [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

* Attach the custom form to objects.
* Populate the multi-select custom field with a value on each object.

To build the calculated custom field that references the multi-select custom field:

1. Create a custom form, or edit an existing one.  
   For information about creating custom forms, see the article [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Select the object or objects that you plan to use with the custom form. 
1. Click**Add a Field**, then **Calculated** to add the multi-select custom field to the form.

1. In the **Label** box, name the new calculated field to indicate that it references the multi-select custom field.  
   For example: "Calculated Multi-select Field."

1. In the **Calculation** box, enter the following code:

   ```
   {DE:Multi-select Custom Field}
   ```

1. Replace "Multi-select Custom Field" with the actual name of your multi-select custom field, as it appears in Workfront.

   ![](assets/calculated-multi-select-custom-field-nwe-350x223.png)

1. (Optional) If the multi-select custom field is already on this form and if this form is already attached to objects, enable the **Update previous calculations**&nbsp;option.  
   This ensures that the new field is automatically populated with the value from the multi-select custom field as it is added to the forms attached to the objects already.

1. Click **Done**.
1. Click **Save +Close**.

### Build a chart that references a calculated custom field {#build-a-chart-that-references-a-calculated-custom-field}

1. (Optional) To ensure that all the calculated fields that you want to chart by are populated with values, select all the objects in your report that contain the custom form with both the multi-select custom field and the calculated custom field, then click **Edit**. 
1. (Optional and conditional) Enable the **Recalculate Custom Expressions** field, then click **Save Changes**.  
   ![](assets/recalculate-custom-expressions-350x259.png)  

1. Go to the report where you want to add the chart for the calculated field that references the multi-select custom field. 
1. Click **Report Actions**, then **Edit**. 

1. Select the <strong>Groupings</strong> tab, then click <strong>Add Grouping</strong>. 
1. Add the<strong>Calculated Multi-select Field</strong> you created as your grouping. 
1. Select the <strong>Chart</strong> tab, and add a chart to your report.<br>For information about adding a chart to a report, see the section <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md#add-a-chart" class="MCXref xref">Add a chart to a report</a> in the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>. 
1. Select the <strong>Calculated Multi-select Field</strong> as one of the fields to display in the chart. 
1. Click <strong>Save + Close</strong>.<br>The report displays the results grouped by the Calculated Multi-select Field in a chart.

