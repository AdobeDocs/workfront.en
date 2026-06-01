---
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: "Calculated custom field example: display the manager of an issue's creator on the issue custom form"
description: Using a calculated custom field, you can display the name of the manager of an issue's creator on a custom form attached to the issue. Using the same statement, you can build similar calculated fields for projects, issues, and other objects.
author: Courtney
feature: Reports and Dashboards
exl-id: f501ce1a-7a80-458b-9b30-2292426c9262
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/97--IY38NM0xV5PLImVpO04wx2ou-Le-2x-07Yl6NQs
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Calculated custom field example: display the manager of an issue's creator on the issue custom form

Using a calculated custom field, you can display the name of the manager of an issue's creator on a custom form attached to the issue. Using the same statement, you can build similar calculated fields for projects, issues, and other objects.

<!--
outdated link: 
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
