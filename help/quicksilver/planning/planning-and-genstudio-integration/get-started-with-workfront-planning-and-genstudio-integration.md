---
title: Get Started with the Workfront Planning and GenStudio for Performance Marketing Integration
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products. Learn some of the basics about how you can streamline your workflows using this integration.
hide: yes
hidefromtoc: yes
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
---
# Get started with the Adobe Workfront Planning and Adobe GenStudio for Performance Marketing integration

<!--update the text in the title everywhere this article is linked from - it changed a few times-->

<!--Better metadata, at publishing:
---
title: Get Started with the Workfront Planning and GenStudio for Performance Marketing Integration
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products. Learn some of the basics about how you can streamline your workflows using this integration.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog

---
-->

<!--use this article to make this one similar to it: https://experienceleague.adobe.com/en/docs/workfront/using/adobe-workfront-integrations/review-approval-integrations/wf-proof-and-genstudio-->

Organizations using both Adobe Workfront Planning and Adobe GenStudio for Performance Marketing often define marketing concepts like Campaigns, Products, and Personas in more detail than what GenStudio supports by default. 

There is a native integration between GenStudio for Performance Marketing and Workfront Planning. This integration allows users in Workfront Planning to manage the Campaigns, Products, Personas, Activations, Channels, and Regions used in GenStudio. It also enables them to configure GenStudio to reference existing record types from Workfront Planning, creating a more connected and consistent marketing workflow.

This integration helps you to avoid duplicate data entry, maintain alignment across planning and activation efforts, and supports your marketing system of record. 

The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products.

With the integration between Workfront Planning and GenStudio for Performance Marketing, you can:

<!--check this list and ensure it's accurate and add/ remove some of the benefits-->

* View the GenStudio workspace in Workfront Planning. 
* Modify your campaigns in GenStudio and have real-time updates of the same information in Workfront Planning. 
* Modify your campaigns in Workfront Planning and have real-time updates of the same information in GenStudio. 

## Integration requirements

* Workfront and GenStudio for Performance Marketing must be enabled to the same organization. 

    For more information about GenStudio, see [Adobe GenStudio for Performance Marketing User Guide](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home).
    
* GenStudio will not be available in Workfront Planning when your company has multiple Workfront instances. <!--this will change-->

* The Workfront instance is part of the Adobe Unified Experience, including using the Identity Management System (IMS). 

    For information, see [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

* Users using both Planning and GenStudio can belong to only one Workfront instance within the IMS organization.

<!--not sure: true for Planning? This is true for GenS and WF Proof: * The integration must be enabled in the Workfront Setup area.-->

## Access requirements

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
   <li><p> Adobe GenStudio for Performance Marketing</p></li>
   </ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Any Workfront Workflow package</p>  
<p>Any Workfront Planning package</p>
   </td> </tr>

<tr> 
   <td role="rowheader"><p>Adobe GenStudio package</p></td> 
   <td> 
<p>???</p>  

   </td> </tr>
 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p> System administrator</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe GenStudio license</p></td> 
   <td><p> ???</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>  
   <p>Configuration for GenStudio: ???</p> 
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>  
   <p>In Workfront Planning: </p>
   <ul>
   <li><p>Contribute or higher permissions to a workspace and record type  </p> </li> 
   <li><p>System Administrators have permissions to all workspaces, including the ones they did not create</p></li>
   </ul>
   <p>In Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <li><p> Any permissions in Adobe GenStudio for Performance Marketing</p></li>
   <li><p> Create permissions in Adobe GenStudio for Performance Marketing to create items</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
 *For more information about Adobe GenStudio for Performance Marketing, see [Adobe GenStudio for Performance Marketing User Guide](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home).


## Overview of the Workfront Planning and GenStudio integration

The following sections describe the following:

* Capabilities for updating Workfront Planning information from GenStudio
* Capabilities for updating GenStudio information from Workfront Planning
* Limitations for what you can and cannot manage in a GenStudio workspace from Workfront Planning. 

<!--add here a link from the GenS articles about what you can/ cannot do from GenStudio that might in the end reflect in Planning - this should come from the GenS team-->

### The GenStudio workspace in Workfront Planning

* If your organization has multiple Workfront instances, the GenStudio workspace is not visible from any of your Workfront instance. <!-- this might change-->
* The GenStudio workspace displays a visual indicator that makes it clear that it is imported from GenStudio. For information, see [Manage the GenStudio workspace in Adobe Workfront Planning](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md). 
* All users who have access to both GenStudio and Workfront Planning can also see the GenStudio workspace in Workfront Planning. 
* Workfront Planning users must be managed through the Adobe Identity Management System (IMS) to be able to view and use the GenStudio workspace from Workfront. 

    Workfront-only users cannot see the GenStudio workspace, even when it is available in Workfront. 
    
    For information, see [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md). 


### Record types

* You can edit record types information (for example, their appearance) from GenStudio in Workfront Planning. 
* You can share GenStudio record types with others in Planning.  
* You can create record types from Planning on the GenStudio workspace. These record types remain only in Planning. They do not display in GenStudio. 
* Record types that are synced with GenStudio display a visual indicator in Workfront Planning that makes it clear that the record types is imported from GenStudio. 

### Records

* You can add or delete records in GenStudio and they become visible in (or are removed from) Workfront Planning. 
* You can add or delete records in Workfront Planning and they become visible in (or are removed from) GenStudio. 
* When you delete records from either Workfront Planning or GenStudio, they are placed in the Recently deleted bin for 30 days. GenStudio does not have a Recently deleted bin. 
* Restoring a record from the Recently deleted bin places them back in Workfront Planning and GenStudio. 
* You can add records from Workfront Planning in the following ways:

    * Manually, from scratch, from any view using the New record button
    * By importing them using a CSV or Excel file
    * Manually, inline, in the table view
    * Manually, directly in the timeline view

    For information, see [Create records](/help/quicksilver/planning/records/create-records.md). 
* You cannot create or delete Activation records from Workfront Planning. 
* You can edit record information on all records in the GenStudio workspace oin Planning in any of the visible fields from Workfront Planning. 

    For information, see [Edit records](/help/quicksilver/planning/records/edit-records.md).

    <!--asking Ani if I delete a record in GS - will it move to Recovery box in Planning?-->

### Fields

* Record fields are imported from GenStudio. You can edit the field settings in Workfront Planning. 
* You can create fields for GenStudio record types in Workfront Planning if you have Manage access in Gen Studio. 
* When you create fields for GenStudio record types in Planning, they are visible from the following areas:
    * Planning views
    * Planning record details pages
    * GenStudio record details pages

    >[!TIP]
    >
    >Fields created in Workfront Planning are not visible in the GenStudio list view.
    
* You can hide fields in the table view of a GenStudio record type in Planning. 
* You cannot delete fields imported from GenStudio from Workfront Planning.
* You can delete fields created in Workfront Planning for GenStudio record types from Workfront Planning. 


### The Created by and Approved by fields

* You can add the Created by and Approved by fields for the GenStudio record types in Workfront Planning from Workfront Planning. 
* The records that display in the Channel and Region record types will display "System" as the Created by user. These records are created automatically when the GenStudio workspace is created in Workfront Planning. 
* The records created in GenStudio after the workspace was made available in Workfront Planning will display the name of the IMS user who created the record in the Created by field, even if the user created the records in GenStudio and is not a Workfront user. 
* The Approved by field displays the name of the approver when a request form is submitted to create a record. 

### Views

* You can create views for GenStudio record types. 

    For information, see [Manage record views](/help/quicksilver/planning/views/manage-record-views.md). 

* You can share the view of a GenStudio record type as you'd share a view for a Planning record type. 
* You cannot create multiple views in GenStudio. 

### Connections

* You can make the following connections between GenStudio record types and other record or object types in Workfront Planning:

    * Two GenStudio record types
    * A GenStudio record type and a Planning record type from the same workspace
    * A GenStudio record type and a Planning record type from another workspace, if the record types are configured to connect from another workspace. 
    * A GenStudio record type and a Workfront object type (projects, portfolios, programs, companies, groups)
    * A GenStudio record type and an AEM Assets object type.

### Request forms and automations

* You can add request forms and automations to a GenStudio record type in Workfront Planning. 

### The Preview environment

* The GenStudio workspace accessible from your Production environment also displays in your Preview environment. 
* You can perform all the activities described in this article on the GenStudio workspace in Workfront Planning in your Preview environment but these changes will not transfer to GenStudio.
    Only changes you make to items in the Production environment sync between Workfront Planning and GenStudio. 
    GenStudio does not have a Preview environment. 

