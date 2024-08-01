---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Reference a custom form in a report
description: You can reference the custom forms of an object in the Views, Filters, and Groupings of a report for that object.
author: Nolan
feature: Reports and Dashboards
exl-id: 8b0d2e7f-cc92-4f43-a91c-ab2b2d8a1c01
---
# Reference a custom form in a report

You can reference the custom forms of an object in the Views, Filters, and Groupings of a report for that object.

You can reference the content of custom forms to include in a report, or you can reference information about the custom forms themselves to include in a report.

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Edit access to Filters,&nbsp;Views, Groupings</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Prerequisites

The custom form must exist before you can reference it in a report.

For more information on creating custom forms, see [Design a form with the form designer](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Reference the content of custom forms

You can reference fields within custom forms. After a custom form is applied to an object, all of the fields associated with that custom form are available to be referenced in a report as any other field on the object would be.

>[!NOTE]
>
>For fields that have multiple options, all options are available in the Filters and Prompts of the report, including those which are hidden.   
>For more information about hiding choices from a custom field with multiple options, see the article [Design a form with the form designer](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

When creating the report, simply use the object type of the form as the field source, and use the name of the custom field as the field name.

For example, you might have a custom form applied to all projects that includes the custom field **Consultant**. To create a report that lists all of the projects where Olivia Kim is the consultant, use the **Project** object type as the field source, and use **Consultant** as the field name. Set the filter qualifier to **Equal**, then type Olivia Kim.

![](assets/qs-consultant-filter-example-350x126.png)

For more information about creating a report, see the article [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Reference information about custom forms

You can reference information about custom forms, such as the name of any custom forms associated with an object.

​Depending on the element (View, Filter, or Grouping), you can reference either:

* The primary custom form applied to an object:

  This is the form that appears first on the Details page of the object.

* All custom forms (if more than one custom form is applied to an object)

You can reference custom forms on Views, Filters, and Groupings:

* [Reference custom forms in a report View (Column)](#reference-custom-forms-in-a-report-view-column) 
* [Reference custom forms in a report Filter](#reference-custom-forms-in-a-report-filter) 
* [Reference custom forms in a report Grouping](#reference-custom-forms-in-a-report-grouping)

### Reference custom forms in a report View (Column) {#reference-custom-forms-in-a-report-view-column}

To display all custom forms associated with an object:

1. Begin creating a report as described in the article [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. On the **Columns** tab, expand the object type that the custom form that you want to reference is applied to, then click **Category Name**.  
   For example, to display all custom forms associated with a task, expand the **Task** field source, then click the **Category Name** field name.  
   ![](assets/qs-category-name-column-350x267.png)

To display only the primary custom form associated with the object:

1. Begin creating a report as described in the article [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. On the **Columns** tab, expand the **Category** field source, then click the **Name** field name.  
   ![](assets/qs-category-name-column-2-350x248.png)

### Reference custom forms in a report Filter {#reference-custom-forms-in-a-report-filter}

To filter on all custom forms associated with the object type:

1. Begin creating a report as described in the article [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. On the **Filters** tab, expand **Categories**, then click **Name**.  
   ![](assets/qs-categories-name-filter-350x311.png)

1. Select the condition qualifier that you want to use:

   * Is Blank
   * Is Not Blank
   * Contains
   * Does Not Contain
   * Equal
   * Not Equal

   For more information about each qualifier, see the article [Filter and condition modifiers](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >If the field you are filtering for has multiple options and you use the **Not Equal** or **Does Not Contain** qualifiers, this filters out the results that contain only the choice you specify. If the field contains additional options including the one specified, those results are not filtered from the report. This includes filtering for multiple Custom Forms if they are attached to the same object.

1. Begin typing the name of the custom form that you want to filter on, then click the name when it appears in the drop-down list.
1. (Optional) Click **Add another Filter Rule**, then repeat steps 2-4 to create additional filter rules.
1. Click **Save+Close**.

To filter only on the primary custom form associated with the object type:

1. Begin creating a report as described in the article [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. On the **Filters** tab, expand the **Category** field source, then click the **Name** field name.  
   ![](assets/qs-category-name-filter-350x437.png)  

1. Select the condition qualifier that you want to use:

   * Is Blank
   * Is Not Blank
   * Contains
   * Does Not Contain
   * Equal
   * Not Equal

   For more information about each qualifier, see the article [Filter and condition modifiers](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. Begin typing the name of the custom form that you want to filter on, then click the name when it appears in the drop-down list.
1. (Optional) Click **Add another Filter Rule**, then repeat steps 2-4 to create additional filter rules.
1. Click **Save+Close**.

### Reference custom forms in a report Grouping {#reference-custom-forms-in-a-report-grouping}

>[!NOTE]
>
>You can group items only by the primary custom form that is associated with the object; you cannot group items by all forms that are associated with the object.

1. Begin creating a report as described in the article [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. On the **Groupings** tab, expand **Category**, then click **Name**.  
   ![](assets/qs-category-name-grouping-350x373.png)
