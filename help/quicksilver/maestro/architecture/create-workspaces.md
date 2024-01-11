---
title: Create workspaces
description: A workspace is a collection of operational record types and taxonomies used by a team and represents the team's work lifecycle. You can fully customize workspaces in Maestro.
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
---
<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Create workspaces

>[!IMPORTANT]
>
>The information in this article refers to Adobe Maestro which is a new offering from Adobe Workfront. 
>
>Currently, Adobe Maestro is part of a beta program which is open to a limited number of customers. You must be a Workfront customer to use Maestro capabilities.
>
>Contact your account representative for more information about joining the beta program for Maestro.
>
>For information, see [Adobe Maestro overview](../maestro-overview.md).

In Adobe Maestro, workspaces are centralized locations for teams to plan work. 

A workspace is a collection of operational record types and taxonomies used by a team and represents the team's work lifecycle. You can fully customize workspaces in Maestro. 

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
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   <p>Current: Work or higher</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls for Maestro</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>You receive Manage permissions to the workspaces you create. </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>You must add the Maestro area to your layout template. For information, see <a href="../access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

For more information about access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>--> 

## Considerations about workspaces

* You can create workspaces for specific organizational units within your organization, to match the unique way each unit works. 
* The record types and taxonomies that a workspace contains should reflect the work lifecycle of an organizational unit. 
* When you create a workspace, only you have the permission to access and manage your workspace. You must share it with other users in order for them to collaborate with you in the same space. For information, see [Share a workspace](/help/quicksilver/maestro/access/share-workspaces.md). 
* You can have a maximum of 1,000 workspaces in your organization. 
* Workspaces contain record types that are unique to each workspace. <!--this might change-->

## Create a workspace

{{step1-to-maestro}}

1. (Conditional) If you don't have any workspaces in your environment, click **Create workspace**

   Or, from an existing workspace, click the downward-pointing to the right of the workspace name, then click **Create workspace**. 

   ![](assets/workspace-drop-down-right-menu.png)

   This opens the Workspaces area of Maestro. 
1. (Optional and conditional) Click **Preview** inside any of the following predefined workspace templates:

    * Marketing management
    * Sales management
    * Product management
    
    There is an indication of what operational record types, taxonomies and how many fields are associated with each template.

    ![](assets/previewing-a-workspace-template.png)

    For information about Maestro workspace templates, see [List of workspace templates](../architecture/workspace-templates.md).

1. Click **Use template** to start creating the workspace from the selected template

    Or

    Click **Create workspace** to create a workspace from scratch.

    One for the following types of workspaces is created:
    
    * An empty workspace where you can start adding record types manually. 
    * A workspace populated with sample record types which you can further customize. 
     
1. Click inside the name of the workspace in the header of the new workspace to rename it, then press Enter

    Or
    
    Click the **More** menu ![](assets/more-menu.png)to the right of the workspace name in the header, then click **Rename**.

1. (Optional) Click **Add record type** to add record types to the workspace.
    
    For information, see [Create record types](../architecture/create-record-types.md).

1. (Optional) Click **Add taxonomy** to add taxonomies to the workspace. 

    For information, see [Create taxonomies](../architecture/create-a-taxonomy.md).
