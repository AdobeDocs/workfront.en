---
title: Maestro overview
description: Use Maestro to create custom objects, fields, and workspaces. 
hidefromtoc: yes
hide: yes
---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->
<!--see the separate article I wrote to have the PMs vet it for this: https://adobe-my.sharepoint.com/personal/alinaw_adobe_com/_layouts/15/doc.aspx?sourcedoc={79f94807-3d73-4015-afc0-5c016fc63cfc}&action=edit-->

# Maestro overview

## Introduction to Adobe Maestro

Maestro is a new offering from Adobe Workfront whose purpose is to unlock comprehensive visibility into the operations details of an organization, and answer critical business questions at each stage of the work management lifecycle.  

Teams and leadership need clear answers to questions like:  

* How are my campaigns, current sales, or current developing products doing? Are we on track? 

* Which work should I prioritize next to have highest return on investment?  

To answer these questions, leadership needs a solution that can ensure a holistic view of every stage of work from planning to execution to delivery to measuring the results. Currently, organizations have tools that can cover some part of the process, but not many have good connections to all phases of work nor can reliably provide end results.  

Maestro wants to solve the problem of managing work across all phases and for all the stakeholders that participate in the work process.  

With Maestro, you can fully customize your workflows, from deciding what object types your organization uses to deciding how these objects link to one another.  

Additionally, Maestro can link to object types from other systems, creating a coherent framework for all your processes.  

## Access required to use Maestro

<!-- the table will change after we implement access levels/ permissions for Maestro-->
<!-- fix the formatting on the table - some lines are way too spaced out-->

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Any</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Product</p></td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Any</p>  
</td>
  </tr>
 </tbody>
</table>

>[!NOTE]
>
>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). 


## Maestro terminology

Although Maestro is part of Workfront, it comes with proprietary concepts and terminology. Ensure you are familiar with the Maestro concepts before embarking in setting up Maestro for your organization. 

The work frame for Maestro is fully customizable. You can create all object types, their attributes and any fields associated with them to suit the exact needs of your organization. 

The following are the main Maestro objects and concepts: 

* **Workspace**: A collection of record types and taxonomies that defines the workflow in a certain organization. 

    ![](assets/workspaces-page-with-templates-thumbnails.png)
    
    One Workfront instance may have an unlimited number of workspaces. 
    
    For more information, see [Create workspaces](../maestro/create-workspaces.md).

* **Record Type**: The Maestro main object type.  
    
    Unlike Workfront where the object types were predefined, in Maestro, you can create your own object types.  
    
    For example, in Workfront the object types of Program, Portfolio, Project, Task, or Issue are already created.  
    
    In Maestro, you can create any object types that meet your organization's workflows. You will later define how the record types relate to one another or form dependencies. 
    
    For more information, see [Overview of operational record types and taxonomies](../maestro/overview-of-record-types-and-taxonomies.md). 

    Maestro has the following record types: 

    * **Operational Record Type**: A Record Type that represents work objects.  

        ![](assets/operational-record-tyoe-blank.png)

        For example, Campaign, Activity, Program can be operational record types.  

        For more information, see [Create operational record types](../maestro/create-operational-record-types.md).

    * **Taxonomy**: A Record Type that captures attributes about an operational record type. 

        ![](assets/taxonomy-record-type-blank.png)

        Maestro distinguishes between an operational record type and a taxonomy record type. A taxonomy is a record without dates, like a static list of attributes.  

        For example, Audience, Region, or Address can be taxonomy-type record types.  

        For more information, see [Create a taxonomy](../maestro/create-a-taxonomy.md).

* **Record**: An instance of a Maestro record type. 

    ![](assets/records-highlighted-in-campaign-record-type-list.png)
    ![](assets/records-highlighted-in-region-taxonomy-type-list.png)
    
    When a Record Type is added to a Workspace, all its Records also become visible in that Workspace. 

    For example, "Campaign" can be an operational record type and "Summer Campaign for EMEA" is a record of the Campaign record type 
    
    Or 
    
    "Region" is a taxonomy-type record type, whereas "Americas-Latin America" or "EMEA - Central Europe" are taxonomy records.  
    
    For more information, see [Create records](../maestro/create-records.md). 

* **Workspace template**: Templates define the initial workspaces, record types, taxonomies, fields, etc., created for a customer after the onboarding questions are answered. 

    ![](assets/workspaces-page-with-templates-thumbnails.png)

    Maestro comes with a Sales, Marketing, and Product Management workspace template. 
    
    For more information, see [Create workspaces](../maestro/create-workspaces.md). 

* **Fields**: Fields are attributes that you can add to operational or taxonomy record types that contain information about the record type. 

    ![](assets/drop-down-list-of-record-fields.png)

    The fields added for a record type automatically become associated with all records of that type and can be used to capture data in those records. 

    Fields display in the view applied to the records (in columns, if the table view is applied) as well as on the Details page of the record. 
    
    For example, Status, Start Date, End Date, Owner are fields for a record type of Campaign.  

    When you create a record type, it comes with a set of predefined fields.  

    The following are types of fields you can associate with Maestro record types:  

    * Number 
    * Percentage 
    * Currency 
    * Single-line text 
    * Paragraph 
    * Single-select 
    * Multi-select 
    * Date 
    * Relationship: Connects two record types. 

    >[!NOTE]
    >
    >    * You can establish a connection between record types and reference the records of the linked record types by adding a Relationship-type field to a record type. 
    >
    >    * Fields are reusable across Record Types.  

    For more information, see [Create record type fields](../maestro/create-fields.md).   

* **Views**: Records display under their respective record type page in different types of views. 

    ![](assets/view-types-drop-down-from-record-type-list.png)

    Views contain personalized settings of a specific View Type, such as the list of fields (columns), a list of records (rows), their order (sort), an applied or applicable filter and grouping, or a timeline.  
    
    The following are views of records on the Record Type page: 

    * Table view. This is the default. 
    * Timeline view 

    Views include the filters and the groupings that are applied to the records displayed on the page.  

    For more information, see [Manage record views](../maestro/manage-record-views.md). 


## Maestro object limitations

The following table shows the limits for how many objects you can create in Maestro. The limitations are subject to change as we move into the next phases of Maestro's development.  

|       Maestro object                                                          |                                                        Limit                                                    |
|-------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------:|
|     Number of Workspaces for one Workfront instance                                      |   1,000                                                                                                         |
|     Number of Record Types for one workspace                                            |   1,000 (this includes taxonomies for the workspace, or objects that you import from third-party applications)  |
|     Number of records for one record type                                               |   10,000                                                                                                        |
|     Number of fields for one record type or taxonomy                            |   500                                                                                                           |
|     Number of characters for a text fields                                                               |   1,000 characters                                                                                              |
|     Size of file that you can paste in a record type table                    |   1MB                                                                                                           |
|     Size of file that you can import through the API for a record type table  |   1.5MB                                                                                                         |
|     Rate at which API requests can be made                                    |   200 requests per minute                                                                                       |
| Size of CSV of Excel file you can import in a table | 10MB |


## Features currently available in Maestro

The following table illustrates the features that will be available in Maestro as well as a timeline of their availability:

|       Feature                                      |     Available in closed beta  |     Available after closed beta  |     In research  |
|----------------------------------------------------|:-----------------------------:|:--------------------------------:|:----------------:|
|     Create workspaces                              |   ✓                           |                                  |                  |
|     Create operational record types                |   ✓                           |                                  |                  |
|     Create taxonomies                              |   ✓                           |                                  |                  |
|     Create individual  records and taxonomies      |   ✓                           |                                  |                  |
|     Create record custom fields                    |   ✓                           |                                  |                  |
|     Link records                                   |   ✓                           |                                  |                  |
|     View records in a table                        |   ✓                           |                                  |                  |
|     View records in a timeline                     |   ✓                           |                                  |                  |
|     Filter records                                 |   ✓                           |                                  |                  |
|     Group records in the timeline view             |   ✓                           |                                  |                  |
|     Group records in the table view                |                               |   ✓                              |                  |
|     Sort records                                   |                               |   ✓                              |                  |
|     Link workspaces                                |                               |   ✓                              |                  |
|     Connect Maestro records to Workfront projects  |                               |   ✓                              |                  |
|     Record details page                            |   ✓                           |                                  |                  |
|     Update record details page layout              |                               |   ✓                              |                  |
| Access levels and permissions | | | ✓ |
|     Submit requests                                |                               |                                  |   ✓              |
|     Creative brief                                 |                               |                                  |   ✓              |


## Enable Maestro for the users in your Workfront instance

First, contact your account manager to obtain access to the current Maestro closed beta program. After your organization has been enrolled in the Maestro beta program, you can add the Maestro area to other users by using a layout template. 

To share the Maestro area using a layout template: 

1. Log in to Workfront as a system administrator.  

1. Add the Maestro icon to the Main Menu using a Layout Template. For information, see [Customize the Main Menu using a layout template](../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md).  

1. Assign the  layout template to the users that you want to have access to Maestro. For information, see [Assign users to a layout template](../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md). 

    All users who can access Maestro in their Main Menu can start creating workspaces, records types, records, and fields.  
 
<!-- the important below will be removed with access levels/ permissions -->

>[!IMPORTANT]
>
>Currently, there are no access levels or permissions associated with the information in Maestro. All items that any user creates are visible to everyone who can access Maestro. 


## Locate Maestro in Adobe Workfront

Ensure that your organization has received access to Maestro and that your system or group administrator has added the Maestro area to your Main Menu.  

To locate Maestro:  

1. Log in to Adobe Workfront. 

1. Click the **Main Menu** ![](assets/main-menu-workfront.png) in the upper-right corner, or click the **Main Menu** ![](assets/main-menu-shell.png) in the upper-left corner, if it's available. 

1. Click **Maestro**. 

1. The Maestro Workspaces area opens. 

1. (Optional and recommended) Continue with some of the following actions, to build your work structure inside Maestro: 

    1. Create a workspace from scratch or using a template. 

    1. Add Record Types to the new workspace. 

    1. Add Taxonomies to the new workspaces. 

    1. Update or create a new View for a set of records inside the Record Type page. 

    1. Using the table view to display a record type, click the **+** icon in the upper right corner to add new record fields. 

    1. Using the table view to view a record type, click the **+** icon in the lower-left corner to add new records. 

    1. Click the name of a record to view more information.

    
