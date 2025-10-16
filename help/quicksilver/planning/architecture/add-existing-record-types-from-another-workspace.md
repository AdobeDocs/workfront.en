---
title: Add Existing Record Types from Another Workspace
description: Record types are the object types of Adobe Workfront Planning. In Workfront Planning, you can add an existing record type created in another workspace.
hidefromtoc: yes
hide: yes
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
---
<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Add existing record types from another workspace

{{planning-important-intro}}

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

As a workspace manager, you can add a record type that exists in another workspace to a workspace that you manage in Adobe Workfront Planning. 

A workspace manager must first designate a record type as a global record type before you can add it into workspaces you manage as an existing record type. Workspace managers can designate a record type as global when they create or edit them, by defining the record type's cross-workspace settings.

   For information, see [Configure cross-workspace capabilities for record types](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md). 

This article describes how you can add a record type from an existing one.  

Before adding records to a workspace from a global record type, also see the article [Cross-workspace record types overview](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md). 


## Access requirements

+++ Expand to view the access requirements for the functionality in this article.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<ul><li><p>Any Workfront package and a Planning Plus package</p></li>
<p>Or</p>
<li><p>Workflow and Planning Prime and Ultimate packages</p></p></li></ul>
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account representative. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr>  
</tbody> 
</table> 

For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 

  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<ul><li><p>Any Workfront package</p></li>
<p>And</p>
<li><p>Any Planning package to create connectable record types</p></li>
<li><p>A Planning Plus package to create global record types</p></li>
</ul>
Or:
<ul><li><p>A Prime or Ultimate Workflow package</p> </li>
And
<li><p>A Planning Prime or Ultimate package</p></li></ul>
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account manager. </p> 
   </td> 

  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and to the record type</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr>  
</tbody> 
</table>-->

## Create a record type by adding an existing one from another workspace

>[!NOTE]
>
>Ensure there is at least one record type designated to be global in at least one other workspace.

1. Start creating a record type, as described in the article [Create record types](/help/quicksilver/planning/architecture/create-record-types.md), then click **Add existing**. <!--check this - the option might have been renamed in the UI-->

   ![Modal to add record type with option to add from another workspace](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

   >[!TIP]
   >
   >When there are no record types configured to be added to other workspaces in your system, the **Add existing** option does not display.

1. Click **Continue**.
1. In the **Choose the record type** box, click the card for the record type that you want to add from an existing workspace, then click **Add**.

   The record type is added to the workspace you selected and the **global record type** icon ![](assets/global-icon.png) displays on the record type's card. 
    
   The following things occur:

   * The following information is also added from the existing global record type:

      * All original fields
      * All record connections
   * You can view records added from other workspaces that use the same global record type, only when you have at least View permissions to those workspaces. 
   * The read-only **Workspace** field is added to the new record type table view. The field displays the workspace where each record was created. 
   
      >[!NOTE]
      >
      >You cannot edit the new record type's appearance, additional settings, or original fields. You can edit the record type and all its original fields and settings only from the original workspace.

1. (Optional) Click, then drag and drop the newly added record type to any section within the workspace. 
1. (Optional) Click the **More** menu on the new record type's card or to the right of the record type name on its page, then click **Delete**.

   For more information, see the section "Delete global record types" in the article [Delete record types](/help/quicksilver/planning/architecture/delete-record-types.md).

<!--This will be released later with another epic: 
1. In the table view, click the **+** icon in the upper-right corner to add new fields. For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md).
1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) in the new record type's card, or to the right of the record type's name on its page, then click **Share** to share it with other users in the same workspace, or adjust their permissions to the record type.
-->

<!--checking with Lilit if we can add automations or request forms to secondary global RTs??--add step with links to those articles if/ when yes-->




   


