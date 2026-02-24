---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: "Calculated custom field example: display the manager of an issue's creator on the issue custom form"
description: Using a calculated custom field, you can display the name of the manager of an issue's creator on a custom form attached to the issue. Using the same statement, you can build similar calculated fields for projects, issues, and other objects.
author: Jenny
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
---
# Calculated custom field example: display the manager of an issue's creator on the issue custom form

Using a calculated custom field, you can display the name of the manager of an issue's creator on a custom form attached to the issue. Using the same statement, you can build similar calculated fields for projects, issues, and other objects.

<!--outdated link: 
>[!TIP]
>
>For information about additional custom text mode examples from other customers, follow the [Text Mode Reporting](https://one.workfront.com/s/topic/0TO0z000000cdHmGAI/text-mode-reporting?tabset-21363=3) topic on our Community site.
-->

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront package</p> </td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license</p> </td> 
   <td>
      <p>Standard</p>
      <p>Plan</p></td>
  </tr> 
  <tr> 
   <td><p>Access level configurations</p></td> 
   <td> <p>Administrative access to Custom forms</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Object permissions</p> </td> 
   <td> <p>Contribute access to the object where the form is attached with access to Edit the Custom Form</p></td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Display the manager of an issue's creator on the issue custom form

The following steps show how you can create a calculated field for an issue custom form where you can capture the name of the manager of the user who created the issue. The process is identical when you want to capture the name of the manager of a user who created a task, a project, a portfolio, for example.

1. Create an issue custom form and add a calculated field to it.

   For information about creating a custom form and adding calculated fields to it, see the following articles:

   * [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)
   * [Add calculated fields to a form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md)

1. Copy and paste the following text mode code into the **Calculation** field of the custom form:

   ```
   {owner}.{manager}.{name}
   ```

   >[!TIP]
   >
   >Custom field calculations are case sensitive.

1. Click **Done**, then **Save + Close**.

   The manager of the user who created the issue displays in the calculated field when the form that contains the field is attached to an issue.
