---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Error message: There is a slight problem. That field is used in a multi-form configuration'
description: When you change a calculation in a calculated custom field on a custom form and an error message tells you that the field is used in a multi-form configuration, you need to replace the field with a new field containing the calculation you want to use.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 43668525-5572-4d82-8eed-0e320249f296
---
# Error message: There is a slight problem. That field is used in a multi-form configuration

## Problem

When you change a calculation on a calculated custom field on a custom form, [!DNL Adobe Workfront] might display the following warning:

There's a slight problem

[The field] is used in a multi-form configuration, if you would like to change this formula you will need to remove this field and replace it with a new one containing the desired calculation.

## Cause

At least two custom forms containing the calculated custom field you're trying to change are attached to a single object in your [!DNL Workfront] instance.

**Example:** Custom forms A and B are both attached to the same task. Both forms contain a calculated custom field called Profit. You encounter the error when you try to edit the calculation in the Profit field on custom form A.

You can't change the calculation for the custom field in one of the forms because that would conflict with the formula in the same field in the other form.
To resolve this conflict, you must find the object where the multiple forms with the same calculated custom field are attached, then do one of the following:

* Remove one of the forms from the object.
* Change the calculation as needed, but do so in all of the custom forms that are attached to the object.
* In all of the custom forms attached to the object, add a new calculated custom field containing the calculation you need and mark the old calculated custom field as obsolete.

This article explains how to find the object and then resolve the problem in one of these three ways.

## Find the object where the custom forms are attached {#find-the-object-where-the-custom-forms-are-attached}

1. Click the **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) in the upper-right corner of [!DNL Adobe Workfront], then click **[!UICONTROL Users]** ![](assets/users-icon-in-main-menu.png).

1. Click **[!UICONTROL Custom Forms]** > **[!UICONTROL Fields]**.
1. Apply the **[!UICONTROL Field List]** view to find the calculated field you are trying to modify, and make note of every custom form on which it is used (e.g. Form 1, Form 2, Form 3) .
1. Click **[!UICONTROL Forms]**, then apply the **[!UICONTROL Form List]** view.
1. Click the **[!UICONTROL Filter]** drop-down list, then **[!UICONTROL New Filter]**.

1. Click **[!UICONTROL Add a Filter Rule]**, then start typing "custom form name" and select this value when it displays in the list.
1. Select **[!UICONTROL Equal]** for the filter modifier, start typing the name of each form you made a note of in Step 1, then select it when it displays.

   **Example:** Custom Form Name Equals Form 1, Form 2, Form 3.

1. Click **[!UICONTROL Save Filter]**, then name the new filter, and click **[!UICONTROL Save Filter]**.

1. In the list of forms, make note of the object type of the filter, such as Task or Issue, that displays in the **[!UICONTROL Type]** column.
1. On each custom form you found in Step 1, create a new Checkbox custom field with a single default value of Yes.

   **Example:** Field 1 on Form 1 = Yes, Field 2 on Form 2 = Yes, Field 3 on Form 3 = Yes. This means "The Calculated Custom Field exists on Form 1," or "The Calculated Custom Field exists on Form 2," and so on.

1. In the **[!UICONTROL Search icon]** ![](assets/search-icon.png) in the upper-right corner of the screen, click **[!UICONTROL Advanced Search]**.
1. Click the object of your custom form (such as Issue), click **[!UICONTROL Filter your results]**, then click **[!UICONTROL Add a filter]**.
1. Start typing the name of a Checkbox field in the **[!UICONTROL Start typing field name]** field and select it when it displays in the list, then select **[!UICONTROL Equal]** and type **[!UICONTROL Yes]** (without quotation marks) in the following box.

   **Example:** Field 1 Equal (Case Sensitive) Yes.

1. Click **[!UICONTROL Add a Filter]** and add all Checkbox fields to your Advanced Search.

   Look for every possible combination.

   **Example:** Build several filters with the combinations you find, as listed below. You should find objects with multiple attached custom forms that contain the same calculated fields. You might find the following scenarios:

   * Field 1= Yes + Field 2 = Yes + Field 3 = Yes (no objects, for example)
   * Field 1= Yes + Field 2 = Yes (no objects, for example)
   * Field 1= Yes + Field 3 = Yes (two objects, for example)

   This means that the calculated field exists on both Form 1 and Form 3, because the corresponding Checkbox fields (Field 1 and Field 3) exist on these objects.

   Field 2 = Yes + Field 3 = Yes (no objects, for example)

1. Continue on to one of the following sections in this article:

   * [Remove one of the custom forms from the object and edit the calculation there](#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there)
   * [Make identical edits in the calculation in all of the attached custom forms](#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms)
   * [Add a new calculated field containing the edited calculation to one or all of the attached custom forms](#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms)

## Remove one of the custom forms from the object and edit the calculation there {#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there}

1. Find the object where the custom forms are attached, as explained in [Find the object where the custom forms are attached](#find-the-object-where-the-custom-forms-are-attached) in this article, then open the object.
1. Remove one of the custom forms from the object, then save the object.

   >[!NOTE]
   >
   >To add the fields from the form you removed from the object, you might need to edit the custom form that remains attached to the object. This way, you can preserve the custom data information on the object.

1. In the custom form you removed, edit the calculation for the custom field you were trying to update originally, then click **[!UICONTROL Save]**.

   This time, [!DNL Workfront] should not encounter a conflict.

1. (Optional) Remove the Checkbox fields from the custom forms or delete them from [!DNL Workfront].

## Make identical edits in the calculation in all of the attached custom forms {#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms}

>[!IMPORTANT]
>
>Data is lost in the objects where the custom form is already attached when you follow these steps. However, if the calculated field references static fields, not calculated fields, you can use [!UICONTROL Recalculate Custom Expressions] option on the object to restore the lost data

1. Find the object where the custom forms are attached, as explained in [Find the object where the custom forms are attached](#find-the-object-where-the-custom-forms-are-attached) in this article.
1. Remove the field from all of the custom forms that are attached to the object, then save the forms.

1. Add the custom field containing the new calculation back to the custom forms.

   >[!IMPORTANT]
   >
   >The calculations must be identical in all of the attached custom forms.

1. (Optional) Remove the Checkbox fields from the forms or delete them from [!DNL Workfront].

## Add a new calculated field containing the edited calculation to one or all of the attached custom forms {#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms}

To avoid losing data in the existing calculated custom field, or if you need to the edited calculation in only one of the custom forms attached to the object you found:

1. Find the object where the custom forms are attached, as explained in [Find the object where the custom forms are attached](#find-the-object-where-the-custom-forms-are-attached) in this article.
1. Add a new calculated custom field containing the calculation you need to one or all of the forms.
1. Rename the old calculated custom field **Obsolete**.

   On all of the forms that were attached to the object, this older calculated custom form preserves its historical data, but users stop using it.

   >[!IMPORTANT]
   >
   >The older field might be referenced in other calculated custom fields, so you need to update those calculations after changing its name.

1. (Optional) Remove the Checkbox fields from the forms or delete them from Workfront.

<!--
<blockquote data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Problem</h2>
<p>You get the following error while editing a calculated Custom Field on a custom form: </p>
<p><em>"<Name of custom field> field is used in a multi-form configuration, if you would like to change this formula you will need to remove this field and replace it with a new one containing the desired calculation."</em> </p>
<h2>Cause</h2>
<p>The error occurs because the following setup exists: currently you have at least one object in your system that has multiple custom forms attached. The calculated field you are editing exists on multiple forms attached to these objects.</p>
<p>You cannot have the same calculated field with different calculations on the same object. For this reason, the system does not allow you to make a change which will result in calculations being different.</p>
<p><a href="../../Resources/Images/Admin and setup/Tips, Tricks, and Troubleshooting/Calculated_field_error.png" class="MCXref xref" xrefformat="{para}"><img src="assets/calculated-field-error.png" alt="" width="542" height="272"></a> </p>
<p>For example, you have a task with custom forms A and B attached to it. Both forms contain the same calculated field, Field 1. You encounter this error when you try to edit the calculation for Field 1 on custom form A. </p>
<h2>Solution</h2>
<p>Remove the field from the custom form and replace it with a new one containing the desired calculation.  </p>
<p>To understand what custom forms are attached to objects, you can build a report for those objects and reference the Category Name field in the view of the report.<br>For more information about referencing custom forms in reports, see the "Referencing Custom Forms in a Report View (Column)" section in <a href="../../reports-and-dashboards/reports/creating-and-managing-reports/reference-custom-form-report.md" class="MCXref xref" xrefformat="{para}">Reference a custom form in a report</a>.</p>
<p>To understand what custom form contains a Custom Field, see the "Accessing Custom Forms and Fields" section in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md" class="MCXref xref" xrefformat="{para}">Custom forms overview</a>.</p>
</blockquote>
-->
