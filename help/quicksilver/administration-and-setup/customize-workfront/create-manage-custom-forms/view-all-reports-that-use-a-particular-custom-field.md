---
title: View all reports that use a particular custom field or widget
description: View all reports that use a particular custom field or widget
draft: Probably
feature: System Setup and Administration
role: Admin
---
# View all reports that use a particular custom field or widget

You can add a custom view in the Custom Forms area that shows which reports are using a particular custom field or widget. This is useful when you need to edit or delete the field or widget, because it might already be implemented in one or more reports. It's important to assess whether those reports will need adjustments in order to keep working properly.

For information about custom fields and widgets in custom forms, see [Add a custom field to a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) and [Add or edit an asset widget in a custom form](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

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
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Administrative access to custom forms</p> <p>For information about how Workfront administrators grants this access, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access level configurations you have, contact your Workfront administrator.

## List the reports that use a particular custom field or widget

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).

1. In the left panel, click **Custom Forms**.
1. Open the **Fields** tab to display a report listing all of custom fields and widgets in your Workfront instance.

   ![](assets/fields-tab-350x221.png)

1. Click the **View** drop down menu in the header at the top of the list, then check for any custom views in the list that include the **Reports** column (which is not a default column on this tab).

   The Reports column is where you can see which reports are using each custom field and widget that has been added to a custom form in your system. It's possible that someone has already created a view that includes the **Reports** column.

1. If you don't see a view that includes the **Reports** column, create a new view that includes it:

   1. Click the **View** drop-down menu, then click **New View**.
   
   1. On the **New View** page that appears, in the box near the upper-left corner, replace **New Parameter View** with a descriptive name for the view, such as *Fields and widgets*.
   
   1. Click **Add Column** near the lower-right corner.
   1. In the **Show in this column** box that displays near the upper-left corner, start typing *report*, then select **Reports** when it appears in the list below the box.
   
   1. (Conditional) If you want to move the **Reports** column you just added to a different horizontal position, drag its header in the **Column Preview** area at the bottom of the page.
   
   1. Click **Done**, then click **Save View**.

1. Click the **View** drop down menu, then select the name of the custom view you just created.
1. In the **Name** column, find the custom field or widget you plan to edit or delete, then look at the **Reports** column on that row to see which reports use it, if any.

   To find the information for this column, Workfront searches for the custom fields and widgets in all report filters, views, groupings.

   If you see a plus sign, you can click that line of text to display a box listing all additional reports that use the field or widget.

   >[!NOTE]
   >
   >The initial load time for this tool can take anywhere from 10 seconds to 2.5 minutes, depending on the amount of data in your system.

   >[!TIP]
   >
   >* If you don't have time to investigate the reports that are using the custom field or widget, you can click Export to create a file that lists them. You could share this file with anyone who owns a report that's using the field or widget and discuss the change that needs to happen, the impact it might have on the report, and what needs to be done to make sure that the report continue to work correctly.
   >* This view is also available in a Parameter report:
   >      
   >1. In the Main Menu, click **Reports**.
   >1. Near the upper-left corner, click **New Report**, then click **Parameter** in the list that displays.
   >      
   >1. Click **Add Column** near the lower-right corner.
   >1. In the **Show in this column** box that displays near the upper-left corner, start typing *report*, then select **Reports** when it appears in the list below the box.
   >1. (Conditional) If you want to move the **Reports** column you just added to a different horizontal position, drag its header in the **Column Preview** area at the bottom of the page.
   >1. Click **Done**, then click **Save+Close**.
   >1. Type a descriptive name for the report, such as *Fields and widgets*.
