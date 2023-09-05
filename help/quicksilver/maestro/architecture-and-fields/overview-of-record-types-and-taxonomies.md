---
title: Overview of record types and taxonomies
description: Record types are the building blocks of a Maestro workspace. 
hidefromtoc: yes
hide: yes
---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Overview of record types and taxonomies

Unlike Workfront where the object types are predefined, in Adobe Maestro, you can create your own object types. For example, in Workfront the object types of Program, Portfolio, Project, Task, or Issue are already created. 

Maestro object types are called "record types". Record types are the building blocks of a Maestro workspace. For information about workspaces, see [Create workspaces](../architecture-and-fields/create-workspaces.md). 
    
## Record type overview
    
In Maestro, you can create custom record types that meet your organization's needs.
 
* The following are Maestro record types: 

    * [Operational Record Type](#operational-record-type): A record type that represents strategic plans, initiatives, or planned work. For example, Campaign, Activity, Tactic, Opportunity can be operational record types. 
    * [Taxonomy](#taxonomy): Record types that capture attributes about an operational record type. For example, Region, Address, Audience can be taxonomies. 

* When you create a record type, everyone in your organization can view, edit, or delete it. <!--this will change with access levels and permissions-->
* You must create a workspace before you can create record types for the workspace.  
* You can have a combined total of 1,000 operational record types and taxonomies in one workspace. This includes record types or taxonomies that you create from scratch or that you import from other systems. 

### Operational Record Type{#operational-record-type}

An operational record type is a Maestro record type that represents work-related objects.  

![](assets/operational-record-type-blank.png)

For more information about operational record types including how to create them, see [Create record types](../architecture-and-fields/create-record-types.md). 

### Taxonomy{#taxonomy}

A taxonomy is a record type that captures attributes about an operational record type. 

![](assets/taxonomy-record-type-blank.png)

For more information about taxonomy record types, see [Create a taxonomy](../architecture-and-fields/create-a-taxonomy.md). 

Although creating taxonomies is identical to creating operational record types, Maestro distinguishes conceptually between an operational record type and a taxonomy record type. The purpose of taxonomies is to enhance operational record types. Taxonomies should not directly represent work objects.  <!--this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.--> 

<!--mimic what you did above for operational record types to say that we can also import taxonomies from other applications too - this will be possible later; for example Team would be a taxonomy record type, etc -->

For example, Audience, Region, or Address can be taxonomy-type record types.  

For more information, see [Create a taxonomy](../architecture-and-fields/create-a-taxonomy.md). 

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
| You can connect the record type to an object from a third-party application |            ✓            |                      |
| You can connect to other Maestro record types               |            ✓            |                    |
| You can view their associated records in a table view       |            ✓            |           ✓          |
| You can view their associated records in a timeline view    |            ✓            |           ✓          |
