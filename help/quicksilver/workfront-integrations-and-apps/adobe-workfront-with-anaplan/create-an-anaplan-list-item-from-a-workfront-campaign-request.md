---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Create an Anaplan list item from an Adobe Workfront campaign request
description: This integration scenario links an Adobe Workfront project with an Anaplan budget list item.
author: Becky
feature: "Workfront Integrations and Apps, Workfront Fusion"
---

# Create an Anaplan list item from an Adobe Workfront campaign request

This integration scenario links an Adobe Workfront project with an Anaplan budget list item.

This scenario watches for new campaign requests added to a request queue. As soon as a campaign request is recorded, a budget line item is added in Anaplan to start the funding process.

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan, Work</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion license**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase Adobe Workfront Fusion as well as Adobe Workfront to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Triggering Event

This scenario is scheduled to execute every 15 minutes.

## Expected Workfront Configuration

You must have the following in Workfront to use this scenario:

* A user profile in Workfront named **Anaplan Integration**, that has system administrator rights.

  For information on creating a user in Workfront, see [Add users](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* A **Campaign Brief** custom form attached to the Request object.

  The following required fields must be included on the custom form to aid in data mapping to Anaplan:

  | Field Name |Field Type |
  |---|---|
  | Total Requested Funds |&nbsp; |
  | Requested Labor Funds |&nbsp; |
  | Requested Expense Funds |&nbsp; |
  | Sent to Anaplan |Checkbox |

  The following optional fields may be present on the form. This scenario maps only the above fields, but any additional fields on the campaign brief may be mapped.

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <thead> 
    <tr> 
     <th>Field Name</th> 
     <th>Field Type</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader">In Market Start Date</td> 
     <td>Date </td> 
    </tr> 
    <tr> 
     <td role="rowheader">In Market End Date</td> 
     <td>Date</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Campaign Overview</td> 
     <td>Paragraph Text Field</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Key Message</td> 
     <td>Paragraph Text Field</td> 
    </tr> 
    <tr> 
     <td role="rowheader">Target Audience</td> 
     <td> <p>Dropdown</p> <p>Include options that fit your processes.</p> </td> 
    </tr> 
   </tbody> 
  </table>

  For information on creating custom forms, see [Create or edit a custom form](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

* A project set up as a request queue to capture new campaign requests. The Campaign Brief form must be attached to these requests.

## Expected Anaplan Configuration

You must have the following in Anaplan to use this scenario:

* A user profile in Anaplan named Workfront** Integration**, that has system administrator rights.
* The Anaplan Model that you want to use for this scenario.
* The List within the Anaplan Model that captures campaign budgets.

  The list's module must support receiving the following attributes:

   * Workfront Request GUID
   * Workfront Project GUID
   * Campaign Name
   * Requested Labor Funds
   * Requested Expense Funds
   * Budget Request Type

  This list and module must store additional details that are necessary for the normal functionality of Anaplan, including the ability to set a budget and communicate that the budget list item is ready to be synced back to Workfront.

For instructions on any of these actions, see the Anaplan documentation.

## Deploying to Workfront Fusion

Complete the following steps to deploy this integration scenario to your Fusion account. This should only be done after completing the required Workfront and Anaplan configuration.

1. Navigate to the Templates menu in Workfront Fusion and click the **Create an Anaplan list item from a Workfront campaign request** scenario template.
1. Replace the variable values for the following Anaplan variables:

   | Variable name |Replace value with |
   |---|---|
   | Anaplan Workspace ID |The ID of a workspace from your Anaplan account. |
   | Anaplan Model ID  |The ID of a model from your Anaplan account and the selected workspace. |
   | Anaplan Module Name |The name of the module that describes the campaign attributes in the selected Anaplan List. |
   | Campaign List Name |The name of the list from your Anaplan account and the selected workspace & model. |

   {style="table-layout:auto"}

   Details on how to set up the files and processes are provided in the Anaplan setup documentation.

1. Select or add an Anaplan connection profile.
1. Update all remaining Anaplan modules with an Anaplan connection, when prompted.
1. Select or add a Workfront connection profile.

   After deploying the template, this is the module you will update to add or remove custom field references from the value of the fields property if you want to alter the default mapped fields to Anaplan.

1. Update all remaining Workfront modules with a Workfront connection, when prompted.

## Other Recommended Scenario Templates

To complete the workflow represented by this template, you must also deploy the following additional template:

* [Apply an Anaplan budget allocation to an Adobe Workfront campaign request or campaign project](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)

Additional scenarios for spend optimization include:

* [Send Adobe Workfront project updates to an Anaplan list item](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

  [Send Adobe Workfront actual hours updates to an an Anaplan list item](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md) 

* [Send Adobe Workfront expenses to an Anaplan list item](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

