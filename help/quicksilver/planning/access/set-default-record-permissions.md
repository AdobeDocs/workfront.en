---
title: Set Default Permissions for Records
description: You can set default permissions for records when you modify the record type or the workspace settings. You can give Open or Restricted permissions to all records that will be added for a record type. 
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
---

# Set default permissions for records 

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}


You can set default permissions for records when you modify the record type or the workspace settings. 

You can give Open or Restricted permissions to all records that will be added for a record type. 


## Access requirements

+++ Expand to view access requirements for the functionality in this article. 

<!--
at GA, check that the Workfront plans article linked below has Planning info
-->

 <table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Any Workfront or Workflow with a Planning package</p> 
Or
<p>Any Workfront Planning as a standalone product package</p> 

 </tr>
   
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Any</p> 
   <p><b>NOTE</b></p>
   <p>Only people with a Standard license can be granted Manage permissions to records. All other licenses can only have View permissions and the Manage option is dimmed for them.</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>  <p>Manage permissions to a workspace and a record type</p>  
   <p><b>IMPORTANT</b></p>
   <p>Only users with Manage permissions to a workspace can share a record</p></td> 
  </tr>
</tbody> 
</table> 

For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerations for setting default record permissions

Consider the following as you configure default record permissions:

* Only one default permission rule can be active per record type at a time.
* Changing the rule only affects records created after the change. Existing records keep their current permissions.
* System administrators and workspace managers always retain Manage access to every record, regardless of the rule.
* Once a record is created, its permissions can be changed independently in its sharing dialog without affecting the default rule.
* For global record types, each workspace (primary and secondary) can configure its own default rule, and new records take on the rule of the workspace they're created in.

## Configure default record permissions for a workspace

1. Go to a workspace > **More** menu ![More menu](assets/more-menu.png) > **Settings** > **Record types**.

    ![Workspace Record types settings area](assets/workspace-record-types-settings-area.png)

1. (Optional) Click inside the cell of a **Record type** to edit record type names.

1. In the **New record permission default** column, click the cell for the record type whose permissions you want to update.

1. Choose from the following options: 

    * **Open**: All workspace contributors can manage newly created record. This is the current default behavior for all existing and new record types. 
    * **Restricted**: Only the record creator and anyone you explicitly add can edit newly created records. Everyone else gets view-only access.

1. (Conditional) If you are changing the default permissions from **Restricted** to **Open**, click **Switch** in the **Switch to Open** box to confirm your choice. 
1. (Conditional) If you selected **Restricted**, add additional editors in the **Who can edit records** column. You can add users, groups, teams, roles, or companies.  

    >[!NOTE]
    >
    >* The record creator is always included and cannot be removed.
    >* You can only select entities that already have Contribute or Manage permissions to the record type.

    Changes are saved automatically. Once saved, the rule takes effect immediately and automatically applies to all records created for that record type going forward.

## Configure default record permissions for a record type

1. Go to a record type > **More** menu ![More menu](assets/more-menu.png) > **Settings** > **Record settings**.

    ![Record settings tab in the record type Settings area](assets/record-settings-tab-in-record-type-settings-area.png)

1. In the **Record permission type** field, click one of the following options: 

    * **Open**: All workspace contributors can manage newly created record. This is the current default behavior for all existing and new record types. 
    * **Restricted**: Only the record creator and anyone you explicitly add can edit newly created records. Everyone else gets view-only access.
1. (Conditional) If you are changing the default permissions from **Restricted** to **Open**, click **Switch** in the **Switch to Open** box to confirm your choice. 
1. (Conditional) If you selected **Restricted**, add additional editors in the **Who can edit records** field. You can add users, groups, teams, roles, or companies.  

    >[!NOTE]
    >
    >* The record creator is always included and cannot be removed.
    >* You can only select entities that already have Contribute or Manage permissions to the record type.

    Changes are saved automatically. Once saved, the rule takes effect immediately and automatically applies to all records created for that record type going forward.