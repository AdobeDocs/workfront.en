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

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

As a workspace manager, you can add a record type that exists in a workspace to a workspace that you manage in Adobe Workfront Planning. 

You must first designate a record type as a centralized before workspace managers can add it into other workspaces as an existing record type.

You can designate a record type as centralized when you create or edit it, as you are defining its cross-workspace settings. 

For information, see [Configure cross-workspace capabilities for record types](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md). 

Before adding records to a workspace from a cenralized record type, see the article [Cross-workspace record types overview](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md). 

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
<ul><li><p>Any Workfront package</p></li>
And
<li><p>Planning Plus package</p></li></ul>
<!--Or:
<ul><li><p>Any Workflow package</p> </li>
And
<li><p>Planning Prime or Ultimate package</p></li></ul>-->
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account manager. </p> 
   </td> 

  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr>  
</tbody> 
</table> 

For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Create a record type from an existing record type

1. Start creating a record type, as described in the article [Create record types](/help/quicksilver/planning/architecture/create-record-types.md), then click **Add existing**. <!--check this - the option might have been renamed in the UI-->

   ![Modal to add record type with option to add from another workspace](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

1. Click **Continue**.
1. In the **Choose record type** box, click the card for the record type that you want to add from an existing workspace, then click **Add**.

   The record type is added to the workspace you selected. 
   
   >[!TIP]
   >
   >When there are no record types configured to be added to another workspace, the option to add them from another workspace does not display, when creating a record type.
   
   The following things occur:

   * The following information is also added from the existing centralized record type:

      * All original fields
      * All record connections
   * You can view records added from other workspaces, only when you have at least View permissions to those workspaces. 
   * The **centralized record type** icon ![Centralized record type icon](assets/global-icon.png) is added to the card of the new record type.
   * The read-only **Workspace** field is added to the new record type table view. The field displays what workspace each record was created in. 
   
      >[!NOTE]
      >
      >* You cannot edit the new record type's appearance, advanced settings, or original fields. You can edit the record type and all its original fields and settings only from the original workspace.

1. (Optional) Click, then drag and drop the newly added record type to any section within the workspace. 

<!--This will be released later with another epic: 1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) in the new record type's card, or to the right of the record type's name on its page, then click **Share** to share it with other users in the same workspace, or adjust their permissions to the record type.-->

1. (Optional) Click on the **More** menu ![More menu](assets/more-menu.png) in the new record type's card, or to the right of the record type's name on its page, then click **Delete**.
1. (Conditional) Type **delete** in the field provided, then click **Permanently delete**.

   The following things occur: 

   * The record type created from a centralized record type is removed from the selected workspace. 
   * The original record type and its fields remain in their original workspace. 
   * The record type remains in all other workspaces where it's been added.
   * The records added to the record type from the current workspace are deleted. All other records added from additional workspaces where the centralized record type was added are preserved. 


   


