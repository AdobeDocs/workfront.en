---
filename: display-or-skip-logic-custom-form
title: Display or skip logic on a Custom Form
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Display logic and skip logic on a custom form
description: You can decide which sections of a custom form should be displayed or skipped based on the choices that a user makes when filling it out.
---

# Display logic and skip logic on a custom form

You can decide which sections of a custom form should be displayed or skipped based on the choices that a user makes when filling it out.

## Access requirements

You must have the following to perform the steps in this article:

<table cellspacing="0"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Administrative access to custom forms</p> <p>For information about how Workfront administrators grants this access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;To find out what plan, license type, or access level configurations you have, contact your Workfront administrator.

## Considerations for using display logic and skip logic

* To add display logic on a custom field or a section break, you must have a multiple choice field (radio buttons, dropdown, or checkboxes) prior to the field you would like to display on the form.  

* If you want to add skip logic on a custom field, the field must be a multiple choice field.
* You cannot add skip logic to a section break.
* You can add both display logic and skip logic to a field if the field is:

   * A multiple choice field
   * Preceded by a multiple choice field
   * Followed by another field

* When copying forms with display logic or skip logic, the logic is copied to the new custom form.
* Keep the following in mind when you create a display rule for a custom form

   * Fields not included in a display logic statement show on a custom form, by default. 
   * Display logic can be applied to section breaks, as well as custom fields. 
   * Skip logic can be applied only to custom fields. 
   * You can create multi-field display logic statements. 
   * You can apply display rules to existing custom forms.

## Create a sample custom form that has display logic

1. Click **Setup** near the upper-right corner of Adobe Workfront on the Global Navigation Bar.  

1. In the left panel, click **Custom Forms** ![](assets/custom-forms-icon.png). 

1. Create the sample custom form:

   1. Click **New Custom Form**, then click **Project** in the drop-down list.
   
   1. In the **Form Title** box, type **Sample custom form - Learning display logic and skip logic**.
   
   1. Click **Add a Field** in the upper left corner.
   1. Add a dropdown field called "Issue Field" by clicking **Dropdown**, then typing **Issue field** in the **Label** box.
   
   1. Click **Save + Close** in the lower left corner.

1. Select the new **Sample custom form - Learning display logic and skip logic** custom form, then click **Edit**. 

1. Add a new single line text field called "Other Research" by clicking **Single Line Text Field**, then typing&nbsp;**Other Research** in the **Label** box.

1. Click **Add Logic** near the lower-left side of the **Edit Custom Form** screen.  

1. In the box that appears, with the **Display Logic** tab open, set up the logic for when the **Other Research** field will appear on the form by clicking **Issue field** in the first drop-down, **Research Needed** in the second drop-down, and **Selected** in the third drop-down.

   Now, when someone selects **Research Needed** in the **Issue field** drop-down, the **Other Research** field will display.

1. Click **Save** to close the **Field Logic** window, then click **Done** in the **Field Settings** area. 

1. Click **Preview** to make sure the logic appears the way you want it on the form.
1. Click **End Preview** when you find that the logic works as expected.
1. Click **Save + Close** on the **Edit Custom Form** window to save the form, then continue on to [Skip logic on a custom form](#skip-logic)below.

## Skip logic on a custom form

Skip logic allows you determine which fields should be skipped, based on selections in the custom form. It functions similarly to display logic, but acts as the inverse: instead of making specific fields appear based on specific selections, you determine which fields should be skipped, based on selections.

To learn about skip logic on custom forms, continue working on the sample custom form you created in the section [Create a sample custom form that has display logic](#display-logic) above:

1. <![CDATA[          ]]>Click **Setup** near the upper-right corner of Adobe Workfront on the Global Navigation Bar.  

1. Click **Custom Forms**. 
1. Select the form **Sample custom form - Learning display logic and skip logic** that you created in the steps above, then click **Edit**. 

1. Select the drop-down field you created named "Issue field." 
1. Click the **Add Logic** button in the **Field Settings** sidebar. 

1. In the **Field Logic** box, make sure the **Skip Logic** tab is selected. 

1. Set the first drop-down to **No more research** and the second drop-down to **Selected**.

1. In the **Then Skip To** drop-down, select **End of form.**

   Now, when someone selects **No more research** in the **Issue field** drop-down field, the form will skip directly to the end of the form without displaying the **Other Research** field.

1. Click **Save**. 
1. Click **Preview** &nbsp;to make sure the logic applies&nbsp;the way you want it. 
1. Click **Done** in the lower left side of the form. 
1. Click **Save + Close** at the bottom of the Custom Forms window to save the changes you made to the form.&nbsp;

