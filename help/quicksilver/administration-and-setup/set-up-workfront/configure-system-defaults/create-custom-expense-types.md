---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Create Custom Expense Types
description: As an [!DNL Adobe Workfront] administrator, you can create custom expense types to define and track the expenses associated with your tasks and projects. Expenses are non-labor costs that can be associated with tasks or projects.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7b76b9e8-fbb8-45a7-9e26-1ddc6d5176d8
---
# Create custom expense types

<!--**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

As an [!DNL Adobe Workfront] administrator, you can create custom expense types to define and track the expenses associated with your tasks and projects. Expenses are non-labor costs that can be associated with tasks or projects.

You can edit or delete any expense types that you create. You cannot delete or edit the built-in [!DNL Workfront] expense types.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td><p>New: [!UICONTROL Standard]</p>
   Or
   <p>Current: [!UICONTROL Plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr>
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Default Expense Types

The Expense Types that are in [!DNL Workfront] by default cannot be deleted or edited include the following:

* [!UICONTROL Advertising]
* [!UICONTROL Consulting]
* [!UICONTROL Entertainment]
* [!UICONTROL General]
* [!UICONTROL Materials]
* [!UICONTROL Travel]

## Create custom expense types

{{step-1-to-setup}}

1. Click **[!UICONTROL Expense Types]**.
1. Click **[!UICONTROL New Expense Type]**.
1. In the **[!UICONTROL New Expense Type]** box that displays, specify the following information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Specify a name for the expense.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Specify a description for the expense.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Calculated Unit]</td> 
      <td> <p>Select the unit of measurement for your expense type from the drop-down list.</p> <p>The following unit of measurements are available:</p> 
       <ul> 
        <li>Mile</li> 
        <li>Kilometer</li> 
        <li>Kilogram</li> 
        <li>Dollar</li> 
        <li>Dollar</li> 
        <li>Day</li> 
        <li>Other - Selecting this option prompts you to name your unit of measurement and define the unit of measurement as something familiar to your organization.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Rate</td> 
      <td> <p>Specify the price per unit. This is a currency formatted field and it represents the cost of each unit established in the <strong>[!UICONTROL Calculated Unit]</strong> field. </p> <p>The rate can contain a numerical value with up to 4 numbers after the decimal. For example, 1.0375</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **[!UICONTROL Create Expense Type]**.\
   The expense type is now available for users to associate it with their expenses on projects and tasks.

## Modify custom Expense Types

{{step-1-to-setup}}

1. Click **[!UICONTROL Expense Types]**.
1. Select the expense type that you want to modify, then click **[!UICONTROL Edit]**.

   The **[!UICONTROL Edit Expense Type]** dialog box is displayed.

1. Make your desired changes, then click **[!UICONTROL Save Changes]**.\
   The expense type is now available for users to associate it with their expenses on projects and tasks.

For more information about how to use expenses and how they can affect the cost of a project, see the article [Manage project expenses](../../../manage-work/projects/project-finances/manage-project-expenses.md).
