---
title: Create Workspaces
description: A workspace is a collection of record types used by a team and represents the team's work lifecycle. You can fully customize workspaces in Adobe Workfront Planning. Record types are organized by sections in a workspace. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
---
<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Create workspaces

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

In Adobe Workfront Planning, workspaces are centralized locations for teams to plan work. 

A workspace is a collection of record types used by a team and represents the team's work lifecycle. You can fully customize workspaces in Adobe Workfront Planning. 

For general information about workspaces, see [Workspaces overview](/help/quicksilver/planning/architecture/workspaces-overview.md). 

## Access requirements

+++ Expand to view access requirements. 

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
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>You receive Manage permissions to the workspaces you create. </p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Layout template</p></td> 
   <td> <p>In the Production environment, all users including the System Administrators must be assigned to a layout template that includes Planning.</p>
<p><span class="preview">In the Preview environment, Standard users and System Administrators have Planning enabled by default.</span></p></td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Create a workspace

You can create a workspace and add record types to it to organize your objects in Workfront Planning. For more informaton about editing a workspace, see [Edit workspaces](/help/quicksilver/planning/architecture/edit-workspaces.md).

{{step1-to-planning}}

1. Click **Create workspace**

   The Create workspace box displays. You can create a workspace from scratch or create it using one of the available templates.  
    
1. (Optional and conditional) Click **Preview** inside any of the following predefined workspace templates:

    * Basic: Marketing Management
    * Advanced: Marketing Management
    * Enterprise: Marketing Management
    * Sales management
    * Product management
    
    The template preview box opens. 
    
    There is an indication of what operational record types, taxonomies and how many fields are associated with each template.

    ![Previewing a workspace template](assets/previewing-a-workspace-template.png)

    For information about Workfront Planning workspace templates, see [List of workspace templates](/help/quicksilver/planning/architecture/workspace-templates.md).

1. From the template preview box, click **Use template** to start creating the workspace from the selected template

    Or

    Click **Back**, then click **New workspace** to create a workspace from scratch.

    One for the following types of workspaces is created:
    
    * An empty workspace named **Untitled Workspace** where you can start adding record types manually, when you create a workspace from scratch. 
    * A workspace named after the template you selected that is populated with sample record types. You can further customize the record types and the workspace.
     
   For Workfront administrators, the new workspace displays on the **Workspaces I'm on** tab.

   For all other users who can create workspaces, the new workspace displays in the **Workspaces** area.

1. Click inside the name of the workspace in the header of the new workspace to rename it, then press Enter. 

1. (Optional and conditional) If you created the workspace from a template, click inside the name of the **Operational Record Types** or **Taxonomies** sections 

   Or 

   Hover the name of a section, then click the **More** menu ![More menu](assets/more-menu.png), then click **Rename** to rename the section. 

      >[!TIP]
      >
      >You can rename any section from any workspace, even if you didn't create the section. 

   For more information about editing workspaces, including editing workspace sections, see [Edit workspaces](/help/quicksilver/planning/architecture/edit-workspaces.md). 

1. (Optional) Click **Add record type** to add record types to the workspace in any section.
    
   For information, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md).

   For more information about editing and deleting record types in a workspace, see [Edit workspaces](/help/quicksilver/planning/architecture/edit-workspaces.md).


