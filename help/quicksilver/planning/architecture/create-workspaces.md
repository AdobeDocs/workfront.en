---
title: Create Workspaces
description: A workspace is a collection of record types used by a team and represents the team's work lifecycle. You can fully customize workspaces in Adobe Workfront Planning. Record types are organized by sections in a workspace. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 604b84c1-4ec6-4d4a-b9f4-4223641ff2ea
---

# Create workspaces

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

In Adobe Workfront Planning, workspaces are centralized locations for teams to plan work. 

A workspace is a collection of record types used by a team and represents the team's work lifecycle. You can fully customize workspaces in Adobe Workfront Planning. 

For general information about workspaces, see [Workspaces overview](/help/quicksilver/planning/architecture/workspaces-overview.md). 

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
<p>Any Workfront or Workflow package</p> 
<p>Any Workfront Planning package</p>
<p>A Prime or higher package to create a workspace using the Planning Designer <!--<span class="preview">or to create multiple workspaces at a time</span>--></p>
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
</tbody> 
</table> -->

## Create a workspace

You can create a workspace and add record types to it to organize your objects in Workfront Planning. 

For more information about editing a workspace, see [Edit workspaces](/help/quicksilver/planning/architecture/edit-workspaces.md).

You can create workspaces in the following ways: 

* Create one workspace from scratch or from a template

   For information, see the section [Create a workspace from scratch or from a template](#create-a-workspace-from-scratch-or-from-a-template) in this article.
* Create one workspace using the AI-powered Planning Designer. This feature is currently in Beta. 

   For information, see [Get started with the Adobe Workfront Planning Designer](/help/quicksilver/planning/general/planning-ai-designer.md).

<!--
<div class="preview">

* Create multiple workspaces using a best-practice multi-workspace template bundle 

   For information, see the section [Create](#create-multiple-workspaces-using-a-best-practice-multi-workspace-template-bundle) in this article

</div>

-->

### Create a workspace from scratch or from a template

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

1. (Optional) Click the back arrow to the left of the new workspace to open the Planning main page. A new workspace card is created for the new workspace in the **Workspaces I'm on** tab. 

   The name of the user who created the workspace is saved on the workspace card as the Owner. 

   >[!NOTE]
   >
   >For users that are currently being transitioned to the Adobe Identity Management System (IMS), workspaces created by Workfront-only users who are not IMS users display as created by the **System**. 
   >
   >For information about IMS, see [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

<!--
<div class="preview">

### Create multiple workspaces using a best-practice multi-workspace template bundle

You can use a multi-workspace template bundle to create 6 workspaces with one click. 

The templates included in the bundle contain workspaces, record types, records, views, and fields to help you get started with your Planning implementation. 

>[!IMPORTANT]
>
>Note that all the names of workspaces, record types, fields, and records included in the bundle are samples and are not a reflection of your own environment. 
>
>We recommend that you use this template bundle as an example of a Planning structure and proceed with creating your own objects. 


{{step1-to-planning}}

1. Click **Create workspace**

   The Create workspace box displays. You can create a workspace from scratch or create it using one of the available templates. 
   
1. Click **Review workspace setup** in the **Start here (Recommended)** area. 
1. (Optional) Click **Preview** inside any of the following predefined workspace templates to open the Preview box for each template:

    * 1.Global Classifications & Taxonomies

         The Global Classifications & Taxonomies template includes all the record types and fields we recommend that you create in your environment for a successful implementation of Workfront Planning. 

         You can later link or import the record types in this template in other workspaces you create. 
    * 2.Fréscopa Global Marketing
    * 3.Fréscopa Social Marketing
    * 4.Fréscopa Media & PR
    * 5.Fréscopa Global Events
    * 6.Fréscopa Executive Company Leadership
    
1. After opening the **Preview** box for each workspace template, click Back to go back to the **Create workspace** box, or click Use templates to use the templates including in the bundle and create workspaces. 

   The workspaces are created and display in the **Workspaces I'm** on and **All Workspaces** tabs for System administrators. All Standard-license users will see the workspaces in their Workspaces area. 

1. Start editing the workspaces you created and adding record types, records, views, and fields that are pertinent to your organization. 

   For more information about best practices to implement Workfront, see the articles in the [Adobe Workfront Planning best practices: article index](/help/quicksilver/planning/best-practices.md/best-practices-article-index.md) section. 

   For information about editing workspaces, see [Edit workspaces](/help/quicksilver/planning/architecture/edit-workspaces.md). 

</div>
-->


