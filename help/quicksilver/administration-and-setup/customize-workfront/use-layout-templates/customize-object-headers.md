---
title: Customize Object Headers Using a Layout Template
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: As an Adobe Workfront administrator or a group administrator , you can use a layout template to configure the fields users see in the object header when they open an object's page.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: cbeaa0d7-a61a-4806-a871-96663d9ce124
---
# Customize object headers using a layout template

As an Adobe Workfront administrator or a group administrator, you can use a layout template to configure the fields users see in the object header when they open an object's page.

>[!IMPORTANT]
>
>Customizing object headers is currently available for projects, tasks, and issues.

![Object header fields](assets/object-header-fields.png)

For information about creating layout templates, see [Create and manage layout templates](../use-layout-templates/create-and-manage-layout-templates.md). 

For information about layout templates for groups, see [Create and modify a group's layout templates](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

After configuring a layout template, you must assign it to users for changes you made to be visible to others. For information about assigning a layout template to users, see [Assign users to a layout template](../use-layout-templates/assign-users-to-layout-template.md).

## Access requirements

+++ Expand to view access requirements for the functionality in this article.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Any</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront license</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Access level configurations</td> 
   <td> <p>To perform these steps at the system level, you need the System Administrator access level.</p>
        <p>To perform them for a group, you must be a manager of that group.</p> </td> 
  </tr> 
 </tbody> 
</table>

For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

## Customize object headers

1. Begin working on a layout template, as described in [Create and manage layout templates](../../customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. In the **Customize what users see** drop-down menu, select **Projects**, **Tasks**, or **Issues**.

    <!--when this will be possible for more than 3 objects, at production, make this more general: update the sentence above to say "select an object you want to customize in the Customize what users see drop-down menu). -->

1. In the [!UICONTROL Header fields] section, mouse over the fields displayed and do one of the following:
    * Click the **x** icon to remove a field
        
        Or
    
    * Click and hold the **grab** icon to drag and drop the field in a new location.

    <!--(NOTE: make sure the default names of these fields have not changed; otherwise, update screen shot)-->

    ![Object header fields hide and move icons](assets/object-header-field-x-and-grab-icons-in-lt.png)

1. You can have up to five fields in the header of an object.
If you already have five fields selected, you must remove a field before you can add a new one.
1. In the **Add field** box, start typing the name of a non-editable Workfront field that you want to add, then select it when it displays in the list. The field is added to the immediate right of the Add field box and will display as the first field in the upper-left corner of the object's header.

    >[!TIP]
    >
    >* You can only add fields that display in the Overview area of the object's Details section and which are non-editable. Non-editable fields are fields that users cannot manually edit. They are automatically calculated by Workfront. 
    >
    >* You can add editable fields that are already part of the default headers (for example, Project Owner, Status, Percent Complete, Assignments).
    >
    >* When you add the "Resolved By" field to the header of an issue, the field changes to "Resolving Issue, Task, or Project", when there is a resolving object associated with the issue.  

   
    ![Add field to header](assets/add-field-to-header-in-lt-list.png)  
  

1. (Optional) Drag and drop the fields added in a different order.       
    
1. Continue customizing the layout template.

    Or

    If you are finished customizing, click **Save**.

    >[!TIP]
    >
    >You can click Save at any time to save your progress, then continue to modify the template later.
