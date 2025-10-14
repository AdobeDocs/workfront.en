---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Send [!DNL Adobe Workfront] actual hours updates to an an [!DNL Anaplan] list item
description: This integration scenario shares actual hours details captured on an [!DNL Adobe Workfront] project with an [!DNL Anaplan] budget list item. Sharing this information allows you to take better advantage of the spend optimization and financial analysis that [!DNL Anaplan] provides.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 450b9a87-79c6-4d10-a9ea-29766b4f5962
---
# Send [!DNL Adobe Workfront] actual hours updates to an an [!DNL Anaplan] list item

This integration scenario shares actual hours details captured on an [!DNL Adobe Workfront] project with an [!DNL Anaplan] budget list item. Sharing this information allows you to take better advantage of the spend optimization and financial analysis that [!DNL Anaplan] provides.

This scenario template delivers a list of hours summarized by project, day, and role recorded on active projects over then last 3 months.

>[!IMPORTANT]
>
>"Campaign" in this article refers to the marketing campaign use case that this scenario represents, and is in no way connected to the [!DNL Workfront Fusion] Adobe Campaign connector or to the recently deprecated [!UICONTROL Campaign] object in [!DNL Workfront].

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Any Adobe Workfront Workflow package and any Adobe Workfront Automation and Integration package</p><p>Workfront Ultimate</p><p>Workfront Prime and Select packages, with an additional purchase of Workfront Fusion.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront licenses</td> 
   <td> <p>Standard</p><p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion license</td> 
   <td>
   <p>Operation-based: No Workfront Fusion license requirement</p>
   <p>Connector-based (legacy): Workfront Fusion for Work Automation and Integration </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>If your organization has a Select or Prime Workfront package that does not include Workfront Automation and Integration, your organization must purchase Adobe Workfront Fusion.</li></ul>
   </td> 
  </tr>
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

For information on Adobe Workfront Fusion licenses, see [Adobe Workfront Fusion licenses](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration).

## Triggering Event

This scenario is scheduled to execute every 15 minutes.

## Expected [!DNL Workfront] Configuration

You must have the following in [!DNL Workfront] to use this scenario:

* A user profile in [!DNL Workfront] named **[!UICONTROL Anaplan Integration]**, that has system administrator rights.

   For information on creating a user in [!DNL Workfront], see [Add users](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Expected [!DNL Anaplan] Configuration

You must have the following in [!DNL Anaplan] to use this scenario:

* A user profile in [!DNL Anaplan] named **[!UICONTROL [!DNL Workfront ] Integration]**, that has system administrator rights.
* The [!DNL Anaplan] Model that you want to use for this scenario.
* The List within the [!DNL Anaplan] Model that you want to use for this scenario.
* A file in [!DNL Anaplan] named **[!UICONTROL Anaplan Actual Hours Import]** that contains the following columns, in this order:

   1. [!UICONTROL Workfront Project GUID]

   2. [!UICONTROL Hours]

   3. [!UICONTROL Hours Estimated Cost]

   4. [!UICONTROL Entry Date]

   5. [!UICONTROL Role Name]

   6. [!UICONTROL Campaign Name]

   7. [!UICONTROL [!DNL Anaplan] List Item ID]

   To prepare the [!DNL Anaplan] Actual Expense Report file:

   1. Copy and paste the following into a text editor or [!DNL Excel]
   1. Save the file in a CSV format
   1. Upload the file into [!DNL Anaplan].

      For instructions, see the [!DNL Anaplan] documentation about importing data into modules from a file.

   1. Make note of the name you gave to the file; it will be used during the deployment of the [!UICONTROL Fusion] scenario template.

   Example CSV contents

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[!DNL Workfront] Project GUID,Hours,Hours Estimated Cost,Entry Date,Role Name,Workfront Project Name,Item ID<br>6218062a000d0442903fcfa21e11f556,2,0,3/7/22,Designer,New Project 6,202000001030</code></pre>

* A **[!UICONTROL Project Actual Hours Import]** process prepared to execute the import of data delivered in a file upload.

For instructions on any of these actions, see the [!DNL Anaplan] documentation.

## Deploying to [!DNL Workfront Fusion]

Complete the following steps to deploy this integration scenario to your [!DNL Fusion] account. This should only be done after completing the required [!DNL Workfront] and [!DNL Anaplan] configuration.

1. Navigate to the [!UICONTROL Templates] menu in [!DNL Workfront Fusion] and click the **[!UICONTROL Send Workfront actual hours updates to [!DNL Anaplan] list item]** scenario template.
1. Replace the variable values for the following [!DNL Anaplan] variables:

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
      <td role="rowheader">[!UICONTROL File Name: Actual Hours Import]</td> 
      <td> <p>Tthe name of the file that will receive project actual hours data.</p> <p> (Example: WorkfrontUpdateLinkedProjects_HoursRoles.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Process Name: Actual Hours Import]</td> 
      <td> <p>The name of the process that will execute the import of project hours data.</p> <p>(Example: WF Int - Load Project Hours by Role)</p> </td> 
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
1. Update all remaining [!DNL Workfront] modules with a [!DNL Workfront] connection, when prompted.

## Other Recommended Scenario Templates

This scenario template is complimented by the following spend optimization scenario templates that may also be deployed:

* [[!UICONTROL Send [!DNL Adobe Workfront] project updates to an [!DNL Anaplan] list item]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Send [!DNL Adobe Workfront] expenses to an [!DNL Anaplan] list item]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

Additional scenarios for linking budget requests:

* [[!UICONTROL Create an [!DNL Anaplan] list item from an [!DNL Adobe Workfront] budget request]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Apply an [!DNL Anaplan] budget allocation to an [!DNL Adobe Workfront] project]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Additional scenarios for linking campaign requests:

* [[!UICONTROL Create an [!DNL Anaplan] list item from an [!DNL Adobe Workfront] campaign request]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Apply an [!DNL Anaplan] budget allocation to an [!DNL Adobe Workfront] campaign request or campaign project]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
