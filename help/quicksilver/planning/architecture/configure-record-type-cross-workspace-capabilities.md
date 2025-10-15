---
title: Configure Cross-workspace Capabilities for Record Types
description: You can enable a record type to either be added to another workspace or be connected from another workspace in Adobe Workfront Planning. 
hidefromtoc: yes
hide: yes
exl-id: d36ab9fb-0275-483d-97be-0a88e170f8e0
---
<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

-->

<!--*******************REPLACE THE "ADVANCED SETTINGS" SECTION IN THE "EDIT RECORD TYPES" ARTICLE WITH A LINK TO THIS ARTICLE INSTEAD AND REMOVE THE STEPS FROM THE "EDIT RECORD TYPES" ARTICLE ON HOW TO ALLOW CROSS-WORKSPACE SETTINGS FOR RECORD TYPES*************-->


<!--this article is linked to the UI - do not delete or change the URL-->

<!--THIS MIGHT ALREADY BE ADDED TO THE "OVERVIEW" ARTICLE, BUT CHECK: add more info here about permissions, how users gain permissions from the original record type, per Lilit: users who add this to another space gain View permissions on that space when they add records to this added record type.

-->

# Configure cross-workspace capabilities for record types

{{planning-important-intro}}

<!--this is linked to the UI in the info icon when you enable a record to be either global or connectable-->

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

You can configure record types to work across multiple workspaces in Adobe Workfront Planning. 

You can designate a record type as one of the following: 

* **A global record type**: users can add global record types to other workspaces they can manage. 
* **A connectable record type**: users can connect to this record type from other workspaces. 

You must first define the cross-workspace capabilities of a record type before workspace managers can either add it to or connect it from other workspaces.

You define the cross-workspace capabilities of a record type when you create or edit a record type. 

For information, see one of the following articles: 

* [Create record types](/help/quicksilver/planning/architecture/create-record-types.md)
* [Edit record types](/help/quicksilver/planning/architecture/edit-record-types.md)

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
<p>To configure connectable record types: </p>
<ul> 
<li><p>Any Workfront package and any Planning package</p></li>
Or
<li><p>Workflow and Planning Prime and Ultimate packages</li></ul>

<p>To configure global record types:</p>

<ul> 
<li><p>Any Workfront package and a Planning Plus package</p></li>
Or
<li><p>Workflow and Planning Prime and Ultimate packages</li></ul>
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
<ul><li><p>A Workflow Prime or Ultimate package</p> </li>
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
</table> -- >

## Configure global record types

<!--this is a UI term; don't change the title of this section-->

As a workspace manager, you can configure a record type to be a global record type. A global record type can be added to other workspaces. 

A workspace manager can add a global record type to a workspace they manage. The record type's original fields are also added to the secondary workspace. 

Users can add records to a global record type from any workspace where they have Contribute permissions and where the global record type is added, including its original workspace. They can view records from workspaces they have only View permissions to.

For more information, see [Cross-workspace record types overview](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).

To configure a record type as global: 

{{step1-to-planning}}

1. Click the workspace whose record types you want to configure as global. 

   The workspace page opens and the record types display. 
1. Do one of the following:

   * Hover over the card of a record type and click the **More** menu ![More menu](assets/more-menu.png) in the upper-right corner of the record type card

      ![More menu options from record type card](assets/more-menu-options-from-record-type-card.png)

   * Click a record type card to open the record type page, then click the **More** menu ![More menu](assets/more-menu.png) to the right of the record type name.
1. Click **Edit** or **Settings**.

   >[!TIP]
   >
   >When a record types is added to another workspace, it displays as a global record type in that workspace. In this case, the Edit and Settings options are dimmed. 

1. (Conditional) If you clicked **Edit**, in the **Edit record type** box, click the **Cross-workspace settings** tab

   Or, if you clicked **Settings**, click the **Cross-workspace settings** section in the left panel.
1. Enable the **Allow adding this record type to other workspaces** setting.

   ![Edit record type Cross-workspace settings with Add to other workspaces enabled](assets/edit-record-type-advanced-settings-add-to-other-workspaces-enabled.png)

   >[!TIP]
   >
   >After you add a global record type to another workspace, this setting can no longer be disabled.

1. In the **Select who can add this record type to workspaces they manage** field, add entities that you want to allow to add this record type to workspaces they manage. 

   Your name is automatically added in the field. 

   You can add individual users, groups, teams, job roles, or companies whose users you want to allow to add this record type to the workspaces they manage. 
   
   You can edit this field, after you save the record type. 

1. (Optional) Remove your name from the **Select who can add this record type to workspaces they manage** field.

   >[!TIP]
   >
   >You must designate at least one entity (user, team, group, role, or company) to be able to enable this setting. 

1. (Conditional) Click **Save** in the **Edit record type** box, or click the back arrow to the left of **Settings** in the page header to save your changes.

   The following things occur:

      * The record type and its fields are now available to be added to another workspace by the people you designated. 

      >[!NOTE]
      >
      >You can edit the record type's appearance and settings and its original fields only from its original workspace. 
         
      * The record type card displays a **global record type** icon ![Global record type icon](assets/global-icon.png) to indicate that the record type is available to be added to other workspaces. 
      * A system-generated **Workspace** field is added to the table view of the record type and its records' details. 
      
         The Workspace field displays the workspace from where each record is created.
         
         This field is read-only and cannot be deleted.
1. (Optional) Go to another workspace and create a record type by using an existing record type. Select the record type you enabled in the steps above. 

   For information, see [Add existing record types from another workspace](/help/quicksilver/planning/architecture/add-existing-record-types-from-another-workspace.md). 

   The record type added from a global record type in the secondary workspace also displays a **global record type** icon ![Global record type icon](assets/global-icon.png). 
1. (Optional) Go back to the original workspace where you created the global record type and edit the record type by following steps 1-4 above <!--ensure this stays accurate-->
1. (Optional) Review the list of workspaces where the global record has been added in the **Workspaces where this record type is used section**. 

   ![Workspaces where this record type is used](assets/workspaces-where-this-record-type-is-used.png)


## Configure connectable record types

<!--this is a UI term; don't change the title of this section-->

You can configure a record type to be connected to from other workspaces when you create or edit the record type. 

To configure a record type as connectable: 

{{step1-to-planning}}

1. Click the workspace whose record types you want to configure as connectable. 

   The workspace page opens and the record types display. 
1. Do one of the following:

   * Hover over the card of a record type and click the **More** menu ![More menu](assets/more-menu.png) in the upper-right corner of the record type card

      ![More menu options from record type card](assets/more-menu-options-from-record-type-card.png)

   * Click a record type card to open the record type page, then click the **More** menu ![More menu](assets/more-menu.png) to the right of the record type name.
1. Click **Edit** or **Settings**.

1. (Conditional) If you clicked **Edit**, in the **Edit record type** box, click the **Cross-workspace settings** tab

   Or, if you clicked **Settings**, click the **Cross-workspace settings** section in the left panel.
   
1. Enable the **Allow connecting to this record type in other workspaces** setting. <!-- check the setting name, I sent this to Lilit to say FROM instead of IN-->

   <!-- add new screen shot with new tab name-->

   ![Edit record type Cross-workspace settings tab with connect from other workspaces enabled](assets/edit-record-type-advanced-settings-connect-from-other-workspaces-enabled.png)

   When enabled, the record type is accessible and can be connected to from other workspaces.

1. Choose from which workspaces the record type can be accessed. Choose from the following options:

   <!--check names of the setting: System wide?? OR All workspaces??-->

   * **All workspaces**: Users can connect to this record type from all workspaces where they have Manage permissions.
   * **Specific workspaces**: From the drop-down menu, add the names of the workspaces where workspace managers can connect to this record type.
1. (Conditional) Click **Save** in the **Edit record type** box, or click the back arrow to the left of **Settings** in the page header to save your changes.

   The following things occur:

      * The record type and its fields are now available to connect to from the workspaces you designated. 
      * The record type card displays a connectable record type icon ![Connectable record type icon](assets/connect-from-other-workspaces-icon.png) to indicate that the record type is available to be connected to from any workspace you designated in your configuration.

1. (Optional) Go to another workspace and add a connection to the record type you enabled for cross-workspace connectability in the steps above. 

   For information, see [Connect record types](/help/quicksilver/planning/architecture/connect-record-types.md). 









