---
title: Edit Workspaces
description: You can edit the information of an existing workspace, like rename it.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 374b6d9c-69a9-4a73-8708-51c14a78c7c9
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/krlFOQ-FeaEJt6oJgGp6FuE-6OaOxeW7sz48WmmuRbE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
    internal-label: Get started
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Edit workspaces


<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>



{{planning-important-intro}}

In Adobe Workfront Planning, workspaces are centralized locations for teams to plan work. 

A workspace is a collection of record types used by a team and represents the team's work lifecycle. You can fully customize workspaces in Adobe Workfront Planning. 

For information about creating workspaces, see [Create workspaces](/help/quicksilver/planning/architecture/create-workspaces.md). 

All changes you make to a workspace are visible to all those who have at least View permissions to the workspace.

You can edit a workspace in the following ways: 

* Manually. 

   This article describes how you can manually edit a workspace. 

* Using the AI-powered Planning Designer. This capability is currently available only in a limited Beta program. 

   For information, see [Get started with the Adobe Workfront Planning Designer](/help/quicksilver/planning/general/planning-ai-designer.md).

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
<ul> 
<li><p>Any Workfront and any Planning package</p></li>
Or
<li><p>Any Workflow and any Planning package</p></li></ul>
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

<!--
Old:
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
   <td>  <p>Manage permissions to the workspace </p>   </td> 
  </tr> 
</tbody> 
</table>
-->

## Edit a workspace

{{step1-to-planning}}
    
1. (Conditional) If you are a Workfront administrator, click one of the following:

   * **Workspaces I'm on** to access workspaces you created
   * **All workspaces** to access workspaces shared with you or workspaces you created

   >[!NOTE]
   >
   ><span class="preview">You cannot edit the workspaces on the **Sample workspaces** tab. We recommend using the multi-workspace template bundle to create workspaces similar to those on the Sample workspace tab and edit your own. For information, see [Create workspaces](/help/quicksilver/planning/architecture/create-workspaces.md).</span> 
  
1. (Optional) Click **Show all** to display additional workspaces. The **Show all** link displays only when you have more than two rows of workspace cards.
1. (Optional) ClicK **Show less** to limit the number of workspaces that display on the screen. 
1. To edit a workspace, do one of the following:

   * Hover over the workspace card, then click the **More** menu ![More menu](assets/more-menu.png) in the upper-right corner of the card
      Or 
   * Click the **search** icon ![Search icon](assets/search-icon.png) in the upper-right corner of the Workspaces page to search for a workspace by name and click a workspace card to open the workspace, then click the **More** menu ![More menu](assets/more-menu.png) to the right of the workspace name. 

   >[!TIP]
   >
   >You can use the following keyboard combination to open the global search box from any Workfront Planning page and search for workspaces :
   >
   >* CTRL+K for Windows  
   >* ⌘+K for Mac 
   >
   >![Global search box](assets/global-search-box.png)
   
1. Click **Edit**.

   The **Edit workspace** box displays.

   ![Edit workspace box](assets/edit-workspace-box.png)

1. Update the following information in the **Edit workspace** box:

   * Add a name for the workspace. <!--did they add a label for this field?-->
   * **Description**: Add information about the workspace. 
   * Select an icon to associate with the workspace. 

1. Click **Save** to close the Edit workspace box and apply your changes.

1. (Optional) To add a new workspace section, do one of the following:

   * Click **Add section** at the bottom of the workspace.
   * Hover over the name of a section and click the **More** menu ![More menu](assets/more-menu.png), then click **Add section above** or **Add section below**.  

1. (Optional) To change the location of a section, do one of the following:

   * Hover over the name of a section and click the **grab** icon ![Grab icon](assets/grab-icon.png), then drag and drop it in the right spot. 
   * Hover over the name of a section and click the **More** menu ![More menu](assets/more-menu.png), then click **Move up** or **Move down**. The section moves up or down inside the workspace. 

1. (Optional) To delete a workspace section, do the following: 
   
   1. Hover over the name of a section, then click the **More** menu ![More menu](assets/more-menu.png), then click **Delete**. <!--add screen shot when UI is final?-->
   1. Select a new section to move all record types to it, then click **Delete**. <!--check the button name; logged a bug to change it to "Delete" from "Delete section".-->

      All record types are moved to the selection section, and the section is deleted. 

1. (Optional) Click **Add record type** to add record types to the workspace.
    
    For information, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md).

1. (Optional) Hover over a record type card, click the **More** menu ![More menu](assets/more-menu.png) in the upper-right corner, then click **Edit** to modify the appearance of a record type. 

   For information, see [Edit record types](/help/quicksilver/planning/architecture/edit-record-types.md). 

1. (Optional) Hover over a record type card, click the **More** menu ![More menu](assets/more-menu.png) in the upper-right corner, then click **Delete** to delete a record type. 

   For information, see [Delete record types](/help/quicksilver/planning/architecture/delete-record-types.md).

1. (Optional) Press-click a record type card to drag it and drop it in a new spot. You can drag and drop record types from one workspace section to another. 

   ![Drag and drop record types in a workspace](assets/drag-and-drop-record-types-in-a-workspace.png)

1. (Optional) Click **Share** in the upper-right corner of the workspace to share the workspace with others.

    For information, see [Share workspaces](/help/quicksilver/planning/access/share-workspaces.md).
