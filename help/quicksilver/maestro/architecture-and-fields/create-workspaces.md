---
title: Create workspaces
description: Create custom workspaces to match how your organizations work.
hidefromtoc: yes
hide: yes
---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Create workspaces

In Adobe Maestro, workspaces are centralized locations for teams to plan work. 

A workspace is a collection of operational record types and taxonomies used by a team and represents the team's work lifecycle. 

## Access requirements

You must have the following to perform the steps described in this article: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan*</p></td>
   <td>
<p>Any</p>
<!--the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>Any</p> 
  <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Product</p></td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">Layout template</td>
   <td> <p>Your system administrator must add the Maestro area in your layout template. For information, see the "Enable Maestro for the users in your Workfront instance" section in the article <a href="../maestro/maestro-overview.md">Adobe Maestro overview</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>*If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## Considerations about workspaces

* You can create workspaces for specific organizational units within your organization, to match the unique way each unit works. 
* The record types and taxonomies that a workspace contains should reflect the work lifecycle of an organizational unit. 
* When you create a workspace, everyone in your organization can view, edit, or delete it.  <!--this will change with access levels and permissions-->
* You can have a maximum of 1,000 workspaces in your organization. 

## Create a workspace

1. (Conditional) If you don't have any workspaces in your system, click the **Main Menu** icon ![](assets/main-menu-workfront.png) in the upper-right corner of Workfront, <!--or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> then click **Maestro** ![](assets/maestro-icon.png).

    Or, from an existing workspace, click the downward-pointing to the right of the workspace name, then click **Create workspace**. 

    ![](assets/workspace-drop-down-right-menu.png)

    This opens the Workspaces area of Maestro. 
1. (Optional and conditional) Click **Preview** inside any of the following predefined workspace templates:

    * Marketing management
    * Sales management
    * Product management
    
    There is an indication of what operational record types, taxonomies and how many fields are associated with each template.

    ![](assets/previewing-a-workspace-template.png)

    For information about the templates available in Maestro, see [List of available workspace templates](../architecture-and-fields/workspace-templates.md).

1. Click **Use template** to start creating the workspace from the selected template

    Or

    Click **Create workspace** to create a workspace from scratch
     
1. Click inside the name of the workspace in the header of the new workspace to rename it, then press Enter

    Or
    
    Click the **More** menu ![](assets/more-menu.png)to the right of the workspace name in the header, then click **Rename**.

1. (Optional) Click **Add record type** to add record types to the workspace.
    
    For information, see [Create record types](../maestro/delete-record-types.md).

1. (Optional) Click **Add taxonomy** to add taxonomies to the workspace. 

    For information, see [Create taxonomies](../architecture-and-fields/create-a-taxonomy.md) 