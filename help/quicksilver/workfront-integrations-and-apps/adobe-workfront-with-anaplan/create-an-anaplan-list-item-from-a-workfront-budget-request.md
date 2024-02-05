---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Create an [!DNL Anaplan] list item from an [!DNL Adobe Workfront] budget request
description: This integration scenario links an [!DNL Adobe Workfront] project (campaign) with an [!DNL Anaplan] budget list item. This is accomplished by adding a budget request to the [!DNL Workfront] project that needs to receive funding. This scenario watches for unprocessed budget requests, then executes a process to create an empty budget list item in [!DNL Anaplan] to kick off budget allocation processes in Anaplan.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: e6505ece-21aa-4397-8d68-543bf89d2f00
---
# Create an [!DNL Anaplan] list item from an [!DNL Adobe Workfront] budget request

This integration scenario links an [!DNL Adobe Workfront] project (campaign) with an [!DNL Anaplan] budget list item. This is accomplished by adding a budget request to the [!DNL Workfront] project that needs to receive funding. This scenario watches for unprocessed budget requests, then executes a process to create an empty budget list item in [!DNL Anaplan] to kick off budget allocation processes in [!DNL Anaplan].

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
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>Your organization must purchase [!DNL Adobe Workfront Fusion] as well as [!DNL Adobe Workfront] to use functionality described in this article.</td> 
  </tr>
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your [!DNL Workfront] administrator.

&#42;&#42;For information on[!DNL  Adobe Workfront Fusion] licenses, see [[!DNL Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Triggering Event

This scenario is scheduled to execute every 15 minutes.

## Expected [!DNL Workfront] Configuration

You must have the following in [!DNL Workfront] to use this scenario:

* A user profile in [!DNL Workfront] named *[!UICONTROL *[!DNL Anaplan] Integration]**, that has system administrator rights.

   For information on creating a user in [!DNL Workfront], see [Add users](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* A **[!UICONTROL Budget Request]** custom form attached to the [!UICONTROL Request] object.

   The following required fields must be included on the custom form to aid in data mapping to [!DNL Anaplan]:

   <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <thead> 
    <tr> 
     <th>Field Name</th> 
     <th>Field Type</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader">[!UICONTROL Budget Request Type]</td> 
     <td> <p>[!UICONTROL Dropdown]</p> <p>Options:</p> 
      <ul> 
       <li> <p>[!UICONTROL Adjustment to Funding]</p> </li> 
       <li> <p>[!UICONTROL Initial Funding]</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Requested Labor Funds]</td> 
     <td> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Requested Expense Funds]</td> 
     <td> </td> 
    </tr> 
   </tbody> 
  </table>

   For information on creating custom forms, see [Create or edit a custom form](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

* Project templates representing campaigns and other projects requiring funding, configured with a [!UICONTROL Budget Request] queue topic. The [!UICONTROL Budget Request] queue topic is assigned to use the [!UICONTROL Budget Request] custom form.
* A **[!UICONTROL Campaign Brief]** form for the project object.

   This form must contain the following fields:

   <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
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
     <td>[!UICONTROL Rich Text Field]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Key Message]</td> 
     <td>[!UICONTROL Rich Text Field]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Target Audience]</td> 
     <td> <p>[!UICONTROL Dropdown]</p> <p>Include options that fit your processes.</p> </td> 
    </tr> 
   </tbody> 
  </table>

   For information on creating custom forms, see [Create or edit a custom form](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

## Expected [!DNL Anaplan] Configuration

You must have the following in [!DNL Anaplan] to use this scenario:

* A user profile in [!DNL Anaplan] named **[!UICONTROL [!DNL Workfront] Integration]**, that has system administrator rights.
* The [!DNL Anaplan] Model that you want to use for this scenario.
* The List within the [!DNL Anaplan] Model that captures campaign budgets.

   The list's module must support receiving the following attributes:

    * [!UICONTROL Workfront Project GUID]
    * [!UICONTROL Campaign Name]
    * [!UICONTROL Requested Labor Funds]
    * [!UICONTROL Requested Expense Funds]
    * [!UICONTROL Budget Request Type]
    * [!UICONTROL Reason for Funding Adjustment]

   This list and module must store additional details that are necessary for the normal functionality of [!DNL Anaplan], including the ability to set a budget and communicate that the budget list item is ready to be synced back to [!DNL Workfront].

For instructions on any of these actions, see the [!DNL Anaplan] documentation.

## Deploying to [!DNL Workfront Fusion]

Complete the following steps to deploy this integration scenario to your [!DNL Fusion] account. This should only be done after completing the required [!DNL Workfront] and [!DNL Anaplan] configuration.

1. Navigate to the [!UICONTROL Templates] menu in [!DNL Workfront Fusion] and click the **[!UICONTROL Create an [!DNL Anaplan] list item from a Workfront budget request]** scenario template.
1. Replace the variable values for the following [!DNL Anaplan] variables:

   | Variable name | Replace value with |
   |---|---|
   | [!UICONTROL [!DNL Anaplan] Workspace ID] | The ID of a workspace from your [!DNL Anaplan] account. |
   | [!UICONTROL [!DNL Anaplan] Model ID] | The ID of a model from your [!DNL Anaplan] account and the selected workspace. |
   | [!UICONTROL [!DNL Anaplan] Module Name] | The name of the module that describes the campaign attributes in the selected [!DNL Anaplan] List. |
   | [!UICONTROL Campaign List Name] | The name of the list from your [!DNL Anaplan] account and the selected workspace & model. |

   {style="table-layout:auto"}

   Details on how to set up the files and processes are provided in the [!DNL Anaplan] setup documentation.

1. Select or add an [!DNL Anaplan] connection profile.
1. Update all remaining [!DNL Anaplan] modules with an [!DNL Anaplan] connection, when prompted.
1. Select or add a [!DNL Workfront] connection profile.

   After deploying the template, this is the module you will update to add or remove custom field references from the value of the fields property if you want to alter the default mapped fields to [!DNL Anaplan].

1. Update all remaining [!DNL Workfront] modules with a [!DNL Workfront] connection, when prompted.

## Other Recommended Scenario Templates

To complete the workflow represented by this template, you must also deploy the following additional template:

* [[!UICONTROL Apply an [!DNL Anaplan] budget allocation to an [!DNL Adobe Workfront] project]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Additional scenarios for spend optimization include:

* [[!UICONTROL Send [!DNL Adobe Workfront] project updates to an [!DNL Anaplan] list item]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Send [!DNL Adobe Workfront] actual hours updates to an an [!DNL Anaplan] list item]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL Send [!DNL Adobe Workfront] expenses to an [!DNL Anaplan] list item]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
