---
title: Share views
description: You can share a view with others to ensure collaboration when using the Adobe Workfront planning capabilities.
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
---
<!--update the metadata and description when we turn this article live-->

# Share views

{{maestro-important-intro}}

You can share a view with others to ensure collaboration when working with records in Adobe Workfront planning capabilities. 

Granting permissions to a workspace does not give other users permissions to the views on the record type pages. You must grant permissions to individual views in a record type page to share them with other users. 

## Access requirements

You must have the following access to perform the steps in this article: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Workfront planning capabilities closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> There are no access controls for Adobe Workfront planning capabilities</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Object permissions</p></td>
   <td> <p>Manage permissions to a view</p>  
    
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Maestro area in the Main Menu. </p> <p>For information, see <a href="/help/quicksilver/maestro/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## Share permissions to a view

You can share views you created or views you have Manage permissions to. 

>[!NOTE]
>
>System Administrators cannot view or share views they did not create themselves. They can only access or share views that are shared with them.
>
>System administrators can have only Manage permissions to a view. 

{{step1-to-maestro}}

1. Open the workspace whose view you want to share, then click a record type card. 

   This opens the record type page.

1. From the view tab, hover over the view you want to share and click the **More** menu ![](assets/more-menu.png) to the right of the view name, then click **Share**. 

   ![](assets/more-menu-for-views-expanded-with-share-option.png)

1. In the **Grant view access to** field, start typing the name of a user or a group, then click it when it displays in the list. 

    ![](assets/sharing-a-view-ui-with-groups.png)

1. Select one of the following permission levels from the drop-down menu: 
    * View
    * Manage

        For information about permission levels and what actions users can perform for each level, see [Overview of sharing permissions in Adobe Workfront planning capabilities](../access/sharing-permissions-overview.md).

        <!--System administrators always receive Manage permissions to views shared with them.--> 

1. Click **Copy link** to copy a link to the view to your clipboard. 
1. Share the copied link with others. Users who receive the link must be active users and log in to Workfront to be able to access the record type page and display it in the selected view. 
1. Click **Save**.

## Remove permissions to a view

{{step1-to-maestro}}

1. Open the workspace whose view you want to share, then click a record type card. This opens the record type page.
1. From the view drop-down menu, hover over the view you want to share and click the **More** menu ![](assets/more-menu.png) to the right of the view name, then click **Share**.
1. Find the user or group what you want to remove, then click **Remove** in the permissions drop-down menu to the right of the user's or group's name.
1. Click **Save**.
   The user or the users that belong to the group removed no longer have access to the view. There is no notificaiton for the users that that have been removed from accessing the view.
