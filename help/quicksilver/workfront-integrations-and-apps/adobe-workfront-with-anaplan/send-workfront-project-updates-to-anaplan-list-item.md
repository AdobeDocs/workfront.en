---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Send [!DNL Adobe Workfront] project updates to an [!DNL Anaplan] list item
description: This integration scenario shares progress, status, and key schedule details from an [!DNL Adobe Workfront] project with an [!DNL Anaplan] budget list item. Sharing this information allows you to take better advantage of the spend optimization and financial analysis that [!DNL Anaplan] provides.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 97e9dac6-f5b5-4d6e-b58b-93acd19048ee
---
# Send [!DNL Adobe Workfront] project updates to an [!DNL Anaplan] list item

This integration scenario shares progress, status, and key schedule details from an [!DNL Adobe Workfront] project with an [!DNL Anaplan] budget list item. Sharing this information allows you to take better advantage of the spend optimization and financial analysis that [!DNL Anaplan] provides.

>[!IMPORTANT]
>
>"Campaign" in this article refers to the marketing campaign use case that this scenario represents, and is in no way connected to the [!DNL Workfront Fusion] Adobe Campaign connector or to the recently deprecated [!UICONTROL Campaign] object in [!DNL Workfront].

## Access requirements

You must have the following access to use the functionality in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] license**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

&#42;&#42;For information on [!DNL Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Triggering Event

This scenario is scheduled to execute every 15 minutes.

## Expected [!DNL Workfront] Configuration

You must have the following in [!DNL Workfront] to use this scenario:

* A user profile in [!DNL Workfront] named **[!UICONTROL [!DNL Anaplan] Integration]**, that has system administrator rights.

   For information on creating a user in [!DNL Workfront], see [Add users](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* A **[!UICONTROL Campaign Brief]** custom form attached to the project object to store custom data values you elect to send to Anaplan.

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
     <td role="rowheader">[!UICONTROL In Market Start Date]</td> 
     <td>[!UICONTROL Date] </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL In Market End Date]</td> 
     <td>[!UICONTROL Date]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Campaign Overview]</td> 
     <td>[!UICONTROL Paragraph Text Field]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Key Message]</td> 
     <td>[!UICONTROL Paragraph Text Field]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Target Audience]</td> 
     <td> <p>[!UICONTROL Dropdown]</p> <p>Include options that fit your processes.</p> </td> 
    </tr> 
   </tbody> 
  </table>

   For information on creating custom forms, see [Design a form with the form designer](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

<!--
<note type="note">  
<p>The above configuration is available through the Marketing Financial Management Configuration blueprint:</p>
<p>https://MYDOMAIN.my.workfront.com/blueprints/7ebe85c4-05a1-4efe-a018-50ee55f5654c/details </p>
<p><span style="color: #ff0000;">This note is currently not marked for publication.</span> </p>
</note>
-->

## Expected [!DNL Anaplan] Configuration

You must have the following in [!DNL Anaplan] to use this scenario:

* A user profile in [!DNL Anaplan] named **[!UICONTROL [!DNL Workfront] Integration]**, that has system administrator rights.
* The [!DNL Anaplan] Model that you want to use for this scenario.
* The List within the [!DNL Anaplan] Model that you want to use for this scenario.
* A **[!UICONTROL Project Update Import]** file that contains the following columns, in this order:

1. [!UICONTROL itemID]

2. [!UICONTROL [!DNL Workfront] Project GUID]

3. [!UICONTROL Campaign Name]

4. [!UICONTROL Percent Complete]

5. [!UICONTROL Planned Start Date]

6. [!UICONTROL Planned Completion Date]

7. [!UICONTROL Planned Hours]

8. [!UICONTROL Planned Cost]

9. [!UICONTROL Planned Expense Cost]

10. [!UICONTROL Actual Labor Cost]

11. [!UICONTROL Planned Labor Cost]

12. [!UICONTROL Status]

To prepare the [!UICONTROL [!DNL Anaplan] Planned Expense Import] file:

1. Copy and paste the following into a text editor or [!DNL Excel]
1. Save the file in a CSV format
1. Upload the file into Anaplan.

   For instructions, see the [!DNL Anaplan] documentation about importing data into modules from a file.

1. Make note of the name you gave to the file; it will be used during the deployment of the [!UICONTROL Fusion] scenario template.

Example CSV contents

<!-- [Copy](javascript:void(0);) -->
<pre><code>"itemID","Workfront Project GUID","Campaign Name","Percent Complete","Planned Start Date","Planned Completion Date","Planned Hours","Planned Cost","Planned Expense Cost","Actual Labor Cost","Planned Labor Cost","Status","Campaign Overview","Key Message","In Market Start Date","In Market End Date","Target Audience"<br>"202000001019","6182bc1f0025e184b2c00d9205e22c49","Launch Be U APAC Styles Catalog","0","2022-03-31","2022-05-31","88.25","0","0","0","0","Planning","","","","",""</code></pre>Optional columns may include:

1. [!UICONTROL Campaign Overview]

2. [!UICONTROL Key Message]

3. [!UICONTROL In Market Start Date]

4. [!UICONTROL In Market End Date]

5. [!UICONTROL Target Audience]

Also include any other fields you wish to set in the mapping.

* A **[!UICONTROL Project Update Import]** process prepared to execute the import of data delivered in a file upload.

For instructions on any of these actions, see the [!DNL Anaplan] documentation.

## Deploying to [!DNL Workfront Fusion]

Complete the following steps to deploy this integration scenario to your Fusion account. This should only be done after completing the required [!DNL Workfront] and [!DNL Anaplan] configuration.

1. Navigate to the [!UICONTROL Templates] menu in [!DNL Workfront Fusion] and click the **[!UICONTROL Send Workfront project updates to [!DNL Anaplan] list item]** scenario template.
1. Replace the variable values for the following [!DNL Anaplan] variables:

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
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Workspace ID]</td> 
      <td>The ID of a workspace from your [!DNL Anaplan] account.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Model ID] </td> 
      <td>The ID of a model from your [!DNL Anaplan] account and the selected workspace.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Campaign List Name]</td> 
      <td>The name of the list from your [!DNL Anaplan] account and the selected workspace &amp; model.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL File Name: Project Update Import]</td> 
      <td>The name of the file that will receive project update data.<p>(Example: WorkfrontUpdateLinkedProject.csv)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Process Name: Project Update Import]</td> 
      <td> <p>The name of the process that will execute the import of project data.</p> <p>(Example: WF Int - Update Campaign Details)</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Workfront] Subdomain]</td> 
      <td>The subdomain of your [!DNL Workfront] account. This is used to create a link back to your [!DNL Workfront] project in a note that may be generated.</td> 
     </tr> 
    </tbody> 
   </table>

   Details on how to set up the files and processes are provided in the [!DNL Anaplan] setup documentation.

1. Select or add an [!DNL Anaplan] connection profile.
1. Update all remaining [!DNL Anaplan] modules with an [!DNL Anaplan] connection, when prompted.
1. Select or add a [!DNL Workfront] connection profile.

   The filter is configured to pull in all incomplete linked project and those projects that were completed in the last 29 minutes. If you change the frequency of the [!DNL Fusion] scenario you will want to update this value once the scenario template has been deployed.

1. On the **[!UICONTROL Build Projects Update CSV]** module, add a new data structure to map the project attributes to CSV columns.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "itemID": 1000001,<br>        "Workfront Project GUID":"text",<br>        "Campaign Name":"text",<br>        "Percent Complete": 10.01,<br>        "Planned Start Date":"2022-02-22",<br>        "Planned Completion Date":"2022-02-22",<br>        "Planned Hours": 12.5,<br>        "Planned Cost": 123.45,<br>        "Planned Expense Cost": 123.45,<br>        "Planned Labor Cost": 123.45,<br>        "Status": "CUR",<br>        "Campaign Overview":"text",<br>        "Key Message":"text",<br>        "In Market Start Date":"2022-02-22",<br>        "In Market End Date":"2022-02-22",<br>        "Target Audience":"text"<br>    }<br>]<br></code></pre>

1. Update all remaining [!DNL Workfront] modules with a [!DNL Workfront] connection, when prompted.

## Other Recommended Scenario Templates

This scenario template is complimented by the following spend optimization scenario templates that may also be deployed:

* [[!UICONTROL Send [!DNL Adobe Workfront] actual hours updates to an an [!DNL Anaplan] list item]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL Send [!DNL Adobe Workfront] expenses to an [!DNL Anaplan] list item]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

Additional scenarios for linking budget requests:

* [[!UICONTROL Create an [!DNL Anaplan] list item from an [!DNL Adobe Workfront] budget request]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Apply an [!DNL Anaplan] budget allocation to an [!DNL Adobe Workfront] project]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Additional scenarios for linking campaign requests:

* [[!UICONTROL Create an [!DNL Anaplan] list item from an [!DNL Adobe Workfront] campaign request]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Apply an [!DNL Anaplan] budget allocation to an [!DNL Adobe Workfront] campaign request or campaign project]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
