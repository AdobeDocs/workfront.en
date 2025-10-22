---
title: Edit Record Types
description: You can edit record types after they have been saved. Record types are the object types of Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
---

# Edit record types

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Record types are the object types of Adobe Workfront Planning. You can edit the appearance of record types that you or anyone else created. For information about creating Workfront Planning record types, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md). 

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
<p>Any Workfront and Planning package</p>
<p>Any Workfront and Planning package</p>
<p><b>NOTE</b></p>
<p>To configure connectable record types: </p>
<ul> 
<li><p>Any Workfront package and any Planning package</p></li>
<p>Or</p>
<li><p>Any Workflow and a Planning Prime or Ultimate package</p></li></ul>

<div class="preview">
<p>To configure global record types:</p>

<ul> 
<li><p>Any Workfront package and a Planning Plus package</p></li>
<p>Or</p>
<li><p>Any Workflow and a Planning Prime or Ultimate package</p></li></ul>
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account representative. </p> 

</div>
   </td> </tr>
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
   <td>   <p>Manage permissions to a workspace and record type </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Only system administrators can enable record types to connect from other workspaces</p> </td> 
  </tr> 

</tbody> 
</table> -->

## Edit record types

{{step1-to-planning}}

1. Click the workspace whose record types you want to edit. 

   The workspace page opens and the record types display. 
1. Do one of the following:

   * Hover over the card of a record type and click the **More** menu ![More menu](assets/more-menu.png) in the upper-right corner of the record type card, then click **Edit** 
   <span class="preview">or **Settings**</span>
      Or
   * Click a record type card to open the record type page, click the **More** menu ![More menu](assets/more-menu.png) to the right of the record type name, then click **Edit** <span class="preview">or **Settings**</span>. 

   <span class="preview">![More menu options from record type card with Settings](assets/more-menu-options-from-record-type-card-with-settings-link.png)</span>

1. In the **Edit record type** box, the **Appearance** tab opens by default. <!--update screen shot below at production-->

   ![Edit record type box appearance tab ](assets/edit-record-type-box-appearance-tab.png) 

   Update the following information in the **Appearance** tab: 

    * Edit the record type name, if needed. <!--did they add a field label for this?-->
    * **Description**: Edit or add a description for the record type with more information about it. 
    * Edit the color and shape of the icon associated with the record type. Do the following: 
        * Select a color to identify the record type. This is the color of the record type icon. 
        * Select an icon from the list, or start typing the name of an icon to describe what it represents, then select it when it displays. This is the icon of the record type. A file icon is selected by default.

1. (Optional and conditional) If you are a system administrator, click the **Advanced settings** <span class="preview">or **Cross-workspace settings**</span> tab and update information about the cross-workspace capabilities of the record type. 

   For more information, see [Configure cross-workspace capabilities for record types](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md). <!--update screen shot at production - Jan 2026-->

   ![Edit record type box with advanced settings tab](assets/edit-record-type-box-advanced-settings-tab.png)

1. Click **Save**.

   If you selected to connect this record from other workspaces, the **Connectable record** icon ![Connect from other spaces icon](assets/connect-from-other-workspaces-icon.png) displays on the record card. 

    <span class="preview">If you selected to allow adding this record to other workspaces, the **Global record** icon ![Global record type icon](assets/global-icon.png) displays on the record card. </span>

1. (Optional) Click the record type card from the workspace area to open the record type's page, then rename the record type in the header.  

1. (Optional) To edit another record type, from the record type page, expand the downward-pointing arrow to the right of a record type name, search for a record type, then select it when it displays in the list.

   ![Record type drop-down on record type page with search box](assets/record-type-drop-down-on-record-type-page-with-search-box.png)
