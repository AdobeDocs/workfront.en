---
title: Configure Cross-workspace Capabilities for Record Type
description: You can enable a record type to either be added to another workspace or be connected from another workspace. 
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

<!--*******************THIS TITLE MIGHT NEED TO CHANGE WHEN WE HAVE THE FINAL NAME FOR THE "GLOBAL" RECORD TYPE - NOT SURE IF WE ARE GOING TO USE "GLOBAL" OR "DYNAMIC", OR ???? ***************; also update TOC file, the miniTOC,  etc when this is finalized-->



<!--this article is linked to the UI - do not delete or change the URL-->
<!--add more info here about permissions, how users gain permissions from the original record type, per Lilit: users who add this to another space gain View permissions on that space when they add records to this imported record type - this info is in the UI - this is what she sent in figma:

Hey, Alina, Lusine. As this page contains not only the "global record types" but also cross-workspace connectivity setting, we shouldn't have this message that's highlighting only the global rt features. I think we should have explanation for each setting both in enabled and disabled states. 

So we'd have the "Allow adding this record type to other workspaces" setting in enabled or disabled state, and display an explanation text below it explaining the capability, as well as a link to help articles for more context. I'd like to include the following key points in the message:  

Once enabled, this record type can be added in other workspaces by designated people 

Members of those workspaces can create and manage records in scope of their workspace 

Any records added by other workspace members will be rolled up to this workspace with view access so members of the current workspace can create views for cross-workspace records.  

Then for the second setting for cross-workspace connections, we'll need a similar explanation text would highlight that the other workspaces can create connections and gain view access to the records in this record type, but will not see the record type in their workspace. (not sure what she means by this last bit, asking in figma also)

-->

# Configure cross-workspace capabilities for record types

<!--this is linked to the UI in the info icon of when you create a record type from a global record type-->

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

The following are cross-workspace capabilities of record types:

* You can designate a record type as centralized. Users can add centralized record types to other workspaces they can manage. 
* You can designate a record type as a connectable. Users can connect to this record type from other workspaces. 

You must first define the cross-workspace capabilities of a record type before workspace managers can either connect it from or import it into other workspaces.

You define the cross-workspace capabilities of a record type when you create or edit a record type. 

For information, see one of the following articles: 

* [Create record types](/help/quicksilver/planning/architecture/create-record-types.md)
* [Edit record types](/help/quicksilver/planning/architecture/edit-record-types.md)

## Access requirements

+++ Expand to view access requirements.  

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
   <td><p> Standard</p>
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
   <td>   <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Configure adding a record type to other workspaces

As a workspace manager, you can configure a record type to be added to other workspaces when you create or edit a record type. 

When you configure adding a record type to other workspaces, a workspace manager can import the record type and all its information to one of the workspaces they manage.

To configure adding a record type to another workspace when you edit the record type:  

{{step1-to-planning}}

1. Click the workspace whose record types you want to edit. 

   The workspace page opens and the record types display. 
1. Do one of the following:

   * Hover over the card of a record type and click the **More** menu ![More menu](assets/more-menu.png) in the upper-right corner of the record type card
      Or
   * Click a record type card to open the record type page, then click the **More** menu ![More menu](assets/more-menu.png) to the right of the record type name.
1. Click **Edit**.

   ![More menu options from record type card](assets/more-menu-options-from-record-type-card.png)

1. In the **Edit record type** box, select the **Advanced settings** tab.
1. Enable the **Allow adding this record type to other workspaces** setting.

   ![Edit record type Advanced settings with Add to other workspaces enables](assets/edit-record-type-advanced-settings-add-to-other-workspaces-enabled.png)

1. In the **Select who can add this record type to workspaces they manage** field, add users that you want to allow to add this record type to workspaces they manage. 

   Your name is automatically added in the field. 

   You can add individual users, or groups, teams, job roles, or companies whose users you want to allow to add this record type to the workspaces they manage. 
   
   You can edit this field, after you save the record type. 
1. (Optional) Remove your name from the **Select who can add this record type to workspaces they manage** field.

1. Click **Save**.

   The following things occur:

      * The record type and its fields are now available to be added to another workspace by the people you designated. 

      >[!NOTE]
      >
      >You can edit the record type and its fields only from the original workspace. 
         
      * The record type card displays a global icon ![Global record type icon](assets/global-icon.png) to indicate that the record type is available to be added to any  workspace whose manager you designated in your configuration. 
      * A system-generated **Workspace** field is added to the record type. 
      
         The Workspace field displays the workspace from where each record has been created.
         
         This field is read-only and cannot be deleted.

## Configure connecting to a record type from other workspaces

You can configure a record type to be connected to from from other workspaces when you create or edit the record type. 

To configure a record type to connect to from other workspaces when you edit the record type:  

{{step1-to-planning}}

1. Click the workspace whose record types you want to edit, 

   The workspace page opens and the record types display. 
1. Do one of the following:

   * Hover over the card of a record type and click the **More** menu ![More menu](assets/more-menu.png) in the upper-right corner of the record type card, then click **Edit**
      Or
   * Click a record type card to open the record type page, click the **More** menu ![More menu](assets/more-menu.png) to the right of the record type name, then click **Edit**. 

   ![More menu options from record type card](assets/more-menu-options-from-record-type-card.png)

1. In the **Edit record type** box, select the **Advanced settings** tab.
1. Enable the **Allow connecting to this record type in other workspaces** setting. <!-- check the setting name, I sent this to Lilit to say FROM instead of IN-->

   ![Edit record type Advanced settings tab with connect from other workspaces enabled](assets/edit-record-type-advanced-settings-connect-from-other-workspaces-enabled.png)

   When enabled, the record type is accessible and can be connected from other workspaces.

1. Choose from which workspaces the record type can be accessed. Choose from the following options:

   * **System wide**: Users can connect to this record type from all workspaces where they have manage permissions.
   * **Specific workspaces**: Add the names of the workspaces where workspace managers can connect to this record type.
1. Click **Edit**.

   The following things occur:

      * The record type and its fields are now available to connect from the workspaces you designated. 
      * The record type card displays a cross-workspace connection icon ![Cross-workspace connection icon](assets/connect-from-other-workspaces-icon.png) to indicate that the record type is available to be connected from any workspace you designated in your configuration.

   The record type becomes available to connect from the designated workspaces. 









