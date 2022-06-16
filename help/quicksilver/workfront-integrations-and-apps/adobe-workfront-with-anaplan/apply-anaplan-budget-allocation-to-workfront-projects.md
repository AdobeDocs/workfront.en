---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Apply an Anaplan budget allocation to an Adobe Workfront project
description: This integration scenario syncs any budget allocations that have been made in Anaplan back to Workfront. The scenario pulls all linked campaign budget items, then passes the budged value to the linked Workfront project if the budget value has been changed.
feature: "Workfront Integrations and Apps, Workfront Fusion"
---

# Apply an Anaplan budget allocation to an Adobe Workfront project

This integration scenario syncs any budget allocations that have been made in Anaplan back to Workfront. The scenario pulls all linked campaign budget items, then passes the budged value to the linked Workfront project if the budget value has been changed.

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

## Expected Anaplan Configuration

You must have the following in Anaplan to use this scenario:

* A user profile in Anaplan named Workfront** Integration**, that has system administrator rights.
* The Anaplan Model that you want to use for this scenario.
* The List within the Anaplan Model that captures campaign budgets.

  The list's module must support receiving the following attributes:

   * Workfront Project GUID
   * Campaign Name
   * Requested Labor Funds
   * Estimated Revenue
   * Brand

  This list and module must store additional details that are necessary for the normal functionality of Anaplan, including the ability to set a budget and communicate that the budget list item is ready to be synced back to Workfront.

* A view in Anaplan named **Campaigns.Update Campaigns in Adobe Workfront**.

  This view must contain the following columns, in this order:

  1. Item Name

  2. Workfront Project GUID

  3. Campaign Name

  4. Budget

  5. Estimated Revenue

  6. Brand

  The view should be filtered to display items that have a Workfront Project GUID and some indicator that budget allocations should be transmitted to Workfront.

For instructions on any of these actions, see the Anaplan documentation.

## Deploying to Workfront Fusion

Complete the following steps to deploy this integration scenario to your Fusion account. This should only be done after completing the required Workfront and Anaplan configuration.

1. Navigate to the Templates menu in Workfront Fusion and click the **Apply Anaplan budget allocations to Workfront projects** scenario template.
1. Replace the variable values for the following Anaplan variables:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <thead> 
     <tr> 
      <th>Variable name</th> 
      <th>Replace value with</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">Anaplan Workspace ID</td> 
      <td>The ID of a workspace from your Anaplan account.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anaplan Model ID </td> 
      <td>The ID of a model from your Anaplan account and the selected workspace.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anaplan Module Name</td> 
      <td>The name of the module that describes the campaign attributes in the selected Anaplan List.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Campaign List Name</td> 
      <td>The name of the list from your Anaplan account and the selected workspace &amp; model.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anaplan View Name</td> 
      <td> <p>The name of the view that contains ready-to-transmit campaign budgets to Workfront.</p> <p>(Example: Campaigns.Load Campaigns to Adobe Workfront) </p> </td> 
     </tr> 
    </tbody> 
   </table>

   Details on how to set up the files and processes are provided in the Anaplan setup documentation.

1. Select or add an Anaplan connection profile.
1. Update all remaining Anaplan modules with an Anaplan connection, when prompted.
1. On the **Convert CSV to JSON Object module**, add a new data structure to map the CSV columns to a usable JSON object.

   <!-- [Copy](javascript:void(0);) --> 
   <pre><code>[<br>&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"Anaplan Name":"text",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"Workfront Project GUID":"text",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"Campaign Name":"text",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"Budget": 100.01,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"Estimated Revenue": 100.01,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"Brand":"text"<br>&nbsp;&nbsp;&nbsp;&nbsp;}<br>]<br></code></pre>

1. When prompted, select this data structure for other modules in this scenario deployment.
1. On the **Check Linked Project** module, select or add a Workfront connection profile.
1. Update all remaining Workfront modules with a Workfront connection, when prompted.

## Other Recommended Scenario Templates

To complete the workflow represented by this template, you must also deploy the following additional template:

* [Create an Anaplan list item from an Adobe Workfront budget request](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)

Additional scenarios for spend optimization include:

* [Send Adobe Workfront project updates to an Anaplan list item](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

  [Send Adobe Workfront actual hours updates to an an Anaplan list item](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md) 

* [Send Adobe Workfront expenses to an Anaplan list item](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

