---
filename: reference-custom-form-report
product-area: reporting
navigation-topic: create-and-manage-reports
title: Reference a custom form in a report
description: You can reference the custom forms of an object in the Views, Filters, and Groupings of a report for that object.
---

# Reference a custom form in a report

You can reference the custom forms of an object in the Views, Filters, and Groupings of a report for that object.

You can reference the content of custom forms to include in a report, or you can reference information about the custom forms themselves to include in a report.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><em>Adobe Workfront</em> license*</td> 
   <td> <p><em>Plan</em> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to&nbsp;Reports,&nbsp;Dashboards,&nbsp;Calendars</p> <p>Edit access to Filters,&nbsp;Views, Groupings</p> <p>Note: If you still don't have access, ask your <em>Workfront administrator</em> if they set additional restrictions in your access level. For information on how a <em>Workfront administrator</em> can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to a report</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your *Workfront administrator*.

## Prerequisites

The custom form must exist before you can reference it in a report.

For more information on creating custom forms, see [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Reference the content of custom forms

You can reference fields within custom forms. After a custom form is applied to an object, all of the fields associated with that custom form are available to be referenced in a report as any other field on the object would be.

>[!NOTE]
>
>For fields that have multiple options, all options are available in the Filters and Prompts of the report, including those which are hidden.   
>For more information about hiding choices from a custom field with multiple options, see the article [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

When creating the report, simply use the object type of the form as the field source, and use the name of the custom field as the field name.

For example, you might have a custom form applied to all projects that includes the custom field `Consultant`. To create a report that lists all of the projects where Olivia Kim is the consultant, use the `Project` object type as the field source, and use `Consultant` as the field name. Set the filter qualifier to `Equal`, then type Olivia Kim.

<!--
<img src="assets/qs-consultant-filter-example-350x126.png" style="width: 350;height: 126;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
-->

![](assets/qs-consultant-filter-example-350x126.png)

For more information about creating a report, see the article [Create a custom report](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Reference information about custom forms

You can reference information about custom forms, such as the name of any custom forms associated with an object.

​Depending on the element (View, Filter, or Grouping), you can reference either:

* The primary custom form applied to an object:

  This is the form that appears first on the Details page of the object.

* All custom forms (if more than one custom form is applied to an object)

You can reference custom forms on Views, Filters, and Groupings:

* [Reference custom forms in a report View (Column)](#referencing-custom-forms-in-a-report-view-(column)) 
* [Reference custom forms in a report Filter](#referencing-custom-forms-in-a-report-filter) 
* [Reference custom forms in a report Grouping](#referencing-custom-forms-in-a-report-grouping)

### Reference custom forms in a report View (Column)

To display all custom forms associated with an object:

<ol> 
 <li value="1"> <p>Begin creating a report as described in the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.</p> </li> 
 <li value="2"> <p>On the <span class="bold">Columns</span> tab, expand the object type that the custom form that you want to reference is applied to, then click <span class="bold">Category Name</span>.<br>For example, to display all custom forms associated with a task, expand the <span class="bold">Task</span> field source, then click the <span class="bold">Category Name</span> field name.<br><draft-comment>
    <img src="assets/qs-category-name-column-350x267.png" style="width: 350;height: 267;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   </draft-comment><img src="assets/qs-category-name-column-350x267.png" style="width: 350;height: 267;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"></p> </li> 
</ol>

To display only the primary custom form associated with the object:

<ol> 
 <li value="1"> <p>Begin creating a report as described in the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.</p> </li> 
 <li value="2"> <p>On the <span class="bold">Columns</span> tab, expand the <span class="bold">Category</span> field source, then click the <span class="bold">Name</span> field name.<br><draft-comment>
    <img src="assets/qs-category-name-column-2-350x248.png" style="width: 350;height: 248;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   </draft-comment><img src="assets/qs-category-name-column-2-350x248.png" style="width: 350;height: 248;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"></p> </li> 
</ol>

### Reference custom forms in a report Filter

To filter on all custom forms associated with the object type:

<ol> 
 <li value="1"> <p>Begin creating a report as described in the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.</p> </li> 
 <li value="2"> <p>On the <span class="bold">Filters</span> tab, expand <span class="bold">Categories</span>, then click <span class="bold">Name</span>.<br><draft-comment>
    <img src="assets/qs-categories-name-filter-350x311.png" style="width: 350;height: 311;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   </draft-comment><img src="assets/qs-categories-name-filter-350x311.png" style="width: 350;height: 311;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"></p> </li> 
 <li value="3"> <p>Select the condition qualifier that you want to use:</p> 
  <ul> 
   <li>Is Blank</li> 
   <li>Is Not Blank</li> 
   <li>Contains</li> 
   <li>Does Not Contain</li> 
   <li>Equal</li> 
   <li>Not Equal<br></li> 
  </ul> <p>For more information about each qualifier, see the article <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Filter and condition modifiers</a>. <br> <note type="note">  If the field you are filtering for has multiple options and you use the 
    <span class="bold">Not Equal</span> or 
    <span class="bold">Does Not Contain</span> qualifiers, this filters out the results that contain only the choice you specify. If the field contains additional options including the one specified, those results are not filtered from the report. This includes filtering for multiple Custom Forms if they are attached to the same object. 
   </note></p> </li> 
 <li value="4"> <p>Begin typing the name of the custom form that you want to filter on, then click the name when it appears in the drop-down list.</p> </li> 
 <li value="5"> <p>(Optional) Click <span class="bold">Add another Filter Rule</span>, then repeat steps 2-4 to create additional filter rules.</p> </li> 
 <li value="6"> <p>Click <span class="bold">Save+Close</span>.</p> </li> 
</ol>

To filter only on the primary custom form associated with the object type:

<ol> 
 <li value="1"> <p>Begin creating a report as described in the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.</p> </li> 
 <li value="2"> <p>On the <span class="bold">Filters</span> tab, expand the <span class="bold">Category</span> field source, then click the <span class="bold">Name</span> field name.<br><draft-comment>
    <img src="assets/qs-category-name-filter-350x437.png" style="width: 350;height: 437;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   </draft-comment><img src="assets/qs-category-name-filter-350x437.png" style="width: 350;height: 437;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"><br></p> </li> 
 <li value="3"> <p>Select the condition qualifier that you want to use:</p> 
  <ul> 
   <li>Is Blank</li> 
   <li>Is Not Blank</li> 
   <li>Contains</li> 
   <li>Does Not Contain</li> 
   <li>Equal</li> 
   <li>Not Equal<br></li> 
  </ul> <p>For more information about each qualifier, see the article <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">Filter and condition modifiers</a>.</p> </li> 
 <li value="4"> <p>Begin typing the name of the custom form that you want to filter on, then click the name when it appears in the drop-down list.</p> </li> 
 <li value="5"> <p>(Optional) Click <span class="bold">Add another Filter Rule</span>, then repeat steps 2-4 to create additional filter rules.</p> </li> 
 <li value="6"> <p>Click <span class="bold">Save+Close</span>.</p> </li> 
</ol>

### Reference custom forms in a report Grouping

>[!NOTE]
>
>You can group items only by the primary custom form that is associated with the object; you cannot group items by all forms that are associated with the object.

<ol> 
 <li value="1"> <p>Begin creating a report as described in the article <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Create a custom report</a>.</p> </li> 
 <li value="2"> <p>On the <span class="bold">Groupings</span> tab, expand <span class="bold">Category</span>, then click <span class="bold">Name</span>.<br><draft-comment>
    <img src="assets/qs-category-name-grouping-350x373.png" style="width: 350;height: 373;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   </draft-comment><img src="assets/qs-category-name-grouping-350x373.png" style="width: 350;height: 373;" data-mc-conditions="QuicksilverOrClassic.Quicksilver"></p> </li> 
</ol>

