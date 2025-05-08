---
title: Examples of Advanced Logic in Custom Forms
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: This article provides examples of expressions used to build advanced logic on custom fields.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
---
# Examples of advanced logic in custom forms

Logic rules allow you to further customize the fields on a custom form.

This article provides examples of expressions used to build advanced logic on custom fields.

For more information about adding logic to a custom form, see [Add logic rules to custom forms and fields](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront plan </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td>
   <p>New: Standard</p>
   <p>or</p>
   <p>Current: Plan</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level configurations</td> 
   <td>Administrative access to custom forms </td> 
  </tr>  
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Validation logic examples

Validation logic is built using formulas, and you can make the logic as simple or as complex as you need. The validation can be based on the values of other fields or the status of objects, and you can provide an error message for when the validation fails.

If the field with the logic applied meets the defined validation conditions when a user fills out the custom form, the field is highlighted and the error message is displayed.

You can apply validation logic to the following field types: single line text, paragraph, single-select dropdown, multi-select dropdown, external lookup, typeahead, date, checkbox group, and radio buttons.

### Only allow project owner to select "Rush" SLA

In this example, a single-select dropdown field has choices for the SLA of Standard – 14 days, Priority – 7 days, and Rush – 2 days.

Validation expression:

```
IF({ownerID}!=$$USER&&{DE:DV - Dropdown - Control Dates}="2",CONCAT("Only ",{owner}.{name}," may select X Rush"))
```

When anyone who is not the project owner (including the system administrator) attempts to select **X Rush**, an error is displayed:

![Only the project owner Claire Stevens may select X Rush](assets/sla-xrush.png)

