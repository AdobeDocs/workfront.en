---
title: Get Started with the Workfront Planning and GenStudio for Performance Marketing Integration
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products. Learn some of the basics about how you can streamline your workflows using this integration.
hide: yes
hidefromtoc: yes
exl-id: 3b2fc764-f384-41bb-9d88-b2b88434ffc6
---
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


# Get started with the Adobe Workfront Planning and Adobe GenStudio for Performance Marketing integration

<!--update the text in the title everywhere this article is linked from - it changed a few times-->

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

Organizations using both Adobe Workfront Planning and Adobe GenStudio for Performance Marketing often define marketing concepts like Campaigns, Products, and Personas in more detail than what GenStudio supports by default. 

There is a native integration between GenStudio for Performance Marketing and Workfront Planning. This integration allows users in Workfront Planning to manage the Campaigns, Products, Personas, Activations, Channels, and Regions used in GenStudio. It also enables them to configure GenStudio to reference existing record types from Workfront Planning, creating a more connected and consistent marketing workflow.

The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products.

## Integration benefits

With the integration between Workfront Planning and GenStudio for Performance Marketing, you can:

<!--check this list and ensure it's accurate and add/ remove some of the benefits-->

* View the GenStudio workspace in Workfront Planning. 
* Modify your campaigns in GenStudio and have real-time updates of the same information in Workfront Planning. 
* Modify your campaigns in Workfront Planning and have real-time updates of the same information in GenStudio. 
* Avoid duplicate data entry.
* Maintain alignment across planning and activation efforts. 

## Integration requirements

Your organization must meet the following requirements for the integration between Workfront Planning and GenStudio for Performance Marketing to exist: 

* Workfront and GenStudio for Performance Marketing must be enabled to the same organization. 

    For more information about GenStudio, see [Adobe GenStudio for Performance Marketing User Guide](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home).
    
<!--No longer the case: * Your organization must have only one Workfront instance. GenStudio will not be available in Workfront Planning when your company has multiple Workfront instances. -->

* Your Workfront instance is part of the Adobe Unified Experience, including using the Identity Management System (IMS). 

    For information, see [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

* Users using both Planning and GenStudio must belong to only one Workfront instance within the IMS organization.

    Workfront-only users cannot see the GenStudio workspace, even when it is available in Workfront. 

<!--not sure: true for Planning? This is true for GenS and WF Proof: * The integration must be enabled in the Workfront Setup area.-->

## Access requirements

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Any Workfront package</p>
<p>Any Planning package</p>  

   </td> </tr>
   <tr> 
<td> 
   <p> Additional products</p> </td> 
   <td> 
   <p> Adobe GenStudio for Performance Marketing</p></td> 
  </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p> Standard</p>
  </td> 
  </tr> 
   
  <tr> 
   <td role="rowheader"><p>Adobe GenStudio for Performance Marketing user roles</p></td> 
   <td><p><ul><li>Any GenStudio user role to access Campaigns, Products, and Personas</li>
   <li>GenSudio System Manager to access Activations and Events</li></ul>
   For information, see <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">User roles and permissions</a>. 
   </p>
  </td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>  
   <p>In Workfront Planning: </p>
   <ul>
   <li><p>Manage permissions to the GenStudio workspace to change the architecture of the workspace, the record types, and fields</p></li>
   <li><p>Contribute permissions to the GenStudio workspace to add, update, or delete records in the GenStudio record space</p> </li>  
   </ul>
   <p>In Adobe GenStudio for Performance Marketing: <p>
   <ul>
   <li><p> Any permissions in Adobe GenStudio for Performance Marketing</p></li>
   <li><p> Create permissions in Adobe GenStudio for Performance Marketing to create items</p></li></ul>
   </td> 
  </tr> 
</tbody> 
</table> 

For information about Adobe Workfront Planning access, see [Adobe Workfront Planning access overview](/help/quicksilver/planning/access/access-overview.md).

For more information about Adobe GenStudio for Performance Marketing, see [Adobe GenStudio for Performance Marketing User Guide](https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/home).


## Overview of the Workfront Planning and GenStudio integration capabilities

Depending on how many Workfront instances your organization has, you automatically have the following permissions to the GenStudio workspace in Planning:  

<!--this table exists in the article Manage GenStudio workspace in Planning-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
    <td role="rowheader"><p>One instance of Workfront</p></td> 
   <td> 
<p>There is one GenStudio workspace in Workfront Planning</p>
<p>All users with access to GenStudio and Workfront Planning have Manage permisisons on the GenStudio workspace</p> 
</td> </tr>
   <tr> 
<td> 
   <p> Multiple instances of Workfront</p> </td> 
   <td> 
   <p>There is one GenStudio workspace in each Workfront Planning instance</p>
<p>All users with access to GenStudio and Workfront Planning have Contribute permisisons on the GenStudio workspace of each instance</p> </td> 
  </tr>
 
  </tbody> 
</table> 

For information about Workfront Planning permissions, see [Overview of sharing permissions in Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md). 

The sections below describe the following:

* Capabilities for updating Workfront Planning information from GenStudio
* Capabilities for updating GenStudio information from Workfront Planning
* Limitations for what you can and cannot manage in a GenStudio workspace from Workfront Planning. 

<!--maybe make 2 sections here once Iskuhi answers - one for one instance and one for multiple WF instances??-->

<!--add here a link from the GenS articles about what you can/ cannot do from GenStudio that might in the end reflect in Planning - this should come from the GenS team-->

### The GenStudio workspace

* When you update the GenStudio workspace in GenStudio, the changes are visible in the GenStudio workspace in Planning. 
* The GenStudio workspace displays a visual indicator in Workfront Planning to identify it as such. 

    ![GenStudio card in Planning](assets/genstudio-card-with-tag-highlighted.png)

    For information, see [Manage the GenStudio workspace in Adobe Workfront Planning](/help/quicksilver/planning/planning-and-genstudio-integration/manage-gen-studio-workspace-in-planning.md). 
*  When you have Manage permissions to the GenStudio workspace in Planning, you can:

    * Update the GenStudio workspace in Planning (name, description, icon)
    * Create sections
    * Add record types
    * Share it with others

        You can share the GenStudio workspace with others who don't have a GenStudio account. You can share it only with users available in the Identity Management System (IMS) of your organization. <!--check to see this is correct--> 
    <!--* Delete the workspace - check to see if this is possible; the link is there, but???-->

* When you have Contribute permissions to the GenStudio workspace in Planning, you cannot modify the workspace from Planning. 

### Record types in the GenStudio workspace

* When you edit the GenStudio record types in GenStudio, the changes are visible in the GenStudio workspace in Planning. 
* Record types visible both in GenStudio and Planning have a GenStudio indicator in Workfront Planning. 

    ![GenStudio record type card in Workfront Planning](assets/genstudio-record-type-with-tag-and-tooltip-highlighted.png)
* When you have Manage permissions to the GenStudio workspace in Planning, you can do the following from Workfront Planning: 
    * Edit GenStudio record types information (their appearance, advanced settings). 
    * Share GenStudio record types with others.  
    * Create record types. These record types remain only in Workfront Planning. They do not display in GenStudio. 
* When you have Contribute permissions to the GenStudio workspace in Planning, you cannot modify the GenStudio record types from Planning. 

### Records in the GenStudio workspace

* When you edit GenStudio records in GenStudio, the changes are visible in all the GenStudio workspaces in all your instances of Workfront. 
* You cannot create or delete Activation records from Workfront Planning. 
* When you have Manage or Contribute permissions to the GenStudio workspace in Planning, you can do the following from Workfront Planning: 
    * Add or delete records and they become visible in (or are removed from) GenStudio. 
    
        Deleted records from either Workfront Planning or GenStudio are placed in the Workfront Planning Recently deleted bin for 30 days. GenStudio does not have a Recently deleted bin. 
    * Restore a record from the Recently deleted bin. Restoring deleted records places them back in Workfront Planning and GenStudio. 
    * Add records in the following ways:

        * Manually, from scratch, from any view using the New record button
        * By importing them using a CSV or Excel file in the table view
        * Manually, in any view in Workfront Planning
        * By submitting a request to a record type request form in Workfront. 

    For information, see [Create records](/help/quicksilver/planning/records/create-records.md). 
* You can edit record information on all records in the GenStudio workspace from Workfront Planning.

    For information, see [Edit records](/help/quicksilver/planning/records/edit-records.md).

### Fields of record types in the GenStudio workspace

* GenStudio record fields are imported to Workfront Planning by default. 
* You cannot add fields to record types in GenStudio. 
* When you have Manage permissions to the GenStudio workspace in Planning, you can do the following from Workfront Planning: 

    * Edit GenStudio field settings. 
    * Create fields for GenStudio record types, if you have Manage access in Gen Studio.
    
        When you create fields for GenStudio record types in Planning, they are visible from the following areas:
        
        * Workfront Planning views
        * Workfront Planning record details pages
        * GenStudio record details pages

        >[!TIP]
        >
        >Fields created in Workfront Planning are not visible in the GenStudio list view.
    
    * Hide fields in the table view of a GenStudio record type in Planning. 
    <!--* Delete fields created in Workfront Planning for GenStudio record types from Workfront Planning. -- this is not possible, per Iskuhi; the link is there but it will generate an error-->

    <!--this is not true: You cannot delete fields imported from GenStudio from Workfront Planning.-->

* When you have Contribute permissions to the GenStudio workspace in Planning:

    * You cannot edit field setting, delete or add fields from the GenStudio workspace in Workfront Planning. 
    * You can hide fields from the table view in Workfront Planning.

#### The Created by and Approved by fields

* You can add the Created by and Approved by fields for the GenStudio record types in Workfront Planning from Workfront Planning. 
* The records that display in the Channel and Region record types will display "System" as the Created by user. These records are created automatically when the GenStudio workspace is created in Workfront Planning. 
* The records created in GenStudio after the workspace was made available in Workfront Planning will display the name of the IMS user who created the record in the Created by field, even if the user created the records in GenStudio and is not a Workfront user. 
* The Approved by field displays the name of the approver when a request form is submitted to create a record in the GenStudio record type in Workfront Planning. 

### Record views in the GenStudio workspace

>[!NOTE]
>
>The GenStudio record types display in the default table view imported from GenStudio. 
>
>You cannot delete the original table view that was imported by default from GenStudio.

* You cannot create multiple views in GenStudio. 

* When you have Manage permissions to the GenStudio workspace in Planning, you can do the following in Workfront Planning:

    * Create views for GenStudio record types. 

        For information, see [Manage record views](/help/quicksilver/planning/views/manage-record-views.md). 

    * Rename, share, export, duplicate, or delete any custom views from the GenStudio record types. 

* When you have Contribute permissions to the GenStudio workspace in Planning, you can do the following in Workfront Planning:

    * Create views for GenStudio record types. 

        For information, see [Manage record views](/help/quicksilver/planning/views/manage-record-views.md). 

    * Rename, export, duplicate, or delete custom views from the GenStudio record types.

        You cannot share views from the GenStudio workspace in Workfront Planning    

### Record connections in the GenStudio workspace

You can create connections between record types in GenStudio workspaces where you have Manage permissions. 

You can make the following connections between GenStudio record types and other record or object types in Workfront Planning:

* Two GenStudio record types
* A GenStudio record type and a Planning record type from the same workspace
* A GenStudio record type and a Planning record type from another workspace, if the record types are configured to connect from another workspace. 
* A GenStudio record type and a Workfront object type (projects, portfolios, programs, companies, groups)
* A GenStudio record type and an AEM Assets object type.

### Request forms and automations in the GenStudio record type

* You can add request forms to a GenStudio record type in Workfront Planning. 

    For information, see [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
* You can configure automations for a GenStudio record type in Workfront Planning.
    
    For information, see [Configure Adobe Workfront Planning automations](/help/quicksilver/planning/records/configure-automations-to-create-records.md).

## The Preview environment

* The GenStudio workspace accessible from your Production environment also displays in your Preview environment of the same Workfront instance. 
* You can perform all the activities described in this article on the GenStudio workspace in Workfront Planning in your Preview environment, but these changes will not be visible from GenStudio.

    Only changes you make to items in the Production environment sync between Workfront Planning and GenStudio. 
    
    GenStudio does not have a Preview environment. 

