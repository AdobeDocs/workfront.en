---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Apply an [!DNL Anaplan] budget allocation to an [!DNL Adobe Workfront] project
description: This integration scenario syncs any budget allocations that have been made in [!DNL Anaplan] back to [!DNL Workfront]. The scenario pulls all linked campaign budget items, then passes the budged value to the linked Workfront project if the budget value has been changed.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 9b8add8f-1978-4ab4-87ac-f1159e7d6cbb
---
# Apply an [!DNL Anaplan] budget allocation to an [!DNL Adobe Workfront] project

This integration scenario syncs any budget allocations that have been made in [!DNL Anaplan] back to [!DNL Workfront]. The scenario pulls all linked campaign budget items, then passes the budged value to the linked [!DNL Workfront] project if the budget value has been changed.

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

* A user profile in [!DNL Workfront] named **Anaplan Integration**, that has system administrator rights.

   For information on creating a user in [!DNL Workfront], see [Add users](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Expected [!DNL Anaplan] Configuration

You must have the following in [!DNL Anaplan] to use this scenario:

* A user profile in [!DNL Anaplan] named **[!DNL Workfront] Integration**, that has system administrator rights.
* The [!DNL Anaplan] Model that you want to use for this scenario.
* The List within the [!DNL Anaplan] Model that captures campaign budgets.

   The list's module must support receiving the following attributes:

    * [!UICONTROL Workfront Project GUID]
    * [!UICONTROL Campaign Name]
    * [!UICONTROL Requested Labor Funds]
    * [!UICONTROL Estimated Revenue]
    * [!UICONTROL Brand]

   This list and module must store additional details that are necessary for the normal functionality of [!DNL Anaplan], including the ability to set a budget and communicate that the budget list item is ready to be synced back to [!DNL Workfront].

* A view in [!DNL Anaplan] named **[!UICONTROL Campaigns.Update Campaigns in Adobe Workfront]**.

   This view must contain the following columns, in this order:

   1. [!UICONTROL Item Name]

   2. [!UICONTROL [!DNL Workfront] Project GUID]

   3. [!UICONTROL Campaign Name]

   4. [!UICONTROL Budget]

   5. [!UICONTROL Estimated Revenue]

   6. [!UICONTROL Brand]

   The view should be filtered to display items that have a [!UICONTROL [!DNL Workfront] Project GUID] and some indicator that budget allocations should be transmitted to [!DNL Workfront].

For instructions on any of these actions, see the [!DNL Anaplan] documentation.

## Deploying to [!DNL Workfront Fusion]

Complete the following steps to deploy this integration scenario to your [!DNL Fusion] account. This should only be done after completing the required [!DNL Workfront] and [!DNL Anaplan] configuration.

1. Navigate to the [!UICONTROL Templates] menu in [!DNL Workfront Fusion] and click the **[!UICONTROL Apply [!DNL Anaplan] budget allocations to Workfront projects]** scenario template.
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
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Module Name]</td> 
      <td>The name of the module that describes the campaign attributes in the selected [!DNL Anaplan] List.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Campaign List Name]</td> 
      <td>The name of the list from your [!DNL Anaplan] account and the selected workspace &amp; model.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] View Name]</td> 
      <td> <p>The name of the view that contains ready-to-transmit campaign budgets to [!DNL Workfront].</p> <p>(Example: [!UICONTROL Campaigns.Load Campaigns to [!DNL Adobe Workfront]]) </p> </td> 
     </tr> 
    </tbody> 
   </table>

   Details on how to set up the files and processes are provided in the [!DNL Anaplan] setup documentation.

1. Select or add an [!DNL Anaplan] connection profile.
1. Update all remaining [!DNL Anaplan] modules with an [!DNL Anaplan] connection, when prompted.
1. On the **[!UICONTROL Convert CSV to JSON Object module]**, add a new data structure to map the CSV columns to a usable JSON object.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Anaplan Name":"text",<br>        "Workfront Project GUID":"text",<br>        "Campaign Name":"text",<br>        "Budget": 100.01,<br>        "Estimated Revenue": 100.01,<br>        "Brand":"text"<br>    }<br>]<br></code></pre>

1. When prompted, select this data structure for other modules in this scenario deployment.
1. On the **[!UICONTROL Check Linked Project]** module, select or add a [!DNL Workfront] connection profile.
1. Update all remaining [!DNL Workfront] modules with a [!DNL Workfront] connection, when prompted.

## Other Recommended Scenario Templates

To complete the workflow represented by this template, you must also deploy the following additional template:

* [[!UICONTROL Create an [!DNL Anaplan] list item from an [!DNL Adobe Workfront] budget request]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)

Additional scenarios for spend optimization include:

* [[!UICONTROL Send [!DNL Adobe Workfront] project updates to an [!DNL Anaplan] list item]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL Send [!DNL Adobe Workfront] actual hours updates to an an [!DNL Anaplan] list item]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL Send [!DNL Adobe Workfront] expenses to an [!DNL Anaplan] list item]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
