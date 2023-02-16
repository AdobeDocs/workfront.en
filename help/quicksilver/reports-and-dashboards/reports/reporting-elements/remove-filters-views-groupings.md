---
product-area: reporting
navigation-topic: reporting-elements
title: Remove filters, views, and groupings
description: You can remove a filter, view, or grouping from lists and reports if you created them or they have been shared with you. You cannot remove default filters, views, or groupings.
author: Lisa
feature: Reports and Dashboards
exl-id: 422d262e-e19d-4070-85f1-77ecb7430342
---
# Remove filters, views, and groupings

<span class="preview">Note that in the Preview environment, the enhanced filter experience (previously called "beta") is now the default. These filters are now called "standard" and the older filter experience is called "legacy."</span>

You can remove a filter, view, or grouping from lists and reports if you created them or they have been shared with you. You cannot remove default filters, views, or groupings.

## Access requirements

You must have the following:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan*</strong></td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations*</strong></td> 
   <td> <p>View or higher access to Filters, Views, Groupings</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permissions</strong></td> 
   <td> <p>View permissions with access to share to the filter, view, or grouping you want to remove</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;To find out what plan, license type, or access you have, contact your Workfront administrator.

## Remove a filter, view, or grouping using the standard builder

You can remove a filter, view, or a grouping for all lists of objects using the standard builder interface.

### Considerations about removing filters, views, and groupings

How you remove a reporting element depends on whether you initially created it, or it was shared with you.

The following scenarios exist when you remove a grouping:

* **If you created the grouping and you remove it**, the grouping is removed from the Workfront system. The grouping is no longer available to any users who you previously shared it with.
* **If the grouping was shared with you and you remove it**, the grouping is removed only for you. The user who originally created it and any other users it has been shared with still have access to the grouping.

### Remove a filter, view, or grouping using the standard builder

1. Go to a list of objects or a report.
1. (Conditional) From a list, click the **Filter**, **View**, or **Grouping** icon, then hover over the filter, view, or grouping you want to remove, click the **More** icon ![](assets/more-icon.png), then **Remove**. The filter, view, or grouping is removed. 
1. (Conditional) From a report, click the **Grouping**, **Filter**, or **View** drop-down menu and select **Remove Grouping**, **Remove Filter**, or **Remove View**.

   The **My Groupings**, **My Filters,** or **My Views** dialog box displays.

   All reporting elements that you have rights to remove are available to remove. Other reporting elements are displayed as dimmed.

1. Click the **x** icon next to any reporting element that you want to remove. 
1. (Conditional) Click **Yes, Delete it** if you selected to delete a filter, view, or grouping that you created and later shared with others.&nbsp;This deletes the filter, view, or grouping from the Workfront system.

   >[!TIP]
   >
   >Removing a filter, view, or grouping that you created without sharing it with others removes it from the system without asking for a confirmation.

1. Click **Done**.

## Remove or delete a filter using the beta builder

You can remove a filter that was shared with you from lists of projects, tasks, or issues using the beta builder interface. The beta builder interface is not available for any other objects, or for views or groupings.

You can also delete filters that you own from lists of projects, tasks, or issues using the beta builder interface.

System default filters can't be removed or deleted.

### Considerations about removing or deleting filters using the beta builder

The following scenarios exist when you remove or delete a filter:

* If the filter was shared with you and you remove it, the filter is removed only for you. The user who originally created it and any other users it has been shared with still have access to the filter.
* If you own the filter and you delete it, the filter is removed from the Workfront system. The filter is no longer available to any users who you previously shared it with.
* If you are a Workfront administrator, you can delete the filter and it is permanently deleted for all users, including the owner.

### Remove a filter using the beta builder

1. Go to a list of projects, tasks, or issues.
1. Click the **Filter** icon ![Filter icon](assets/filter-nwepng.png) and enable the beta builder if needed.
1. Hover over a filter under **Shared with me**, click the **More** menu ![More icon](assets/more-icon-spectrum.png), then click **Remove**.

   ![Remove filter](assets/new-filters-more-menu-remove-filter.png)

1. Select **Remove** on the confirmation message to permanently remove the filter.   

### Delete a filter using the beta builder

1. Go to a list of projects, tasks, or issues.
1. Click the **Filter** icon ![Filter icon](assets/filter-nwepng.png) and enable the beta builder if needed.
1. Hover over a filter that you have permissions to delete, click the **More** menu ![More icon](assets/more-icon-spectrum.png), then click **Delete**.

   ![Delete filter](assets/new-filters-more-menu-options-with-delete.png)

1. (Optional) Click **Cancel** on the confirmation message to avoid the deletion and return to the list of filters.
1. Click **Delete** on the confirmation message to confirm the deletion.
                        
   The filter is deleted for you and all users who had permissions to it.

