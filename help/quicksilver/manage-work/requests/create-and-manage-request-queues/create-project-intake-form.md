---
product-area: requests
navigation-topic: create-and-manage-request-queues
title: Create Project Intake Forms
description: You can use project intake forms to simplify the process of creating projects in Workfront
author: Becky
feature: Work Management, Requests
role: User, Admin
---
# Create project intake forms

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Project intake forms are a type of request form that allows users to request projects. The projects are created from the form, without needing to create a project from a submitted issue.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

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
   <td> 
   <p>New license: Standard </p>
   Or
   <p>Current license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator to create project intake forms. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Other products</td> 
   <td> <p>Your organization must have purchased Workfront Planning to use Planning features such as automations.</p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Capabilites and limitations to Project Intake Forms

### Capabilities

Project intake forms include the following capabilities:

#### Workfront Planning automations

Workfront project intake forms support Workfront Planning Automations, to configure the created project-specific properties.

   For more information on Planning automations, see [Configure Adobe Workfront Planning automations](/help/quicksilver/planning/records/configure-automations-to-create-records.md).

### Approval configuration

Project intake forms include the ability to configure approvers for submitted requests.

### Limitations

#### Supported field types

Project Intake Forms can include fields from any custom form with the Project object type. 

The following field types are currently not supported in Project Intake Forms:

* Section
* Formula
* Rollup
* Single line rollup
* Planning connection
* Native field references  that are referred to Project native fields, which are read-only (for example, `workRequiredExpression`)

#### Requesting experience

Project intake forms can be used only with the new requesting experience. 

For information on the new requesting experience, see [Create and submit requests](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

#### Sharing

Project intake forms do not support public sharing. Sharing options include:

* **Anyone**: Anyone in the system can use the form to submit a project request.
* **Specified users**: You can select which specific users have access to the project request form.

## Create a project intake form

{{step1-to-requests}}

1. Enable the **Switch to a new experience** setting, in the upper-right corner of he screen. 
1. Click **Request forms** in the upper-right corner of the screen.

   >[!NOTE]
   >
   >Because only Workfront administrators can create intake forms, the Request forms button is only visible to administrators.

   A list of currently available request forms appears. This includes request forms from Workfront Planning.

1. Click **New request form** in the upper-right corner of the screen.
1. Enter a name for the request form. By default, the name of the form is **Untitled form**. 
1. Select the object type **Project** near the top of the dropdown list. Currently, this is the only available Workfront project type. Other items in the list belong to Workfront Planning.
1. (Optional) Add a **Description** for the request form. 
1. Click **Create**. The request form for the selected record type opens in the Form tab. 

   The project intake form builder opens to the Form tab.

   The intake form contains the following information, by default:

   * **Default section**: This is the default section break that Workfront applies to the request form. All record fields display in the **Default section** area. 
   * **Subject** field: The field which will identify the request in Workfront. The configuration and the value of the Subject field are not editable.
   * All the fields associated with projects. 

      The fields contained in the request form will be visible to everyone submitting a project request. 

1. To add fields to the form, click on the field type in the left navigation, then select the field.
1. (Optional) To remove a field, hover over the field on the form that you want to remove, then click the **x** icon to remove it. 
1. (Optional) To remove the **Default section** from the form, do the following:

   1. Remove all fields from the Default Section. 
   1. Click the **Content elements** tab and add a new section, then add a name for the section. 
   1. Add fields to the new section. 
   1. Click the **x** icon to remove the **Default section**. 
1. Click any field, then use the controls in the right panel in the form to define their size, or any of the following information:

   * **Label**: This is the name of the field as it will appear on the request form. This does not change the name of the record field.
   * **Instructions**: Add more information about the field.
   * **Make a required field**: When selected, the field must have a value. Otherwise, the form cannot be submitted. 
   * **Add logic**: Define what conditions must be met in order for the field to display or be hidden.

   >[!TIP]
   >
   >   The field type of each field displays at the top of the right panel, after you select the field on the form. 
   >     

1. (Optional) Click the **Content elements** tab on the left side of the form, and add any of the following elements:

   * **Descriptive text**
   * **Section break** 

   For more information about building a custom form, see [Create a custom form](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md). 

1. Click the **Automations** tab on the left side of the form, then do any of the following:

   * Select a project template
   * Attach any custom forms
   * Set a project owner
   * Add the project to a portfolio or program

   Any selections you make here will be applied to projects created from this intake form.

1. (Optional) Click **Preview** to view how the form will display for other users when they will use it to submit a new record.

1. (Optional) Click the **Configuration** tab, then add at least one user or team< to the **Approvers** field to approve new requests for this intake form. 

   * When you associate an intake form with approvers, any new request must first be approved by all approvers before it generates a project. 
   * You can add one or several approvers to an intake form. 
   * If at least one approver rejects the request, the request is rejected and the project is not created. 
   * All approvers must make a decision before a project is either approved or rejected.
   * If a team is set as an approver, only one decision is required from the team.

      For more information about adding approvals to request forms, see [Add approval to a request form](/help/quicksilver/planning/requests/add-approval-to-request-form.md). 

1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) to the right of the form's name in the header, then click **Edit** to update the name of the form.

1. Click **Publish** to publish the form and obtain a unique link for it. 

   The following things occur:

   * The **Publish** button is removed.
   * The **Unpublish** button is added to the form. Clicking it will prevent the form from being accessible. 
   * A **Share** button is added to the form.
   * The form becomes available in the Requests area of the Main menu in Workfront.

1. Click **Share** to share the form with others. 
1. Click the left-pointing arrow to the left of the form's name in the header to close the form. 

   The **Request forms** table view opens and the the form is added to it.

1. (Optional) Hover over the name of a request form in the table view, then click the **More** menu ![More menu](assets/more-menu.png) to the right of the form name, and click one of he following:

   * **Edit form**: Click this to further edit information on the form.
   * **Unpublish**: Click this to unpublish the form which removes it from the Requests area in Workfront.
   * **Share**: Click this to modify who has access to the form.
   * **Copy link**: Click this to quickly copy the request form's link without opening the form.
   * **Delete**: Click this to delete the form. All requests and records added using the form are not deleted. The form cannot be recovered. 

1. Click the left-pointing arrow to the left of **Request forms** in the header to close the request forms table.  

