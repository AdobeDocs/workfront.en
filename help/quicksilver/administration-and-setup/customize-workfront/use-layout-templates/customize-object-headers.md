---
title: Customize object headers using a layout template
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: As an Adobe Workfront administrator or a group administrator , you can use a layout template to configure the fields users see in the object header when they open an object's page.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: cbeaa0d7-a61a-4806-a871-96663d9ce124
---
# Customize object headers using a layout template

As an Adobe Workfront administrator or a group administrator, you can use a layout template to configure the fields users see in the object header when they open an object's page.

>[!IMPORTANT]
>
>Customizing object headers is currently available only for projects.

<!--drafted for task headers: replace above with this: Customizing object headers is currently available for projects <span class="preview">and tasks</span>. -->

<!--drafted for task AND issue headers: replace above with this when issue custom headers are coming too: Customizing object headers is currently available for projects <span class="preview">, tasks</span>, and <span class="preview">issues</span>. -->

For information about layout templates for groups, see [Create and modify a group’s layout templates](../../manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md). 

![](assets/object-header-fields.png)

## Access requirements

You must have the following access to perform the steps in this article:


<table>
  <tr>
   <td><strong>Adobe Workfront plan</strong>
   </td>
   <td>Any
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront license</strong>
   </td>
   <td>Plan
   </td>
  </tr>
  <tr>
   <td>Access level configurations*
   </td>
   <td>You must be a Workfront or a group administrator.
<p>
   </td>
  </tr>
</table>

If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see [Create or modify custom access levels](../../add-users/configure-and-grant-access/create-modify-access-levels.md). 

## Customize object headers

1. Begin working on a layout template, as described in [Create and manage layout templates](../../customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. In the **Customize what users see** drop-down menu, select **Projects**.

    <!--(NOTE: when more objects are supported, update this to say "select an object you want to customize in the Customize what users see drop-down menu). -->

1. In the [!UICONTROL Header fields] section, mouse over the fields displayed and do one of the following:
    * Click the **x** icon to remove a field
        
        Or
    
    * Click and hold the **grab** icon to drag and drop the field in a new location.

    <!--(NOTE: make sure the default names of these fields have not changed; otherwise, update screen shot)-->

    ![](assets/object-header-field-x-and-grab-icons-in-lt.png)

1. You can have up to five fields in the header of an object.
If you already have five fields selected, you must remove a field before you can add a new one.
1. In the **Add field** box, start typing the name of a non-editable Workfront field that you want to add, then select it when it displays in the list. The field is added to the immediate right of the Add field box and will display as the first field in the upper-left corner of the object's header.

    >[!TIP]
    >
    >Non-editable fields are fields that users cannot manually edit. They are automatically calculated by Workfront. You can only add fields that display in the Overview area of the object's Details section. 

    <!--drafted for task customizable headers - add is as a second bullet for the TIPS above and make what is there the first bullet: 
    * Editable fields that are already part of the default headers (for example, Project Owner, <span class="preview">Status, Percent Complete, Assignments</span>) are allowed. -->

    ![](assets/add-field-to-header-in-lt-list.png)  
  

1. (Optional) Drag and drop the fields added in a different order.       
    
1. Continue customizing the layout template.

    Or

    If you are finished customizing, click **Save**.

    >[!TIP]
    >
    >You can click Save at any time to save your progress, then continue to modify the template later.
