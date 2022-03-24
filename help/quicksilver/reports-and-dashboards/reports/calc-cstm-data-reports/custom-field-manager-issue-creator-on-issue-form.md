---
filename: custom-field-manager-issue-creator-on-issue-form
content-type: reference
product-area: reporting
navigation-topic: calculate-custom-data-reports
title: Calculated custom field example: display the manager of an issue's creator on the issue custom form
description: Using a calculated custom field, you can display the name of the manager of an issue's creator on a custom form attached to the issue. Using the same statement, you can build similar calculated fields for projects, issues, and other objects.
---

# Calculated custom field example: display the manager of an issue's creator on the issue custom form

Using a calculated custom field, you can display the name of the manager of an issue's creator on a custom form attached to the issue. Using the same statement, you can build similar calculated fields for projects, issues, and other objects.

>[!TIP]
>
>For information about additional custom text mode examples from other customers, follow the [Text Mode Reporting](https://one.workfront.com/s/topic/0TO0z000000cdHmGAI/text-mode-reporting?tabset-21363=3) topic on our Community site.

## Access requirements

You must have the following access to perform the steps in this article:

<table cellspacing="15"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Access level configurations*</strong> </td> 
   <td> <p>Administrative access to Custom forms<br>For information about granting administrative access from the access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Object permissions</strong> </p> </td> 
   <td> <p>Contribute access to the object where the form is attached with access to Edit the Custom Form</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects in Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Display the manager of an issue's creator on the issue custom form

The following steps show how you can create a calculated field for an issue custom form where you can capture the name of the manager of the user who created the issue.&nbsp;The process is identical when you want to capture the name of the manager of a user who created a task, a project, a portfolio, for example.

1. Create an issue custom form and add a calculated field to it.

   For information about creating a custom form and adding calculated fields to it, see the following articles:

   * [Create or edit a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md) 
   * [Add calculated data to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)

1. Copy the following text mode code and paste it in the **Calculation** field of the custom form:

   ```
   Owner.Manager.Name
   ```

   >[!TIP]
   >
   >Custom field calculations are case sensitive.

1. Click **Done**, then **Save + Close**.

   The manager of the user who created the issue displays in the calculated field when the form that contains the field is attached to an issue.

