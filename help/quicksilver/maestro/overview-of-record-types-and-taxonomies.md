---
title: Overview of Adobe Maestro record types 
description: Record types are the building blocks of a Maestro workspace. 
hidefromtoc: yes
hide: yes
---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Overview of Adobe Maestro record types

Unlike Workfront where the object types are predefined, in Adobe Maestro, you can create your own object types. For example, in Workfront the object types of Program, Portfolio, Project, Task, or Issue are already created. 

Maestro object types are called "record types". Record types are the building blocks of a Maestro workspace. For information about workspaces, see [Create workspaces](../maestro/create-workspaces.md). 
    
## Record type overview
    
In Maestro, you can create custom object types that meet your organization's needs.

You can also import record types from other applications.

<!--Will be available later: You can also define how the record types relate to one another or form dependencies.--> 
    
There are two kinds of Maestro record types: 

* [Operational Record Type](#operational-record-type)
* [Taxonomy](#taxonomy)

You can have a combined total of 500 operational record types and taxonomies in one workspace.

### Operational Record Type{#operational-record-type}

An operational record type is a Maestro record type that represents work objects.  

![](assets/operational-record-type-blank.png)

You can do the following to add operational record types to a Maestro workspace: 

* Create an operational record type from scratch. For example, Campaign, Activity, or Program can be operational record types that you create from scratch in Maestro. 
* Import the following object types from other applications and they become Maestro operational record types:

    * Projects from Adobe Workfront <!--add to this list when we could import more objects from other apps-->

    For more information, see [Create record types](../maestro/create-record-types.md). 

### Taxonomy{#taxonomy}

A taxonomy is a record type that captures attributes about an operational record type. 

![](assets/taxonomy-record-type-blank.png)

Although creating taxonomies is identical to creating operational record types, Maestro distinguishes conceptually between an operational record type and a taxonomy record type. The purpose of taxonomies is to enhance operational record types. Taxonomies should not directly represent work objects.  <!--this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.--> 

<!--mimic what you did above for operational record types to say that we can also import taxonomies from other applications too - this will be possible later; for example Team would be a taxonomy record type, etc -->

For example, Audience, Region, or Address can be taxonomy-type record types.  

For more information, see [Create a taxonomy](../maestro/create-a-taxonomy.md).

