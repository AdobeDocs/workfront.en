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
TQID: https://experienceleague.adobe.com/lf8hEp6JYtT4mZPP5f6e5M-gX4juYH-hRZF8kGonN3E
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
    internal-label: Measurement
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Create custom expense types

<!--**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

As an [!DNL Adobe Workfront] administrator, you can create custom expense types to define and track the expenses associated with your tasks and projects. Expenses are non-labor costs that can be associated with tasks or projects.

You can edit or delete any expense types that you create. You cannot delete or edit the built-in [!DNL Workfront] expense types.

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] license</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Default expense types

The default expense types in [!DNL Workfront] that cannot be deleted or edited include the following:

* [!UICONTROL Advertising]
* [!UICONTROL Consulting]
* [!UICONTROL Entertainment]
* [!UICONTROL General]
* [!UICONTROL Materials]
* [!UICONTROL Travel]

## Create custom expense types

{{step-1-to-setup}}

1. Click **[!UICONTROL Expense Types]**.
1. Click **[!UICONTROL New expense type]**.
1. In the **[!UICONTROL New Expense Type]** dialog box, enter the following information:

   * **Name** - A name for the expense.
   * **Description** - A description of the expense.
   * **Calculated Unit** - Select the unit of measurement for your expense type from the drop-down list. The following units of measurement are available:
      
      * Mile
      * Kilometer
      * Kilogram
      * Dollar
      * Hour
      * Day
      * Other - Selecting this option prompts you to name your unit of measurement and define the unit of measurement as something familiar to your organization.

   * **Rate** - The price per unit. This is a currency formatted field and it represents the cost of each unit established in the **Calculated Unit** field. The rate can contain a numerical value with up to 4 numbers after the decimal. For example, 1.0375.

1. Click **[!UICONTROL Save]**.
   
   The expense type is now available for users to associate it with their expenses on projects and tasks.

## Modify custom expense types

{{step-1-to-setup}}

1. Click **[!UICONTROL Expense Types]**.
1. Select the expense type that you want to modify, then click the **[!UICONTROL Edit]** icon ![Edit icon](assets/edit-icon.png).

   The **[!UICONTROL Edit Expense Type]** dialog box appears.

1. Make your desired changes, then click **[!UICONTROL Save]**.
   
   The expense type is now available for users to associate it with their expenses on projects and tasks.

For more information about how to use expenses and how they can affect the cost of a project, see the article [Manage project expenses](../../../manage-work/projects/project-finances/manage-project-expenses.md).
