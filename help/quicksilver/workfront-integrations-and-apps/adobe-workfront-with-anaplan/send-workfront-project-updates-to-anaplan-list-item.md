---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Send Adobe Workfront project updates to an Anaplan list item
description: This integration scenario shares progress, status, and key schedule details from an Adobe Workfront project with an Anaplan budget list item. Sharing this information allows you to take better advantage of the spend optimization and financial analysis that Anaplan provides.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 97e9dac6-f5b5-4d6e-b58b-93acd19048ee
---
# Send Adobe Workfront project updates to an Anaplan list item

This integration scenario shares progress, status, and key schedule details from an Adobe Workfront project with an Anaplan budget list item. Sharing this information allows you to take better advantage of the spend optimization and financial analysis that Anaplan provides.

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

* A **Campaign Brief** custom form attached to the project object to store custom data values you elect to send to Anaplan.

  The following fields represent examples of fields that may be included on the custom form to aid in data mapping to Anaplan, but they are not required for this integration scenario:

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

<!--
<note type="note">  
<p>The above configuration is available through the Marketing Financial Management Configuration blueprint:</p>
<p>https://MYDOMAIN.my.workfront.com/blueprints/7ebe85c4-05a1-4efe-a018-50ee55f5654c/details </p>
<p><span style="color: #ff0000;">This note is currently not marked for publication.</span> </p>
</note>
-->

## Expected Anaplan Configuration

You must have the following in Anaplan to use this scenario:

* A user profile in Anaplan named Workfront** Integration**, that has system administrator rights.
* The Anaplan Model that you want to use for this scenario.
* The List within the Anaplan Model that you want to use for this scenario.
* A **Project Update Import** file that contains the following columns, in this order:

1. itemID

  2. Workfront Project GUID

  3. Campaign Name

  4. Percent Complete

  5. Planned Start Date

  6. Planned Completion Date

  7. Planned Hours

  8. Planned Cost

  9. Planned Expense Cost

  10. Actual Labor Cost

  11. Planned Labor Cost

  12. Status

  To prepare the Anaplan Planned Expense Import file:

   1. Copy and paste the following into a text editor or Excel
   1. Save the file in a CSV format
   1. Upload the file into Anaplan.

      For instructions, see the Anaplan documentation about importing data into modules from a file.
   
   1. Make note of the name you gave to the file; it will be used during the deployment of the Fusion scenario template.

  Example CSV contents

  <!-- [Copy](javascript:void(0);) --> 
  <pre><code>"itemID","Workfront Project GUID","Campaign Name","Percent Complete","Planned Start Date","Planned Completion Date","Planned Hours","Planned Cost","Planned Expense Cost","Actual Labor Cost","Planned Labor Cost","Status","Campaign Overview","Key Message","In Market Start Date","In Market End Date","Target Audience"<br>"202000001019","6182bc1f0025e184b2c00d9205e22c49","Launch Be U APAC Styles Catalog","0","2022-03-31","2022-05-31","88.25","0","0","0","0","Planning","","","","",""</code></pre>Optional columns may include:

1. Campaign Overview

  2. Key Message

  3. In Market Start Date

  4. In Market End Date

  5. Target Audience

  Also include any other fields you wish to set in the mapping. 

* A **Project Update Import** process prepared to execute the import of data delivered in a file upload.

For instructions on any of these actions, see the Anaplan documentation.

## Deploying to Workfront Fusion

Complete the following steps to deploy this integration scenario to your Fusion account. This should only be done after completing the required Workfront and Anaplan configuration.

1. Navigate to the Templates menu in Workfront Fusion and click the **Send Workfront project updates to Anaplan list item** scenario template.
1. Replace the variable values for the following Anaplan variables:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
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
      <td role="rowheader">Campaign List Name</td> 
      <td>The name of the list from your Anaplan account and the selected workspace &amp; model.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">File Name: Project Update Import</td> 
      <td>The name of the file that will receive project update data.<p>(Example: WorkfrontUpdateLinkedProject.csv)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Process Name: Project Update Import</td> 
      <td> <p>The name of the process that will execute the import of project data.</p> <p>(Example: WF Int - Update Campaign Details)</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Workfront Subdomain</td> 
      <td>The subdomain of your Workfront account. This is used to create a link back to your Workfront project in a note that may be generated.</td> 
     </tr> 
    </tbody> 
   </table>

   Details on how to set up the files and processes are provided in the Anaplan setup documentation.

1. Select or add an Anaplan connection profile.
1. Update all remaining Anaplan modules with an Anaplan connection, when prompted.
1. Select or add a Workfront connection profile.

   The filter is configured to pull in all incomplete linked project and those projects that were completed in the last 29 minutes. If you change the frequency of the Fusion scenario you will want to update this value once the scenario template has been deployed.

1. On the **Build Projects Update CSV** module, add a new data structure to map the project attributes to CSV columns.

   <!-- [Copy](javascript:void(0);) --> 
   <pre><code>[<br>&nbsp;&nbsp;&nbsp;&nbsp;{<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"itemID": 1000001,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"Workfront Project GUID":"text",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"Campaign Name":"text",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"Percent Complete": 10.01,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"Planned Start Date":"2022-02-22",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"Planned Completion Date":"2022-02-22",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"Planned Hours": 12.5,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"Planned Cost": 123.45,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"Planned Expense Cost": 123.45,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"Planned Labor Cost": 123.45,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"Status": "CUR",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"Campaign Overview":"text",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"Key Message":"text",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"In Market Start Date":"2022-02-22",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"In Market End Date":"2022-02-22",<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;"Target Audience":"text"<br>&nbsp;&nbsp;&nbsp;&nbsp;}<br>]<br></code></pre>

1. Update all remaining Workfront modules with a Workfront connection, when prompted.

## Other Recommended Scenario Templates

This scenario template is complimented by the following spend optimization scenario templates that may also be deployed:

* [Send Adobe Workfront actual hours updates to an an Anaplan list item](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md) 
* [Send Adobe Workfront expenses to an Anaplan list item](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

Additional scenarios for linking budget requests:

* [Create an Anaplan list item from an Adobe Workfront budget request](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md) 
* [Apply an Anaplan budget allocation to an Adobe Workfront project](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Additional scenarios for linking campaign requests:

* [Create an Anaplan list item from an Adobe Workfront campaign request](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md) 
* [Apply an Anaplan budget allocation to an Adobe Workfront campaign request or campaign project](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
