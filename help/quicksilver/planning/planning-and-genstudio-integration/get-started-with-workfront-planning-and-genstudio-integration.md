---
title: Get Started with the Workfront Planning and GenStudio for Performance Marketing Integration
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products. Learn some of the basics about how you can streamline your workflows using this integration.
hide: yes
hidefromtoc: yes
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
---
# Get started with the Workfront Planning and GenStudio for Performance Marketing integration

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
   <li><p> Adobe Workfront Planning<p></li>
   <p><li> Adobe GenStudio for Performance Marketing<p></li>
   </ul></td> 
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
   <td role="rowheader"><p>Adobe Workfront Planning package</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account manager. </p> 
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
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p> System administrator</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Contribute or higher permissions to a workspace and record type  </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> 

 *For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


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
* You can share GenStudio record types with others in Planning.  <!--checking with Ani H.-->
* You can create record types from Planning on the GenStudio workspace. <!-- checking with Ani where these show up in GenS-->
* Record types that are synced with GenStudio display a visual indicator that makes it clear that the record types is imported from GenStudio.

### Records

* You can add or delete records in GenStudio and they become visible in (or are removed from) Workfront Planning. 
    You can add or delete records in Workfront Planning and they become visible in (or are removed from) GenStudio. 
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
* You can create more fields for GenStudio record types in Workfront Planning if you have Manage access in Gen Studio. 
* When you create fields for GenStudio record types in Planning, they are visible from the following areas:
    * Planning views
    * Planning record details pages
    * GenStudio record details pages

    >[!TIP]
    >
    >Fields created in Workfront Planning are not visible in the GenStudio list view.
    
* You can hide fields in the table view of a GenStudio record type in Planning, but you cannot delete fields from Workfront Planning.


<!-- checking: 
I had this from Iskuhi, so not sure if you CAN create fields in Planning?? - only the newly added fiedsl can be changed or the reference fields. - from this: https://experience.adobe.com/?commentID=6848549f00000091e5f5a16636e381c0#/@adobeinternalworkfront/so:hub-Hub/workfront/project/67649bc00000545810daad1cd1fbb9cc/updates 
-->

<!--document who shows up in the Created by and Updated by fields - not clear, asking-->

### Views

* You can create views for GenStudio record types. 

    For information, see [Manage record views](/help/quicksilver/planning/views/manage-record-views.md). 

* You can share the view of a GenStudio record type as you'd share a view for a Planning record type. 

### Connections

* You can make the following connections between GenStudio record types and other record or object types in Workfront Planning:

    * Two GenStudio record types and 
    * A GenStudio record type and a Planning record type from the same workspace
    * A GenStudio record type and a Planning record type from another workspace, if the record types are configured to connect from another workspace. 
    * A GenStudio record type and a Workfront object type (projects, portfolios, programs, companies, groups)