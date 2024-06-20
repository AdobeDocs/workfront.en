---
product-area: projects;user-management
keywords: attach,apply
navigation-topic: work-with-custom-forms
title: Add a custom form to an object
description: You can add an existing custom form to any of the objects listed below. A custom form contains custom fields where you can store information about the object.
author: Alina
feature: Get Started with Workfront
exl-id: c06666a7-ab78-4311-8fcb-1d1a68034133
---
# Add a custom form to an object

<!--Audited: 12/2023-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

You can add an existing custom form to any of the objects listed below. A custom form contains custom fields where you can store information about the object.

* Projects (including business cases)
* Tasks
* Issues
* Companies
* Portfolios
* Programs
* Documents
* Users
* Iterations
* Expenses
* Billing records

You can add a custom form only to the types of objects for which the form was created.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the actions described in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
<tr> 
  <td role="rowheader">Adobe Workfront license</td> 
  <td> <p>New: Contributor or higher </p>
 <p>or</p> 
<p>Current: Request or higher </p> 
</td> 
 </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to the objects for which you manage custom forms</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the object for which you want to attach a custom form.</p> <p>View or higher permissions to the custom form, with permission to <b>Attach to Custom Data</b> objects (projects, tasks, and issues). For more information, see <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Share a custom form</a>.</p> <p>Important: If you do not have a Plan license with administrative access to&nbsp;Custom&nbsp;Forms, you must have specific permissions to at least view the custom form, as described in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Share a custom form</a>. These permissions must be granted to you even if the form is visible system-wide. </p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Prerequisites

Your Workfront administrator or a user with a Plan license and administrative access to custom forms must create custom forms in your environment before you can add them to objects. For more information, see [Create or edit a custom form](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Add a custom form to an object

You can add a custom form to an object in two ways:

* [Add a custom form to an object by editing the object](#add-a-custom-form-to-an-object-by-editing-the-object) 
* [Add a custom form to an object from the Details area](#add-a-custom-form-to-an-object-from-the-details-area)

### Add a custom form to an object by editing the object {#add-a-custom-form-to-an-object-by-editing-the-object}

1. Go to the object where you want to add the custom form.
1. Click the **More** menu ![](assets/more-icon.png), then click **Edit** ![](assets/edit-icon.png).  
1. Click **Custom Forms** > **Add Forms**, then select up to 10 forms from the drop-down menu.

1. (Optional) Update the information in the editable fields on the custom form.

   You must update all required fields on the forms you add. 

1. Click **Save**.

### Add a custom form to an object from the Details area {#add-a-custom-form-to-an-object-from-the-details-area}

1. Go to the object where you want to add the custom form.
1. Click the **`<Object type>` Details** section in the left panel. For example, click **Project Details** to add custom forms to a project or **Issue Details** to add custom forms to an issue. 
1. Click the **Add custom form** field in the upper-right corner, then select up to 10 custom forms from the list that displays.

   If the form contains any required fields (marked with a red asterisk), you don't have to complete them at this time.

   The selected forms are automatically attached to the object. 

1. (Optional) Update the information in the custom fields of the form, then click **Save Changes**.

## Multiple custom forms on an object

You can add up to 10 custom forms on a given object, allowing you to make fields available to some users and not to others, or allowing you to better meet the form requirements of multiple projects.

**Example:** If an existing project has a custom form already, and more custom fields are needed for this project, which exist on another custom form, you can add a second form to the project with the additional fields, rather than add the fields to the existing custom form.

## Add a custom form to multiple objects in bulk

You can add custom forms to multiple objects by selecting them in a list.

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
>Adding custom forms to objects is identical for all objects except for projects. 
>
>For information about adding custom forms to projects in bulk, see the article [Edit projects](../../manage-work/projects/manage-projects/edit-projects.md).


1. Navigate to a list of objects.
1. Select multiple objects in the list.  

1. Click the **More** menu ![](assets/more-icon.png), then click the **Edit** icon  ![](assets/edit-icon.png).

   Or

   Click the **Edit** icon ![](assets/edit-icon.png) at the top of the list.
1. Click **Custom Forms** in the left panel.
1. in the **Make a selection** drop-down menu, select the form you want to associate with all the selected objects.

   >[!NOTE]
   >
   >If you cannot find the form in the drop-down menu, this means that at least one of the objects has the form already associated with it. Determine which object that is, and eliminate it from your selection, before you can add the form to the remaining objects.
   

1. Click **Save Changes**.

   If the form contains any required fields (marked with a red asterisk), you don't have to complete them at this time.
