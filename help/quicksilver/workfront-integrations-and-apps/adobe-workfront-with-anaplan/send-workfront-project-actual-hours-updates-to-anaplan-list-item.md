---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Send [!DNL Adobe Workfront] actual hours updates to an an Anaplan list item
description: This integration scenario shares actual hours details captured on an [!DNL Adobe Workfront] project with an Anaplan budget list item. Sharing this information allows you to take better advantage of the spend optimization and financial analysis that Anaplan provides.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 450b9a87-79c6-4d10-a9ea-29766b4f5962
---
# Send [!DNL Adobe Workfront] actual hours updates to an an Anaplan list item

This integration scenario shares actual hours details captured on an [!DNL Adobe Workfront] project with an Anaplan budget list item. Sharing this information allows you to take better advantage of the spend optimization and financial analysis that Anaplan provides.

This scenario template delivers a list of hours summarized by project, day, and role recorded on active projects over then last 3 months.

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
   <td>Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

&#42;&#42;For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Triggering Event

This scenario is scheduled to execute every 15 minutes.

## Expected Workfront Configuration

You must have the following in [!DNL Workfront] to use this scenario:

* A user profile in [!DNL Workfront] named **Anaplan Integration**, that has system administrator rights.

   For information on creating a user in [!DNL Workfront], see [Add users](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Expected Anaplan Configuration

You must have the following in Anaplan to use this scenario:

* A user profile in Anaplan named [!DNL Workfront&#x200B;**] Integration**, that has system administrator rights.
* The Anaplan Model that you want to use for this scenario.
* The List within the Anaplan Model that you want to use for this scenario.
* A file in Anaplan named **Anaplan Actual Hours Import** that contains the following columns, in this order:

   1. Workfront Project GUID

   2. Hours

   3. Hours Estimated Cost

   4. Entry Date

   5. Role Name

   6. Campaign Name

   7. Anaplan List Item ID

   To prepare the Anaplan Actual Expense Report file:

   1. Copy and paste the following into a text editor or Excel
   1. Save the file in a CSV format
   1. Upload the file into Anaplan.

      For instructions, see the Anaplan documentation about importing data into modules from a file.

   1. Make note of the name you gave to the file; it will be used during the deployment of the [!UICONTROL Fusion] scenario template.

   Example CSV contents

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[!DNL Workfront] Project GUID,Hours,Hours Estimated Cost,Entry Date,Role Name,Workfront Project Name,Item ID<br>6218062a000d0442903fcfa21e11f556,2,0,3/7/22,Designer,New Project 6,202000001030</code></pre>

* A **Project Actual Hours Import** process prepared to execute the import of data delivered in a file upload.

For instructions on any of these actions, see the Anaplan documentation.

## Deploying to Workfront Fusion

Complete the following steps to deploy this integration scenario to your Fusion account. This should only be done after completing the required [!DNL Workfront] and Anaplan configuration.

1. Navigate to the Templates menu in [!DNL Workfront Fusion] and click the **Send Workfront actual hours updates to Anaplan list item** scenario template.
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
      <td>The ID of a model from your [!DNL Anaplan] account and the selected workspace.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Campaign List Name</td> 
      <td>The name of the list from your Anaplan account and the selected workspace &amp; model.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">File Name: Actual Hours Import</td> 
      <td> <p>Tthe name of the file that will receive [!UICONTROL project] actual hours data.</p> <p> (Example: [!DNL WorkfrontUpdateLinkedProjects_HoursRoles].csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Process Name: Actual Hours Import</td> 
      <td> <p>The name of the process that will execute the import of project hours data.</p> <p>(Example: WF Int - Load Project Hours by Role)</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Workfront Subdomain</td> 
      <td>The subdomain of your [!DNL Workfront] account. This is used to create a link back to your [!DNL Workfront] project in a note that may be generated.</td> 
     </tr> 
    </tbody> 
   </table>

   Details on how to set up the files and processes are provided in the Anaplan setup documentation.

1. Select or add an Anaplan connection profile.
1. Update all remaining Anaplan modules with an Anaplan connection, when prompted.
1. Select or add a [!DNL Workfront] connection profile.
1. Update all remaining [!DNL Workfront] modules with a [!DNL Workfront] connection, when prompted.

## Other Recommended Scenario Templates

This scenario template is complimented by the following spend optimization scenario templates that may also be deployed:

* [Send [!DNL Adobe Workfront] project updates to an Anaplan list item](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [Send [!DNL Adobe Workfront] expenses to an Anaplan list item](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

Additional scenarios for linking budget requests:

* [Create an Anaplan list item from an [!DNL Adobe Workfront] budget request](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [Apply an Anaplan budget allocation to an [!DNL Adobe Workfront] project](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Additional scenarios for linking campaign requests:

* [Create an Anaplan list item from an [!DNL Adobe Workfront] campaign request](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [Apply an Anaplan budget allocation to an [!DNL Adobe Workfront] campaign request or campaign project](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
