---
title: Add display logic and skip logic to a custom form
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: You can decide which sections of a custom form should be displayed or skipped based on the choices that a user makes when filling it out.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c687c4a8-a99d-4ac0-b785-5bfe503a7e2c
---
# Add display logic and skip logic to a custom form

You can decide which sections of a custom form should be displayed or skipped based on the choices that a user makes when filling it out.

## Access requirements

You must have the following to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Administrative access to custom forms</p> <p>For information about how Workfront administrators grants this access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;To find out what plan, license type, or access level configurations you have, contact your Workfront administrator.

## Considerations for using display logic and skip logic

* To add display logic on a custom field, widget, or section break, at least one multiple choice field (radio buttons, dropdown, or checkboxes) must be positioned prior to it on the form.

  For information about custom fields and widgets in custom forms, see [Add a custom field to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) and [Add or edit an asset widget in a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

* You cannot add skip logic to a widget or section break. You can add it only to a multiple choice field (radio buttons, dropdown, or checkboxes).   

* You can add both display logic and skip logic to a custom field all of the following is true about the custom field:

   * It is a multiple choice field (radio buttons, dropdown, or checkboxes)
   * It is preceded by a multiple choice field
   * It is followed by another custom field

* When copying forms with display logic or skip logic, the logic is copied to the new custom form.
* Keep the following in mind when you create a display logic rule for a custom form

   * Custom fields not included in a display logic statement show on a custom form, by default. 
   * You can create multi-field display logic statements.

## Create a sample custom form that has display and skip logic

The best way to learn how to add display and skip logic to a custom form is through the practical example explained in the two following sections:

* [Display logic](#display-logic) 
* [Skip logic](#skip-logic)

### Display logic {#display-logic}

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).  

1. In the left panel, click **Custom Forms** ![](assets/custom-forms-icon.png). 

1. Create the sample custom form:

   1. Click **New Custom Form**, then click **Project** in the drop-down list.
   
   1. In the **Form Title** box, type **Sample custom form - Learning display logic and skip logic**.
   
   1. Click **Add a Field** in the upper left corner.
   1. Add a dropdown field called *Issue Field* by clicking **Dropdown**, then typing **Issue field** in the **Label** box. 
   
   1. Under **Choices**, add the following choices in the text boxes:

      Research needed

      No more research
   
   1. Click **Save + Close** in the lower left corner.

1. Select the new **Sample custom form - Learning display logic and skip logic** custom form, then click **Edit**. 

1. Add a new single line text field called *Other Research* by clicking **Single Line Text Field**, then typing **Other Research** in the **Label** box.

1. Click **Add Logic** near the lower-left side of the **Edit Custom Form** screen.  

1. In the box that appears, with the **Display Logic** tab open, set up the logic for when the **Other Research** field will appear on the form by clicking **Issue field** in the first drop-down, **Research Needed** in the second drop-down, and **Selected** in the third drop-down. 
1. Click **Save** to close the **Field Logic** window, then click **Done** in the **Field Settings** area.

   Now, when someone selects **Research Needed** in the **Issue field** drop-down, the **Other Research** field will display.

1. Click **Preview** to make sure the logic appears the way you want it on the form.
1. Click **End Preview** when you find that the logic works as expected.
1. Click **Save + Close** on the **Edit Custom Form** window to save the form, then continue on to [Skip logic](#skip-logic) below.

### Skip logic {#skip-logic}

Skip logic functions similarly to display logic, but acts as the inverse: instead of making specific custom multiple-choice fields appear based on specific selections, you determine which ones should be skipped, based on users' selections.

To learn about this, continue working on the sample custom form you created in the section [Display logic](#display-logic) in this article:

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).  

1. Click **Custom Forms**. 
1. Select the form **Sample custom form - Learning display logic and skip logic** that you created in the steps above, then click **Edit**. 

1. Select the drop-down field you created named *Issue field*. 
1. Click the **Add Logic** button in the **Field Settings** sidebar. 

1. In the **Field Logic** box, make sure the **Skip Logic** tab is selected. 

1. Set the first drop-down to **No more research** and the second drop-down to **Selected**.

1. In the **Then Skip To** drop-down, select **End of form.**

   Now, when someone selects **No more research** in the **Issue field** drop-down field, the form will skip directly to the end of the form without displaying the **Other Research** field.

1. Click **Save**. 
1. Click **Preview**  to make sure the logic applies the way you want it. 
1. Click **Done** in the lower left side of the form.
