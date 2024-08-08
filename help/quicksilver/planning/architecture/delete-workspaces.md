---
title: Delete workspaces
description: You can delete workspaces when they are no longer relevant.
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
---
<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Delete workspaces

{{planning-important-intro}}

In Adobe Workfront Planning, workspaces are centralized locations for teams to plan work. For more information, see [Create workspaces](/help/quicksilver/planning/architecture/create-workspaces.md). 

You can delete workspaces that are no longer relevant. 

We recommend recreating some or all of the record types, records, fields, and views associated with the workspace that you want to delete in another workspace before deleting it.

## Access requirements

+++ Expand to view access requirements for Workfront Planning. 

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
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>  
</td>
  </tr>

  <tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
    
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For more information about access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

+++

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Considerations about deleting workspaces

* When you delete workspaces, all the record types, records, their fields, and views are also deleted. 
* Deleted workspaces and the information they contain cannot be recovered. 

## Delete a workspace

{{step1-to-planning}}

1. (Conditional) If you are a Workfront administrator, click **My workspaces** to access workspaces you created, or **Other workspaces** to access workspaces others shared with you. <!--change it to Workspaces I'm on-->

1. Click the card of the workspace you want to delete.

   The workspace page displays. 

<!--***********Replace the first step with this:*******

1. (Optional) Click **Show more** to display additional workspaces. The **Show more** link displays only when you have workspaces that display on more than two rows.
1. (Optional) ClicK **Show less** to limit the number of workspaces that display on the screen. 
1. To delete a workspace, do one of the following:

   * Hover over the workspace card, then click the **More** menu ![](assets/more-menu.png) in the upper-right corner of the card, then click **De,ete**. 
   * Click a workspace card to open the workspace. 
   
   ***********Add (Conditional) If you clicked a workspace card,******to the step below****-->

1. Click the **More** menu ![](assets/more-menu.png) next to the workspace name, then click **Delete**.

   ![](assets/permanently-delete-workspace-confirmation.png)
   
1. Type "**delete**" in the space provided, then click **Permanently delete**. This is not case sensitive. 

    The workspace is deleted and cannot be recovered. Any record types, records, fields, and views associated with them are also deleted. <!--ensure this is right at or before GA-->
