---
filename: use-existing-calc-field-new-custom-form
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Using an existing calculated custom field on a new custom form
description: You can use the same calculated custom field on custom forms that belong to different objects. For example, you can use the Profit calculated field that you created for the project custom form on a task custom form.
---

# Using an existing calculated custom field on a new custom form

You can use the same calculated custom field on custom forms that belong to different objects. For example, you can use the Profit calculated field that you created for the project custom form on a task custom form.

For information about adding a calculated custom field to a custom form, see [Add calculated data to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

When using an existing calculated custom field, the calculation does not transfer to the new form. You must add the calculation again, on the same field, on the new custom form.

>[!TIP]
>
>This is when using the calculation stored in the **Instructions** field of the custom form helps.

You can also have a different calculation for the same field, on the new form. Keeping the same name for the calculated custom field ensures cohesiveness and consistency in your naming convention.

>[!IMPORTANT]
>
>Calculated custom fields can become outdated over time. To ensure that you always view the up-to-date calculation in these fields, do one of the following:
>
>* Select the Recalculate Custom Expressions option when editing objects in bulk.
>* Select the Update previous calculations option when editing a Calculated Custom Field on a custom form.
>

