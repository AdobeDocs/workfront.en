---
title: Record types overview
description: Record types are the building blocks of a Adobe Workfront Planning workspace.
hidefromtoc: yes
hide: yes
recommendations: noDisplay, noCatalog
exl-id: 1de095b3-78d9-44df-a678-51f4238deb91
---
<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Record types overview

{{planning-important-intro}}

Unlike Workfront where the object types are predefined, in Adobe Workfront Planning, you can create your own object types. For example, in Workfront the object types of Program, Portfolio, Project, Task, or Issue are already created. 

Workfront Planning object types are called "record types" and they exist only when users create them. Record types are the building blocks of a Workfront Planning workspace. For information about workspaces, see [Create workspaces](/help/quicksilver/planning/architecture/create-workspaces.md). 
    
## Record type overview
    
In Workfront Planning, you can create custom record types that meet your organization's needs.

For information about creating record types, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md). 
 
* When you create a workspace from a template, record types are created in the following workspace sections: 

    * **Operational Record Types**: Record types that represent strategic plans, initiatives, or planned work. For example, Campaign, Activity, Tactic, Opportunity are operational record types. 
    * **Taxonomies**: Record types that capture attributes about an operational record type. For example, Region, Address, Audience are taxonomies. 

* When you create a record type in a workspace that you created from scratch, you can place the record type in any section you create in the workspace. 
* When you create a record type, only you and those you give permissions to access the workspace can view the record type. 
* You must create a workspace before you can create record types for the workspace.  
* You can have a total of 1,000 record types in one workspace, regardless of how many sections the workspace has. This includes record types that you create from scratch or that are created when using a template. 


<!--

### Operational Record Type{#operational-record-type}

An operational record type is a Wrorkfront Planning record type that represents work-related objects.  

(***********insert screen shot**************)
For more information about operational record types including how to create them, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md). 

### Taxonomy{#taxonomy}

A taxonomy is a record type that captures attributes about an operational record type. 

(**********add screen shot**********)

Although creating taxonomies is identical to creating operational record types, Workfront Planning distinguishes conceptually between an operational record type and a taxonomy record type. The purpose of taxonomies is to enhance operational record types. Taxonomies should not directly represent work objects.  (***********this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.***********) 

(********mimic what you did above for operational record types to say that we can also import taxonomies from other applications too - this will be possible later; for example Team would be a taxonomy record type, etc*************)

For example, Audience, Region, or Address can be taxonomy-type record types.  

## Similarities and differences between operational record types and taxonomies

The following table illustrates some of the similarities and differences between operational record types and taxonomies: 

| Record type and characteristic                              | Operational Record Type | Taxonomy Record Type |
|-------------------------------------------------------------|:-----------------------:|:--------------------:|
| They are part of a workspace                                |            ✓            |           ✓          |
| You can create them automatically, from a workspace template                    |            ✓            |           ✓          |
| You can create them manually, from scratch                    |            ✓            |           ✓          |
| You can create them by copying and pasting information from an external file or list                   |            ✓            |           ✓          |
| You can create by importing an Excel or CSV file                    |            ✓            |                     |
| You can create read-only record types by connecting to object types from other applications                    |            ✓            |                     |
| They represent work-related objects                         |            ✓            |                      |
| They represent attributes about work-related objects        |                         |           ✓          |
| You can create from scratch                                 |            ✓            |           ✓          |
| You can create by importing an Excel or CSV file            |            ✓            |                      |
| You can connect the record type to an object from another application|            ✓            |                      |
| You can connect to other record types               |            ✓            |                    |
| You can view their associated records in a table view       |            ✓            |           ✓          |
| You can view their associated records in a timeline view    |            ✓            |           ✓          |

-->