---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Send [!DNL Adobe Workfront] expenses to an Anaplan list item
description: This integration scenario shares expense-related details from an [!DNL Adobe Workfront] project with an Anaplan budget list item. Sharing this information allows you to take better advantage of the spend optimization and financial analysis that Anaplan provides.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: f9198017-9bbb-4776-86aa-3f78705dbb22
---
# Send [!DNL Adobe Workfront] expenses to an Anaplan list item

This integration scenario shares expense-related details from an [!DNL Adobe Workfront] project with an Anaplan budget list item. Sharing this information allows you to take better advantage of the spend optimization and financial analysis that Anaplan provides.

## Triggering Event

This scenario is scheduled to execute every 15 minutes.

## Expected Workfront Configuration

You must have the following in [!DNL Workfront] to use this scenario:

* A user profile in [!DNL Workfront] named **Anaplan Integration**, that has system administrator rights.

   For information on creating a user in [!DNL Workfront], see [Add users](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* A **Campaign Brief** custom form attached to the project object to store custom data values you elect to send to Anaplan.

   The form must contain the following fields:

   | Field Name | Field Type |
   |---|---|
   | Last Transmission Date | Date |
   | Integration Notes | Paragraph Text Field |

   For information on creating custom forms, see [Create or edit a custom form](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

## Expected Anaplan Configuration

You must have the following in Anaplan to use this scenario:

* A user profile in Anaplan named [!DNL Workfront&#x200B;**] Integration**, that has system administrator rights.
* The Anaplan Model that you want to use for this scenario.
* The List within the Anaplan Model that you want capture campaign budgets.
* An **Anaplan Actual Expense Import** file that contains the following columns, in this order:

   1. Workfront Expense GUID

   2. Workfront Project GUID

   3. Actual Amount

   4. Description

   5. Expense Type

   6. Effective Date

   7. Campaign Name

   8. Anaplan List Item ID

   To prepare the Anaplan Actual Expense Import file:

   1. Copy and paste the following into a text editor or Excel.
   1. Save the file in a CSV format.
   1. Upload the file into Anaplan.

      For instructions, see the Anaplan documentation about importing data into modules from a file.

   1. Make note of the name you gave to the file; it will be used during the deployment of the [!UICONTROL Fusion] scenario template.

   Example CSV contents

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>"Workfront Expense GUID","Workfront Project GUID","Actual Amount","Description","Expense Type","Effective Date","Campaign Name","Anaplan List Item ID"<br>"622aead400423eb2e4479fece9a72987","6218062a000d0442903fcfa21e11f556","2345","Expense 1","","2022-03-09","New Project 6","202000001030"</code></pre>

* An **Anaplan Planned Expense Import** file that contains the following columns, in this order:

   1. Workfront Expense GUID

   2. Workfront Project GUID

   3. Actual Amount

   4. Description

   5. Expense Type

   6. Effective Date

   7. Campaign Name

   8. Anaplan List Item ID

   To prepare the Anaplan Planned Expense Import file:

   1. Copy and paste the following into a text editor or Excel
   1. Save the file in a CSV format
   1. Upload the file into Anaplan.

      For instructions, see the Anaplan documentation about importing data into modules from a file.

   1. Make note of the name you gave to the file; it will be used during the deployment of the [!UICONTROL Fusion] scenario template.

   Example CSV contents

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>"Workfront Expense GUID","Workfront Project GUID","Planned Amount","Description","Expense Type","Planned Date","Campaign Name","Anaplan List Item ID"<br>"622aead400423eb2e4479fece9a72987","6218062a000d0442903fcfa21e11f556","1234","Expense 1","Entertainment","2022-03-08","New Project 6","202000001030"</code></pre>
   &nbsp;

* A **Project Update Import** process prepared to execute the import of data delivered in a file upload.

>[!NOTE]
>
>There are separate import files for planned and actual expenses so that they can be reported independently across their planned and effective dates respectively.

For instructions on any of these actions, see the Anaplan documentation.

## Deploying to Fusion

Complete the following steps to deploy this integration scenario to your Fusion account. This should only be done after completing the required [!DNL Workfront] and Anaplan configuration.

1. Navigate to the Templates menu in [!DNL Workfront Fusion] and click the **Send Workfront expenses updates to Anaplan list item** scenario template.
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
      <td>The ID of the workspace from your Anaplan account that you want to use for this scenario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Anaplan Model ID </td> 
      <td>The ID of the model from your [!DNL Anaplan] account and the selected workspace that you want to use for this scenario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Campaign List Name</td> 
      <td>The name of the list from your [!DNL Anaplan] account and the selected workspace and model that you want to use for this scenario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">File Name: Actual Expense Import</td> 
      <td> <p>The name of the file that will receive project actual expense data.</p> <p> (Example: WorkfrontUpdateLinkedProjects_ActExpenses.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">File Name: Planned Expense Import</td> 
      <td> <p>The name of the file that will receive project planned expense data.</p> <p> (Example: WorkfrontUpdateLinkedProjects_PlannedExpenses.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Process Name: Project Update Import</td> 
      <td> <p>The name of the process that will execute the import of project expense data.</p> <p>(Example: WF Int - Load Project Expenses)</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Details on how to set up the files and processes are provided in the Anaplan setup documentation.

1. Select or add an Anaplan connection profile.
1. Update all remaining Anaplan modules with an Anaplan connection, when prompted.
1. Select or add a [!DNL Workfront] connection profile.
1. Update all remaining [!DNL Workfront] modules with a [!DNL Workfront] connection, when prompted.
1. On the **[!UICONTROL Build Actual Expense CSV]** module, add a new data structure to map the project attributes to CSV columns.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Workfront Expense GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Actual Amount": 100.01,<br>        "Description":"text",<br>        "Expense Type":"text",<br>        "Effective Date":"text",<br>        "Campaign Name":"text",<br>        "Anaplan List Item ID": 10000001<br>    }<br>]<br></code></pre>

1. On the **[!UICONTROL Build Planned Expense CSV]** module, add a new data structure to map the project attributes to CSV columns.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Workfront Expense GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Planned Amount": 100.01,<br>        "Description":"text",<br>        "Expense Type":"text",<br>        "Planned Date":"text",<br>        "Campaign Name":"text",<br>        "Anaplan List Item ID": 10000001<br>    }<br>]<br></code></pre>

## Other Recommended Scenario Templates

This scenario template is complimented by the following spend optimization scenario templates that may also be deployed:

* [Send [!DNL Adobe Workfront] project updates to an Anaplan list item](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [Send [!DNL Adobe Workfront] actual hours updates to an an Anaplan list item](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

Additional scenarios for linking budget requests:

* [Create an Anaplan list item from an [!DNL Adobe Workfront] budget request](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [Apply an Anaplan budget allocation to an [!DNL Adobe Workfront] project](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Additional scenarios for linking campaign requests:

* [Create an Anaplan list item from an [!DNL Adobe Workfront] campaign request](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [Apply an Anaplan budget allocation to an [!DNL Adobe Workfront] campaign request or campaign project](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
