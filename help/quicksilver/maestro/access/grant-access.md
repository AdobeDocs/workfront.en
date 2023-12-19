---
title: Grant access to Adobe Maestro
description: Learn how to grant access and share information in Adobe Maestro.
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
exl-id: 475a519d-d3bd-4461-8099-0e296d556d34
---
<!--update the metadata and description when we turn this article live; also, update title after Bob adds Maestro as a product-->

# Grant access to Adobe Maestro

>[!IMPORTANT]
>
>The information in this article refers to Adobe Maestro which is a new offering from Adobe Workfront. 
>
>Currently, Adobe Maestro is part of a beta program which is open to a limited number of customers. You must be a Workfront customer to have access to Maestro
>
>Contact your account representative for more information about joining the beta program for Maestro.
>
>For information, see [Adobe Maestro overview](../maestro-overview.md).  

All users in your organization can have access to Maestro, if the following prerequisites are in place:

<!--the first requisite will be removed when we go to GA-->

* Your organization is enrolled in the Adobe Maestro closed beta program. 
* As a system administrator, you must add the Maestro area to the Main Menu using a layout template. 

    Maestro does not display in the Main Menu by default for any user, including system administrators. 

    For information, see [Customize the Main Menu using a layout template](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md). 

<!-- take out the note below when we release permissions-->

>[!NOTE]
>
>There are no access levels or permissions associated with users or the information in Maestro. All users that have Maestro enabled in their environment can view, edit, and delete all the information any other user adds to Maestro. 

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
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
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
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any to uses Maestro</p>
   <p>System administrator or Plan to share the Maestro area in a Layout Template</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area to your layout template. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
When permissions is released:

* leave as is for Access levels (I think)
* Add a new row for Permissions: System admin or Manage access to the workspace to share a workspace with others
-->

## Share the Maestro area in the Main Menu with others

<!--First, contact your account manager to obtain access to the current Maestro closed beta program.--> 

After your organization has been enrolled in the Maestro beta program, you can add the Maestro area to the Main Menu of all users by using a layout template. 

1. Log in to **Workfront** as a Workfront administrator.  

1. Add the **Maestro** icon ![](assets/maestro-icon.png) to the **Main Menu** using a **Layout Template**. 
    
    For information, see [Customize the Main Menu using a layout template](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).

1. Assign the layout template to the users that you want to have access to Maestro. 

    For information, see [Assign users to a layout template](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

    All users assigned to the template can now access Maestro in their Main Menu. 
    
    Users can start creating workspaces, records types, records, and fields.

<!--

## Share permissions to a workspace

The following users can share a workspace with other users:

* System administrators can share all workspaces, including the ones that they did not create.
* All other users can share only workspaces for which they have Manage permissions to. 

To share a workspace with others: 

1. Click the **Main Menu** icon ![](assets/dots-main-menu.png) in the upper-right or the **Main Menu** icon ![](assets/lines-main-menu.png) in the upper-left corner or Workfront, if available, then click **Maestro**.
1. Open the workspace you want to share, then click **Share** in the upper-right corner of the screen. (*************add screen shot when UI is finalized and maybe edit the steps*********)
1. In the field provided, start typing the name of a user or a group (******ensure you can share with groups*******), then click it when it displays in the list. 
1. Select one of the following permission levels from the drop-down menu: 
    * View
    * Contribute
    * Manage

        For information about permission levels and what actions users can perform for each level, see [Overview of sharing permissions in Adobe Maestro](../access/sharing-permissions-overview.md).
1. Click **Save**.


## Remove permissions to a workspace

1. Click the **Main Menu** icon ![](assets/dots-main-menu.png) in the upper-right or the **Main Menu** icon ![](assets/lines-main-menu.png) in the upper-left corner of Workfront, if available, then click **Maestro**.
1. Open the workspace you want to remove permissions to, then click **Share** in the upper-right corner of the screen. (********add screen shot when UI is finalized and maybe edit the steps???****)
1. Click the drop-down menu to the right of a user or group name, then click **Remove**. 
1. Click **Save**.

    The user or the users that belong to the group removed no longer have access to the workspace or its objects. 

-->