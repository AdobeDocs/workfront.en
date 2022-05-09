---
filename: create-custom-expense-types
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Create custom expense types
description: Create custom expense types
---

# Create custom expense types

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

You can keep track of expenses on projects and tasks. Expenses are non-labor costs and can be associated with tasks or projects.

As the Adobe Workfront administrator, you can create custom expense types, to define the expenses associated with your tasks and projects. Some expense types are already in Workfront by default.

You can edit or delete any expense types that you create. You cannot delete or edit default expense types.

## Access requirements

You must have the following access to perform the steps in this article: 

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>You must be a Workfront administrator. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Grant a user full administrative access</a>.</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Default Expense Types

The Expense Types that are in Workfront by default cannot be deleted or edited include the following:

* Advertising
* Consulting
* Entertainment
* General
* Materials
* Travel

## Create custom expense types

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront.
1. Click **Expense Types**.
1. Click **New Expense Type**.  
   The **New Expense Type** dialog box is displayed.

1. Specify the following information:

   <table cellspacing="0"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Name</td> 
      <td>Specify a name for the expense.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Description</td> 
      <td>Specify a description for the expense.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Calculated Unit</td> 
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
      <td> <p>Specify the price per unit. This is a currency formatted field and it represents the cost of each unit established in the <strong>Calculated Unit</strong> field. </p> <p>The rate can contain a numerical value with up to 4 numbers after the decimal. For example, 1.0375</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Click **Create Expense Type**.  
   The expense type is now available for users to associate it with their expenses on projects and tasks.

## Modify custom Expense Types

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront.
1. Click **Expense Types**.
1. Select the expense type that you want to modify, then click **Edit**.

   The **Edit Expense Type** dialog box is displayed.

1. Make your desired changes, then click **Save Changes**.  
   The expense type is now available for users to associate it with their expenses on projects and tasks.

For more information about how to use expenses and how they can affect the cost of a project, see the article [Manage project expenses](../../../manage-work/projects/project-finances/manage-project-expenses.md). 
