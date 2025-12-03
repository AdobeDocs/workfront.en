---
title: Hierarchy and Breadcrumb Overview
description: You can create multiple workspace hierarchies between the record types in a workspace.
hide: yes
hidefromtoc: yes
exl-id: 2f83c427-4439-499d-a0b2-fc8630552cae
---
<!--update the metadata with real information when making this available in TOC and in the left nav:

---
title: Hierarchy and Breadcrumb Overview
description: You can create multiple workspace hierarchies between the record types in a workspace. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hide: yes 
hidefromtoc: yes 
---
-->

# Hierarchy and breadcrumb overview

As a workspace manager, you can define flexible but structured hierarchies between record types and and other object types in Adobe Workfront Planning. 

The following are benefits of using hierarchies in your workspaces: 

* To organize work in a way that reflects how your teams actually plan, operate, and deliver. 
* Users understand where they are, how record types connect, and how strategy flows into execution by referring to a set of breadcrumbs that indicate their place in the system. 
* Offer a better navigation, and create clarity and continuity across all workflows. 
* Hierarchies do not enforce a rigid, system-defined structure, and instead allow you to define flows that fit how your organization works, supporting both flexibility and consistency across all stages of work.

## Considerations when working with hierarchies

* As a workspace manager, you can create multiple hierarchies for one workspace.
* If a connection between the selected record types already exists, the system reuses the existing connection.
* If no connection exists, Workfront will automatically create one as part of the hierarchy setup.
* The following are rules for hierarchy setup:
    * A record type can only have one parent record type in a given workspace. 
    
        For example, a Tactic record type cannot have both a Campaign and a Goal record type as a parent in the same workspace. 
    * A record can be connected to multiple parent records of the same type, when you connect one to many or many to many record types.
        For example, Tactic A can belong to both Campaign X and Campaign Y. 
    * A record type can connect to multiple children  record types. 
        
        For example, a Campaign record type can be the parent to multiple other record types, like Tactics, Tests, and other record types.
    * Hierarchies can include both Planning record types and Workfront object types.

        For example, you can have a Campaign record type with Planning Tactics and Workfront Projects as the children. 
    * Global record types may appear in multiple workspaces inside multiple hierarchies. 
    * Workfront object types can also appear in multiple hierarchies and across different workspaces.
    <!--Not sure what this means: * Shared record can't be part of hierarchies.-->
    * The record types with connections that do not create a corresponding field on their linked record types can also be part of hierarchies. New connections that are created during hierarch setup will always create a corresponding field on the linked record types, by default.

## Considerations when viewing breadcrumbs


