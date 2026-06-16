---
title: Restrict Access to Financial Data in Custom Fields
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: When you create a custom field, you can define optional settings to restrict access to financial data.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 3380cce6-8372-43c0-8520-473442ea0eb4
---
# Restrict access to financial data in custom fields

When you create a custom field, you can define optional settings to restrict access to financial data. This way, users who have certain permissions set in their access levels can see the data, and they are prevented from seeing financial data that they should not have access to.

For information about creating a custom field, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

For information about access levels, see [Access levels overview](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md). For information about sharing and permissions, see [Overview of sharing permissions on objects](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td>Any</td> 
  </tr>  
  <tr> 
   <td>Adobe Workfront license</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>Administrative access to custom forms</td> 
  </tr>  
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Restrict access to financial data on a custom field

1. Create a new custom form or open an existing form.

   For information, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Add a custom field to the form or select an existing field.

   These field types can be restricted based on financial data access:

   * Single line text
   * Paragraph
   * Single-select dropdown
   * Multi-select dropdown
   * Checkbox group
   * Radio buttons
   * External lookup
   * Multi-select external lookup
   * Calculated

1. In the **Format** field, select **Currency**.

   >[!NOTE]
   >
   >For calculated fields, any format is allowed. All other field types must use the **Currency** format, or the **Finance permission type** field will be unavailable.

1. (Optional) For calculated fields only, turn on the **Automatic permission** option to allow the finance permissions to automatically come from the fields in the formula.

1. Select an option for the **Finance permission type**.

   Users must have this finance permission type before they can view or edit this custom field on the form.

   * **No permissions required:** All users can see this field
   * **General:** Users must have permissions to edit or view General Finance
   * **Bill:** Users must have permissions to edit or view billing rates
   * **Cost:** Users must have permissions to edit or view cost rates

   For calculated fields:
   
   * The **Finance permission type** field is not available for manual setting of permissions if the **Automatic permission** field is turned on.
   * The fields used in the formula determine whether the permission field is active. If the permission field is blank (and automatic permissions are not turned on), the fields in the formula do not support the finance permissions.
   * Access is required for all fields in the formula. For example, if two fields are used in a calculated field, and one of them has billing permission applied and the second has cost permission applied, then the user must have permissions to view both billing and cost rates to see the calculated value.

1. To save your changes, click **Apply** and continue building your form.

   Or
   
   Click **Save and Close**.

## Example

Two projects are shared with a user:

* The user has permissions to edit all finance options on the first project
* The user has permissions to view billing rates and general finance on the second project

When the user edits the first project, all financial fields on the custom form are editable. When the user edits the second project, the fields set to **Bill** or **General** are view-only, and the fields set to **Cost** are not visible.

When the user views the projects in a list or report:

* Finance fields are viewable or editable according to the permissions and the report settings
* Finance fields are blank if the user does not have permissions to view them

Exporting project details shows the same same financial field values (or blank fields) as in the list.

When bulk editing both projects, the billing and general finance fields show as read-only, and the cost fields show N/A.
